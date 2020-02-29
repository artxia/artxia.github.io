---
layout: handbook-page-toc
title: "IAM.3.03 - Service Account Restrictions Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# IAM.3.03 - Service Account Restrictions

## Control Statement

Individual user or administrator use of service accounts for O/S, applications, and databases is prohibited.

## Context

Preventing interactive login via a service accounts by individual users and administrators reduces the risk of unauthorized access to systems and data. In many cases, service accounts are set up with highly privileged access and therefore, this control aims to prevent the hijacking of that access by individuals who otherwise would not have it. All service accounts should be set by default to `do not allow login` and monitoring should be in place to alert in the event an account is set to allow interactive login. 

## Scope

This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership

Control owner: 
* Security Management

Process owner: 
* Infrastructure
* IT-Ops

## Guidance

All service accounts should be set by default to `do not allow interactive login`

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Remote Connections control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/824).

### Policy Reference

## Framework Mapping

* ISO

* SOC2 CC

* PCI

