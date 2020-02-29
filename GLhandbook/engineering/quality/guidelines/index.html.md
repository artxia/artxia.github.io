---
layout: handbook-page-toc
title: "Guidelines"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

Guidelines are high-level directives on how we carry out operations and solve challenges in the Quality Engineering department.

#### Child Pages
##### [Reliable tests](/handbook/engineering/quality/guidelines/reliable-tests/)
##### [Debugging QA Test Failures](/handbook/engineering/quality/guidelines/debugging-qa-test-failures/)
##### [Tips and Tricks](/handbook/engineering/quality/guidelines/tips-and-tricks/)

## Weights

We use Fibonacci Series for weights and limit the highest number to 8. The definitions are as below:

| Weight      | Description                                                                                                                                                                               |
|-------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 - Trivial | Simple and quick changes (e.g. typo fix, test tag update, trivial documentation additions)                                                                                                |
| 2 - Small   | Straight forward changes, no underlying dependencies needed. (e.g. new test that has existing factories or page objects)                                                                  |
| 3 - Medium  | Well understood changes with a few dependencies. Few surprises can be expected. (e.g. new test that needs to have new factories or page object / page components)                        |
| 5 - Large   | A task that will require some investigation and research, in addition to the above weights (e.g. Tests that need framework level changes which can impact other parts of the test suite)  |
| 8 - X-large | A very large task that will require much investigation and research. Pushing initiative level                                                                                             |
| 13 or more  | Please break the work down further, we do not use weights higher than 8.                                                                                                                  |

## Submitting and Reviewing code

For test automation changes, it is crucial that every change is reviewed by at least one Senior Test Automation Engineer in the Quality team.

We are currently setting best practices and standards for Page Objects and REST API clients. Thus the first priority is to have test automation related changes reviewed and approved by the team.
For test automation only changes, the quality team alone is adequate to review and merge the changes.

## Test Automation & Planning

* **Test plans as collaborative design document**: Test Plans as documented in [Test Engineering](/handbook/engineering/quality/test-engineering/) are design documents that aim to flush out optimal test coverage.
It is expected that engineers in every cross-functional team take part in test plan discussions.
* **E2E test automation is a collective effort**: Software Engineers in Test should not be the sole responsible party that automates the End-to-end tests.
The goal is to have engineers contribute and own coverage for their teams.
* **We own test infrastructure**: Test infrastructure is under our ownership, we develop and maintain it with an emphasis on ease of use, ease of debugging, and orchestration ability.
* `Future` **Disable feature by default until E2E test merged**: If a feature is to be merged without a QA test,
it **must** be behind a feature flag (disabled by default) until a QA test is written and merged as well.

## Test Failures

