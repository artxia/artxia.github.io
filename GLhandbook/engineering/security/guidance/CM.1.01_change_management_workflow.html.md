---
layout: handbook-page-toc
title: "CM.1.01 - Change Management Workflow Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# CM.1.01 - Change Management Workflow

## Control Statement

Change scope, change type, and roles and responsibilities are pre-established and documented in a change control workflow; notification and approval requirements are also pre-established based on risk associated with change scope and type.

## Context

Having a structured workflow and guidance on change management helps reduce the risk of GitLab experiencing platform or application instability by increasing the predictability and reproducibility of the change management process.

## Scope

This control applies to all systems within our GitLab.com production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This doesn't include third-party systems that support the business of GitLab.com, which can be found in CM.3.01.

## Ownership

* Control Owner: `Infrastructure`
* Process owner(s):
    * Infrastructure

## Guidance

There are two primary changes that occur in production: infrastructure changes and code changes. Infrastructure changes are done in accordance with the [Change Management](https://about.gitlab.com/handbook/engineering/infrastructure/change-management/) process. Code changes are made in accordance to our contribution, review, and approval processes, which is described as part of the [Service Lifecycle Workflow](https://about.gitlab.com/handbook/engineering/security/guidance/SLC.1.01_service_lifecycle_workflow.html) control. Changes made to third-party systems ared related to the [Third-Party Change Management Workflow](https://about.gitlab.com/handbook/engineering/security/guidance/CM.3.01_third_party_change_management_workflow.html) control, which is currently still being developed.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Change Management Workflow control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/781).

Examples of evidence an auditor might request to satisfy this control:

* Copy of the GitLab change management workflow
* Sample of issues or other documentation showing the change management workflow is followed

### Policy Reference

* [Change Management](https://about.gitlab.com/handbook/engineering/infrastructure/change-management/) 
* [Service Lifecycle Workflow](https://about.gitlab.com/handbook/engineering/security/guidance/SLC.1.01_service_lifecycle_workflow.html)
* [Third-Party Change Management Workflow](https://about.gitlab.com/handbook/engineering/security/guidance/CM.3.01_third_party_change_management_workflow.html)

## Framework Mapping

* ISO
  * A.12.1.2
  * A.12.6.2
  * A.14.2.1
  * A.14.2.2
  * A.14.2.4
* SOC2 CC
  * CC2.3
  * CC8.1
* PCI
  * 1.1.1
  * 10.4.2
  * 6.4
  * 6.4.5
  * 6.4.5.1
  * 6.4.5.2
  * 6.4.5.3
  * 6.4.5.4
  * 6.4.6
