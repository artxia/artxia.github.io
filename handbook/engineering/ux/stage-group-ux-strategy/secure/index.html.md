---
layout: handbook-page-toc
title: "Secure UX"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Overview
Secure tools help your team follow and enforce security best practices effortlessly as part of the DevOps cycle. The Secure UX team’s goal is to provide the best experience in taking pre-emptive security measures before deploying your code, while the [Defend UX](/handbook/engineering/ux/stage-group-ux-strategy/defend/) team’s goal is to provide the best experience in keeping your application safe after your code is in production. See the [Defend and Secure UX](/handbook/engineering/ux/stage-group-ux-strategy/secure-and-defend/) page for more about our team and how our two teams work together.

### User
We have different user types we consider in our experience design effort. Even when a user has the same title, their responsibilities may vary by organization size, department, org structure, and role. Here are some of the people we are serving:

* [Software Developer](/handbook/marketing/product-marketing/roles-personas/#sasha-software-developer)
* [Development Tech Lead](/handbook/marketing/product-marketing/roles-personas/#delaney-development-team-lead)
* [DevOps Engineer](/handbook/marketing/product-marketing/roles-personas/#devon-devops-engineer)
* [Security Analyst](/handbook/marketing/product-marketing/roles-personas/#sam-security-analyst)
* Compliance Associate
* Security Engineer
* Chief Information Security Officer

Generally, developers are the users of the vulnerability reports in the MR/pipeline while security professionals are the users of the Security Dashboards.

### UX scorecards
##### Primary jobs to be done (JTBD)

**Static Analysis**

| Product Category | JTBD                                                         | Walkthrough                                                  | Recommendations                                              | Score | Rescore |
| ---------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ----- | ------- |
| SAST             | When committing changes to my project, I want to be made aware if I am adding risk through vulnerable code, so that I know my changes can be merged without increasing the risk of my project. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/400) | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/479) | D     |         |

**Composition Analysis**

| Product Category    | JTBD                                                         | Walkthrough                                                  | Recommendations                                              | Score | Rescore |
| ------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ----- | ------- |
| License Compliance  | When new licenses are added to a project I want to be aware so I can commit work that is compliant with my organization's rules. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/478) | [view epic](https://gitlab.com/groups/gitlab-org/-/epics/1618) | D     |         |
| License Compliance  | When my organization has license compliance rules to follow I want to be able to whitelist or blacklist licenses so that I can ensure any new code merged in a project is in compliance. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/402) | [view issue](https://gitlab.com/groups/gitlab-org/-/epics/1618) | F     |         |
| License Compliance  | When a merge request is disallowed, I want to know why, so I can resolve the issue and proceed with the MR. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/534) |                                                              | C     |         |
| License Compliance  | When new vulnerabilities are detected in a merge request, I want to disallow the merge request, so the team can review the vulnerabilities to resolve or decide on the next steps. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/533) |                                                              | D     |         |
| Dependency Scanning | When dependencies are out-of-date, I want to be made aware so I can update them to reduce potential security vulnerabilities and avoid the potentially high cost of larger updates. | [view epic](https://gitlab.com/groups/gitlab-org/-/epics/2396) |                                                              |       |         |
| Dependency Scanning | When my dependencies have reported vulnerabilities, I want to learn more about the information, so I can make an informed decision on taking action against on how to proceed. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/806) |                                                              |       |         |
| Dependency Scanning | When my organization has a compliance policy with dependencies, I want to be aware if I’m breaking a company policy, so I can make sure my project dependencies are in compliance with my org compliance. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/584) |                                                              |       |         |
| Dependency Scanning | When I need to audit 3rd party licenses and dependencies, I want to be able to view them, so I can have them on record for auditing purposes and be able to share them with auditors and customers. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/583) |                                                              |       |         |

**Shared**

