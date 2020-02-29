---
layout: handbook-page-toc
title: "SYS.1.08 - Enterprise Protection Logging"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

#  SYS.1.08 - Enterprise Protection Logging

## Control Statement

If applicable, GitLab's managed enterprise protection deployments generate audit logs. These audit should be retained for one year with 90 days of data immediately available for analysis or in accordance with [Record Retention Policy](/handbook/people-group/code-of-conduct/#record-retention-policy), whichever is longer.

## Context

Logging is the foundation for a variety of other security controls including monitoring, incident response, and configuration management. Without comprehensive and reliable logs, large parts of our security compliance program wouldn't be possible. This control is left vague by design. As we develop our system maps and inventories this control will likely become a bit more targeted.

An auditor will look to validate in-scope systems are generating logs, those logs are collected, retained the required amount of time and utilized to monitor for performance, health, and anomalies. To validate the control is working properly, the auditor should require additional pieces of information to demonstrate audit logging is functioning properly. Those information items include:

* Review of the audit and accountability policy and procedures
* Confirmation that audit events are reviewed and updated on a recurring basis
* Review what should be collected for auditing and cross-reference against what is collected
* Determine what defines a production system to validate the correct systems are being audited
* Confirm log validation processes are working as intended
* Master asset listing to confirm correct systems are being protected
* Log collection process(es) 

## Scope

This control applies to all systems within our production environment and GitLab-issued team member endpoints. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership

* Control Owner: `Security Operations`
* Process owner(s):
    * Security Operations
    * IT Ops

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Enterprise Protection Logging control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/911).

Examples of evidence an auditor might request to satisfy this control:

* 

### Policy Reference

## Framework Mapping

* PCI
  * 5.2
  * 10.7