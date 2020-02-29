---
layout: handbook-page-toc
title: "Risk Management"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Risk Assessments

Risk assessments help GitLab identify, prioritize, and manage security risks. They're important to help protect customer data and meet GitLab [security compliance controls](/handbook/engineering/security/sec-controls.html#risk-management), which are important for compliance standards such as SOC2 and PCI-DSS. A risk assessment should ideally be completed for every service in the [Tech Stack Applications](/handbook/business-ops/tech-stack-applications/) table and reviewed either quarterly or as substantial changes are made, whichever is most feasible. Additionally, risk assessments are used as part of [Data Protection Impact Assessments](/handbook/engineering/security/dpia-policy/#dpia-assessment) (DPIAs).

At GitLab, our risk assessment framework is based on a combination of [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/publications/detail/sp/800-30/rev-1/final) and the [Mozilla Rapid Risk Assessment (RRA)](https://infosec.mozilla.org/guidelines/risk/rapid_risk_assessment), but customized to be collaborative, asynchronous, and done within GitLab itself. All risk assessment work is done within the [Risk Assessment](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments) repository.

### Creating a New Risk Assessment

* Risk assessments are maintained as markdown files in the [Risk Assessment](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments) repository.
* To create a new risk assessment, create an MR in the Risk Assessment repository.
    * Using the [risk assessment template](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/blob/master/templates/risk-assessment-template.md), the MR should create a new file titled `[Service Name]-risk-assessment` in the `assessments/` directory.
    * To make additions or changes, push commits like you would any other MR.
    * Anyone can contribute to risk assessment MRs.
* The risk assessment process is designed to be [iterative](/handbook/values/#iteration). The MR should be merged when you or others feel there's enough information for it to be useful and then continually iterated on after being merged. A good baseline is for it to be merged when at least one risk has been identified and scored.
* For every identified risk, follow the risk [remediation and tracking](/handbook/engineering/security/#risk-remediation-and-tracking) process.
* To iterate on a risk assessment after it's been merged, see [Contributing to a Risk Assessment](/handbook/engineering/security/#contributing-to-a-risk-assessment).

#### Internal & External Risk Considerations

Risk assessments should consider both internal and external risks. This is important because the [Verizon 2019 Data Breach Investigation Report (DBIR)](https://enterprise.verizon.com/resources/reports/dbir/2019/summary-of-findings/) found 39% of breaches involved internal actors (whether intentional or accidental). By considering both internal and external risks, we can more accurately define and work to mitigate GitLab's risk surface.

#### Fraud & Abuse Considerations

Risk assessments should specifically consider risks related to fraud and abuse. This is important because fraud and abuse [results in millions of lost dollars](https://www.fbi.gov/scams-and-safety/common-fraud-schemes/internet-fraud) from victims every year. Fraud and abuse can also directly impact GitLab's product and service offerings. For those reasons, every risk assessment should explicitly address fraud and abuse related risks.

### Risk Remediation and Tracking

* Create a new risk [remediation issue](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/issues/new?issuable_template=Risk%20Remediation%20Template).
* Update the [Risk Registry](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/blob/master/Risk%20Registry.md) with a link to the remediation issue and the risk status.

#### Accepting Risk

There may be instances where a risk cannot or won't be remediated. In such cases, follow the [Risk Exception](/handbook/engineering/security/risk-management.html#risk-exceptions) process.

### Contributing to a Risk Assessment

* Risk assessments are [located](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/tree/master/assessments) in the `assessments/` directory. To contribute to a risk assessment, please [create an MR](/handbook/communication/#everything-starts-with-a-merge-request) to propose the change or start a discussion.
* [Everything is a draft](/handbook/values/#everything-is-in-draft), so iteration to risk assessments is encouraged.
* Anyone can contribute to a risk assessment, including team members outside of the Security department.
* If the status of an identified risk is changed, update the [Risk Registry](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/blob/master/Risk%20Registry.md).

### Review and Revision of Risk Assessments

Risk assessments should be continually reviewed and revised to keep the information in risk assessments current and relevant. **At a minimum, every risk assessment should be reviewed once per year or as significant changes are made to the system, whichever comes first.** 

To conduct a risk assessment review:

* Create a risk assessment review [issue](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/issues/new?issuable_template=Risk%20Assessment%20Review).
* Conduct the review by following the instructions in the review issue template.
* If new risks are identified or the status of an identified risk is changed, update the [Risk Registry](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/blob/master/Risk%20Registry.md).

Upcoming risk assessment reviews are tracked in the [Risk Assessment Review](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/blob/master/Risk%20Assessment%20Reviews.md) document. A risk assessment should be added after the initial MR has been merged.

### Closing a Risk Assessment

Sometimes it may be appropriate to close a risk assessment. Some reasons a risk assessment may be closed are the vendor is no longer used or the type of data stored or processed changes. To close a risk assessment, open an MR and: 

* Add `(CLOSED)` to the end of `# GitLab Risk Assessment`, to get `# GitLab Risk Assessment (CLOSED)`
* Immediately under the `# GitLab Risk Assessment (CLOSED)` section, write that the risk assessment is being closed, why it's being closed, and provide any supporting links.
* As risk assessments are a function of DPIAs, the closure of any risk assessments should be reviewed and merged by a Security Compliance manager.

[This MR](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/merge_requests/23) can be used as an example of this process.

## Risk Exceptions

Risk management is a way to identify and document most of the risks associated with how we perform our work as GitLab team-members. Every decision we make as a company involves risk and the purpose of documenting that risk is not to influence decision making or slow down processes unnecessarily, but rather to give GitLab decision makers as much information about that decision as possible so the best possible decision can be made. 

Risk exceptions are a way to document when the business benefits outweigh the risks associated with a particular decision. In order to gather the evidence we need to show auditors we are making these decision with security risks in mind, we are processing exceptions through [risk exception issues](https://gitlab.com/gitlab-com/gl-security/compliance/risk-assessments/issues/new?issuable_template=Risk%20Acceptance%20Template). 

The goal with these exceptions is to make a ["steel man" case](/handbook/values/#assume-positive-intent) for why a particular decision might increase the overall risk to the organization. This is not meant to deter the appropriate exception approver from accepting that risk, but rather to make that decision as informed as possible. There will always be times when a process meant to reduce risk in 80% of cases simply won't apply to a particular decision and this exception process will help guide all parties involved through that decision making process.
