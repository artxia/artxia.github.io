---
layout: markdown_page
title: "People Ops Engineering"
---
## On this page
{:.no_toc}

- TOC
{:toc}

## Overview

As GitLab continues to scale, our need for tools and automation to manage our growth expands
along with it. To help, People Ops has a dedicated engineering team to make our team more efficient and
improve the effectiveness of core People Ops responsibilities like recruiting and [onboarding](https://about.gitlab.com/handbook/general-onboarding/onboarding-processes/).

### Working with us

If you'd like to request engineering assistance with an issue related to People Ops processes
or tools ([like BambooHR](https://about.gitlab.com/handbook/people-group/#using-bamboohr)), please start by
[creating an issue](https://gitlab.com/gitlab-com/people-group/people-operations-engineering/issues/new) in the People Ops Engineering project.

### Our workflow

The [People Ops Engineering board](https://gitlab.com/gitlab-com/people-group/people-operations-engineering/-/boards/1312849)
serves as the single source of truth on the engineering team's priorities. Issues follow a linear sequence, with a `Workflow::`
label indicating an issue's current status:

1. `Workflow::Triage`: Issues start here. Issues in triage must be further defined before they're able to
be made ready for development. Once the problem and a proposal for solving it is defined to the point where an
engineer can begin work, it can be moved to `Workflow::Ready for Development`.
* `Workflow::Waiting`: Issues that are waiting from input from someone or are waiting on a dependency. These are
blocked issues that need input or progress from others before they can progress.
2. `Workflow::Ready for Development`: Issues that are groomed and are ready for an engineer to begin work. They're
well defined in terms of the problem, and have a proposal that's defined enough for us to begin work; not every detail
needs to have been defined, but an engineer should be able to start work on this issue by reading the issue description alone.
   * Engineers beginning work on a ready for development issue should assign the issue to themselves and move it to `Workflow::In Progress`.
3. `Workflow::In Progress`: Issues that are actively being worked on by a developer.
4. `Workflow::Verification`: Issues that have engineering work complete and ready for evaluation. At this point, the developed solution
should be evaluated (by the issue reporter or another stakeholder) to verify that it solves the original problem.
   * Once signed off, the issue can be closed.

## Current systems

### Source of truth

For all automations mentioned in this page, BambooHR database acts as the single
souce of truth. We make use of a [fork](https://gitlab.com/gitlab-com/people-ops/bamboozled/)
from the [Bamboozled](https://github.com/Skookum/bamboozled) Ruby gem, and interact
with BambooHR using an bot user with limited access to employee details.

#### Data confidentiality

The bot user used for automations has read-only access to the following employee
details. We actively ensure that no extremely confidential information is accessible
through this bot user.

TODO: Add list of fields accessible by the bot.

### Partially automated processes

#### Onboarding issue creation

PeopleOps specialists make use of GitLab's
[ChatOps](https://docs.gitlab.com/ee/ci/chatops/) functionality to automate
creation of onboarding issues that contain onboarding tasks relevant to the
incoming team member. The Slack command used for this is:

```
/pops run onboarding <id_in_BambooHR_URL>
```

The Slack command triggers a pipeline in the `employment` project, which will
run the job `onboarding`, and reply with a link to the newly created onboarding
issue. The onboarding issue will be automatically assigned to the PeopleOps
Specialist who ran the command and the incoming team member's Manager.

The onboarding tasks that are applicable to all team members are listed in the
general [`onboarding.md`](https://gitlab.com/gitlab-com/people-ops/employment/blob/master/.gitlab/issue_templates/onboarding.md)
file. It will be included by default in the onboarding issue.

The job then grabs various details of the incoming team member, like country of
residence, entity through which they are hired, division, department, job title
etc. For each of these details, it checks for the existence of a task file in
the [`onboarding_tasks` folder](https://gitlab.com/gitlab-com/people-ops/employment/blob/master/.gitlab/issue_templates/onboarding.md)
of the `employment` project. These tasks files are of the format
`country_<country name>.md`, `entity_<entity name>.md`, `division_<division name>.md`,
`department_<department name>.md`, etc. If such a file is found, it includes
contents of those files also in the onboarding issue.

`Note:` Due to some technical difficulties, the onboarding issue created by the
command will contain onboarding tasks applicable to other job families at
GitLab. PeopleOps specialists will have to manually delete all of them except
the one applicable to the incoming team member. An issue to improve
this can be found [here](https://gitlab.com/gitlab-com/people-ops/people-operations-engineering/issues/5).

##### Interns
If you want to create the onboarding issue for interns, you can use the same Slack command. The biggest difference is that it will read from a different template. The template is determined by the division: `onboarding_intern_<division>.md`. Currently there's only one division that has set up a template:

- [Engineering](https://gitlab.com/gitlab-com/people-group/employment/-/blob/master/.gitlab/issue_templates/onboarding_intern_engineering.md)

This is a first iteration of creating onboarding issues for interns, we can move to a similar method as we do for the "regular" onboardings.

#### Offboarding issue creation

PeopleOps specialists make use of GitLab's
[ChatOps](https://docs.gitlab.com/ee/ci/chatops/) functionality to automate
creation of offboarding issues that contain offboarding tasks relevant to the
incoming team member. The Slack command used for this is:

```
/pops run offboarding <id_in_BambooHR_URL>
```

The Slack command triggers a pipeline in the `employment` project, which will
run the job `offboarding`, and reply with a link to the newly created offboarding
issue. The offboarding issue will be automatically assigned to the PeopleOps
Specialist who ran the command and the outgoing team member's Manager.

The job then grabs various details of the outgoing team member, like country of
residence, entity through which they are hired, division, department, job title
etc. For each of these details, it checks for the existence of a task file in
the [`offboarding_tasks` folder](https://gitlab.com/gitlab-com/people-ops/employment/blob/master/.gitlab/issue_templates/offboarding.md)
of the `employment` project. These tasks files are of the format
`country_<country name>.md`, `entity_<entity name>.md`, `division_<division name>.md`,
`department_<department name>.md`, etc. If such a file is found, it includes
contents of those files also in the offboarding issue.

`Note:` Due to some technical difficulties, the offboarding issue created by the
command will contain offboarding tasks applicable to other job families at
GitLab. PeopleOps specialists will have to manually delete all of them except
the one applicable to the outgoing team member. An MR with a suggestion to improve
this can be found [here](https://gitlab.com/gitlab-com/people-group/employment/merge_requests/960).

### Fully automated processes

PeopleOps make use of GitLab's [scheduled pipelines] features to automate Slack announcements
related to team member events like hiring and anniversaries. These are configured in the
[`employment`](https://gitlab.com/gitlab-com/people-group/employment/pipeline_schedules)
project.

A Slack bot named `PeopleOps Bot` is configured to post these announcements to
relevant Slack channels.

#### Anniversary announcements

A scheduled pipeline is configured to automatically send a message
congratulating all team members celebrating a work anniversary that week to the
Slack channel `#team-member-updates`. The message will contain list of all such
team members and the number of years they are celebrating at GitLab.

Currently, the pipeline is scheduled to be run at 10:00 AM UTC on every
Thursday.

#### New hire announcements

A scheduled pipeline is configured to automatically send a message containing a
list of all new team members who are joining GitLab in the following week. It
includes details like name, email address, joining date, and their job title.
The message also includes a link to a [Sisense chart](https://app.periscopedata.com/app/gitlab/503779) containing a
detailed breakdown and overview of the hiring process over time.

For the time being, this message is sent to the Slack channel
`#peopleops-alerts`, and is manually copy-pasted to `#team-member-updates` by a
PeopleOps specialist after manual verification of the details. Once the
onboarding process is streamlined enough, this manual work could be removed and
the bot could directly post to `#team-member-updates`.

Currently, the pipeline is scheduled to be run at 04:00 PM UTC on every
Thursday.

#### Informing PeopleOps Specialists about details missing in BambooHR for upcoming new hires

For the new hire announcements to be accurate, it is required to ensure the
BambooHR details of team members joining the following week is as complete as
possible. To help PeopleOps team in this task, another scheduled pipeline is
run to verify if the BambooHR details of all incoming team members is complete.
This pipeline notifies PeopleOps specialists in `#peopleops-alerts` channel
about people whose details are missing and the details that are missing for each
person.

Since PeopleOps Specialists should have enough time to fix these missing
details before new hire announcements are sent, it is necessary this job should
be run an adequate amount of time before the new hire announcements job is run.
Currently, the pipeline is scheduled to be run at 02:00 PM on every Wednesday.

#### Closing outdated onboarding issues

It is expected that onboarding issues be completed and closed within 30 days of
opening. To remind team members about this, we are using the `due date`
functionality in GitLab issues. When an onboarding issue is created, we
automatically set a due date of 35 days to it (we open onboarding issues the
week before the team member joins, so 35 days gives them almost
30 days to complete onboarding tasks after they actually start at GitLab).
GitLab will send a reminder notification email to all the assignees of the issue
near the due date.

In addition to this due date, team members get an additional 30 days to complete
and close the onboarding issue. In total, a team member gets around 60 days
to complete their onboarding issue.

We have another scheduled pipeline to close the outdated issues (issues that
have been open for more than 60 days). This pipeline will add a comment on the
issue that it is being automatically closed and what the team members should do
if they have onboarding tasks remaining.

Currently, the pipeline is scheduled to be run at 09:30 PM on every Friday. It
will close all the onboarding issues created before 60 days from that date.
