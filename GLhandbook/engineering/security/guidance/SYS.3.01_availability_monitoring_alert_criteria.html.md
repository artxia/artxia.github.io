---
layout: handbook-page-toc
title: "SYS.3.01 - Availability Monitoring Alert Criteria Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# SYS.3.01 - Availability Monitoring Alert Criteria

## Control Statement

GitLab defines availability monitoring alert criteria, how alert criteria will be flagged, and identifies authorized personnel for flagged system alerts.

## Context

In order for alerts to be configured for availability, we first have to establish what criteria we use for altering. This control simply formalizes the need for GitLab to explicitly define what criteria we use for availability alerting.

## Scope

This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership

* Control Owner: `Infrastructure`
* Process owner(s):
    * Infrastructure

## Guidance

This control is not meant to dictate what criteria we use for our availability monitoring, only that we define what our alerting criteria is. Alerting criteria is stored in the `gitlab-com/runbooks` [repository](https://gitlab.com/gitlab-com/runbooks). This control can be tested by viewing the alerting criteria in the `yml` files which define the alerting critieria within the repository. To validate the history of an alerting criteria file, you can view each respective `yml` file's commit history. The files defining the alerting criteria contain all the information prescribed by this control, so validating the files are there and using the commit history to determine from when is sufficient to test this control.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Availability Monitoring Alert Criteria control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/920).

Examples of evidence an auditor might request to satisfy this control:

* Copies of the monitoring runbooks and other monitoring tool configuration documentation
* Examples of how alert criteria are applied against monitoring tools (e.g., monitoring tool configuration files)
* User export from PagerDuty and on-call Slack apps

### Policy Reference 

* [Monitoring of GitLab.com](/handbook/engineering/monitoring/)
* [GitLab.com Availability](/handbook/engineering/performance-indicators/#gitlab-com-availability)
* [Monitoring Alert Criteria](https://gitlab.com/gitlab-com/runbooks/tree/master/rules)
* [PagerDuty Alerts](/handbook/support/on-call/#pagerduty-alerts)

## Framework Mapping

* ISO
  * A.12.1.3
  * A.17.2.1
* SOC2 CC
  * CC7.2
* SOC2 Availability
  * A1.1
