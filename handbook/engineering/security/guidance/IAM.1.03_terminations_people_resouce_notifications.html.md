---
layout: handbook-page-toc
title: "IAM.1.03 - Terminations: People Resources Notifications Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# IAM.1.03 - Terminations: People Resources Notifications

## Control Statement
The People Operations Management system sends a notification to relevant personnel, or system, in the event of a termination of an information system user. Notification can be manual or automated.

## Context
The purpose of this control is to ensure there is a process in place to remove access to user accounts that is no longer necessary. The People Operations Management system is the source-of-record for the status of GitLab teammembers and therefore, any changes to status need to be communicated to downstream systems in order to ensure proper logical access management. This control helps ensure that only authorized and active accounts can be accessed and used to prevent any unauthorized use or access of GitLab customer, GitLab teammember, and partner data.

For the purposes of the Gitlab Control Framework [GCF](https://about.gitlab.com/handbook/engineering/security/sec-controls.html#gitlab-control-framework-gcf), the control activites captured here are incorporated into [IAM.1.02 - Logical Access De-Provisioning](https://about.gitlab.com/handbook/engineering/security/guidance/IAM.1.02_logical_access_deprovisioning.html) control. 

## Scope
This control applies to any system or service where user accounts can be provisioned. As noted above, this control is NA for GitLab as the outlined control activites have been incorporated into [IAM.1.02 - Logical Access De-Provisioning ](https://about.gitlab.com/handbook/engineering/security/guidance/IAM.1.02_logical_access_deprovisioning.html)

## Ownership

[IAM.1.02 ownership breakdown](https://about.gitlab.com/handbook/engineering/security/guidance/IAM.1.02_logical_access_deprovisioning.html#ownership)
* Control Owners:
    * People Ops
    * IT Ops
* Process Owners:
    * IT Ops (50%)
    * System Owners (50%)

## Additional control information and project tracking
Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Terminations: People Resources Notifications control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/807).

### Policy Reference
*  [Access Control Policy and Procedures](/handbook/engineering/security/#access-control-policy-and-procedures)
*  [GitLab Offboarding Guidelines](https://about.gitlab.com/handbook/offboarding/offboarding_guidelines/)
*  [Access Management Process](https://about.gitlab.com/handbook/engineering/security/#access-management-process)
*  [Logical Access Deprovisioning](https://about.gitlab.com/handbook/engineering/security/#deprovisioning)
*  [Access Reviews](https://about.gitlab.com/handbook/engineering/security/#access-reviews)


## Framework Mapping
* ISO
  * A.7.3.1
  * A.9.2.1
  * A.9.2.2
  * A.9.2.3
  * A.9.4.1
  * A.9.2.6
  * A.18.1.3
* SOC2 CC
  * CC6.2
  * CC6.3
  * CC6.6
  * CC6.7
* PCI
  * 8.1.2
  * 8.1.3
  * 8.1.4
