---
layout: handbook-page-toc
title: "DM.4.02 - Encryption of Data at Rest Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# DM.4.02 - Encryption of Data at Rest

## Control Statement

Red, orange, and yellow data at rest is encrypted.

## Context

Encrypting data at rest helps ensure the confidentiality and integrity of that data. In the event a production instance, data store, or backup is compromised, without encryption, the data is near certain to be accessed, modified, and/or stolen. Encrypting sensitive data at rest adds another roadblock and layer of complexity for the adversary and helps protect customer, employee, and partner data.

## Scope

This control applies to red, orange, and yellow data stored in the production environment and to any enduser devices that store such data. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com

## Ownership

* Control Owner: `Infrastructure`
* Process owner(s):
    * Infrastructure

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Encryption of Data at Rest control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/797).

Examples of evidence an auditor might request to satisfy this control:

* Reference to production architecture in the handbook
* Resource export from Google Cloud showing implementation of production architecture practices and state of encryption for SSDs, HDDs, and Postgres.

## Guidance

This control can be tested by verifying the at-rest encryption status for any production resources. For compute instances, this can be done by verifying the compute resource's drive encryption status. For other resources such as managed databased (e.g., RDS and CloudSQL), this can be done by verifying the at rest encryption status through the resource's dashboard or other summary. For vendors such as GCP who encrypt data at rest by default, consider providing vendor's [documentation](https://cloud.google.com/security/encryption-at-rest/) showing the default at rest encryption.

### Policy Reference

## Framework Mapping

* ISO
  * A.18.1.4
  * A.18.1.5
  * A.8.2.3
* PCI
  * 3.4
  * 3.5
  * 3.5.3
  * 3.6
  * 3.6.3
  * 8.2.1
