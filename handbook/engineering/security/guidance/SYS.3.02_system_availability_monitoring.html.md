---
layout: handbook-page-toc
title: "SYS.3.02 - System Availability Monitoring Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# SYS.3.02 - System Availability Monitoring

## Control Statement

Critical systems are monitored in accordance to predefined availability criteria and alerts are sent to authorized personnel.

## Context

This control is related to GitLab control # SYS.3.01 (Availability Monitoring Alert Criteria). The purpose of this control is to ensure that there is monitoring and alerting based on that availability criteria. This control is meant to create actionable information from the uptime/availability thresholds we have established for ourselves. The idea is to clearly state what our availability requirements are and then hold ourselves accountable to those requirements.

## Scope

This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership

* Control Owner: `Infrastructure`
* Process owner(s):
    * Infrastructure

## Guidance

The particular tooling used isn't as important as the use of those tools being applied consistently across production and there being documented process of its use. This control can be tested by viewing the availability monitoring tool dashboards. To validate availability monitoring for a specific day, the dashboard can be filtered by day.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [System Availability Monitoring control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/921).

Examples of evidence an auditor might request to satisfy this control:

*  Documentation showing how GitLab.com is monitored, such as handbook entries and runbooks
*  Documentation showing the alerting threshold for the GitLab.com monitoring
*  Documentation describing how and to whom monitoring alerts are sent

### Policy Reference

* [Monitoring of GitLab.com](/handbook/engineering/monitoring/)
* [GitLab Readiness](/handbook/engineering/infrastructure/production/#gitlabcom)

## Framework Mapping

* ISO
  * A.12.1.3
  * A.17.2.1
* SOC2 CC
  * CC7.2
* SOC2 Availability
  * A1.1
