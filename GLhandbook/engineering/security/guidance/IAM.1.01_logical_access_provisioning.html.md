---
layout: handbook-page-toc
title: "IAM.1.01 - Logical Access Provisioning Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# IAM.1.01 - Logical Access Provisioning

## Control Statement
Logical access provisioning to information systems requires approval from appropriate personnel.

## Context
The purpose of this control is to ensure there is a process in place to review and authorize new user account requests. Ensuring only people who require access to a system or service receive access helps improve GitLab's overall security posture by limiting the number of accounts with access and reducing the overall likelihood of an account being compromised.

## Scope
This control applies to any system or service where user accounts can be provisioned.

## Ownership
Control ownership:
* IT Operations

Process ownership:
* IT Operations
* Managers
* Systems Owners

## Guidance
Provisioning should be based on predetermined roles with business justification and management approval. The process owner should use role-based authentication whenever possible to make this control easier and to segregate out this function from that of other system functions.

## Additional control information and project tracking
Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Logical Access Provisioning control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/805).

## Policy Reference
*  [Access Control Policy](/handbook/engineering/security/#access-control-policy-and-procedures)
*  [Access Request Process](https://about.gitlab.com/handbook/engineering/#access-requests)
*  [Access Management Process](https://about.gitlab.com/handbook/engineering/security/#access-management-process)
*  [Access Request Template](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=New%20Access%20Request)


## Framework Mapping
* ISO
  * A.9.2.1
  * A.9.2.2
  * A.9.2.3
  * A.9.4.1
  * A.12.5.1
  * A.18.1.3
* SOC2 CC
  * CC6.1
  * CC6.2
  * CC6.3
  * CC6.6
  * CC6.7
* PCI
  * 7.1.4
  * 8.1.2
