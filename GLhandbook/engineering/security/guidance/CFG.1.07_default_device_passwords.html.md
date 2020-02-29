---
layout: handbook-page-toc
title: "CFG.1.07 - Default Device Passwords Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# CFG.1.07 - Default Device Passwords

## Control Statement

Vendor-supplied default passwords are changed according to GitLab standards prior to device installation on the GitLab network or immediately after software or operating system installation.

## Context

Changing the default password will strengthen the baseline configuration and reduce the ability for the system/device to become compromised.

## Scope

This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership

* Control Owner: `Infrastructure`
* Process owner(s): 
    * IT Ops
    * Infrastructure

## Guidance

Default, vendor-provided credentials should be changed before connecting an endpoint or application to GitLab's production network. In some cases, the vendor may generate secure, randomized passwords unique to GitLab as part of its offering and underlying automation. However, those can be used as they're unique and randomly generated in response to an action initiated by GitLab. To test for this control, provide vendor documentation showing default credentials are not used or otherwise disabled for CloudVM, OS Login, Kibana, and Grafana. Provide specific configurations showing alternative authentication (such as OAuth) is used for OS Login, Prometheus, and Thanos.

If anyone discovers production systems or tools that have the ability to use default credentials that is not listed above, please reach out to the [security compliance team](/handbook/engineering/security/compliance.html#contact-the-compliance-team) and we will add those systems/tools to this testing.

## Additional control information and project tracking

Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Default Device Passwords control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/790).

Examples of evidence an auditor might request to satisfy this control:

* Sample or documentation of the new user account creation process for critical accounts and systems showing no default password can be used and users must set a strong and unique password
* Non-confidential samples of Terraform and Chef configs showing default passwords aren't used for GitLab.com infrastructure

### Policy Reference

## Framework Mapping

* PCI
  * 2.1
  * 2.1.1
