---
layout: markdown_page
title: "Releases"
---

## Resources

| Description        | Location            |
|--------------------|---------------------|
| Release orchestration | [Link](https://gitlab.com/gitlab-org/release-tools/) |
| Manual release management | [Link](https://gitlab.com/gitlab-com/chatops) |
| Deployment tool | [Link](https://gitlab.com/gitlab-com/gl-infra/deployer) |
| Patcher tool (Private) | [Link](https://ops.gitlab.net/gitlab-com/gl-infra/patcher) |
| Release documentation | [Link](https://gitlab.com/gitlab-org/release/docs) |
| Release related tasks issue tracker | [Link](https://gitlab.com/gitlab-org/release/tasks/) |
| Delivery team issue tracker | [Link](https://gitlab.com/gitlab-com/gl-infra/delivery/issues) |
| Creating patch release for self-managed release| [Youtube Video][creating patch release] |
| GitLab.com auto-deploy run through | [Youtube Video][auto-deploy] |

## Overview and terminology

* **Monthly self-managed release**: GitLab version (XX.YY.0) [published every month on the 22nd](https://gitlab.com/gitlab-org/release/docs/blob/master/general/monthly/process.md). From this monthly release, [patch](https://gitlab.com/gitlab-org/release/docs/blob/master/general/patch/process.md), [non-critical](https://gitlab.com/gitlab-org/release/docs/blob/master/general/security/process.md#non-critical-security-releases), and [critical](https://gitlab.com/gitlab-org/release/docs/blob/master/general/security/process.md#critical-security-releases) security releases are created as needed
* **GitLab.com releases**: [Auto-deploy releases](https://gitlab.com/gitlab-org/release/docs/blob/master/general/deploy/auto-deploy.md) that are deployed from [auto-deploy branches created from master][auto-deploy], on regular intervals

The `self-managed release` is a collection of many successfully deployed `auto-deploy`
releases on GitLab.com.

**The main priority** of both types of releases **[is GitLab availability & security](/handbook/engineering/#prioritizing-technical-decisions)**
as an application running on both GitLab.com and for customers running GitLab
in their own infrastructure.

With these two types of releases, GitLab Inc. has to balance _at the same time_
the workflows normally found in SaaS companies with the ones found in companies
that publish packaged software.

## GitLab.com releases

GitLab.com receives regular updates according to our [auto-deploy schedule](#gitlabcom-releases-1).
This means that GitLab.com **lives in the now** and [semver] versioning used by self-managed
installations does not apply to it.

For example, developers might be working in the `12.3` milestone on items that
will be a part of `12.3.0` release but GitLab.com will only "know" of the commit
SHA that the developer created.

Users on GitLab.com therefore receive features and bug fixes earlier than
users of self-managed installations.

## Self-managed releases

The `self-managed release` is a [semver] versioned package of features that
are already released on GitLab.com through `auto-deploys`.
This means that the official published version of GitLab is a **historical
snapshot** of items that are released to users on GitLab.com. As such,
the `self-managed release` is created from a _backport_ branch named by the
targeted semver version with a stable suffix, eg. `12-3-stable`.

Self-managed users receive features and bug fixes only after a new [semver]
version is created and published.

Our [maintenance policy] describes in detail the cadence of our major, minor and patch releases for self-managed users. The major release yearly cadence was defined [after an all stakeholder discussion](https://gitlab.com/gitlab-com/Product/issues/50).

## Timelines

The only guaranteed date throughout the release cycle is the 22nd. On this date,
the `self-managed release` will be published together with the release announcement.

**All other dates** are **a guideline only** and cannot be considered a deadline
when it comes to what will be included into any type of release. This includes the
[development month] and the dates defined there as well as any promises given to
customers. This is strictly because there are a lot of moving parts to be considered
when preparing a release which includes working on highest priority and severity
issues as well as security related issues.

Keep in mind that, if it is absolutely necessary to get a certain feature
ready for a specific version, merge the feature early in the development cycle.
Merges closer to the release date are absolutely not guaranteed to be included
in that specific monthly `self-managed release`.
For GitLab.com releases, timelines are different and described below.

### GitLab.com releases

In June 2019, GitLab.com transitioned to more frequent deploys through `auto-deploys`
as a first step towards continuous deployments. The [auto deploy transition] document
was created to serve as a transition overview document as we progress further
towards even more frequent deployments. As we transitioned, the timelines
for GitLab.com releases have changed and the current general process is
described below.

New auto-deploy branches are created twice a week, at the beginning (Sunday, depending on a timezone) and the middle (Wednesday, depending on the timezone) of the week.

Once a new branch is created, only commits that pass the CI tests are eligible for deployments ("green build"). This means that if specs are failing in
[gitlab-org/gitlab], the deployments cannot progress further.


Automated tasks in the [release-tools] project are setup to drive the next steps:

- Every hour, a task runs to cherry-pick merge requests labeled with `pick into auto-deploy` (See [Labels of importance]).
- Every hour, a task searches for the latest "green build" in the auto-deploy branch.
  - If it finds a commit that has not been previously deployed, it will start the process of creating a new package
  - If it the commit has already been deployed, the task will not take any actions.

When a new package is built, it is automatically deployed to `staging.gitlab.com`.
As part of the deployment to this environment, set of automated QA integration tests are ran.

When the automated QA test pass, the deployment automatically progresses to the
[canary] stage.

Automated deployments to **any production environment** (including [canary]), are
halted during the blackout period. Currently, the blackout period is:

* Between every Friday 23:00 UTC and Monday 07:00 UTC.
* 28th of November (US thanksgiving, limited availability company wide).
* 24th and 25th of December (Christmas according to Gregorian calendar, limited availability company wide).
* 1st of January (New Years day, limited availability company wide).

During the blackout period, manual deployment can be triggered through GitLab ChatOps if the deployment fixes **a P1/S1 availability or security issue**.

When the release reaches the [canary] stage and no new exceptions or alerts are
reported, release is considered to be ready for deployment to GitLab.com.

The promotion to the rest of the GitLab.com is triggered manually by the release
managers and this can happen at any point in time. Depending on the amount of
changes, this means that release managers can trigger a deployment to the rest
of the production fleet, shortly after [canary] stage is successfully completed.

Each deployment will trigger a notification in the Slack channel `[#announcements](https://gitlab.slack.com/archives/C8PKBH3M5)`.
After each successful deployment, QA issue is created in [release/tasks] issue tracker.
The purpose of these notifications are to inform the people who are involved in the
process that their change is going through environments. This allows them to
execute any manual testing or other tasks related to the release of their fix/feature.

### Self-managed releases

The `self-managed release` timelines are concentrated around the 22nd. One week
before the release date, the release managers will start preparing for the release
by ensuring that the GitLab.com releases are in a consistent state. This means
that what gets into the `self-managed release` fully depends on **the state of
GitLab.com releases**.

The `self-managed release` will only contain code that is successfully running
on GitLab.com at the time the release manager decides to finalise the release.

This can be as early as 5 work days or as late as 1 day before the 22nd.
This fluctuation comes from a possibility of 22nd being at or right after the weekend
or instability on GitLab.com in the run-up to the 22nd.
The release manager preparing the final release will post an announcement in [#releases](https://gitlab.slack.com/archives/C0XM5UU6B), [#development](https://gitlab.slack.com/archives/C02PF508L) and [#g_delivery](https://gitlab.slack.com/archives/CCFV016SV)
with a link to the final branch.

As mentioned earlier, if it is absolutely necessary to include a certain feature/fix
in that months `self-managed` release, merge it early in the development cycle or
no later than a couple of weeks before.
The same applies for items that need to go to the next
release; if it is absolutely necessary to include it in the next months release, merge
it after the `self-managed release` has been prepared.

Just because a merge request has a milestone of the current release `XX.YY` set,
does not mean that it will end up in the same release. Milestone describes
the target release, but only guarantee that it will be included in the same
release is if it is running on GitLab.com around the time release preparation starts.

## Labels of importance

For both types of releases, there are a few labels of specific importance.

### GitLab.com releases

For code that needs to be deployed to GitLab.com with higher priority than the
regular cadence, we have `~pick into auto-deploy` label.

The automated systems that create a new GitLab.com release will look for this label
specifically, and any merge request with this label will be automatically cherry-picked
into the active auto-deploy branch. In case the merge request cannot be picked,
which can happen if there is a conflict in the files being picked, the message
will be posted in the merge request asking the author to create a new merge request
targeting the currently active release branch.

The label should be only used under the following circumstances, when the merge
request:

- Fixes a P1/P2 and/or S1/S2 bug
- Resolves a regression that can lead to P1/P2 or S1/S2 problem
- Urgent performance or availability fix that can improve the stability of
GitLab.com

**For new features or non-urgent fixes**, the label **should not be used** because
the new release is only days or hours away.

Directions on how to how to know whether a MR is deployed to GitLab.com are in the [release/docs](https://gitlab.com/gitlab-org/release/docs/blob/master/general%2Fdeploy%2Fauto-deploy.md#auto-deploy-status).

### Self-managed releases

Similar to the above mentioned label, each `self managed release` has a label
to highlight that a certain merge request should be backported to the targeted
release. For example, releases in the 12.3 series will have `Pick into 12.3`
label which will signal that this merge request should be included in one of the
[next patch releases being created][creating patch release]. The patch releases are created as needed but only according to our [maintenance policy].

The label should be applied in the following situations:

- The backport (stable) branch has been created, the release on the 22nd is not created
and the merge request fixes a critical regression.
- The 22nd has passed and the merge request fixes a bug.

The label should not be applied to merge requests:

- Introducing new features
- Resolving a security vulnerability because process for security releases differs
from the regular release

[semver]: https://semver.org
[canary]: /handbook/engineering#canary-testing
[development month]: /handbook/engineering/workflow/#product-development-timeline
[auto deploy transition]: https://gitlab.com/gitlab-org/release/docs/blob/21cbd409dd5f157fe252f254f3e897f01908abe2/general/deploy/auto-deploy-transition.md#transition
[maintenance policy]: https://docs.gitlab.com/ee/policy/maintenance.html
[gitlab-org/gitlab]: https://gitlab.com/gitlab-org/gitlab
[release-tools]: https://gitlab.com/gitlab-org/release-tools
[release/tasks]: https://gitlab.com/gitlab-org/release/tasks/
[labels of importance]: #labels-of-importance
[creating patch release]: https://youtu.be/lHag9jARbIg
[auto-deploy]: https://www.youtube.com/watch?v=_G-EWRpCAz4
