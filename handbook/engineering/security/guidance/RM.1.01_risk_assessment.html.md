---
layout: handbook-page-toc
title: "RM.1.01 - Risk Assessment Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# RM.1.01 - Risk Assessment

## Control Statement

GitLab performs risk assessments of production applications and services. Results from risk assessment activities are reviewed to prioritize mitigation of identified risks. Completed risk assessments are continually reviewed and revised.

## Context

Risk assessments are important because they identify, prioritize, and help tracking the remediation of risks to GitLab. The purpose of this control is to set an appropriate cadence for risk assessments and ensure the mitigation efforts to address those risks are reasonably prioritized. The goal of a risk assessment is to convey what the risks and their priority are to the audience.

## Scope

This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership

* Control Owner: `Security Compliance`
* Process owner(s):
    * System Owners
    * Data Protection Officers
    * Security Compliance

## Guidance

This control can be tested by verifying that when a risk assessment is required by process, one is created, and that when a risk assessment is created and performed, it's done so according to the [process documented in the handbook](/handbook/engineering/security/#risk-assessments).

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Risk Assessment control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/866).

Examples of evidence an auditor might request to satisfy this control:

* A copy of GitLab's risk assessment policy and procedures.
* A non-confidential risk assessment or summary.
* A risk assessment log showing completed risk assessments, their dates, and planned risk assessments (e.g., the risk registry).
* Sample risk assessment issues.

### Policy Reference

* [Risk assessment handbook section](/handbook/engineering/security/#risk-assessments)

## Framework Mapping

* SOC2 CC
  * CC3.1
  * CC3.2
  * CC3.3
  * CC3.4
  * CC5.1
  * CC5.2
* PCI
  * 12.2
