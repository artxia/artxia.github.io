---
layout: handbook-page-toc
title: "Debugging Failing tests"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Overview

These guidelines are intended to help you to investigate failures in the [end-to-end tests](https://docs.gitlab.com/ee/development/testing_guide/end_to_end/index.html) so that they can be properly addressed.

This will involve analysing each failure and creating an issue to report it.

It might also involve [fixing tests](#fixing-the-test), putting them in [quarantine](#quarantining-tests), or [reporting bugs in the application](#bug-in-code).

The tests run on a scheduled basis, and their results are posted to Slack.

#### Scheduled QA test pipelines

The following are the QA test pipelines that are monitored every day.

| Environment | Tests type | Schedule | Slack channel |
| ----------- | ---------- | -------- | ------------- |
| [Production](https://ops.gitlab.net/gitlab-org/quality/production/pipelines) | Smoke | [Every 2 hours](https://ops.gitlab.net/gitlab-org/quality/production/pipeline_schedules/41/edit). | [`#qa-production`](https://gitlab.slack.com/messages/CCNNKFP8B) |
| [Canary](https://ops.gitlab.net/gitlab-org/quality/canary/pipelines) | Smoke | [Every 2 hours](https://ops.gitlab.net/gitlab-org/quality/canary/pipeline_schedules/37/edit), and [after each deployment to Canary](https://ops.gitlab.net/gitlab-com/gl-infra/deployer/pipelines). The bi-hourly schedule is useful to catch [failures introduced by a configuration change](https://gitlab.com/gitlab-org/quality/team-tasks/issues/244#note_251069010). | [`#qa-production`](https://gitlab.slack.com/messages/CCNNKFP8B) |
| [Staging](https://ops.gitlab.net/gitlab-org/quality/staging/pipelines) | Smoke | [Every 2 hours](https://ops.gitlab.net/gitlab-org/quality/staging/pipeline_schedules/38/edit), and [after each deployment to Staging](https://ops.gitlab.net/gitlab-com/gl-infra/deployer/pipelines). The bi-hourly schedule is useful to catch [failures introduced by a configuration change](https://gitlab.com/gitlab-org/quality/team-tasks/issues/244#note_251069010). | [`#qa-staging`](https://gitlab.slack.com/messages/CBS3YKMGD) |
| [Staging](https://ops.gitlab.net/gitlab-org/quality/staging/pipelines) | Full, Orchestrated | [After each deployment to Staging](https://ops.gitlab.net/gitlab-com/gl-infra/deployer/pipelines). | [`#qa-staging`](https://gitlab.slack.com/messages/CBS3YKMGD) |
| [Nightly packages](https://about.gitlab.com/handbook/engineering/development/enablement/distribution/maintenance/dev-gitlab-org.html#automated-tasks) | Full | [Daily at 4:00 am UTC](https://gitlab.com/gitlab-org/quality/nightly/pipeline_schedules/9530/edit). | [`#qa-nightly`](https://gitlab.slack.com/messages/CGLMP1G7M) |
| [GitLab `master`](https://gitlab.com/gitlab-org/gitlab/pipelines) | Full | When the `package-and-qa job` executes from a [scheduled pipeline every 2 hours](https://gitlab.com/gitlab-org/gitlab/pipeline_schedules/23503/edit). | [`#qa-master`](https://gitlab.slack.com/archives/CNV2N29DM) |
| [GitLab FOSS `master`](https://gitlab.com/gitlab-org/gitlab-foss/pipelines) | Full | When the `package-and-qa job` executes from a [scheduled pipeline every 2 hours](https://gitlab.com/gitlab-org/gitlab-foss/pipeline_schedules/23141/edit). | [`#qa-master`](https://gitlab.slack.com/archives/CNV2N29DM) |

For each pipeline there is a notification of success or failure (except for `master` pipelines, which only report failures).
If there's a failure, we use emoji to indicate the state of investigation of the failure:

- The :eyes: emoji, to show you're investigating a failing pipeline.
- The :boom: emoji, when there's a new failure.
- The :fire_engine: emoji, when a failure is already reported.
- The :retry: emoji, when there's a system failure (e.g., Docker or runner failure).

### Time to triage

* The [DRI](/handbook/people-group/directly-responsible-individuals/) should decide in the first 20 minutes of analysis, whether the failure can be fixed or it has to be quarantined.
* In any case, the counterpart TAE is kept informed about the issue.
* If the DRI finds that the issue can be fixed, they should spend not more than 2 hours in fixing the failure. Any test failure whose fix takes more than 2 hours, should be quarantined.
* Please refer to the [Quality Department pipeline triage rotation](/handbook/engineering/quality/guidelines/#quality-department-pipeline-triage-rotation) page to know who the current DRI is.

### Steps for debugging QA pipeline test failures

#### 1. Initial analysis

Start with a brief analysis of the failures. The aim of this step is to make a quick decision about how much time you can spend investigating in each failure.

In the relevant Slack channel:

1. Apply the :eyes: emoji to indicate that you're investigating the failure(s).
1. If there's a system failure (e.g., Docker or runner failure), retry the job and apply the :retry: emoji.
1. Look into the [QA failures board](https://gitlab.com/groups/gitlab-org/-/boards/1385578) to see if the failure is already reported or not.
1. If the failure is already reported, add a :fire_engine: emoji. It can be helpful if you reply to the failure notification with a link to the issue(s), but this isn't always necessary, especially if the failures are the same as in the previous pipeline and there are links there.

Your priority is to report all new failures, so if there are many failures we recommend that you identify whether each failure is old (i.e., there is an issue open for it), or new. For each new failure, open an issue that includes only the required information. Once you have opened an issue for each new failure you can investigate each more thoroughly and act on them appropriately, as described in later sections.

The reason for reporting all new failures first is that engineers may find the test failing in their own merge request, and if there is no open issue about that failure they will have to spend time trying to figure out if their changes caused it.

#### 2. Create an issue

1. Create an issue in [https://gitlab.com/gitlab-org/gitlab/issues](https://gitlab.com/gitlab-org/gitlab/issues)
using the [QA failure](https://gitlab.com/gitlab-org/gitlab/issues/new?issuable_template=QA%20failure) template.
1. In the relevant Slack channel, add the :boom: emoji and reply to the failure notification with a link to the issue.

#### 3. Investigate the failure further

The aim of this step is to understand the failure. The results of the investigation will also let you know what to do about the failure.

The following points can help with your investigation:

- Understand the intent of the test. Manually performing the test steps can help.
- Stack trace: The stack trace shown in the job's log is the starting point for investigating the test failure.
- Screenshots and HTML captures: These are available for download in the job's artifact for up to 1 week after the job run.
- QA Logs: These are also included in the job's artifact and are valuable for determining the steps taken by the tests before failing.
- Sentry logs for Staging: If staging tests fail due to a server error, there should be a record in [Sentry](https://sentry.gitlab.net).
You can search for all unresolved staging errors linked to the `gitlab-qa` user with the query [`is:unresolved user:"username:gitlab-qa"`](https://sentry.gitlab.net/gitlab/staginggitlabcom/?query=is%3Aunresolved+user%3A%22username%3Agitlab-qa%22). However, note that some actions aren't linked to the `gitlab-qa` user, so they might only appear in the [full unresolved list](https://sentry.gitlab.net/gitlab/staginggitlabcom/?query=is%3Aunresolved).
- Kibana logs for Staging: Various application logs are sent to [Kibana](https://nonprod-log.gitlab.net/app/kibana#/discover), including Rails, Postgres, Sidekiq, and Gitaly logs.
- Reproducing the failure locally:
  - You can try running the test against your local GitLab instance to see if the failure is reproducible. E.g.:

  `CHROME_HEADLESS=false bundle exec bin/qa Test::Instance::All http://localhost:3000 qa/specs/features/browser_ui/1_manage/project/create_project_spec.rb`
  - Use the environment variable `QA_DEBUG=true` to enable logging output including page actions and Git commands.
  - You can also use the same docker image (same sha256 hash) as the one used in the failing job to run GitLab in a container on your local.
  In the logs of the failing job, search for `Downloaded newer image for gitlab/gitlab-ce:nightly` or `Downloaded newer image for gitlab/gitlab-ee:nightly`
  and use the sha256 hash just above that line.
  To run GitLab in a container on your local, the docker command similar to the one shown in the logs can be used. E.g.:

  `docker run --publish 80:80 --name gitlab --net test --hostname localhost gitlab/gitlab-ce:nightly@sha256:<hash>`
  - You can now run the test against this docker instance. E.g.:

  `CHROME_HEADLESS=false bundle exec bin/qa Test::Instance::All http://localhost qa/specs/features/browser_ui/1_manage/project/create_project_spec.rb`
  - Additional information about running tests locally can be found in the [QA readme](https://gitlab.com/gitlab-org/gitlab/tree/master/qa#running-specific-tests).

- Determine if the test is [flaky](https://docs.gitlab.com/ee/development/testing_guide/flaky_tests.html#whats-a-flaky-test): check the logs or run the test a few times. If it passes at least once but fails otherwise, it's flaky.

##### Checking Docker image

Sometimes tests may fail due to an outdated Docker image. To check if that's the case, follow the below instructions to see if some merged code is available or not in a Docker image.

##### Checking test code

If you suspect that certain test is failing due to the `gitlab/gitlab-{ce|ee}-qa` image being outdated, follow the below steps:

1. Locally, run `docker run -it --entrypoint /bin/sh gitlab/gitlab-ce-qa:latest` to check for GitLab QA CE code, or `docker run -it --entrypoint /bin/sh gitlab/gitlab-ee-qa:latest` to check for GitLab QA EE code
2. Then, navigate to the `qa` directory (`cd /home/qa/qa`)
3. Finally, use `cat` to see if the code you're looking for is available or not in certain file (e.g., `cat page/project/issue/show.rb`)

> Note: if you need to check in another tag (e.g., `nightly`), change it in one of the scripts of step 1 above.

##### Checking application code

1. Locally, run `docker run -it --entrypoint /bin/sh gitlab/gitlab-ce:latest` to check for GitLab CE code, or `docker run -it --entrypoint /bin/sh gitlab/gitlab-ee:latest` to check for GitLab EE code
2. Then, navigate to the `gitlab-rails` directory (`cd /opt/gitlab/embedded/service/gitlab-rails/`)
3. Finally, use `cat` to see if the code you're looking for is available or not in certain file (e.g., `cat public/assets/issues_analytics/components/issues_analytics-9c3887211ed5aa599c9eea63836486d04605f5dfdd76c49f9b05cc24b103f78a.vue`.)

> Note: if you want to check another tag (e.g., `nightly`) change it in one of the scripts of step 1 above.

#### 4. Classify and triage the failure

The aim of this step is to categorise the failure as either a stale test, a bug in the test, a bug in the application code, or a flaky test.

##### Test is stale due to an application change
{:.no_toc}

In this case, you've found that the failure was caused by some change in the application code and the test needs to be updated. You should:

- Include your findings in a note in the issue about the failure.
- Apply the ~"failure::stale-test" label.
- If possible, mention the merge request which caused the test to break, to keep the corresponding engineer informed.

##### Bug in test
{:.no_toc}

In this case, you've found that the failure was caused by a bug in the test itself, not in the application code. You should:

- Include your findings in a note in the issue about the failure.
- Apply the ~"failure::broken-test" label.

##### Bug in application code
{:.no_toc}

In the case you've found that a failure was caused by a bug in the application code:

- Include your findings in a note in the issue about the failure.
- If there is an issue open already for the bug, mention the test failure in the issue with all the details, cc-ing the corresponding Software Engineer in Test (SET) and Quality Engineering Manager (QEM).
- If there is no issue open for the bug, create an issue mentioning the failure details, cc-ing the corresponding Engineering Managers (EM), QEM, and SET.
- Communicate the issue in the corresponding Slack channels.
- Do *not* [quarantine](#quarantining-tests) the test immediately unless the bug won't be fixed quickly (e.g. if it is a minor/superficial bug). Instead, leave a comment in the issue for the bug asking if the bug can be fixed in the current release. If if can't, quarantine the test.
- When the reason for quarantining a test is because of a low severity bug in the code which will not be fixed in the upcoming couple of releases, add `type: :bug` in the `quarantine` tag.

To find the appropriate team member to cc, please refer to the [Organizational Chart](/company/team/org-chart/). The [Quality Engineering team list](/handbook/engineering/quality/#quality-engineering-teams) and [DevOps stage group list](/handbook/product/categories/#devops-stages) might also be helpful.

**Example**

```ruby
it 'is quarantined', quarantine: { issue: 'https://gitlab.com/gitlab-org/gitlab/issues/<issue_id>', type: :bug }
```

##### Flaky Test
{:.no_toc}

In this case, you've found that the failure is due to flakiness in the test itself:

- Include your findings in a note in the issue about the failure.
- Apply the ~"failure::flaky-test" label.
- [Quarantine](#quarantining-tests) the test and refer the issue to the concerned member of the [Quality Engineering team](/handbook/engineering/quality/#quality-engineering-teams).

**Example**

```ruby
it 'is quarantined', quarantine: 'https://gitlab.com/gitlab-org/gitlab/issues/<issue_id>'
```

### Following up on failures

#### Fixing the test

If you've found that the test is the cause of the failure (either because the application code was changed or there's a bug in the test itself), it will need to be fixed. This might be done by another SET or by yourself. However, it should be fixed as soon as possible. In any case, the steps to follow are as follows:

- Create a merge request (MR) with the fix for the test failure.
- Apply the ~"Pick into auto-deploy" and ~P1 labels.

If the test was flaky:

- Confirm that the test is stable by ensuring it passes 3 to 5 times while in quarantine.

*Note: the number of passes needed to be sure a test is stable is just a suggestion. You can use your judgement to pick a different threshold.*

If the test was in quarantine, [remove it from quarantine](#dequarantining-tests).

#### Quarantining Tests

We should be very strict about quarantining tests. Quarantining a test is very costly and poses a higher risk because it allows tests to fail without blocking the pipeline, which could mean we miss new failures. The aim of quarantining the tests is *not* to get back a green pipeline, but rather to reduce the noise (due to constantly failing tests, flaky tests, etc.) so that new failures are not missed. Hence, a test should be quarantined only under the following circumstances:

- There is a bug in the application code or in the test that won't be fixed in the current release.
- The test is flaky or failing for an unknown reason and requires further investigation.

Following are the steps to quarantine a test:

- Open a merge request.
- Assign the `quarantine: '<issue_link>'` metadata to the test with a link to the issue.
  - If the example has a `before` hook, the `:quarantine` meta should be assigned to the outer context to avoid running the `before` hook.
- The merge request **should** have the following labels:
  - ~"Quality", ~"QA", ~"bug", ~"Pick into auto-deploy" (you can use the following quick action in the MR description: `/label ~"Quality" ~"QA" ~"bug" ~"Pick into auto-deploy"`)
- The merge request **can** have the following labels:
  - a DevOps stage label ( ~"devops::create", ~"devops::manage", etc.)
  - ~"failure::flaky-test" if you know for sure the failure is due to flakiness
- The merge request **should** have the current milestone

To be sure that the test is quarantined quickly, ask in the `#quality` Slack channel for someone to review and merge the merge request, rather than assigning it directly.

Here is an [example quarantine merge request](https://gitlab.com/gitlab-org/gitlab/merge_requests/23334/diffs).

#### Dequarantining Tests

Failing to dequarantine tests periodically reduces the effectiveness of the test suite. Hence, the tests should be dequarantined on or before the due-date mentioned in the corresponding issue.

Before dequarantining a test:

- If the test failure was originally discovered in [nightly](https://gitlab.com/gitlab-org/quality/nightly/pipelines), MR or [master](https://gitlab.com/gitlab-org/gitlab/pipelines) pipeline, please make sure that the test passes on your local against GDK with latest code and that it has passed a few times
in the nightly pipeline's quarantine job for that test.
- If the test failure was originally discovered in [staging](https://ops.gitlab.net/gitlab-org/quality/staging/pipelines), [canary](https://ops.gitlab.net/gitlab-org/quality/canary/pipelines) or [production](https://ops.gitlab.net/gitlab-org/quality/production/pipelines) pipeline, please make sure that the test passes in the CI pipeline against that environment.
You can trigger a CI pipeline against a live environment by clicking "Run Pipeline" button on the [staging](https://ops.gitlab.net/gitlab-org/quality/staging/pipelines), [canary](https://ops.gitlab.net/gitlab-org/quality/canary/pipelines) or [production](https://ops.gitlab.net/gitlab-org/quality/production/pipelines) pipelines page
and setting the `RELEASE` variable to the release that has your changes. See [Running Gitlab-QA pipeline against a specific GitLab release](https://about.gitlab.com/handbook/engineering/quality/guidelines/tips-and-tricks/#running-gitlab-qa-pipeline-against-a-specific-gitlab-release)
for instruction on finding your release version created and tagged by the Omnibus pipeline.

To dequarantine a test:

- Create a merge request that removes the `:quarantine` tag.
- Close the issue created as part of the quarantining process.

As with quarantining a test, you can ask in the `#quality` Slack channel for someone to review and merge the merge request, rather than assigning it.

#### Re-evaluating tests

If the due date of a failing test issue is reached, you should re-evaluate if the failing test should really be covered at the end-to-end test level, or if it should be covered in a lower level of the [testing levels pyramid](https://docs.gitlab.com/ee/development/testing_guide/testing_levels.html).

If you decide to delete the test, open a merge request to delete it and close the test failure issue. In the MR description or comment, mention the stable counterpart TAE for the test's stage for their awareness. Then open a new issue to cover the test scenario in a different test level.

If you decide the test is still valuable but don't want to leave it quarantined, you could replace `:quarantine` with `:skip`, which will skip the test entirely (i.e., it won't run even in jobs for quarantined tests). That can be useful when you know the test will continue to fail for some time (e.g., at least the next milestone or two).

### Training Videos

Two videos walking through the triage process were recorded and uploaded to the [GitLab Unfilitered](https://www.youtube.com/channel/UCMtZ0sc1HHNtGGWZFDRTh5A) YouTube channel.
  - [Quality Team: Failure Triage Training - Part 1](https://www.youtube.com/watch?v=Fx1DeWoTG4M)
    - Covers the basics of investigating pipeline failures locally.
  - [Quality Team: Failure Triage Training - Part 2](https://www.youtube.com/watch?v=WeQb8GEw6PM)
    - Continued discussion with a focus on using Docker containers that were used in the pipeline that failed.
