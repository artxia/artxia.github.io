---
layout: handbook-page-toc
title: "SG.1.01 - Policy and Standard Review Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# SG.1.01 - Policy and Standard Review

## Control Statement

GitLab's policies and standards are reviewed, updated if required, approved by management, and communicated to authorized personnel annually.

## Context

The purpose of this control is to ensure GitLab's policies and procedures are kept up-to-date and relevant, changes are appropriately reviewed and approved, and GitLab team members have a way to track those changes.

Due to the nature of how GitLab operates and it's value of being iterative, continual updates are made to the related security policies and standards (as deemed necessary) that have been listed as in-scope for this control. Changes made to these procedures are always reviewed prior to being updated in GitLab's handbook. Evidence of changes can be identified via the related handbook page's markdown file in the www-gitlab-com project repo or by visiting the [Handbook Changelog](https://about.gitlab.com/handbook/CHANGELOG.html).

## Scope

All policies and standards having a direct impact to how GitLab carries out it's IT/Security practices are in-scope for this control. Policies and standards impacting the broader organization have been determined to be entity level policies which are considered as part of the Entity Level Controls (ELC) documented within the [Sarbanes-Oxley (SOX) Compliance](https://about.gitlab.com/handbook/internal-audit/sarbanes-oxley/) Handbook page. 

The specific policies and standards described in the [Policy Reference](#policy-reference) section below are subject to this control.

## Ownership

Control Owner:

* Security Compliance

Process Owner:

* Security

## Guidance

Create process to have policies and standards reviewed and updated on a recurring, annual basis.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Policy and Standard Review control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/875).

### Policy Reference
- [Engineering Department](https://about.gitlab.com/handbook/engineering/) Policies and Standards
  - [Development Department](https://about.gitlab.com/handbook/engineering/development/)
  - [Infrastructure Department](https://about.gitlab.com/handbook/engineering/infrastructure/)
    - [Backup Policies](https://about.gitlab.com/handbook/engineering/infrastructure/production/#backups) and [Backup Recovery Testing](https://gitlab.com/gitlab-com/gl-infra/gitlab-restore/postgres-gprd/blob/master/README.md)
    - [Change Management](https://about.gitlab.com/handbook/engineering/infrastructure/change-management/)
    - [Disaster Recovery](https://about.gitlab.com/handbook/engineering/infrastructure/library/disaster-recovery/) and [Disaster Recovery - Databases](https://about.gitlab.com/handbook/engineering/infrastructure/database/disaster_recovery.html)
    - [Incident Management](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/)
    - [Production Architecture Page](https://about.gitlab.com/handbook/engineering/infrastructure/production/architecture/)
  - [Quality Department](https://about.gitlab.com/handbook/engineering/quality/)
  - [Security Department](https://about.gitlab.com/handbook/engineering/security/)
    - [Data Classification Policy](https://about.gitlab.com/handbook/engineering/security/data-classification-policy.html)
    - [Data Protection Impact Assessment (DPIA) Policy](https://about.gitlab.com/handbook/engineering/security/dpia-policy/)
    - [Incident Response Guide](https://about.gitlab.com/handbook/engineering/security/sec-incident-response.html)
    - [GitLab Password Policy Guidelines](https://about.gitlab.com/handbook/security/#gitlab-password-policy-guidelines)
    - [Risk Management](https://about.gitlab.com/handbook/engineering/security/risk-management.html)
    - [Security Incident Communications Plan](https://about.gitlab.com/handbook/engineering/security/security-incident-communication-plan.html)
    - [Security Operations On-Call Guide](https://about.gitlab.com/handbook/engineering/security/secops-oncall.html#major-incident-response-workflow) for Major Incidents
    - [Third Party Vendor Security Review Procedures](https://about.gitlab.com/handbook/engineering/security/third-party-vendor-security-review.html)
    - [Vulnerability Management](https://about.gitlab.com/handbook/engineering/security/vulnerability_management/#vulnerability-management-overview)
  - [Support Team](https://about.gitlab.com/handbook/support/)
    - [Incident Management for Self-Managed Customers](https://about.gitlab.com/handbook/support/incident-management/)
  - [GitLab Security Practices](https://about.gitlab.com/handbook/security/)
    - [Business Continuity Plan](https://about.gitlab.com/handbook/business-ops/gitlab-business-continuity-plan.html)
    - [Data Team](https://about.gitlab.com/handbook/business-ops/data-team/) Policies and Standards
    - [IT Ops](https://about.gitlab.com/handbook/business-ops/it-ops-team/) Policies and Standards
      - [Inventory Management](https://about.gitlab.com/handbook/business-ops/it-ops-team/#fleet-intelligence-fleetsmith) <!-- Fleetsmith will be deprecated for DriveStrike. When this happens, this link needs to be updated. -->
- General Policies and Standards
  - [Offboarding Procedures](https://about.gitlab.com/handbook/offboarding/offboarding_guidelines/)

## Framework Mapping

* ISO
  * A.5.1.1
  * A.5.1.2
  * A.12.1.1
  * A.12.5.1
  * A.12.6.2
* SOC2 CC
  * CCC1.4
  * CC2.1
  * CC2.3
  * CC3.1
  * CC3.2
  * CC5.1
  * CC5.2
  * CC5.3
* PCI
  * 1.5
  * 2.5
  * 3.5
  * 3.5.1
  * 3.5.2
  * 3.5.3
  * 3.5.4
  * 3.6
  * 3.6.1
  * 3.6.2
  * 3.6.3
  * 3.6.4
  * 3.6.5
  * 3.6.6
  * 3.6.7
  * 3.6.8
  * 4.3
  * 5.4
  * 6.7
  * 7.3
  * 8.1
  * 8.1.1
  * 8.1.2
  * 8.1.3
  * 8.1.4
  * 8.1.5
  * 8.1.6
  * 8.1.7
  * 8.1.8
  * 8.4
  * 8.8
  * 9.10
  * 9.10
  * 10.9
  * 11.6
  * 12.1.1
  * 12.4
