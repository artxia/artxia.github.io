---
layout: handbook-page-toc
title: "Business Operations"
description: "Business Technologies Group"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

{::options parse_block_html="true" /}

## Purpose
* Architect the data flow and operational processes of the enterprise applications.
* Facilitating systems, workflows and processes for operational teams that work closely together - [Sales](/handbook/sales), [Marketing](/handbook/marketing) and [Customer Success](/handbook/customer-success/).
* Managing or tracking applications, license allocation, admins, and contracts for the tech stack.
* Creating processes, systems and documentation for interdepartmental groups.
* Maintaining an accurate and up-to-date data warehouse (product) and building our analyses for stakeholders in other functions as-needed (service).
     * The result of that service may be a dashboard, which can become a new product that is maintained.
     * As a service function, the data team can often be responsible for support, answering questions such as "Where does a dashboard exist?" or "What does a metric mean?"

## Teams
* [Business Engagement Team](/handbook/business-ops/business_systems/)
    - [open an issue](https://gitlab.com/gitlab-com/business-ops/Issues.help/issues)
* [Data](/handbook/business-ops/data-team/)
* [IT-Operations](/handbook/business-ops/it-ops-team/)
    - [open an issue](https://gitlab.com/gitlab-com/business-ops/itops/issue-tracker/issues)
    - [Access Requests](https://gitlab.com/gitlab-com/access-requests/issues)
    - [Laptop Requests](https://gitlab.com/gitlab-com/laptop-requests)
* [IT Help](/handbook/business-ops/it-help/)
    - [open an issue](https://gitlab.com/gitlab-com/business-ops/bizops-IT-help/hd-issue-tracker/issues)
* [Procurement](/handbook/finance/procurement/)

## Reaching the Teams (internally)
 
- Groups in GitLab
    - `@gitlab-com/business-ops/bizops-IT-help`
    - `@gitlab-com/business-ops/bizops-bsa`
    - `@gitlab-com/business-ops`
    - `@gitlab-com/business-ops/itops`
    - `@gitlab-com/business-ops/procurement`
- Channels in Slack
    - `#business-operations`
    - `#bzo-business-systems-analyst-specialist`
    - `#it_help`
    - `#sysadmin-it`

## Data Quality Process
Data isn't perfect, processes change, people make mistakes. We recognize that and make sure that when we identify an opportunity to be more correct we are moving quickly to resolution.

Our [Data Quality Process](/handbook/business-ops/data-team/data-quality-process/) is meant to capture and document these improvements as they're discovered, and to ensure that communication is made to impacted parties in a timely manner. Learn more about [Data Quality](/handbook/business-ops/data-team/data-quality).

## Business Continuity Plan
GitLab's Business Continuity Plan and associated procedures are documented in our [Business Continuity Plan](/handbook/business-ops/gitlab-business-continuity-plan.html) handbook section.

## Templates
*  [Rollout Plan](https://gitlab.com/gitlab-com/www-gitlab-com/issues/new?issuable_template=public-rollout-plan)
*  [Change Management: Third Party Applications Changes](https://gitlab.com/gitlab-com/business-ops/change-management/issues/new?issuable_template=Third%20Party%20Change%20Management)
*  [Change Management: Internal Tool Changes](https://gitlab.com/gitlab-com/business-ops/change-management/issues/new?issuable_template=Internal_Change_Management)
*  [Software application selection: Request for Proposal](https://docs.google.com/document/d/1_Q2b5opYUQ9TlGmF2vOJ6anu0spVFMkNO6YCR4UjYXM/edit?usp=sharing)
*  [Software application selection: User Stories](https://docs.google.com/spreadsheets/d/1c1R0pqKr8YwXXATzFVEUaofF2luNrHbmcNkKAWisebs/edit?usp=sharing)

## Documentation
*  We work closely with the Marketing and Sales Operations teams. [Learn more](/handbook/business-ops/resources) about Go to Market (GTM) terms, workflows, and contacting these groups.
*  We work closely with the Support, Fulfillment, and Finance teams on the customer portal integration and coordinate changes when needed.
   *  [How to use the Customer Portal-Admin](/handbook/internal-docs/customers-admin/)
   *  [Portal Analysis, Integrations, and Flow](/handbook/business-ops/business_systems/portal/)

## Projects

Business operations projects follow the following structure of stages. 

##### Stage 0 - Assessment `BTG Stage:: 0-Assessment`

This stage is essentially a backlog of proposals which are subject to review.
For example:  New or replacement technology or changes to processes.
* Identify business problem
* Identify value proposition
* Identify dependencies and risks
* Identify executive sponsor
* Identify the resources available for the project
* Evaluate how the project fits into the roadmap
* Proposed timeline

##### Stage 1 - Discovery `BTG Stage:: 1-Discovery`

This stage is for approved projects and identifying the teams and resources dedicated to the project.
* Identify budget
* Create request for proposal
* Consult Security and Procurement Teams
* Identify or create requirements or user stories
* Identify project team
* Identify stakeholders
* Identify technical team
* Identify potential solutions and/or potential vendors

##### Stage 2 - Planning `BTG Stage:: 2-Planning`

In this phase, the project plan is finalized, the scope is identified, and signoff of all business teams is required before moving into implementation.
* gather requirements and user stories
* define what is in and out of scope
* project plan signoff

##### Stage 3 - Action `BTG Stage:: 3-Action`

This stage will be for projects with established plans for building and testing.
* technical team and BSA team designs solution
* technical team builds/implements
* user acceptance testing in stage/sandbox when possible
* training as necessary
* technical team and BSA teams create documentation

##### Stage 4 - Strike `BTG Stage:: 4-Strike`
This stage will be for projects in which all proposed changes have been implemented and the project is wrapped up.

* team retrospective
* audit reporting

## Labels

| Label                            | Description                                                                                     | project/group          | type   |
|:-------                          |:-------                                                                                         |:----------:            |:-------:|
| BusinessOPS                      | BZO is actively involved                                                                        | gitlab-com, gitlab-org | -      |
| BusinessOPS-FYI                  | No direct action needed from Bizops, but awareness for potential support/questions              | gitlab-com, gitlab-org | -      |
| BSA                              | business systems analyst work                                                                   | gitlab-com, gitlab-org | -      |
| BSS                              | business systems specialist work                                                                | gitlab-com, gitlab-org | -      |
| BZO-Features Wanted              |  feature requests | gitlab-org | - |
| IT-Help                          | IT-Help work                                                                                    | gitlab-com, gitlab-org | -      |
| IT-Ops                           | IT-Ops work                                                                                     | gitlab-com, gitlab-org | -      |
| IT:: to do, IT::done             | indicates if IT needs to do work                                                                | gitlab-com             | scoped |
| waiting on license               | cannot complete AR without new license order                                                    | gitlab-com             | -      |
| BizOPS-Status::1-Needs Review    | This has not been looked at.                                                                    | gitlab-com, gitlab-org | scoped |
| BizOPS-Status::2-Backlog         | This work is in the backlog and will be pulled forward when expedient                           | gitlab-com, gitlab-org | scoped |
| BizOPS-Status::3-Working         | This work is in progress.                                                                       | gitlab-com, gitlab-org | scoped |
| BizOPS-Status::4-Change          | This needs a change in order to be approved or merged                                           | gitlab-com, gitlab-org | scoped |
| BizOPS-Status::5-Needs Info      | This needs information from requestor to move forward                                           | gitlab-com, gitlab-org | scoped |
| BizOPS-Status::6-On Hold         | This is on hold for a longer period of time                                                     | gitlab-com, gitlab-org | scoped |
| BizOPS-Status::7-Ready to Deploy | This is ready to be merged or the work executed                                                 | gitlab-com, gitlab-org | -      |
| BizOPS-Status::8-Denied          | This work is considered incomplete and won't be worked on or will not be worked on at this time | gitlab-com, gitlab-org | scoped |
| BizOPS-Priority::1               | Critical                                                                                        | gitlab-com, gitlab-org | scoped |
| BizOPS-Priority::2               | Important not urgent                                                                            | gitlab-com, gitlab-org | scoped |
| BizOPS-Priority::3               | No rush to do, but please do it.                                                                | gitlab-com, gitlab-org | scoped |
| BizOPS-Process                   | Change or addition to process/operations                                                        | gitlab-com, gitlab-org | -      |
| blocker                          | This blocks other work                                                                          | gitlab-com, gitlab-org | -      |
| laptop-request                   | laptop request                                                                                  | gitlab-com, gitlab-org | -      |

## Business Operations Team Organization

![](/handbook/business-ops/images/team1.png)

## Tech Stack
The GitLab [Tech Stack](/handbook/business-ops/tech-stack-applications/) is the approved list of applications. It lists additional information such as the Business Purpose, Who should have access, Contact/Admin, Data Classification, Okta information, and Sox Compliance information.

### Making global changes

To make changes to global configurations or settings for any third-party services in the Tech Stack, please follow the [third-party change management process](/handbook/business-ops/third-party-change-management/).

## Offsites
* [December 2019 Fast Boot, Washington, DC](/handbook/business-ops/offsites)

## Features Wanted
As part of dogfooding, we label features we request or support with the label `BZO-Feature Wanted`. [Check out](https://gitlab.com/groups/gitlab-org/-/boards/1355408) our issue board with this label.

## Business Ops READMEs

Get to know the people who work in GitLab's Business Ops team by visiting our [READMEs](/handbook/business-ops/readmes/).

## What is the difference between Business Ops, Sales Ops, Marketing Ops, Marketing Programs, IT Operations, and IT Helpdesk?

| Business Operations                                                                                                                | Sales Operations                                                                                                                                                 | Marketing Operations                                                                   | Marketing Programs                                                                                                   | IT Operations                                                                                                                                                                                                | IT Helpdesk                                                                                                                             |
| :---                                                                                                                               | :---                                                                                                                                                             | :---                                                                                   | :---                                                                                                                 | :---                                                                                                                                                                                                         | :---                                                                                                                                    |
| Answering the question: “How do we build go-to-market infrastructure to support company growth and pivots?”                        | Quota assignments                                                                                                                                                | Day-to-day management, maintenance and integrations in the entire tech stack           | Day-to-day program and marketer support, including landing pages, Marketo program and Salesforce campaign management | Ensures sufficient controls and streamlines cross-fuctional & cross-system processes, such as onboarding & provisioning                                                                                      | Triage all IT related questions as they arise                                                                                           |
| Strategic analytics and data management                                                                                            | Field &amp; RD Forecasting                                                                                                                                       | New technology review, implementation, customization, documentation and administration | Development and growth of webcast program                                                                            | Build and maintain controls via monitoring, source controls, and automated processes to enable sufficient controls, without the inefficiencies of complete separation of duties via organizational hierarchy | Build a knowledge base of IT practices and pragmatic problem solving in the handbook                                                    |
| Cross-functional process automation and optimization                                                                               | Sales Compensation                                                                                                                                               | Lead management & Data enrichment                                                      | Improve and develop newsletter program                                                                               | Development and maintenance of automation of systems and processes for G&A and with Engineering to eliminate bottlenecks and slow manual activities.                                                         | Account management for password resets and lockout                                                                                      |
| New business technology review                                                                                                     | Sales/Marketing SLAs                                                                                                                                             | Grow the opt-in communication channel                                                  | Support Field Marketing with conference, event & VIP invitation, reminder and follow-up                              |                                                                                                                                                                                                              | On call support for immediate software and hardware issues during local business hours                                                  |
| Holistic business systems administration, development, integration, architecture, and planning around the entire GTM tool stack.   | Ad hoc analysis for CRO                                                                                                                                          | Marketing process design                                                               |                                                                                                                      |                                                                                                                                                                                                              | Diagnose computer errors and provide technical support                                                                                  |
| Prioritization of business operations issues                                                                                       | Sales Process Training/Documentation                                                                                                                             | Marketing & Sales process training and documentation                                   |                                                                                                                      |                                                                                                                                                                                                              | Troubleshoot software and hardware                                                                                                      |
| Prioritization and resolution of non-development customer portal process and support issues                                        | Sales Enablement functions and sales training on process flows                                                                                                   | Prioritization of Marketing-related business operations issues                         |                                                                                                                      |                                                                                                                                                                                                              | Support Weekly IT Onboarding Sessions for new Team Members                                                                              |
| Prioritization and resolution of non-development license app and signups process and support issues                                | Salesforce administration, development, architecture, customizations, and technical documentation                                                                | Marketing tech stack implementations, development and integrations                     |                                                                                                                      |                                                                                                                                                                                                              | Train end-users how to setup and use new technologies                                                                                   |
| Reporting infrastructure                                                                                                           | Evaluate, purchase and implement new technologies into GitLab tech stack                                                                                         | Marketo and Salesforce administration to support marketing activities                  |                                                                                                                      |                                                                                                                                                                                                              | Provide technical support over the phone or Web                                                                                         |
|                                                                                                                                    | Reporting and business analysis related to the sales function                                                                                                    | List pull requests                                                                     |                                                                                                                      |                                                                                                                                                                                                              | Use specialized help desk support software to take control of end-users' computers to troubleshoot, diagnose and resolve complex issues |
|                                                                                                                                    | Prioritization of Sales-related business operations issues.<br>This means consolidating all of the requests from sales into a single funnel with prioritization. |   |   |   |   |