| Product Category | JTBD                                                         | Walkthrough                                                  | Recommendations                                              | Score | Rescore |
| ---------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ----- | ------- |
| Shared           |                                                              | [view issue](https://gitlab.com/gitlab-org/gitlab/issues/34368) | [view issue](https://gitlab.com/gitlab-org/gitlab/issues/34369) | C     |         |
| Shared           | When reviewing vulnerabilities for multiple projects, I want to see them all in one location, so that I can prioritize my efforts to resolve or tirage them while seeing the larger picture. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/401) | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/460) | D     |         |
| Shared           | When I want to configure my security tools, I want to be able to configure them to address my own business risk policies, so that I can be assured my company is monitoring risk based on our business risk policies. | [view issue](https://gitlab.com/gitlab-org/gitlab-design/issues/592) |                                                              |       |         |



### Team
* [Valerie Karnes](https://gitlab.com/vkarnes) - UX Manager
* [Tali Lavi](https://gitlab.com/tlavi) - UX Researcher
* [Kyle Mann](https://gitlab.com/kmann) - Sr. Product Designer
* [Camellia Yang](https://gitlab.com/cam.x) - Sr. Product Designer
* [Annabel Dunstone Gray](https://gitlab.com/annabeldunstone) - Product Designer
* [Becka Lippert](https://gitlab.com/beckalippert) - Product Designer

#### Team structure
We've divided the Secure stage into dedicated experience groups to align with a similar [split](/handbook/product/categories/#secure-section) undertaken by our engineering and PM counterparts.

**Security Testing**

| Group | Features                                                     | Designer(s)           |
| ---------------- | ------------------------------------------------------------ | --------------------- |
| Static Analysis | SAST, Secret Detection, Malware Scanning | Becka Lippert         |
| Dynamic Analysis | DAST, IAST | Camellia Yang         |


**Compliance & Auditing**

| Group            | Features                                                     | Designer(s)         |
| --------------------------- | ------------------------------------------------------------ | ------------------- |
| Composition Analysis       | Dependency Scanning, Container Scanning, License Compliance | Kyle Mann           |



The Secure & Defend UX teams work closely together and have shared coverage in the following areas:

- Security Dashboard
- Control Center
- Status, Metrics and Reporting
- Security Configuration

This segmentation gives us a better opportunity to:
- Grow our expertise and knowledge within our subgroup while sharing relevant information with the rest of the team.
- Evolve and maintain relationships with our dedicated engineering team and PMs.
- Serve as the known main point of contact.
- Deeply understand our users' needs by initiating and/or leading research activities specific to our experience group.
- Focus on iterating and progressing our experiences from MVC to Lovable.

Read more about how we've created these dedicated experience groups [here.](https://gitlab.com/gitlab-org/gitlab-design/issues/458)

### How we work
We follow the [GitLab workflow](/handbook/engineering/workflow/#product-development-timeline) with [additional dates](/handbook/engineering/ux/stage-group-ux-strategy/secure-and-defend/) and actions that directly tie to our work. 

### Team meetings
* Secure UX weekly meeting on Wednesdays at 10:30am EST. 
* Product Design and Secure PMs bi-weekly on Wednesdays at 10:00am EST
* Product Design does a bi-weekly grooming session on Tuesdays at 10:30am EST

Our Secure UX weekly meeting is to discuss topics relevant to Secure design, UX, and research. Some example topics could include: 
- Updates on in-flight and planned research
- Updates on design issues
- Design reviews
- Issues that might be at risk or have blockers
- Recently discovered insights while conducting researching
- Updates to our UX Scorecards
- Updates on changes to UX workflows and processes
- Updates on pilot initiatives we are working on
- Strategy iterations

Some topics are better suited for a dedicated meeting, and should be created on an as-needed basis:
- Milestone planning and grooming
- Design critiques 
- Research report readouts 
- Syncing on troublesome issues 

##### Labels we use
We have 4 scoped labels to help us identify which experience group a particular issue falls into and which designer should be subsequently assigned. 

`Secure UX::Shared`
- Issues relating to Status, Reporting & Metrics • IA and Core Functionality.
- Examples: Adding Secure to the left nav, security configurations, Dashboard designs.
- Who to ping: If no designer is assigned: Any Secure designer. If a designer is assigned, ping them in the issue.

`Secure UX::Security Testing & Scanning`
- Issues relating to security testing, scanning, and detection of vulnerabilities or weaknesses.
- Examples: MR Widget security report design, Secret detection, DAST - list of scanned URLs in MR.
- Who to ping: Camellia Yang

`Secure UX::Compliance & Auditing`
- Issues relating to features that support Compliance and/or Auditing activities.
- Examples: Security gates, License Compliance, Dependency list.
- Who to ping: Kyle Mann

`Secure UX:: Prevention & Detection`
- Issues relating to features that support Attack Surface and Attack Emulation
- Examples: Vulnerability Management
- Who to ping: Valerie Karnes (interim)

See our [UX Workflow](https://about.gitlab.com/handbook/engineering/ux/ux-department-workflow/#how-we-use-labels) page for more on how we use labels.

##### Problem and solution validation issues 
When working on a `workflow::problem validation` or `workflow:solution validation` issue requiring implementation in the next 2 releases, ensure there is a placeholder implementation issue. This issue must be attached to the epic, have a tentative milestone and the corresponding labels, particularly the group label, so that it shows up on the issue boards for our counterparts.
### Our strategy
The Secure UX team is working together to [uncover customers core needs](https://gitlab.com/groups/gitlab-org/-/epics/1611), what our users’ workflows looks like, and defining how we can make our users tasks easier. Our strategy involves the following actions:

* [UX Scorecards and recommendations](/handbook/engineering/ux/ux-scorecards/) (quarterly)
* Internal understanding: stakeholder interviews (annually)
* Iterating on Secure product [foundation's document](https://gitlab.com/gitlab-org/gitlab-design/issues/333) (ongoing)
* Performing heuristic evaluations on at least 3 competitors, based competitors the 3 user type is using (annually, ongoing)
* We talk to our customer (ongoing)
* We talk to our users (ongoing)
* We outline current user workflows and improve them (upcoming, ongoing)

Additionally, we value the following:
* Testing our features with usefulness and usability studies
* Drinking our own wine and partnering closely with our internal Security and Compliance teams for feedback and feature adoption
* Partnering with our sales and account team to connect directly with customers and learn why customers did (or didn’t) choose our product
* Collaborating with stakeholders on proof of concept discoveries to better understand future consideration
* Prioritizing issues that are likely to increase our number of active users

The source of truth lives with shipped features, therefore we:
* Make data-driven decisions quickly and thoughtfully
* Optimize to deliver our solutions as soon as possible
* Learn, iterate, test, and repeat

### Follow our work
Our [Secure and Defend UX YouTube channel](https://www.youtube.com/playlist?list=PL05JrBw4t0KrFCe5BgUkzFrZifjforQOz) includes UX Scorecard walkthroughs, UX reviews, group feedback sessions, team meetings, and more.
