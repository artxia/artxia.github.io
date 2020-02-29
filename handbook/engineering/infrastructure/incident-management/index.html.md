---
layout: handbook-page-toc
title: "Incident Management"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Incidents

Incidents are **anomalous conditions** that result in&mdash;or may lead
to&mdash;service degradation or outages. These events require human
intervention to avert disruptions or restore service to operational status.
Incidents are _always_ given immediate attention.

### Is GitLab.com Experiencing an Incident?

If you're observing issues on GitLab.com or working with users who are
reporting issues, please follow the instructions found on the
[On-Call](/handbook/on-call/) page and alert the Engineer On Call (EOC).

If any of the dashboards below are showing major error rates or deviations,
it's best to alert the Engineer On Call.

#### Critical Dashboards

1. What alerts are going off? [AlertManager](https://alerts.gprd.gitlab.net/)
1. How does do these dashboards look?
   1. [Triage dashboard](https://dashboards.gitlab.net/d/RZmbBr7mk/gitlab-triage?orgId=1&refresh=30s)
   1. [General Triage dashboard](https://dashboards.gitlab.net/d/general-triage/platform-triage?orgId=1)
      1. What services are showing availability issues?
      1. What services are saturated?

## Incident Management

The goal of incident management is to organize chaos into swift incident
resolution. To that end, incident management provides:

1. well-defined [roles and responsibilities](#roles-and-responsibilities) for members of the incident team,
1. control points to manage the flow **information** and the **resolution path**,
1. a **root-cause analysis** (RCA),
1. and a post-incident review that assigns a **severity** classification after assessing the impact and scope of the incident.

### Ownership

There is only ever **one** owner of an incident&mdash;and only the owner of
the incident can declare an incident resolved. At anytime the incident owner
can engage the next role in the hierarchy for support. With the exception of
when GitLab.com is not functioning correctly, the incident issue should
be assigned to the current owner.

### Roles and Responsibilities

It's important to clearly delineate responsibilities during an incident.
Quick resolution requires focus and a clear hierarchy for delegation of
tasks. Preventing overlaps and ensuring a proper order of operations is vital
to mitigation. The responsibilities outlined in the roles below are
cascading–**and ownership of the incident passes from one role to the next as
those roles are engaged**. Until the next role in the hierarchy engages, the
previous role assumes all of the subsequent roles' responsibilities and
retains ownership of the incident.

| **Role** | **Description** |
| -------- | ------------------------|
| `EOC`    | **Engineer On Call** |
|          | The Production **Engineer On Call** is generally an SRE and can declare an incident. If another party has declared an incident, once the EOC is engaged they own the incident. The EOC gathers information, performs an initial assessment, and determines the [incident severity](#incident-severity) level. |
| `IMOC`   | **Incident Manager On Call** |
|          | The **Incident Manager** is generally a Reliability Engineering manager and is engaged when incident resolution requires coordination from multiple parties. The IMOC is the tactical leader of the incident response team&mdash;not a person performing technical work. The IMOC assembles the incident team by engaging individuals with the skills and information required to resolve the incident. |
| `CMOC`   | **Communications Manager On Call** |
|          | The **Communications Manager** is generally a Reliability Engineering manager. The CMOC disseminates information internally to stakeholders and externally to customers across multiple media (e.g. GitLab issues, Twitter, status.gitlab.com, etc.). |

These definitions imply several on-call rotations for the different roles.

#### Engineer on Call (EOC) Responsibilities

1. **As EOC, your highest priority for the duration of your shift is the stability of GitLab.com.**
1. The Single Source of Truth (SSOT) for who is EOC is the the [SRE Schedule in Pagerduty](https://gitlab.pagerduty.com/schedules#P05EL5A). The chatops bot in the [`#production` Slack Channel](https://gitlab.slack.com/archives/production) will tell you this with `/chatops run oncall prod`.
1. Alerts that are routed to Pagerduty need to acknowledged within 15 minutes, otherwise they will be escalated to the oncall IMOC.
   1. Alert-manager alerts in [`#alerts`](https://gitlab.slack.com/archives/alerts) and [`#alerts-general`](https://gitlab.slack.com/archives/alerts-general) are an important source of information about the health of the environment and should be monitored during working hours.
   1. If the Pagerduty alert noise is too high, your task as an EOC is clearing out that noise by either fixing the system or changing the alert.
   1. If you are changing the alert, it is your responsibility to explain the reasons behind it and inform the next EOC that the change occurred.
   1. Each event (may be multiple related pages) should result in an issue in the `production` tracker.  See [production queue usage](/handbook/engineering/infrastructure/production/#implementation) for more details.
1. If sources outside of our alerting are reporting a problem, and you have not received any alerts, it is still your responsibility to investigate. [Declare a low severity incident](#declaring-an-incident) and investigate from there.
   1. Low severity ([S3/S4](/handbook/engineering/infrastructure/production/#severity)) incidents (and issues) are cheap, and will allow others a means to communicate their experience if they are also experiencing the issue.
   1. **"No alerts" is not the same as "no problem"**
1. GitLab.com is a complex system. It is ok to not fully understand the underlying issue or its causes. However, if this is the case, as EOC you should engage with the IMOC to find a team member with the appropriate expertise.
   1. Requesting assistance does not mean relinquishing EOC responsibility. The EOC is still responsible for the incident.
   1. The [GitLab Organizational Chart](/company/team/org-chart/) and the [GitLab Team Page](/company/team/), which lists areas of expertise for team members, are important tools for finding the right people.
1. As soon as an [S1/S2](/handbook/engineering/infrastructure/production/#severity) [incident is declared](#declaring-an-incident), join the `The Situation Room Permanent Zoom`. The Zoom link is in the `#incident-management` topic.
   1. GitLab works in an asynchronous manner, but incidents require a synchronous response. Our collective goal is high availability of 99.95% and beyond, which means that the timescales over which communication needs to occur during an incident is measured in seconds and minutes, not hours.
1. Keep in mind that a GitLab.com incident is not an "infrastructure problem". It is a company-wide issue, and as EOC, you are leading the response on behalf of the company.
   1. If you need information or assistance, engage with Engineering teams. If you do not get the response you require within a reasonable period, escalate through the IMOC.
   1.  As EOC, require that those who may be able to assist to join the Zoom call and ask them to post their findings in the incident issue or active incident Google doc. Debugging information in Slack will be lost and this should be strongly discouraged.

1. By acknowledging an incident in Pagerduty, the EOC is implying that they are working on it. To further reinforce this acknowledgement, post a note in Slack that you are joining the `The Situation Room Permanent Zoom` as soon as possible.
   1.  If the EOC believes the alert is incorrect, comment on the thread in `#production`. If the alert is flappy, create an issue and post a link in the thread. This issue might end up being a part of RCA or end up requiring a change in the alert rule.
1. _Be inquisitive_. _Be vigilant_. If you notice that something doesn't seem right, investigate further.
2. After the incident is resolved, the EOC should start on performing an [incident review](#incident-review) (RCA) and [assign themselves](#incident-review-issue-creation-and-ownership) as the initial owner. Feel free to take a breather first, but do not end your work day without starting the RCA.

#### Incident Manager on Call (IMOC) Responsibilities

1. The SSOT for who is IMOC is the the [SRE Managers Schedule in Pagerduty](https://gitlab.pagerduty.com/schedules/PQEEYGD)
1. The IMOC should monitor ongoing incidents and engage with the incident if it escalates to a user-impacting (S1 or S2) incident.
1. The IMOC should engage if requested by the EOC.
1. The time that the IMOC engages should be recorded in the incident issue by the IMOC co-assigning themselves to the issue. If GitLab.com is down, record the time in the Google working doc.
1. For non-critical issues, or critical (S1, S2) issues with a short duration, the IMOC will also take on the role of CMOC.
1. The IMOC should ensure that the appropriate team members from other teams engage within an appropriate amount of time.
   1. During a user-impacting incident, the appropriate time response time is minutes.
   1. If the IMOC is unable to obtain a response through Slack channels, they should escalate to a manager or director to obtain assistance.
1. They evaluate information provided by team members, lend technical direction, and coordinate troubleshooting efforts.
1. If applicable, coordinate the incident response with [business contingency activities](/handbook/business-ops/gitlab-business-continuity-plan.html).
1. After the incident is resolved, the IMOC is responsible for conducting the [post-incident review](#post-incident-review).

To page the Incident Manager on call you can:

1. Run a [response play](https://about.gitlab.com/handbook/on-call/#site-reliability-engineers-sres)
1. Type `/pd trigger` in the `#production` channel

#### Communications Manager on Call (CMOC) Responsibilities

1. For serious incidents that require coordinated communications across multiple channels, the IMOC will select an CMOC for the duration of the incident.
1. The CMOC is responsible for updating internal parties, executive-level managers, and users.
1. The CMOC is responsible for contacting the Community Advocates Team via the [#community-advocates](https://gitlab.slack.com/messages/community-advocates) Slack channel, mentioning them with the `@advocates` Slack handle. 
1. Once Community Advocates have been notified, an update to the [GitLab Status](https://twitter.com/gitlabstatus) Twitter handle will be made.   
1. During a critical S1-level incident, the CMOC should aim to update the [GitLab Status](https://twitter.com/gitlabstatus) about every 15 minutes.
1. Updates and the status of gitlab.com are shared by the [GitLab Status](https://twitter.com/gitlabstatus) Twitter handle, not the company handle [GitLab](https://twitter.com/gitlab).
1. The [social marketing team](/handbook/marketing/corporate-marketing/social-marketing/) can assist in major crises if there is not a Community Advocate available online; this should not occur often. Please alert the social team by using `@social` in your Slack Message if necessary.
1. During a critical S1-level incident, the CMOC should aim to update the [GitLab Status](https://twitter.com/gitlabstatus) about every 15 minutes.

### Runbooks

[Runbooks](https://gitlab.com/gitlab-com/runbooks) are available for
engineers on call. The project README contains links to checklists for each
of the above roles.

**In the event of a GitLab.com outage**, a mirror of the runbooks repository is available on at https://ops.gitlab.net/gitlab-com/runbooks.

### Declaring an Incident

The following steps can be automated in Slack by typing `/start-incident`. If the command fails, manually do the following:
1. Create an issue with the label `Incident`, on the `production` queue with the template for [Incident](https://gitlab.com/gitlab-com/gl-infra/production/issues/new?issuable_template=incident). If it is not possible to generate the issue, start with the tracking document and create the incident issue later.
1. Ensure the initial severity label is accurate.

Optional - not required for post deployment patches and as needed for the incident:
1. If S1/S2 outage, Create an issue with the label `~IncidentReview` on the `infrastructure` queue with the template for [`incident_review`](
https://gitlab.com/gitlab-com/gl-infra/infrastructure/issues/new?issuable_template=incident_review). If it is not possible to generate the issue, start with the tracking document and create the incident issue later.
1. The EOC should assign the incident issue to themselves.
   1. Incident ownership is documented through the assignee field on the issue.
   1. When handing over ownership to a new owner, at the end of shift, or end of rotation, assignment on the issue should be updated.
1. Create and associate a google doc with [the template](https://docs.google.com/document/d/1NMZllwnK70-WLUn_9IiiyMWeXs-JKPEiq-lordxJAig/edit#), to both issues, production and infrastructure. Populate and use the google doc as source of truth during the incident. This doc is mainly for real time multiple access when we cannot use the production issue for communication.
1. Contact the CMOC for support during the incident.

Issue [`infra/5543`](https://gitlab.com/gitlab-com/gl-infra/infrastructure/issues/5543) tracks automation for incident management.

### Definition of Outage vs Degraded vs Disruption

This is a first revision of the definition of Service Disruption (Outage), Partial Service Disruption, and Degraded Performance per the terms on Status.io.
Data is based on the graphs from the [Key Service Metrics Dashboard](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1)

Outage and Degraded Performance incidents occur when:

1. `Degraded` as any sustained 5 minute time period where a service is below its documented Apdex SLO or above it's documented error ratio SLO.
2. `Outage` (Status = Disruption) as a 5 minute sustained error rate above the Outage line on the error ratio graph

SLOs are documented in the [runbooks/rules](https://gitlab.com/gitlab-com/runbooks/blob/master/rules/service_apdex_slo.yml)

To check if we are Degraded or Disrupted for GitLab.com, we look at these graphs:
1. Web Service
  - [Error Ratio](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=8&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=web&var-stage=main&var-sigma=2)
  - [Apdex](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=web&var-stage=main&var-sigma=2&fullscreen&panelId=7)
2. API Service
  - [Error Ratio](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=8&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=api&var-stage=main&var-sigma=2)
  - [Apdex](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=7&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=api&var-stage=main&var-sigma=2)
3. Git service(public facing git interactions)
  - [Error Ratio](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=8&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=git&var-stage=main&var-sigma=2)
    - [Apdex](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=7&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=git&var-stage=main&var-sigma=2)
4. GitLab Pages service
  - [Error Ratio](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=8&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=pages&var-stage=main&var-sigma=2)
    - [Apdex](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=7&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=pages&var-stage=main&var-sigma=2)
5. Registry service
  - [Error Ratio](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=8&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=registry&var-stage=main&var-sigma=2)
    - [Apdex](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=7&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=registry&var-stage=main&var-sigma=2)
6. Sidekiq
  - [Error Ratio](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=sidekiq&var-stage=main&var-sigma=2&fullscreen&panelId=8)
    - [Apdex](https://dashboards.gitlab.net/d/general-service/service-platform-metrics?orgId=1&fullscreen&panelId=7&var-PROMETHEUS_DS=Global&var-environment=gprd&var-type=sidekiq&var-stage=main&var-sigma=2)

A Partial Service Disruption is when only part of the GitLab.com services or infrastructure is experiencing an incident.  Examples of partial service disruptions are instances where GitLab.com is operating normally except there are:
1. delayed CI/CD pending jobs
1. delayed repository mirroring
1. high severity bugs affecting a particular feature like Merge Requests
1. Abuse or degradation on 1 gitaly node affecting a subset of git repos.  This would be visible on the Gitaly service metrics


### Security Incidents

If an incident may be security related, engage the Security Operations on-call following the [Security Incident Response Guide](/handbook/engineering/security/sec-incident-response.html).

## Communication

Information is an asset to everyone impacted by an incident. Properly managing the flow of information is critical to minimizing surprise and setting expectations. We aim to keep interested stakeholders apprised of developments in a timely fashion so they can plan appropriately.

This flow is determined by:

1. the type of information,
1. its intended audience,
1. and timing sensitivity.

Furthermore, avoiding information overload is necessary to keep every stakeholder’s focus.

To that end, we will have:

1. a dedicated Zoom call for all incidents. A link to the Zoom call can be found in the topic for the [`#incident-management`](https://gitlab.slack.com/archives/incident-management) room in Slack.
1. a Google Doc as needed for multiple user input based on the [shared template](https://docs.google.com/document/d/1NMZllwnK70-WLUn_9IiiyMWeXs-JKPEiq-lordxJAig/edit#)
1. a dedicated [`#incident-management`](https://gitlab.slack.com/archives/incident-management)  channel for internal updates
1. regular updates to status.gitlab.com via status.io that disseminates to various media (e.g. Twitter)
1. a dedicated repo for issues related to [Production](https://gitlab.com/gitlab-com/production) separate from the queue that holds Infrastructure's workload: namely, issues for incidents and changes.

### Status

We manage incident [communication](#communication) using status.io, which updates [status.gitlab.com](https://status.gitlab.com). Incidents in status.io have **state** and **status** and are updated by the incident owner.

Definitions and rules for transitioning state and status are as follows.

| **State** | **Definition** |
| --------- | -------------- |
| Investigating | The incident has just been discovered and there is not yet a clear understanding of the impact or cause. If an incident remains in this state for longer than 30 minutes after the EOC has engaged, the incident should be escalated to the IMOC.|
| Identified | The cause of the incident is believed to have been identified and **a step to mitigate has been planned and agreed upon**. |
| Monitoring | The step has been executed and metrics are being watched to ensure that we're operating at a baseline  |
| Resolved | The incident is closed and status is again Operational.  |

Status can be set independent of state. The only time these must align is when an issues is

| **Status** | **Definition** |
| ---------- | -------------- |
| Operational | The default status before an incident is opened and after an incident has been resolved. All systems are operating normally. |
| Degraded Performance | Users are impacted intermittently, but the impacts is not observed in metrics, nor reported, to be widespread or systemic. |
| Partial Service Disruption | Users are impacted at a rate that violates our SLO. The IMOC must be engaged and monitoring to resolution is required to last longer than 30 minutes. |
| Service Disruption | This is an outage. The IMOC must be engaged. |
| Security Issue | A security vulnerability has been declared public and the security team has asked to publish it. |


## Incident Review

> The primary goals of writing an [Incident Review] are to ensure that the incident is documented, that all contributing root cause(s) are well understood, and, especially, that effective preventive actions are put in place to reduce the likelihood and/or impact of recurrence.<sup>[1](#google-sre-chapter-15)</sup>

Not every incident requires a review. But, if an incident matches any of the following criteria, an incident review must be completed:

1. A service disruption occurred
1. Data loss of any kind
1. A resolution time longer than 30 minutes
1. A monitoring failure

#### Incident Review Process

Incident reviews (of S1/S2 incidents) have two steps:

1. [Authoring of the Incident Review](#authoring-the-incident-review).
2. [Review of the Root Cause and Corrective Actions](#review-of-root-cause-and-corrective-actions).

#### Authoring the Incident Review

The first step in the Incident Review process is the synchronous review of the incident by representatives of the teams involved in the resolution of the incident. This step is conducted as close to the incident date as possible and does not require a complete Incident Review write up. The outcome of this first step should be a published Incident Review, per defined [timelines](#incident-review-timeline).

#### Review of Root Cause and Corrective Actions

Incident reviews second step is engaging with the customer, through the point of contact such as a TAM. This should always involve sharing the findings from the first step in an async form. In case of a customer requiring a sync to discuss the finding, the Infrastructure management will organise the discussion with important stakeholders of this process, per defined [timelines](#incident-review-timeline) 

1. CMOC for the Incident updates the TAM team on expected AIR timelines.
1. CMOC provides TAM published review. CMOC can also include a recording of the review, if the recording does not contain sensitive information.
1. TAM communicates to CMOC whether their customer(s) would like a synchronous review. If so, the TAM requests the availability of the customer and the CMOC schedules a review based on this availability.
1. Customer can add a set of questions prior to the meeting and all participants can collaborate on any changes or additions to corrective actions.

#### Incident Review Timeline

1. Incident resolution: Incident Review issue is created and [CMOC and EOC are assigned](#incident-review-issue-creation-and-ownership).
2. Incident resolution + 2 days: CMOC sets expectations with TAM on delivery date of Incident Review.
1. Incident resolution + 7 days: Incident Review is authored and ready for review by additional stakeholders.

#### Incident Review Issue Creation and Ownership 

Incident Reviews are conducted in [production](https://gitlab.com/gitlab-com/gl-infra/production/issues) issues&mdash;except in the case of extenuating circumstances when Infrastructure or Engineering management determines a synchronous video call should be held. The issues should have the `~IncidentReview` label attached.

1. Every incident must be assigned a DRI, most of the time this will be the EOC who responded to, or declared the incident. The incident review should be assigned to the DRI, immediately when it is created.
1. The output of an incident review should include one or more issues labeled `~Corrective Action`.  Linking already existing issues for corrective action is appropriate if the incident was similar to a prior event and corrective actions overlap.
1. The DRI is responsible for selecting and assigning corrective actions that should be prioritized and resolved within a specific timeframe.
1. All issues labeled `~Corrective Action` must have an assigned priority label, it is the responsibility of the DRI to ensure that the priorities are set.
1. For high priority `~Corrective Action` issues, a due date should be set on the issue to ensure that expectation are set for resolving them.
1. After discussion on the Incident Review issue has ended and all `~Corrective Action` issues have been linked, the issue can be closed.

The infrastructure team keeps track of [Corrective
Actions](https://gitlab.com/groups/gitlab-com/gl-infra/-/boards/1181205?&label_name[]=corrective%20action)
on a dedicated board. The prioritization and assignment of issues is collectively handled by the Reliability Engineering managers.

## Severities

### Incident Severity

**Incident severities encapsulate the impact of an incident and scope the resources allocated to handle it**. Detailed definitions are provided for each severity, and these definitions are reevaluated as new circumstances become known. Incident management uses our standardized severity definitions, which can be found under our [issue workflow documentation](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/doc/development/contributing/issue_workflow.md#severity-labels).

### Alert Severities

1. Alerts severities do not necessarily determine incident severities. A single incident can trigger a number of alerts at various severities, but the determination of the incident's severity is driven by the above definitions.
1. Over time, we aim to automate the determination of an incident's severity through service-level monitoring that can aggregate individual alerts against specific SLOs.

<a name="google-sre-chapter-15">1</a>: Google SRE Chapter 15 - Postmortem Culture: Learning from Failure
