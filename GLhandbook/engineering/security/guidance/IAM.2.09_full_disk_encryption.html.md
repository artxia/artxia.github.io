---
layout: markdown_page
title: "IAM.2.09 - Full Disk Encryption (Not Applicable)"
---
 
## On this page
{:.no_toc}
 
- TOC
{:toc}
 
# IAM.2.09 - Full Disk Encryption (Not Applicable)
 
## Control Statement

Where full disk encryption is used, logical access must be managed independently of operating system authentication; decryption keys must not be associated with user accounts.
 
## Context

Separating user accounts from decryption keys decreases the likelihood that an attacker with possession or control of a GitLab system can access any data contained on that system.
 
## Scope

`N/A`

_Full disc encryption is not applicable to the GitLab environment as we do not process credit card numbers._

Encryption is covered by the following controls:

[DM.4.01 - Encryption of Data in Transit](https://about.gitlab.com/handbook/engineering/security/guidance/DM.4.01_encryption_of_data_in_transit.html)

[DM.4.02 - Encryption of Data at Rest](https://about.gitlab.com/handbook/engineering/security/guidance/DM.4.02_encryption_of_data_at_rest.html)
 
## Additional control information and project tracking
Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Full Disk Encryption issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/820) . 
 
## Framework Mapping

* PCI DSS V3.2.1 - Requirement `3.4.1`