* **Fix failing test in `master` first**: [Failing tests on `master` are treated as the highest priority](/handbook/engineering/workflow/#broken-master).
* **Flaky tests are quarantined until proven stable**: A flaky test is as bad as no tests or in some cases worse due to the effort required to fix or even re-write the test.
As soon as detected it is quarantined immediately to stabilize CI, and then fixed as soon as possible, and monitored until it is fixed.
* **Close issue when the test is moved out of quarantine**: Quarantine issues should not be closed unless tests are moved out of quarantine.
* **Quarantine issues should be assigned and scheduled**: To ensure that someone is owning the issue, it should be assigned with a milestone set.
* **Make relevant stage group aware**: When a test fails no matter the reason, an issue should be created and made known to the relevant product stage group as soon as possible.
In addition to notifying that a test in their domain fails, enlist help from the group as necessary.
* **Failure due to bug**: If a test failure is a result of a bug, link the failure to the bug issue. It should be fixed as soon as possible.
* **Everyone can fix a test, the responsibility falls on the last who worked on it**: Anyone can fix a failing/flaky test, but to ensure that a quarantined test isn't ignored,
the last engineer who worked on the test is responsible for taking it out of [quarantine](https://gitlab.com/gitlab-org/gitlab/blob/master/qa/README.md#quarantined-tests).

### Debugging Test Failures

See [Debugging QA Pipeline Test Failures](/handbook/engineering/quality/guidelines/debugging-qa-test-failures/)

### Priorities

Test failure priorities are defined as follow:

* ~P1: Tests that are needed to verify fundamental GitLab functionality.
* ~P2: Tests that deal with external integrations which may take a longer time to debug and fix.

## Building as part of GitLab

* **GitLab features first**: Where possible we will implement the tools that we use as GitLab features.
* **Build vs buy**: If there is a sense of urgency around an area we may consider buying/subscribing to a service to solve our Quality challenges in a timely manner.
This is where building as part of GitLab is not immediately viable. An issue will be created to document the decision making process in our [team task](https://gitlab.com/gitlab-org/quality/team-tasks) issue tracker.
This shall follow our [dogfooding](/handbook/engineering#dogfooding) process.

## Quality Department pipeline triage rotation

This is a schedule to share the responsibility of debugging/analysing the failures
in the various scheduled pipelines that run on multiple environments.

Please refer to the [Debugging Failing tests](/handbook/engineering/quality/guidelines/debugging-qa-test-failures/)
guidelines for an exhaustive [list of scheduled pipelines](/handbook/engineering/quality/guidelines/debugging-qa-test-failures/#scheduled-qa-test-pipelines)
and for [specific instructions on how to do an appropriate level of investigation and determine next steps for the failing test](/handbook/engineering/quality/guidelines/debugging-qa-test-failures/#steps-for-debugging-qa-pipeline-test-failures).

### Responsibility

* During the scheduled dates, the support tasks related to the test runs become the Directly Responsible Individual's ([DRI](/handbook/people-group/directly-responsible-individuals/)'s) highest priority.
* Reporting and analyzing the End to End test failures in [Staging](https://ops.gitlab.net/gitlab-org/quality/staging/pipelines), [Canary](https://ops.gitlab.net/gitlab-org/quality/canary/pipelines) and [Production](https://ops.gitlab.net/gitlab-org/quality/production/pipelines) pipelines takes priority over [Nightly](https://gitlab.com/gitlab-org/quality/nightly/pipelines), MR, [GitLab `master`](https://gitlab.com/gitlab-org/gitlab/pipelines) or [GitLab FOSS `master`](https://gitlab.com/gitlab-org/gitlab-foss/pipelines) pipelines.
* If there is a time constraint, the DRI should report and analyze the failures in [Staging](https://ops.gitlab.net/gitlab-org/quality/staging/pipelines), [Canary](https://ops.gitlab.net/gitlab-org/quality/canary/pipelines) and [Production](https://ops.gitlab.net/gitlab-org/quality/production/pipelines) pipelines just enough to determine if it is an application or an infrastructure problem, and [escalate as appropriate](/handbook/engineering/development/processes/Infra-Dev-Escalation/process.html). All the reported failures in those pipelines should be treated as ~P1/~S1 until it's determined that they're not. That means they should be investigated ASAP, ideally within 2 hours of the report. If the DRI will not be able to do so, they should delegate any investigation they're unable to complete to the Secondary. If the Secondary is not available or will also not be able to complete the investigations, solicit help in the #quality slack channel.
* It is important that all other failure investigations are completed in a timely manner, ideally within 24 hours of the report. If the DRI is unable to investigate all the reported failures on [all the pipelines](/handbook/engineering/quality/guidelines/debugging-qa-test-failures/#scheduled-qa-test-pipelines) on time, they should delegate the remaining work to the Secondary. If the Secondary is not available, solicit help in the #quality slack channel.
* By the end of the schedule, the DRI should write a hand-off note specifying the highlights of that week and submit an issue in the [triage repository](https://gitlab.com/gitlab-org/quality/pipeline-triage/issues/new).

### Schedule

**January 2020 | February 2020 | March 2020 | April 2020 | May 2020 | June 2020**

| **Start Date** | **DRI**                                                     | **Secondary**                                               |
| -------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |
| 2019-01-06     | [Tomislav Nikić](/company/team/#asktomislav)                | [Rémy Coutable](/company/team/#rymai)                       |
| 2020-01-13     | [Rémy Coutable](/company/team/#rymai)                       | [Walmyr Lima e Silva Filho](/company/team/#walmyrlimaesilv) |
| 2020-01-20     | [Walmyr Lima e Silva Filho](/company/team/#walmyrlimaesilv) | [Grant Young](/company/team/#grantyoung)                    |
| 2020-01-27     | [Grant Young](/company/team/#grantyoung)                    | [Nailia Iskhakova](/company/team/#niskhakova)               |
| 2019-02-03     | [Nailia Iskhakova](/company/team/#niskhakova)               | [Mark Fletcher](/company/team/#markglenfletcher)            |
| 2020-02-10     | [Mark Fletcher](/company/team/#markglenfletcher)            | [Rémy Coutable](/company/team/#rymai)                  |
| 2020-02-17     | [Jennie Louie](/company/team/#jennielouie)                  | [Mark Lapierre](/company/team/#mdlap)                       |
| 2020-02-24     | [Mark Lapierre](/company/team/#mdlap)                       | [Zeff Morgan](/company/team/#zeffer)                        |
| 2020-03-02     | [Zeff Morgan](/company/team/#zeffer)                        | [Jen-Shin Lin](/company/team/#godfat)                       |
| 2020-03-09     | [Jen-Shin Lin](/company/team/#godfat)                       | [Mark Fletcher](/company/team/#markglenfletcher)             |
| 2020-03-16     | [Désirée Chevalier](/company/team/#dchevalier2)             | [Dan Davison](/company/team/#sircapsalot)                   |
| 2020-03-23     | [Dan Davison](/company/team/#sircapsalot)                   |                 |
| 2020-03-30     |                                                             | [Sanad Liaquat](/company/team/#sanadliaquat)                |
| 2020-04-06     | [Sanad Liaquat](/company/team/#sanadliaquat)                | [Albert Salim](/company/team/#caalberts)                     |
| 2020-04-13     | [Albert Salim](/company/team/#caalberts)                    | [Jen-Shin Lin](/company/team/#godfat)                |
| 2019-04-20     | [Tomislav Nikić](/company/team/#asktomislav)                | [Erick Banks](/company/team/#ebanks)                        |
| 2019-04-27     | [Erick Banks](/company/team/#ebanks)                        | [Walmyr Lima e Silva Filho](/company/team/#walmyrlimaesilv) |
| 2019-05-04     | [Walmyr Lima e Silva Filho](/company/team/#walmyrlimaesilv) | [Rémy Coutable](/company/team/#rymai)                       |
| 2019-05-11     | [Rémy Coutable](/company/team/#rymai)                       | [Tiffany Rea](/company/team/#treagitlab)                    |
| 2019-05-18     | [Tiffany Rea](/company/team/#treagitlab)                    | [Grant Young](/company/team/#grantyoung)                    |
| 2020-05-25     | [Grant Young](/company/team/#grantyoung)                    | [Sofia Vistas](/company/team/#svistas)                      |
| 2020-06-01     | [Sofia Vistas](/company/team/#svistas)                      | [Nailia Iskhakova](/company/team/#niskhakova)               |
| 2019-06-08     | [Nailia Iskhakova](/company/team/#niskhakova)               | [Mark Fletcher](/company/team/#markglenfletcher)            |
| 2020-06-15     | [Mark Fletcher](/company/team/#markglenfletcher)            | [Jennie Louie](/company/team/#jennielouie)                  |
| 2020-06-22     | [Jennie Louie](/company/team/#jennielouie)                  | [Mark Lapierre](/company/team/#mdlap)                       |
| 2020-06-29     | [Mark Lapierre](/company/team/#mdlap)                       | [Zeff Morgan](/company/team/#zeffer)                        |

### Responsibilities of the DRI and Secondary for scheduled pipelines
* The DRI does the [triage](/handbook/engineering/quality/guidelines/debugging-qa-test-failures/#steps-for-debugging-qa-pipeline-test-failures) and they let the counterpart TAE know of the failure.
* The DRI makes the call whether to fix or quarantine the test.
* The fix/quarantine MR should be reviewed by either the Secondary or the counterpart TAE (based on whoever is available). If both of them are not available immediately, then any other TAE can review the MR.  In any case, both the Secondary and the counterpart TAE are always CC-ed in all communications.
* The DRI should periodically take a look at [the list of unassigned quarantined issues](https://gitlab.com/gitlab-org/gitlab/issues?state=opened&label_name[]=QA&label_name[]=bug) and work on them.
* If the [DRI](/handbook/people-group/directly-responsible-individuals/) is not available during their scheduled dates (for more than 2 days), they can swap their schedule with another team member. If the DRI's unavailability during schedule is less than 2 days, the Secondary can help with the tasks.

### Responsibilities of the DRI and Secondary for deployment pipelines
* The DRI helps the delivery team debug test failures that are affecting the release process.
* The Secondary fills in when the DRI is not available.

### Engineering productivity team rotation and escalation

In order to provide better input during the planning phase of a release, the schedule will include a member of the Engineering Productivity team during the second week of the month.

* The Engineering Productivity team will use [#quality](https://gitlab.slack.com/archives/C3JJET4Q6) to signal assistance in triaging a failure.
* The Engineering Productivity team will cover the backup responsibility of the Secondary if the assigned EPE is not able to fulfill the responsibilities.
