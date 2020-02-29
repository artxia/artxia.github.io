---
layout: handbook-page-toc
title: "SYS.1.06 - Log Reconciliation: CMDB Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# SYS.1.06 - Log Reconciliation: CMDB

## Control Statement

GitLab reconciles the established device inventory against the enterprise log repository quarterly; devices which do not forward log data are remediated.

## Context

This control is a partner control to CON.1.04 (Configuration Check Reconciliation: CMDB). The purpose of this control is to validate that all devices in the device inventory have corresponding logs. This control is simply a validation of both logging configurations and the GitLab device inventory.

## Scope

This control applies to all production hosts and enduser devices. A production host is one used to host GitLab.com and its subdomains. An enduser devices refers to team member laptops.

## Ownership

* Control Owner: `IT Ops, Infrastructure`
* Process owner(s): 
    * IT Ops: `50%`
    * Infrastructure: `50%`

## Guidance

Logs for team member devices can be collected using, for example, tools such as Drivestrike; such tools often have the capability to automatically identify and alert on devices which are not sending logs. Production hosts not sending logs can be alerted on by comparing a list of hosts which have recently sent logs with a known source of all hosts, where if the former doesn't have all the hosts from the latter, it's an indicator that logs aren't being sent from those missing hosts.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/909).

Examples of evidence an auditor might request to satisfy this control:

* Copy of the GitLab device inventory
* Handbook entry for the device inventory process
* Handbook entry for the log reconciliation process
* Sample of remediation issues or other documentation showing remediation of devices not forwarding logs

### Policy Reference

## Framework Mapping

* ISO
  * A.12.4.1
* SOC2 CC
  * CC1.2
  * CC3.2
  * CC3.4
  * CC4.1
  * CC4.2
  * CC5.1
  * CC5.2
