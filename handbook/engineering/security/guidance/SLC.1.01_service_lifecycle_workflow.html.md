---
layout: handbook-page-toc
title: "SLC.1.01 - Service Lifecycle Workflow Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# SLC.1.01 - Service Lifecycle Workflow

## Control Statement

Major software releases go through all phases of the Service Life Cycle: Plan, Create, Verify, Package, Secure, Release, Configure, Monitor

## Context

The purpose of this control is to formalize the documentation and approval of software changes before those changes are implemented. This rigid process helps protect GitLab from insecure code being quickly pushed out into production without proper vetting.

## Scope

This control applies to all major software releases to GitLab.com.

## Ownership

* Control Owner: `Delivery`
* Process owner(s):
    * Delivery
    * Infrastructure

## Guidance

Most of this process is already captured in current GitLab workflow; the difficult part of this process will be coverage of all major software changes. Below is a detailed description of the workflow by stages:

Step 1: Planning

*  [Product Section Vision - Dev](https://about.gitlab.com/direction/dev/) explains the `Manage`, `Plan`, and `Create` steps of the cycle.
* Product Development [Workflow](https://about.gitlab.com/handbook/product-development-flow/) describes the validation and build tracks for the proposed changes.


Step 2: Create - coding

*  The entire engineering workflow is documented here, which describes the process from the [basics](https://about.gitlab.com/handbook/engineering/workflow/#basics) such as how to pick something to work on ***and includes the link to the project where the issues are housed*** -- *this is the starting point for the testing of SLC artifacts*

* Instructions on scoped labels used in [updating issues](https://about.gitlab.com/handbook/engineering/workflow/#updating-issues-throughout-development) using  ***the scoped labels `workflow::` series*** through development to the [product development timeline](https://about.gitlab.com/handbook/engineering/workflow/#product-development-timeline) -- *following the scoped labels can be useful in testing the different parts of the cycle*

*  The handbook section on [code review](https://docs.gitlab.com/ee/development/code_review.html) process-- *this is represented within issues as the `Reviewer Roulette` function*

* in the GitLab Docs, [guidelines](https://about.gitlab.com/handbook/engineering/workflow/code-review/) are documented. 


Step 3: Verify - code review/ security review

*  All code merged into the GitLab.com codebase must be reviewed by an authorized [Reviewer](https://about.gitlab.com/handbook/engineering/workflow/code-review/#reviewer), as described in our [code review documentation](https://docs.gitlab.com/ee/development/code_review.html)  

*  The security release process is documented in the [handbook](https://about.gitlab.com/handbook/engineering/infrastructure/blueprint/release/security/)-- *is useful for testing the `Verify` step of the DevOps cycle and `Secure` value stage


Step 4: Change Management

*  The Change Management process is documented in the [handbook](https://about.gitlab.com/handbook/engineering/infrastructure/change-management/). It provides guidance on using the appropriate label based on the type of [change](https://about.gitlab.com/handbook/engineering/infrastructure/change-management/#change-type), such as `DeploymentNewFeature`.


Step 5: Packing and Release 

*  Infrastructure for the GitLab system is defined as code and deployed using [Terraform](https://gitlab.com/gitlab-com/gitlab-com-infrastructure) and [Chef](https://gitlab.com/gitlab-cookbooks). These act as baseline configurations for our production systems. Changes made to those repositories - and therefore to our infrastructure - is subject to the same review process as our codebase.

*  Engineering Workflow section in the handbook notes [labels and milestones](https://about.gitlab.com/handbook/engineering/workflow/#use-group-labels-and-group-milestones) and more specific information on the [workflow labels](https://about.gitlab.com/handbook/engineering/workflow/#use-group-labels-and-group-milestones) 

*  For other Infrastructure team specifics, there's the Infrastructure [Library](https://about.gitlab.com/handbook/engineering/infrastructure/library/) page. 


Step 6: Configure and Monitor

*  The design of the CI/CD pipeline for GitLab.com is documented in the [handbook](https://about.gitlab.com/handbook/engineering/infrastructure/design/cicd-pipeline/)


*  Coupled with [GitLab Flow](https://docs.gitlab.com/ee/topics/gitlab_flow.html) and the [working in CE/EE codebase blueprint](https://about.gitlab.com/handbook/engineering/infrastructure/library/ce-ee-codebases/), this covers most of the SDLC. 


*  For a description of how GitLab uses the CI/CD internally for the GitLab system, there's this Infrastructure [page](https://about.gitlab.com/handbook/engineering/infrastructure/library/cicd-pipeline/).

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Service Lifecycle Workflow control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/888).

Examples of evidence an auditor might request to satisfy this control:

* Documentation outlining our development and release workflows
* Sample releases and their respective reviews
* Sample pipeline artifacts and merge request reviews
* Feature requests would be a great example of this process since they are planned via epics and issues, created via MR's, and then run through a GitLab pipeline to satisfy the remaining requirements for this control

### Policy Reference

* [Handbook>Engineering Workflow](https://about.gitlab.com/handbook/engineering/workflow/)
* [CI/CD Pipeline](https://about.gitlab.com/handbook/engineering/infrastructure/library/cicd-pipeline/)
* [Blueprint: Working in CE and EE codebases](https://about.gitlab.com/handbook/engineering/infrastructure/library/ce-ee-codebases/)
* [Security Releases](https://about.gitlab.com/handbook/engineering/infrastructure/library/release/security/)
* [Code Review](https://about.gitlab.com/handbook/engineering/workflow/code-review/)
* For deployment:[Terraform Project](https://gitlab.com/gitlab-com/gitlab-com-infrastructure) and [Chef cookbook Project](https://gitlab.com/gitlab-cookbooks)
* [Change Management](https://about.gitlab.com/handbook/engineering/infrastructure/change-management/)

## Framework Mapping

* ISO
  * A.14.1.1
  * A.14.2.5
* SOC2 CC
  * CC8.1
* PCI
  * 6.3
