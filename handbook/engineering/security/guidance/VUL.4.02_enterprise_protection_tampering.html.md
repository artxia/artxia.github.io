---
layout: handbook-page-toc
title: "VUL.4.02 - Enterprise Protection Tampering Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# VUL.4.02 - Enterprise Protection Tampering

## Control Statement

Endpoint protection mechanisms cannot be disabled or altered by users unless specifically authorized by management

## Context

This control outlines the mechanisms utilized to protect endpoints should be secured to not allow disablement or alteration which support the security of the endpoint that is connected to the GitLab network.

## Scope

This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.


## Ownership

* gitlab.com and live production environments
  * Security Operations - responsible for maintenance and monitoring of Uptycs
  * Infrastructure - responsible for addressing Uptycs findings

* Laptops
  * Security Management- responsible for enforcement of endpoint management
  * IT-Ops - responsible for rolling out endpoint management tool, monitoring tool, reporting on non-compliance devices - trigger an alert

## Guidance

Any production systems we are not utilizing Uptycs or Fleetsmith on should have a documented justification for why it isn't applicable. It is fine to have different tools securing different systems, but the more different solutions we use, the more complexity we introduce into the maintenance of this control.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Enterprise Protection Tampering control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/1113).

### Policy Reference

## Framework Mapping

* PCI
  * 5.3
