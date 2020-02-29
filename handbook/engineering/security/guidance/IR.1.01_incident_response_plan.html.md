---
layout: handbook-page-toc
title: "IR.1.01 - Incident Response Plan Control Guidance"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# IR.1.01 - Incident Response Plan

## Control Statement

GitLab defines the types of incidents that need to be managed, tracked and reported, including:

* Procedures for the identification and management of incidents
* Procedures for the resolution of confirmed incidents
* Key incident response systems
* Incident coordination and communication strategy
* Contact method for internal parties to report incidents
* Support team contact information
* Notification to relevant management in the event of a security breach
* Provisions for updating and communicating the plan
* Provisions for training of support team
* Preservation of incident information
* Management review and approval, quarterly, or when major changes to the organization occur

## Context
The purpose of this control is to ensure GitLab creates, implements, and maintains an effective plan to identify, resolve, and prevent incidents within its application, systems, and services. By having an organized and continually evolving incident response plan, GitLab can maintain the availability, reliability, performance, and confidentiality offered to GitLab customers, GitLab team-members, and partners. Since this control is related to incident response, there is no easy way to test this unless citing examples of an actual incident. Hence this can be tested by proving that GitLab has sufficient documentation in place for an efficient Incident Response plan,  which can include documentation pertaining to the handbook pages, Merge requests, and issues opened in reference to and in adherence to the IR plan.

## Scope
This control applies to all systems within our production environment. The production environment includes all endpoints and cloud assets used in hosting GitLab.com and its subdomains. This may include third-party systems that support the business of GitLab.com.

## Ownership
* Control Owner: `Infrastructure`
* Process owner(s):
    * `Security Operations`
    * `Infrastructure`

## Additional control information and project tracking
Non-public information relating to this security control as well as links to the work associated with various phases of project work can be found in the [Incident Response Plan control issue](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/issues/839).

Examples of evidence an auditor might request to satisfy this control:
* Provide copies of the Incident Response pages, which are linked to and described below
* Provide sample reports and other outputs of the various functions listed below, such as Infrastructure and/or Security incident issues

### Policy Reference
1. Procedures for the identification and management of incidents: 
*  [Incident management documented in the GitLab Handbook](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/)
*  [Incident Management for Self-Managed Customers](https://about.gitlab.com/handbook/support/incident-management/)

2. Procedures for the resolution of confirmed incidents. 
*  [Security issue triage process](https://about.gitlab.com/handbook/engineering/security/#issue-triage)
*  [Security severity labelling](https://about.gitlab.com/handbook/engineering/security/#severity-and-priority-labels-on-security-issues)
*  [Major Incident Response Workflow](https://about.gitlab.com/handbook/engineering/security/secops-oncall.html#major-incident-response-workflow)
*  [Additional documentation](https://about.gitlab.com/handbook/security/#panic-email) on using the `panic` email and a [procedure for the security team's response](https://about.gitlab.com/handbook/security/#checklist-for-when-panic-is-triggered) to those alerts

3. Key incident response systems:
*  [Incident management documented in the GitLab Handbook](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/) 

4. Incident coordination and communication strategy:
    *  [S1 and S2 Incidents](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/#s1-and-s2-incidents). Information about our most critical incident severities.
    *  [Incident Steps](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/#incident-steps). Defines the steps involved with handling an incident.
    *  [Communication](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/#communication). Describes communication procedures during an incident.
    *  [CMOC and IMOC checklist](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/#cmoc-and-imoc-checklist). A checklist of actions for the CMOC and IMOC response roles to perform.
    *  [Incident runbooks](https://gitlab.com/gitlab-com/runbooks/tree/master/incidents) are available and maintained in the `runbooks` project
    *  [Database-specific runbooks](https://gitlab.com/gitlab-com/runbooks/blob/master/incidents/database.md)
    *  [Additional runbooks](https://gitlab.com/gitlab-com/runbooks)

5. Contact method for internal parties to report incidents
*  [Process for engaging security on-call](https://about.gitlab.com/handbook/engineering/security/#engaging-the-security-on-call)
*  [Security operations on-call guide](https://about.gitlab.com/handbook/engineering/security/secops-oncall.html#gitlab-security-operations-on-call-guide)

6. Support team contact information
*  [Incident Management Support](https://about.gitlab.com/handbook/support/incident-management/)
*  [On-Call Runbooks](https://about.gitlab.com/handbook/engineering/infrastructure/team/reliability/incident-management/#on-call-runbooks). 

7. Notification to relevant management in the event of a security breach
*  [Security Incident Comms Plan](https://gitlab.com/gitlab-com/gl-security/secops/operations/issues/205)

8. Provisions to contact support team
*  [Support Team function in the handbook](https://about.gitlab.com/handbook/support/) 
*  [Support page](https://about.gitlab.com/support/) contains information to contact the Support team

9. Production Infrastructure related IR Plan: 
*  Production infrastructure incidents are documented in the `production` project
*  The `#incident-management` Slack channel is used for synchronous incident communication via chat
    *  In the channel, the `Production-watch` app monitors the aforementioned `production` project and notifies channel participants of the issue
*  The `Situation Room` permanent Zoom [channel](https://gitlab.zoom.us/j/777594211) is used for synchronous communication via audio/video conference
    *  A link to the channel is included in the description for the `#incident-management` Slack channel

10. Alert mechanisms:
*  [Security Incident and Alert Lifecycle in GitLab](https://gitlab.com/gitlab-com/gl-security/secops/operations/issues/388)



## Framework Mapping
* ISO
  * A.16.1.1
  * A.16.1.2
  * A.16.1.4
  * A.16.1.5
  * A.16.1.6
  * A.16.1.7
* SOC2 CC
  * CC7.4
  * CC7.5
* PCI
  * 11.1.2
  * 11.5.1
  * 12.10
  * 12.10.1
  * 12.10.4
  * 12.10.5
  * 12.10.6
