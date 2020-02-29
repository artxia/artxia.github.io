---
layout: handbook-page-toc
title: "CFG.1.04 - Configuration Check Reconciliation: CMDB Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# CFG.1.04 - Configuration Check Reconciliation: CMDB

## Control Statement

GitLab reconciles the established device inventory against the enterprise log repository quarterly; devices which do not forward security configurations are remediated.

## Context

This control helps to close the loop between device inventory information and production logs. If all production systems are sending the appropriate logs, there should be a parity between the device inventory GitLab collects and the logs generated from those systems. This control is meant to be a check on the "Configuration Check" control. This reconciliation ensures that all systems that should be forwarding security configuration information, are.

## Scope

This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership

* Control Owner: `IT Ops`
* Process owner(s): 
    * IT Ops: `100%`

## Guidance

Security configurations for endpoints can be collected using, for example, endpoint management tools such as Fleetsmith.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/787).

Examples of evidence an auditor might request to satisfy this control:

* Copy of the GitLab device inventory
* Handbook entry for the device inventory process
* Handbook entry for the log reconciliation process
* Sample of remediation issues or other documentation showing remediation of devices not forwarding security configurations

### Policy Reference

## Framework Mapping

* SOC2
  * CC6.1
