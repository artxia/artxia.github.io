---
layout: markdown_page
title: "Third Party Vendor Security Review process"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Process Overview

Security Compliance performs annual security reviews of vendors for corporate tools and services that may process GitLab data. As part of [New Vendor Evaluations](/handbook/finance/procurement/#1-new-vendor-evaluation) and [Vendor Contract Renewals](/handbook/finance/procurement/#2-existing-vendor-negotiation-for-renewals-and-true-ups), a security review will
will be required for all vendors and systems that will be processing, storing, and/or transmitting data 
[classified](/handbook/engineering/security/data-classification-policy.html) 
as Yellow or higher. Security Compliance identifies potential risks of the introduction of the third party to our environment and any compensating controls if applicable. Security management approval is required for vendors processing Red data and vendors with major risks identified during the review. A risk exception must be filed for vendors that cannot be approved by Security in order to proceed with contracting. The Security Compliance [runbook](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/blob/master/runbooks/Vendor_Security_Report_Review.md) and [security review template](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/new#) outline the steps and criteria.

This vendor security review process is not meant to slow down the procurement process, but a certain amount of friction to this process is inevitable. The goal of the vendor security review is to identify and document all risks associated with the use of a vendor tool or service and to reduce the likelihood that GitLab data will be exposed or mishandled. This extra scrutiny is due to the fact that GitLab no longer controls our data when it is processed, transmitted, or stored by a third party.

### Email template for requesting security documentation
You can help expedite this process by sending the following message to the vendor:

> Because the use of your tool or service requires the protection of GitLab data, our Security Compliance team will need some additional information in order to ensure that this data will be appropriately secured. If you have gone through an independent security certification process for SOC1, SOC2 Type 2, and have undergone a recent PenTest, please provide a copy of those reports or summary results. If you have not gone through that process please complete our information security questionnaire and answer only the applicable questions. We appreciate your partnership in helping GitLab complete its due diligence requirements.

### Security Documentation Decision Tree
In the event that the vendor cannot provide the above information, the following shows what documentation is required in order to complete this vendor security review process:

Does the vendor have an external audit report that shows how security controls were tested and those testing results? (e.g. SOC2 Type 2 reports, ISO 27001 audit reports, etc.)
   * `If yes`, does the scope of that report cover the services that GitLab will be using?
      * `If yes`, please please request this report and share with the security compliance team for review. Also, please request a [penetration testing report](#recent-penetration-testing-report)
        * `If no`, does the vendor have an external audit report that does cover these services?
         * `If yes`, please request this report and share with the security compliance team for review. Also, please request a [penetration testing report](#recent-penetration-testing-report)
         * `If no`, please continue through this decision tree
   * `If no`, Does the vendor have a point in time assessment of the design of security controls (e.g. CSA CAIQ self-assessment, SOC2 Type 1, etc.)?
      * `If yes`, please request this report and share with the security compliance team for review. Also, please request a [penetration testing report](#recent-penetration-testing-report)
      * `If no`, please continue through this decision tree

Is the vendor willing to fill out GitLab's information security questionnaire so we can assess the maturity of their information security program?
   * `If yes`, please share the [GitLab Information Security Questionnaire](https://docs.google.com/spreadsheets/d/1isL6fkYX45Wb0BewozUPROnGgirmonTENFuBGapS_Xk/edit#gid=1307424571) with the vendor. Also, please request a [penetration testing report](#recent-penetration-testing-report)
      * **Note: It can take vendors some time to complete these questionnaires so the earlier we start this process the better **
   * `If no`, please complete a [risk exception](/handbook/engineering/security/risk-management.html#risk-exceptions) so we can document the fact that we are proposing to move forward with a vendor for which we have no insight into the maturity of their security program.

#### Recent Penetration Testing Report
Penetration testing reports have a very different scope and goal than audits of an information security program audit, but they are very useful when assessing the maturity of a vendor's information security program. The fact that a vendor has completed such a test indicates that they are operating a mature security program and are reducing the likelihood of a vulnerability existing in architecture or software. For this reason we request a copy of a recent penetration testing report as a part of all documentation requests as well as a current state of the remediations associated with any findings in that report.

#### What if a vendor is providing a security whitepaper instead?
Unfortunately, security whitepapers rarely give us all of the information we need. When a company generates these whitepapers they are always from the perspective of everything the vendor feels like they are doing well, but won't have any information about what controls are not in place or not yet mature. For this reason we won't accept whitepapers in place of audit reports or the GitLab Information Security Questionnaire, but the vendor can absolutely attach the whitepaper and reference any information in there when completing our questionnaire if that makes the process easier for the vendor.
 
## Vendor Security Reports Review

### Finance issue
When a Finance issue is opened for new services, there is a section for `Data Processing` that must be completed by the business owner requesting the service. This will initiate the secuity review which must be followed in tandem with the Contract and Approval Workflow. The instructions ask for security reports and certifications including SOC1, SOC2 Type 2, and the latest Penetration test. The label ~"SecurityReview::NotStarted" is applied by the template.

### Security Compliance intake 
Security Compliance monitors the [Finance Security Review dashboard](https://gitlab.com/gitlab-com/finance/-/boards/1375804) for new requests. If the service or tool uses GitLab data classified as Yellow or above, the Security Compliance DRI will open a [Compliance issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues?scope=all&utf8=✓&state=all&label_name[]=Vendor%20Security%20Review) 
using the [Vendor Security Report Review template](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/new?issue%5Bassignee_id%5D=&issue%5Bmilestone_id%5D=). The label "SecurityReview::Blocked" will be used in the Finance issue until the security compliance team has received all documentation needed to perform this review. At that point the Finance issue label will then be updated to "SecurityReview::Started". Information is requested from the vendor as needed to complete the review. Updates in the Finance issue must be kept current, along with the appropriate scoped label. The label ~"SecurityReview::Completed" is used once the Security review is finished and ready for Step 5 of the procurement template.

### Vendor Security Report Review
Reports and questionnaires returned by the vendor are [reviewed for noted exceptions and gaps](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/blob/master/runbooks/Vendor_Security_Report_Review.md). Exceptions are recorded according to the instructions within the template and shared in the original Finance issue. The Security Compliance DRI then selects the appropriate `Security Approval` in Step 5 of the template. If management approval is needed, the additional steps are followed to tag for review.

## Criteria
Security reviews are largely operating on a guidance basis where Security Compliance provides recommendations after reviewing reports based on identified risks. As specifications and requirements are identified by stakeholders, those will be added to this page as security guidance for sourcing.

## SLA
Security Compliance commits to a 3-business day SLA for completion when not waiting on input from the vendor. The scoped lables will be used to audit SLAs.

## Accepting risks identified during the procurement process
If the result of a vendor security review is either:
1. We were not able to get any security documentation from the vendor; or
1. We identified 1 or more findings that indicate the vendor's security program is not appropriately mature or has known flaws
then our findings will be presented to the Senior Director of Security for a final determination on whether or not that vendor can be approved from a security perspective.

If a GitLab team wants to move forward with a vendor without security approval, then a [risk exception](/handbook/engineering/security/risk-management.html#risk-exceptions) is required.

The purpose of this risk exception is to ensure that when GitLab leadership is approving of these risks, they do so with full context and insight into the tangible dangers presented by that risk to our team-members and customers. The output of this process also gives us a record to track organizational risk which is required in external audits.
