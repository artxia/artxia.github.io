---
layout: handbook-page-toc
title: "Security Compliance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Security Compliance Mission

1. Enable GitLab sales by providing customers information and assurance about our information security program and remove security as a barrier to adoption by our customers.
1. Implement a comprehensive compliance program at GitLab to document and formalize our information security program through independent evaluation.

## Roadmap

Our [internal roadmap](https://gitlab.com/groups/gitlab-com/gl-security/compliance/-/roadmap) shows our current and planned projects and the currently defined components of work for each.
   * **Note: This link will only display if you are logged in as a GitLab team-member and is not visible to the public.**

Our [Trust Center](/security/), shows our current state of industry compliance, our commitment to retaining the trust of our customers, and the direction GitLab is headed in terms of security compliance.

### A basic overview of our active security compliance projects include:
1. Perform remediation work to bring each evaluated control to a state of "full compliance" (meaning we believe we would pass an audit of that control)
   * This work began in Q3 of 2019.
1. Perform testing of each control to validate that all control processes are operating effectively
   * This work began in Q3 of 2019.

### Upcoming security compliance projects include:
1. SOC2 Type 1 Audit
   * This work is planned to start in February 2020 and is planned to be completed no later than May 2020.
1. GCF "Phase 2" controls
   * This project is planned to start in mid-2020

## GitLab's Control Framework (GCF)

GitLab has adopted an umbrella control framework that provides compliance with a number of industry compliance requirements and best practices. For information about how we developed this framework and a list of all of our security controls, please see the [security controls handbook page](/handbook/engineering/security/sec-controls.html).

The GCF is mapped to the requirements for achieving a SOC2 certification, for more information please see our [SOC2 page](/handbook/engineering/security/soc2.html)

### Control and Project Owners

The following are the [directly responsible individuals](/handbook/people-group/directly-responsible-individuals/) (DRIs) for the different components of building and implementing the GCF.

* SOC2 Framework Mapping: [@lcoleman](https://gitlab.com/lcoleman)
* PCI-DSS Framework Mapping: [@nsarosy](https://gitlab.com/nsarosy)
* ISO 27001 Framework Mapping: [@jburrows001](https://gitlab.com/jburrows001)
* SOX 404-focused IT general control testing: [@twsilveira](https://gitlab.com/twsilveira)
* Controls: A [control domain owner](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/1131) is the DRI for the rollout and operation for the controls in their respective domain(s): 

## Continuous Monitoring

The Security Compliance team is responsible for completing the activities which continually assess the design and operating effectiveness of the controls established by the GCF.

### Gap Analysis

The purpose of a gap analysis is to identify gaps between GCF controls and documented GitLab process. Gap analysis project work is done in a [private project](https://gitlab.com/gitlab-private/sec-compliance/gcf-gap-analysis) due to the sensitive nature of the assessment findings. The project will have an issue for every GCF control in scope for the gap analysis. GitLab's [first gap analysis](https://gitlab.com/gitlab-private/sec-compliance/gcf-gap-analysis) can serve as an example for how future gap analyses can be organized and executed.

### Remediation

The remediation phase fills the gaps identified during the gap analysis and get each in-scope control into a state of audit readiness.

#### Definition of Done

A control is considered to be remediated if:

1. The process addressing the requirements of the control (as defined by the security compliance team) is documented in the GitLab handbook
1. The process documented above is the same process being used by all GitLab team-member involved in operation of the security control
1. The collection of testing evidence that will prove the above 2 points can begin
    *  Testing encompasses both "test of design" (sample of 1) and then if that passes, a test of "operating effectiveness" (random sampling)

#### Deadlines

* **All [SOX-related controls](https://gitlab.com/groups/gitlab-com/gl-security/compliance/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name%5B%5D=Control_Tracking&label_name%5B%5D=SOX-basedControlRequirement) must be ready for Internal Audit testing by 2020-02-01.** This means the control should be remediated, tested, and all gaps identified during testing also remediated until there are no more gaps. In order for all controls to be ready by 2020-02-01 some controls will need to be remediated before this date if the control is foundational to other controls which require remediation or an earlier deadline is needed in order for the [security compliance DRI](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/-/boards/1237688?&label_name%5B%5D=Control_Tracking) to balance the remediation involved in all controls.
* **All SOC2-related controls that aren't SOX-related must be generating audit-ready evidence by 2020-05-31.** Team-members working on remediation must determine, based on this timeline, the appropriate deadlines for any given stage of remediation or testing, as every control's circumstance and background is different. Similar to the above controls, some of these will be foundational so an earlier due date will be required.

Trust in an important part of the work everyone does at GitLab and the security compliance team trusts that other teams in the organization will make a good faith effort to meet these deadlines, we also ask for trust that the deadlines involved in remediating security controls are not arbitrary and reflect the many competing security needs of the organization.

GitLab's [first remediation project](https://gitlab.com/groups/gitlab-com/gl-security/compliance/-/epics/30) can serve as an example for how future remediation efforts can be organized and executed.

### Testing

Controls which have been remediated should be tested to see whether the process documented in the GitLab handbook, runbooks, and other sources are followed.

### Group Peer Reviews

The Security Compliance team will occassionally perform group peer reviews on one or more controls per review. The purpose of these reviews is to leverage the experience and perspective of the entire team to dig deep into past, current, and future work on or operation of a given control. The date of a control's most recent review is documented in the [GCF Remediation Status](https://docs.google.com/spreadsheets/d/1XuAGxPInNJpxwIFtour5XIybmejFXv3ERZjT_5AkmsU/edit#gid=0) sheet.

## Contact the Compliance Team

* Email
   * `security-compliance@gitlab.com`
* Tag us in Gitlab
   * `@gitlab-com/gl-security/compliance`
* Slack
   * `@sec-compliance-team`
* [GitLab compliance project](https://gitlab.com/gitlab-com/gl-security/compliance/compliance)

**Note: If you have an urgent request and you're not getting a response from the above team tags, the security compliance manager (@jburrows001) has their cell phone number in their slack profile. **
