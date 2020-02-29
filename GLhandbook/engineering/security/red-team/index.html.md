---
layout: handbook-page-toc
title: "Red Team"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Red Team Overview

GitLab's internal red team extends the objectives of penetration testing by examining the security posture of the organization and their ability to implement effective cyber defenses.

Penetration testing is a specialized type of assessment conducted on information systems or individual system components to identify vulnerabilities that could be exploited by adversaries. Such testing can be used to either validate vulnerabilities or determine the degree of resistance organizational information systems have to adversaries within a set of specified constraints (e.g., time, resources, and/or skills).

Red team exercises provide more comprehensive assessments that reflect real-world conditions over penetration testing. The exercises can further be used to improve security awareness and training and to assess levels of security control effectiveness. GitLab utilizes NIST 800-53 Revision 4 security control CA-8 to define the red team and their mission. The control can be found on [NIST.gov](https://nvd.nist.gov/800-53/Rev4/control/CA-8).

The Red Team operates under a pre-defined set of [rules of engagement](./red-team-roe.html).  The rules of engagement exist to inform GitLab's team members on how the team operates during engagements.  It provides guidelines for determining scope, the ethics we employ during our engagements, how we collaborate as a security team, and how we escalate vulnerabilities and exploits we discover during those engagements.

Further details can be found in the [job family description](/job-families/engineering/security-engineer/#red-team).



## Red Team Operations

Most Red Team operations are planned and approved before any actions are conducted (see [Red Team Open Scope](#red-team-open-scope) for more information). Each operations consists of the following steps:

- [Threat modeling](#threat-modeling)
- [Proposing an operation](#proposing-an-operation)
- [Documenting an operation](#documenting-an-operation)
- [Completing an operation](#completing-an-operation)
- [Delivering a report](#delivering-a-report)
- [Completing redmediation](#completing-redmediation)
- [Completing a restrospective](#completing-a-restrospective)
- [Iterating an operation](#iterating-an-operation)

### Threat Modeling

GitLab maintains a document titled "Data Classification Policy" (team members can find this by searching Google Docs) that categorizes digital assets based on levels of sensitivity.

The Red Team maintains a [secure project](https://gitlab.com/gitlab-red-team/threat-modeling) that builds threat models on top of these classification policies.

While planning a new operation, the first step is to ensure there is alignment with an existing threat model. If not, the existing model should be updated or a new model created.

### Proposing an Operation

Operations should have a clear goal, generally in alignment with one of the following:

- Test a specific detection and/or response capability
- Test a hypothesis that a specific asset in a threat model could be compromised
- Identify a specific security gap in order to justify a new project, policy, or procedure

Any GitLab team member can participate in the proposal or discussion of an upcoming operation. The process is as follows:

- Create a new project in the [Proposed Red Team Operations](https://gitlab.com/gitlab-com/gl-security/gl-redteam/proposed-red-team-operations) group.
    - When you create the project, choose "Create from template", select "Group" templates, and choose "Proposed Operations".
    - Choose the next numerical available from the existing projects and name the new project "Proposed - RTxxx {Short Description}"
- Create an issue in the new project and tag all relevant participants to initiate a discussion.

### Documenting an Operation

Ongoing operations are documented in GitLab projects in a group that is, by default, accessible only to the Red Team. Completed operations will be moved into a group that is accessible to all GitLab team members. Because of this, it is important to keep the following in mind:

- We do not expose identifying information of individual users inside reports.
- We do not expose secrets such as passwords, private keys or API keys.
- We try to write the reports in a way that is consumable to folks of various technical backgrounds.

New operations can be documented as follows:

- Create a new project in the secure [Attack Operations](https://gitlab.com/gitlab-red-team/attack-operations) group.
    - When you create the project, choose "Create from template", select "Group" templates, and choose "Ongoing Operations".
    - Name the operation to match what was proposed in the "Proposing an operation" step above.
- Create a new Google Drive folder under "Red Team Resources" - "AttackOps". This is used for testing artifacts that won't be shared with all GitLab team members once the operation is complete.
- Create a private Slack channel with the operation number and short name for example; rt-001 - parimeter testing. Invite all of Red Team and any other relevant parties. 

### Completing an Operation

An operation may be considered complete after the Red Team has worked through the proposed activities. There may still be work for the Blue Team to do (identifying activities in logs, etc), but this may be more productive after the operation is shared with all GitLab team members.

The following steps should be taken:

- If not already done, grant permission to the relevant Blue Team managers to the ongoing project.
- Open new issues for any specific mitigations or actions that should be put in place and tag the appropriate Blue Team management. 
- Open a new issue, tagging the appropriate Blue Team management and asking for their approval to make the information available to all GitLab team members.
- Wait until the report has been reviewed and all tagged members agree it is safe for release.

### Delivering a Report

At this point, there is value in having the operation accessible to all GitLab team members.

The following steps should be taken:

- Ensure all testing artifacts have been moved to the secure Google Drive location. This is generally items in the project's "Data" folder.
- Create a NEW project in the [Red Team Operations](https://gitlab.com/gitlab-com/gl-security/gl-redteam/completed-red-team-operations) group. This will ensure no sensitive information from git commit histories is accidentally transferred over.
    - When you create the project, choose "Create from template", select "Group" templates, and choose "Completed Operations".
    - Name the operation to match what was proposed in the "Proposing an operation" step above.
- Announce availability of the report in the #security-department Slack channel.

### Completing Redmediation

Red Team will work with the SecOps and other teams as necessary to advise remediations.  We attempt to automate as much of each operation as possible to aid in validating that remediation are, in fact, completed and effective.  At this stage of an operation, all issues related to the operation are properly addressed and validated by the Red Team.

The steps to follow are:
- Red Team members will create an issue called "Remediations" in the new project which was created above, where the report is shared.
    - Relevant SecOps team members will be tagged.
    - All items in the Mitre Attack column chart should be reviewed by SecOps, and the chart completed to indicate what was possible to detect.
    - The checklist provided in the "Recommendations" section of the report should be reviewed by SecOps and modified to state whether each items is addressed, planned to be addressed, not an issue, or an acceptable risk.


### Completing a Restrospective

The Red Team follows GitLab engineerings recommendation to perform regular [retrospectives](/handbook/engineering/management/team-retrospectives/).  These may be performed on a regular cadence or, at minimum, just prior to completing an individual operation depending on need.  The objective is to improve the performance of the team by taking an honest look at what went well, what went poorly, and specific, actionable takeaways to iteratively improve the team in terms of our technical and collaborative skills.

The steps are all outlined in the link above. A new issue should be opened on the operation's project to ensure the retrospective is completed.

### Iterating an Operation

There are multiple reasons to iterate over past/completed operations. The Gitlab environment is changing, new attack techniques are discovered, the Blue Team has improved detections and want to re-assess those regarding past scenarios/operations.  
In those situations, the Red Team is creating a new branch in the chosen past operation project, naming the branch with an increased version number (i.e. v.1.x.x), and configuring the branch as the default one. This way, it is possible to iterate over past operations, make appropriate changes to the new versions and continue the cycle described above. Operations may therefore have multiple branches, having the initial operation in the master branch and the potential multiple versions/iteration that were performed over time on it in separate branches.

## Red Team Open Scope
Some activities are considered open-scope, meaning that they can be conducted at any time, from any source IP address, and against any GitLab-managed asset without prior approval or notification. The output may or may not be included in the reporting for planned operations, depending on the results and whether or not it is helpful to the Blue Team.

This includes:

- Port scanning.
- Web crawling and scraping.
- Manually and programmatically querying the GitLab API.
- Accessing and cloning any public projects, issues, snippets, etc. on www.gitlab.com.
- Accessing other data intended to be open to the public, such as logging platforms.
- Attempting to log in to any publicly-exposed administrative interface with common and default credentials.
- Attempting to validate credential data such as GCP service accounts, SSH keys, and API keys found in public locations.

If these activities are detected by SecOps, they should be treated as potentially malicious and acted upon appropriately. Unless part of a planned operation, there should never be an assumption that suspicious behaviour is a Red Team activity.

Conducting open-source intelligence (OSINT) gathering against non-GitLab managed assets, such as social media sites, is also considered open-scope and may be conducted outside of planned operations.

If an open-scope activity uncovers a vulnerability that puts GitLab at immediate risk of compromise, SecOps will be notified via the official paging procedures.