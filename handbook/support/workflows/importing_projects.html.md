---
layout: handbook-page-toc
title: Importing Projects for Customers
category: GitLab.com
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

This workflow is meant to provide guidance on when GitLab Team members might offer to import projects on behalf of customers or prospects as a courtesy, and the process for doing the imports.

Due to the shifting nature of what issues might be relevant, the specifics of this workflow may change.

If helpful, [there is a video recording from 2019-05-22](https://drive.google.com/open?id=1v0LQi0povBlP2RhpsD1drfpux5kFq7Fq)(internal) where the first half is a walkthrough of the process, and the second half talks through troubleshooting issues.

## Related macros

- `GitLab.com::Import::Verify import criteria`
- `GitLab.com::Import::Require group permission`
- `GitLab.com::Import::Offer import`

## Criteria

The Support Team can offer to import a few projects as a best effort courtesy, but anything complex with a hundreds of users or projects is out of scope. These users should be referred to [Professional Services](/services/migration/).

Additionally:

1. The import method is a GitLab project export file.
1. The requestor should be an existing customer or a prospect.
1. The import was attempted and failed one or more times.
1. The target location is a group (not a personal namespace, can be transferred if necessary).
1. Target group is not empty.
1. No import error is found (see below).

### Identifying import errors

If the user is getting a version import/export error, ensure that the export originated from a [compatible version of GitLab](https://docs.gitlab.com/ee/user/project/settings/import_export.html#version-history).

The following are often reported by users as errors, but are known:

- Repository size may differ. See [comment for explanation](https://gitlab.com/gitlab-org/gitlab-ce/issues/59847#note_158425967). As artifacts are part of repository size, whether they are present can make a _big_ difference.
- Repository size says 0. See [CE 19188](https://gitlab.com/gitlab-org/gitlab-ce/issues/19188).

See [500 errors workflow](/handbook/support/workflows/500_errors.html) for more details on searching Kibana and Sentry.

- In Kibana, search sidekiq log: use
  - json.path and filter: json.severity: (not `INFO`) or
  - json.controller: `Projects::ImportsController` with error status
- In Sentry, search/look for: `Projects::ImportService::Error` ; make sure to remove `is:unresolved` filter

If there is an error, search for an existing issue, for example [award emoji on snippets](https://gitlab.com/gitlab-org/gitlab-ce/issues/62250). Similar errors where the metadata is throwing an error and no issue exists, consider creating one from Sentry.

If no error is found and the import is partial, most likely it is a timeout issue.

### Pre-Approved Cases

#### Case 1: Large imports

Due to [CE issue #52956](https://gitlab.com/gitlab-org/gitlab-ce/issues/52956), users with large projects (~1GB+) will often hit the timeout. Imports stop when it hits an error or a timeout, but will always create the barebones resulting in partial imports.

Options to reduce project size:

- cutting down the repo size (if that's what's large) via a cleanup first using [docs](https://docs.gitlab.com/ee/user/project/repository/reducing_the_repo_size_using_git.html#using-git-filter-branch) and ensuring/running `git gc` and `housekeeping`
- cutting down what's exported by editing the `import_export.yml` file (in self-managed instance), see this and 2-3 following comments: https://gitlab.com/gitlab-org/gitlab-ce/issues/52956#note_112117847

Note, these are noted in the macro `GitLab.com::Import::Verify import criteria`.

#### Case 2: User mapping of items

An admin is required to corrently map users in GitLab as [per our documentation](https://docs.gitlab.com/ee/user/project/settings/import_export.html). Without an admin account, repo commits will have correct user attribution, but issues, MRs, etc. will not. There is a [feature proposal to not require an admin user](https://gitlab.com/gitlab-org/gitlab-ce/issues/36338) being discussed.

#### Other cases

When in doubt, file an issue in [dotcom-escalations](https://gitlab.com/gitlab-com/support/dotcom/dotcom-escalations/issues) and ask for a manager's input. If a manager approves, proceed with the import.

## Process

### Verify Permissions

Before offering to do the import, verify the following:

1. User is a group owner.
1. User has rights to create new projects in the space.

If not verified, let the user know we might be able to offer an import, but a group owner needs to contact us or they need to adjust their settings (depending on which of the above is not verified) using `GitLab.com::Import::Verify import criteria` macro.

### Offer import and gather information

Once verified:

1. Offer for the GitLab team to do an import on their behalf as a courtesy using the `GitLab.com::Import::Offer import` macro.
1. Ask the user to (in macro):
    1. confirm the group where the project should be imported.
    1. confirm no project currently exists in the namespace with the project's name.
    1. provide a copy of their project's export. Recommended sites: send.firefox.com (up to 1GB, expires after 24 hours), wetransfer.com (up to 2 GB).
    1. Depending on the case:
        - _Correctly mapped users_: that _all_ active users have accounts on GitLab.com with matching _company_ email address as their primary email account. All email addresses in the project export should have the company domain.
        - _No user mapping_: provide the username for items to be attributed to.
    1. Provide date/time with timezone when they will send us the export at least 1 business day in advance.
1. If scheduling ahead of time, create the infra issue with all available information (see below for details).

### After receiving export

1. When receiving the project export: download, and ensure it unpacks. If not, ask the user for another copy.
1. For _correctly mapped users_ only:
    1. In a command line window, navigate to the folder where the project export resides.
    1. Use the [export file user checker](https://gitlab.com/gitlab-com/support/toolbox/dcef) to verify that all the email addresses exist on GitLab.com. If not, respond to the customer with the list of email addresses not in GitLab.com.
        - Reminder: The API and importer only checks primary email address, so users will match only on the one email address. Users can temporarily switch primary/secondary and switch them back if necessary.
        - If the customer responds that emails not in GitLab.com are employees no longer with the company, we can proceed. Items will be mapped to the admin account then the ghost user once the account is deleted.
    1. Also check that domain of email addresses belong to the company in the resulting list.
    1. Create a folder to unpack into: `mkdir project_export`
    1. Unpack the project into a folder: `tar -zxvf filename.tar.gz -C project_export`
    1. Navigate into the resulting folder using: `cd project_export`
    1. Rename the project.json file: `mv project.json project_old.json`
    1. Strip usernames using: `cat project_old.json | python -m json.tool | sed "s/\"username\": \"\([^\"]*\)\"/\"username\": \"dont_have_this_username\"/g" > project.json`
    1. Move out of the folder: `cd ..`
    1. Repack the folder to a `tar.gz` format: `tar -zcvf project-export-filename.tar.gz -C project_export .`
    1. Upload the resulting file to a secure temporary location and use the link to this file when filling in the import issue.
1. Assuming success, respond to the user that we have the export and will send an update when the import is complete.

### Request import

1. Fill in the `import` template on the [infra issue tracker](https://gitlab.com/gitlab-com/gl-infra/infrastructure/issues/new?issuable_template=import) with all available information.
    - If scheduling ahead of time, add date/time with timezone and post in Slack #production (no ping). Add export link later. Example message: "Hi team, got an import request scheduled for 2019-00-00 at 00:00 UTC. Appreciate if you could assign this to whomever is on-call at the time. LINK"
    - If not scheduling, use today's date and "at earliest convenience". Ping the on-call (check chatops) with the request. Example: "Hi @user, got an import request. Could you kick this off when you have a few minutes? LINK"
1. For _correctly mapped users_ only: Fill out an `access request` template on the [access-requests tracker](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=New%20Access%20Request) for admin level access to perform the import (see subsection for details).
1. Add infra issue link as internal note to the ZD ticket.
1. Delete any local copies of the export.
1. Imports may take a long time, so pass it on to the next region if necessary.
1. A message will be sent to #announcements channel on Slack when done. Close infra issue.
1. Ensure the export file is deleted (if applicable).
1. Let the user know the import is done and they should double check its completeness.
1. After customer confirms everything looks okay, if applicable, submit [account removal request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=Remove%20Access%20Request) to delete admin account.

#### Access request information

Use the `Free form request information` section (replace `group` with org or group name): 
```
Admin user access for customer import for infra's use with username: `group-import` 
Import request: INFRA-ISSUE-LINK
```

`Account Creation Information`: 
```
GitLab PRD | Role: `admin` | Rationale: `customer import`
```

Expiration timeframe: 
```
EXPIRES: `TRUE` | AFTER: `for the duration of project`
```