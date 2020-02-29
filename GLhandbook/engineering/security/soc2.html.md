---
layout: handbook-page-toc
title: "GitLab SOC2 Security Compliance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## What is SOC2?

SOC2 is a security control report developed by the American Institute of Certified Public Accountants (AICPA) based on the Statement on Standards for Attestation Engagements no. 18 (SSAE 18).

For additional information on SOC2, feel free to check out our [Compliance Unfiltered SOC2 video](https://www.youtube.com/watch?v=-T7kELeK3rs)!

### What are the different types of SOC reports?

* SOC1 - Type 1
   * SOC1 Type 1 reports evaluate the design of controls relating to financial reporting.
* SOC1 - Type 2
   * SOC1 Type 2 reports evaluate the design and operating effectiveness of controls relating to financial reporting.
* SOC2 - Type 1
   * SOC2 Type 1 reports evaluate the design of controls relating to security controls within various Trust Service Principles.
* SOC2 - Type 2
   * SOC2 Type 2 reports evaluate the design and operating effectiveness of controls relating to security controls within various Trust Service Principles.
* SOC3
   * SOC3 reports are general use report that can be freely shared and show that an organization has been evaluated the same as a SOC2 Type 2 examination, but this report doesn't show the testing process or results.

## Why is GitLab pursuing SOC2 certification?

SOC2 is becoming an industry standard for validating that a baseline of security program maturity is in place within an organization.

Customer benefits:
* SOC2 certification will increase customer confidence in our information security program
* SOC2 is an easy way for our customers to manage GitLab as a vendor since SOC2 reports are becoming the industry standard for vendor security management

GitLab benefits:
* SOC2 reports enable our sales team to quickly share the state of our security program with potential customers
* SOC2 reports reduce the need for GitLab's security compliance team to fill out individual security questionnaires since SOC2 reports are often accepted in place of those questionnaires
* SOC2 is a good way to ensure we are meeting all requirements of a strong and comprehensive information security program and we aren't focusing only on certain areas of security
* An external examination such as SOC2 is a good way to report on the results of the security mechanisms we have put in place instead of relying solely on the design of those security mechanisms

## Is GitLab SOC2 compliant?

Not yet, but GitLab has a [target date](#when-are-we-going-to-be-compliant) for its first SOC2 examination in 2020.

## What are we doing to become SOC2 compliant?

GitLab has started the process of [establishing security controls](/handbook/engineering/security/sec-controls.html), [rolling out those controls](https://gitlab.com/groups/gitlab-com/gl-security/compliance/-/epics/30), and [testing those controls](https://gitlab.com/groups/gitlab-com/gl-security/compliance/-/epics/65) but this is a lengthy process.

### What's the difference between SOC2 controls and the GCF?

The GitLab Control Framework (GCF) is an overarching set of security controls that satisfy many underlying compliance requirements (e.g. SOC2, ISO, GLBA, etc.).

SOC2 is a subset of the requirements that the GCF satisfies.

### What are the major milestones for the SOC2 project?

1. Establish a set of [security controls](/handbook/engineering/security/sec-controls.html)
   * Completed in FY20 Q1
1. Perform a gap analysis of these security controls
   * Completed in FY20 Q2
1. [Remediate these security controls](https://gitlab.com/groups/gitlab-com/gl-security/compliance/-/epics/30)
   * This is in progress and expect to finish in FY21
1. [Test these security controls](https://gitlab.com/groups/gitlab-com/gl-security/compliance/-/epics/65)
   * This is in progress and expect to finish in FY21
1. Start our evidence collection period
1. Work with a CPA firm to complete a SOC2 audit

### What will be the scope of our SOC2 examination?

GitLab's SOC2 report will cover the people, process, and technology that make up GitLab.com. The exact inventory of systems that comprise this scope are still being developed but any system that is connected to systems/services that operate GitLab.com is likely to be included in the scope of this audit.

Additional information about the systems involved in our upcoming SOC2 examination can be found at our [SOC2 Description of System page](/handbook/engineering/security/soc2-sdos.html).

### When are we going to be compliant?

External audit targets:
* SOC2 Type 1 certification by 2020-08-01
* SOC2 Type 2 certification by 2021-02-01

### Why is it going to take that long?

1. We don't want to roll out controls specific to SOC2 only to go back to our teams next year with controls specific to ISO. Instead we are taking a longer-term view of our compliance needs and created a [comprehensive security control framework](/handbook/engineering/security/sec-controls.html) that will allow us to gather security control evidence and work with teams in a more [efficient](/handbook/values/#efficiency) manner.
1. SOC2 Type 2 reports require 6 months worth of operating security controls in order to validate the effectiveness of the controls. If we want to be audited for a SOC2 Type 2 report on 2020-07-01 we need to have all controls designed, remediated, tested, and producing audit-ready evidence as of 2020-01-01.

## How will this SOC2 project impact other teams at GitLab?

Creating security controls from scratch is a difficult process. Each GitLab team-member is iterating on processes, developing new features, reconfiguring systems, etc. every day. Security controls require a certain amount of stability in order to generate effective evidence we can present to external auditors. Combine this with the collaborative approach the security compliance team is trying to take and it makes this process especially challenging. The security compliance team doesn't want to go out to GitLab teams with archaic requirements that have been around for 10 years just because auditors are used to those requirements and the evidence to expect from each. Instead, we want collaborate with GitLab teams and innovate ways to gather evidence and be flexible in the requirements we are establishing in order to create an industry-leading security compliance program. Since GitLab creates new and innovative software, this process is really challenging since the security compliance team don't have deep technical expertise in all areas of the company. Instead we have to parter with GitLab teams to come up with the best way to approach each security control and generate meaningful evidence we can use in an audit.

TL;DR: There's just no way to establish a security program that is external-audit-ready without adding a certain amount of friction for our teams. Please know that we take this extra friction seriously and work **hard** to minimize that friction as much as possible.

## Who is responsible for the SOC2 project?

* The security compliance team is responsible for the creation of security controls and the advisement of audit requirement relating to those controls
* Every GitLab team is responsible for operating the processes required by SOC2 that the various teams and the security compliance team work together to create and document
* GitLab's leadership is responsible for supporting this initiative and giving all GitLab teams the resources (e.g. time and tools) they require to work with the security compliance team as they work towards this audit

## Where can I submit feedback for this SOC2 project?

Please add a comment to [this feedback issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/1097).

You can also [contact the security compliance team](/handbook/engineering/security/compliance.html#contact-the-compliance-team) if there's any way we can help.