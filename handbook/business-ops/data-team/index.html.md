---
layout: handbook-page-toc
title: "Data Team"
description: "GitLab Data Team Handbook"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .toc-list-icons .hidden-md .hidden-lg}

{::options parse_block_html="true" /}

----

## <i class="fab fa-gitlab fa-fw color-orange font-awesome" aria-hidden="true"></i>Quick Links
[Primary Project](https://gitlab.com/gitlab-data/analytics/){:.btn .btn-purple-inv}
[dbt docs](https://dbt.gitlabdata.com/){:.btn .btn-purple-inv}
[Sisense](https://app.periscopedata.com/app/gitlab/){:.btn .btn-purple-inv}
[Epics](https://gitlab.com/groups/gitlab-data/-/roadmap?layout=MONTHS&sort=start_date_asc){:.btn .btn-purple}
[OKRs](/company/okrs/){:.btn .btn-purple}
[GitLab Unfiltered YouTube Playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0KrRVTZY33WEHv8SjlA_-keI){:.btn .btn-purple}

## <i class="fas fa-book fa-fw icon-color font-awesome" aria-hidden="true"></i>Data Team Handbook
 
 * [Data Infrastructure](/handbook/business-ops/data-team/data-infrastructure/)
 * [Data Quality](/handbook/business-ops/data-team/data-quality/)
 * [Data Quality Process](/handbook/business-ops/data-team/data-quality-process/)
 * [KPI Definition Mapping](/handbook/business-ops/data-team/metrics/)
 * [Sisense](/handbook/business-ops/data-team/periscope/)
 * [SQL Style Guide](/handbook/business-ops/data-team/sql-style-guide)
 * [dbt Guide](/handbook/business-ops/data-team/dbt-guide)
 * [Python Style Guide](/handbook/business-ops/data-team/python-style-guide)

----

🌎📚💻🏁🛠🔍👑📊 

Many of the sections on this page will have emojis just below the heading. For more information about what they convey [read the documentation page.](/handbook/business-ops/data-team/documentation)

----

## <i class="fas fa-bullhorn fa-fw color-orange font-awesome" aria-hidden="true"></i>Contact Us

* [Data Team Project](https://gitlab.com/gitlab-data/analytics/)
* [#data](https://gitlab.slack.com/messages/data/) on Slack
* [What time is it for folks on the data team?](https://www.worldtimebuddy.com/?pl=1&lid=2950159,6173331,4487042,4644585&h=2950159)

#### Slack 
[🌎📚](/handbook/business-ops/data-team/documentation)

The Data Team uses these channels on Slack:

* [#data](https://gitlab.slack.com/messages/data/) is the primary channel for all of GitLab's data and analysis conversations. This is where folks from other teams can link to their issues, ask for help, direction, and get general feedback from members of the Data Team.
* [#data-daily](https://gitlab.slack.com/messages/data-daily/) is where the Data Team tracks day-to-day productivity, blockers, and fun. Powered by [Geekbot](https://geekbot.com/), it's our asynchronous version of a daily stand-up, and helps keep everyone on the Data Team aligned and informed.
* [#data-lounge](https://gitlab.slack.com/messages/data-lounge/) is for links to interesting articles, podcasts, blog posts, etc. A good space for casual data conversations that don't necessarily relate to GitLab.
* [#business-operations](https://gitlab.slack.com/messages/business-operations/) is where the Data Team coordinates with Business Operations in order to support scaling, and where all Business Operations-related conversations occur.
* [#analytics-pipelines](https://gitlab.slack.com/messages/analytics-pipelines/) is where slack logs for the ELT pipelines are output and is for data engineers to maintain.
* [#dbt-runs](https://gitlab.slack.com/messages/dbt-runs/), like #analytics-pipelines, is where slack logs for [dbt](https://www.getdbt.com/) runs are output. The Data Team tracks these logs and triages accordingly.
* [#data-triage](https://gitlab.slack.com/messages/data-triage/) is an activity feed of opened and closed issues and MR in the data team project.

#### Meetings 
[🌎📚](/handbook/business-ops/data-team/documentation)

The [Data Team's Google Calendar](https://calendar.google.com/calendar?cid=Z2l0bGFiLmNvbV9kN2RsNDU3ZnJyOHA1OHBuM2s2M2VidW84b0Bncm91cC5jYWxlbmRhci5nb29nbGUuY29t) is the SSOT for meetings.
It also includes relevant events in the data space.
Anyone can add events to it.
Many of the events on this calendar, including Monthly Key Reviews, do not require attendance and are FYI events.
When creating an event for the entire Data Team, it might be helpful to check their working hours in Google Calendar and discuss out of working hour meetings ahead of scheduling. Please consider alternating who is meeting after working hours when such meetings are necessary.

The Data Team has the following recurring meetings:
* Data Analyst Team Meeting - [Agenda](https://docs.google.com/document/d/1jOBjCY9-Fp655byvyaPom5Y8a0vH8xvdRrsxz95xfdU/edit?usp=sharing). This meeting occurs weekly on Tuesdays at 1400 UTC.
* Data Engineering Milestone Planning - This meeting is biweekly on the last day of the milestone at 1500 UTC
* Data Engineering Live Learning Session - This meeting is monthly on the first Tuesday that's not a milestone planning.
* Data Ops - Meeting includes Data team, Finance Business Partner, SalesOps Liaison, and FP&A, though anyone is welcome. It occurs weekly on Tuesdays at 1600 UTC.
* Social Calls- Social calls have no agenda. They are 30 minutes weekly to catch up on life and other occurrences. They occur every Tuesday at 1800 UTC.

##### Meeting Tuesday 
[🌎📚](/handbook/business-ops/data-team/documentation)

The team honors *Meeting Tuesday*.
We aim to consolidate all of our meetings into Tuesday, since most team members identify more strongly with the [Maker's Schedule over the Manager's Schedule](http://www.paulgraham.com/makersschedule.html).

<div class="alert alert-purple center">
  <p class="purple center" style="font-size: 34px ; text-align: center ; margin: auto">
    <strong>We <i class="fab fa-gitlab orange font-awesome" aria-hidden="true"></i> Data</strong>
  </p>
</div>
{:.no_toc}

## <i class="fas fa-seedling fa-fw icon-color font-awesome" aria-hidden="true"></i>Charter 
[🌎💡](/handbook/business-ops/data-team/documentation)

The Data Team is a part of the Finance organization within GitLab, but we serve the entire company. We do this by maintaining a data warehouse where information from all business systems are stored and managed for analysis.

Our charter and goals are as follows:

* Build and maintain a centralized data warehouse (Snowflake) that can support data integration, aggregation, and analysis requirements from all functional groups within the company
* Create a common data framework and governance practice
* Create and maintain scalable ELT pipelines that support the data sources needed for analysis
* Work with functional groups through [Finance Business Partners](/handbook/finance/financial-planning-and-analysis/#manager-financial-planning--analysis) to establish the single source of truth (SSOT) for company Key Performance Indicators (KPIs)
* Establish a change management process for source systems, data transformations, and reporting
* Develop a Data Architecture plan in conjunction with functional groups
* Develop a roadmap for systems evolution in alignment with the Company’s growth plans
* Collaborate with infrastructure to maintain our self-hosted Snowplow pipeline for web event analytics
* Create and evangelize analyses produced in our business intelligence tool (Sisense); support others learning to and creating their own analyses

## <i class="far fa-compass fa-fw color-orange font-awesome" aria-hidden="true"></i>Data Team Principles 
[🌎💡](/handbook/business-ops/data-team/documentation)

The Data Team at GitLab is working to establish a world-class data analytics and engineering function by utilizing the tools of DevOps in combination with the core values of GitLab.
We believe that data teams have much to learn from DevOps.
We will work to model good software development best practices and integrate them into our data management and analytics.

A typical data team has members who fall along a spectrum of skills and focus.
For now, the data function at GitLab has Data Engineers and Data Analysts; eventually, the team will include Data Scientists. Review the [team organization section](/handbook/business-ops/data-team/#-team-organization) section to see the make up of the team.

Data Engineers are essentially software engineers who have a particular focus on data movement and orchestration.
The transition to DevOps is typically easier for them because much of their work is done using the command line and scripting languages such as bash and python.
One challenge in particular are data pipelines.
Most pipelines are not well tested, data movement is not typically idempotent, and auditability of history is challenging.

Data Analysts are further from DevOps practices than Data Engineers.
Most analysts use SQL for their analytics and queries, with Python or R.
In the past, data queries and transformations may have been done by custom tooling or software written by other companies.
These tools and approaches share similar traits in that they're likely not version controlled, there are probably few tests around them, and they are difficult to maintain at scale.

Data Scientists are probably furthest from integrating DevOps practices into their work.
Much of their work is done in tools like Jupyter Notebooks or R Studio.
Those who do machine learning create models that are not typically version controlled.
Data management and accessibility is also a concern.

We will work closely with the data and analytics communities to find solutions to these challenges.
Some of the solutions may be cultural in nature, and we aim to be a model for other organizations of how a world-class Data and Analytics team can utilize the best of DevOps for all Data Operations.

Some of our beliefs are:

* Everything can and should be defined in code
* Everything can and should be version controlled
* Data Engineers, Data Analysts, and Data Scientists can and should integrate best practices from DevOps into their workflow
* It is possible to serve the business while having a high-quality, maintainable code base
* Analytics, and the code that supports it, can and should be open source
* There can be a single source of truth for every analytic question within a company
* Data team managers serve their team and not themselves
* [Glue work](https://www.locallyoptimistic.com/post/glue-work/) is important for the health of the team and is recognized individually for the value it provides. [We call this out specifically as women tend to over-index on glue work and it can negatively affects their careers.](https://noidea.dog/glue)
* We focus our limited resources where data will have the greatest impact
* Lead indicators are just as important, if not moreso, than lag indicators
* All business users should be able to learn how to interpret and calculate simple statistics

## <i class="far fa-compass fa-fw icon-color font-awesome" aria-hidden="true"></i> Team Organization 
[🌎📚](/handbook/business-ops/data-team/documentation)

### Data Analysts

The Data Analyst Team operates in a hub and spoke model, where some analysts are part of the central data team (hub) while others are embedded (spoke) or distributed (spoke) throughout the organization.

**Central** - those in this role report to and have their priorities set by the Data team. They currently support those in the Distributed role, cover ad-hoc requests, and support all functional groups (business units).

**Embedded** - those in this role report to the data team but their priorities are set by their functional groups (business units).

**Distributed** - those in this role report to and have their priorities set by their functional groups (business units). However, they work closely with those in the Central role to align on data initiatives and for assistance on the technology stack.

All roles mentioned above have their MRs and dashboards reviews by members in the Data team. Both Embedded and Distributed data analyst or data engineer tend to be subject matter experts (SME) for a particular business unit.

#### Data Support

##### Central 

###### Data Analysts  

| Role | Team Member | Type | Prioritization Owners | 
| ------ | ------ | ------ | ------ |  
| Manager, Data | [@kathleentam](https://gitlab.com/kathleentam) | Central | [@wzabaglio](https://gitlab.com/wzabaglio) | 

[Board](https://gitlab.com/groups/gitlab-data/-/boards/1446961?assignee_username=kathleentam) 

##### Engineering 

| Role | Team Member | Type | Prioritization Owners | 
| ------ | ------ | ------ | ------ | 
| Junior Data Analyst, Engineering | [@ken_aguilar](https://gitlab.com/ken_aguilar) | Embedded | [@kathleentam](https://gitlab.com/kathleentam) |

[Board](https://gitlab.com/groups/gitlab-data/-/boards/1496166?&label_name[]=Engineering)

##### Finance

| Role | Team Member | Type | Prioritization Owners | 
| ------ | ------ | ------ | ------ | 
| Data Analyst, Finance | [@iweeks](https://gitlab.com/iweeks) | Embedded | [@wwright](https://gitlab.com/wwright) |

Board: [Finance Board](https://gitlab.com/groups/gitlab-data/-/boards/1312981?assignee_username=iweeks&&label_name[]=Finance)

##### Marketing

| Role | Team Member | Type | Prioritization Owners | 
| ------ | ------ | ------ | ------ | 
| Marketing Operations Manager | [@rkohnke](https://gitlab.com/rkohnke) | Distributed | [@rkohnke](https://gitlab.com/rkohnke) |
| Junior Data Analyst, Marketing | [@jeanpeguero](https://gitlab.com/jeanpeguero) | Embedded | [@rkohnke](https://gitlab.com/rkohnke) | 

Board: [Marketing Board](https://gitlab.com/groups/gitlab-data/-/boards/1486061?&label_name[]=Marketing)

##### Sales

| Role | Team Member | Type | Prioritization Owners | 
| ------ | ------ | ------ | ------ | 
| Senior Sales Analytics Analyst | [@JMahdi](https://gitlab.com/JMahdi) | Distributed | [@mbenza](https://gitlab.com/mbenza) |
| Senior Sales Analytics Analyst | [@mvilain](https://gitlab.com/mvilain) | Distributed | [@mbenza](https://gitlab.com/mbenza) |
| Senior Sales Analytics Analyst | [@DavidMack](https://gitlab.com/DavidMack) | Distributed | [@mbenza](https://gitlab.com/mbenza) |
| Data Analyst, Sales | [@derekatwood](https://gitlab.com/derekatwood) | Embedded | [@mbenza](https://gitlab.com/mbenza) |


##### People 

| Role | Team Member | Type | Prioritization Owners | 
| ------ | ------ | ------ | ------ | 
| Senior Data Analyst, People Team | [@Pluthra](https://gitlab.com/Pluthra)  | Embedded | [@kathleentam](https://gitlab.com/kathleentam) | 

Board: [People Board](https://gitlab.com/groups/gitlab-data/-/boards/1435002?label_name[]=People)

##### Product

| Role | Team Member | Type | Prioritization Owners | 
| ------ | ------ | ------ | ------ | 
| Sr. Data Analyst, Product | [@mpeychet](https://gitlab.com/mpeychet) | Embedded | Primary (DRI): [@sfwgitlab](https://gitlab.com/sfwgitlab) | 
| Data Analyst, Product | [@eli_kastelein](https://gitlab.com/eli_kastelein) | Embedded | Primary (DRI): [@sfwgitlab](https://gitlab.com/sfwgitlab)| 

Board: [Growth Board](https://gitlab.com/groups/gitlab-data/-/boards/1082241)

### Data Engineers

Though Data Engineers are sometimes given assignments to better support business functions **no members of the the data engineering team are embedded or distributed**. This allows them to focus on our data platform with an appropriate development cadence. 

| Role | Team Member | Assigned Groups | Prioritization Owners | 
| ------ | ------ | ------ | ------ |
| Manager, Data | [@jjstark](https://gitlab.com/jjstark) | GTM | [@wzabaglio](https://gitlab.com/wzabaglio) | 
| Staff Data Engineer | [@tayloramurphy](https://gitlab.com/tayloramurphy) | G&A | [@jjstark](https://gitlab.com/jjstark) |
| Senior Data Engineer | [@m_walker](https://gitlab.com/m_walker) | R&D | [@jjstark](https://gitlab.com/jjstark) |
| Data Engineer | [@msendal](https://gitlab.com/msendal) | TBD | [@jjstark](https://gitlab.com/jjstark) |

---

## <i class="fas fa-chart-line fa-fw color-orange font-awesome" aria-hidden="true"></i> Data Analysis Process

Analysis usually begins with a question.
A stakeholder will ask a question of the data team by creating an issue in the [Data Team project](https://gitlab.com/gitlab-data/analytics/) using the appropriate template.
The analyst assigned to the project may schedule a discussion with the stakeholder(s) to further understand the needs of the analysis, though the preference is always for async communication.
This meeting will allow for analysts to understand the overall goals of the analysis, not just the singular question being asked, and should be recorded.
All findings should be documented in the issue.
Analysts looking for some place to start the discussion can start by asking:
* How can your favorite reports be improved?
* How do you use this data to make decisions?
* What decisions do you make and what information will help you to make them quicker/better?

An analyst will then update the issue to reflect their understanding of the project at hand.
This may mean turning an existing issue into a meta issue or an epic.
Stakeholders are encouraged to engage on the appropriate issues.
The issue then becomes the SSOT for the status of the project, indicating the milestone to which it has been assigned and the analyst working on it, among other things.
The issue should always contain information on the project's status, including any blockers that can help explain its prioritization.
Barring any confidentiality concerns, the issue is also where the final project will be delivered, after peer/technical review.
When satisfied, the analyst will close the issue.
If the stakeholder would like to request a change after the issue has been closed, s/he should create a new issue and link to the closed issue.

The Data Team can be found in the #data channel on slack.

### Working with the Data Team

1. Once a KPI or other Performance Indicate is defined and assigned a prioritization, the metric will need to be added to Sisense by the data team.
2. **Before** syncing with the data team to add a KPI to Sisense, the metric must be:
    * Clearly defined in the relevant section in the handbook and added to the GitLab KPIs [with all of its parts](/handbook/ceo/kpis/#parts-of-a-kpi).
    * Reviewed with the Financial Business Partner for the group.
    * Approved and reviewed by the executive of the group.
3. Once the KPI is ready to be added into Sisense, create an issue on the [GitLab Data Team Issue Tracker](https://gitlab.com/gitlab-data/analytics/issues) using the [KPI Template](https://gitlab.com/gitlab-data/analytics/blob/master/.gitlab/issue_templates/KPI%20Template.md) or [PI Request Template](https://gitlab.com/gitlab-data/analytics/blob/master/.gitlab/issue_templates/Visualization%20or%20Dashboard-%20New%20Request.md).
    * The Data team will verify the data sources and help to find a way to automate (if necessary).
    * Once the import is complete, the data team will present the information to the owner of the KPI for approval who will document in the relevant section of the handbook.

### SLO for inbound requests 
* One of the Data Analyst performance indicators is to have [% of issues requested triaged with first response within 36 hours (per business unit)](/handbook/business-ops/metrics/#percent--of-issues-requested-triaged-with-first-response-within-36-hours-per-business-unit)
* We aim to complete each request at a an SLO is < 4 weeks (2 milestones).

### Can I get an update on my dashboard?

The data team's priorities come from our OKRs.
We do our best to service as many of the requests from the organization as possible.
You know that work has started on a request when it has been assigned to a milestone.
Please communicate in the issue about any pressing priorities or timelines that may affect the data team's prioritization decisions.
Please do not DM a member of the data team asking for an update on your request.
Please keep the communication in the issue.

## <i class="fas fa-tasks fa-fw icon-color font-awesome" aria-hidden="true"></i>How we Work

### Documentation

The data team, like the rest of GitLab, works hard to document as much as possible. We believe [this framework](https://www.divio.com/blog/documentation/) for types of documentation from Divio is quite valuable. For the most part, what's captured in the handbook are tutorials, how-to guides, and explanations, while reference documentation lives within in the primary analytics project. We have aspirations to tag our documentation with the appropriate function as well as clearly articulate the [assumed audiences](https://v4.chriskrycho.com/2018/assumed-audiences.html) for each piece of documentation.

### OKR Planning

Data Team OKRs are derived from the higher level BizOps/Finance OKRs as well as the needs of the team.
At the beginning of a FQ, the team will outline all actions that are required to succeed with our KRs *and* in helping other teams measure the success of their KRs.
The best way to do that is via a team brain dump session in which everyone lays out all the steps they anticipate for each of the relevant actions.
This is a great time for the team to raise any blockers or concerns they foresee.
These should be recorded for future reference.

These OKRs drive ~60% of the work that the central data team does in a given quarter.
The remaining time is divided between urgent issues that come up and ad hoc/exploratory analyses.
Specialty data analysts (who have the title "Data Analyst, Specialty") should have a similar break down of planned work to responsive work, but their priorities are set by their specialty manager.

### Milestone Planning

The data team currently works in two-week intervals, called milestones.
Milestones start on Tuesdays and end on Mondays.
This discourages last-minute merging on Fridays and allows the team to have milestone planning meetings at the top of the milestone.

Milestones may be three weeks long if they cover a major holiday or if the majority of the team is on vacation or at Contribute.
As work is assigned to a person and a milestone, it gets a weight assigned to it.

Milestone planning should take into consideration:
* vacation timelines
* conference schedules
* team member availability
* team member work preferences (specialties are different from preferences)

The milestone planning is owned by the Manager, Data. 

The timeline for milestone planning is as follows:
* Meeting Preparation - Responsible Party: Milestone Planner
   * Investigate and flesh out open issues.
   * Assign issues to the milestone based on alignment with the Team Roadmap.
   * Note: Issues are not assigned to an individual at this stage, except where required.

| Day | Current Milestone | Next Milestone |
| ---- | ---- | ---- |
| 0 - 1st Wednesday |  **Milestone Start** <br><br>[Roll Milestone](https://gitlab.com/gitlab-data/analytics/issues/new?issuable_template=Milestone%20Rolling) | - |
| 7 - 2nd Tuesday | **Midpoint** <br><br>Any issues that are at risk of slipping from the milestone must be raised by the assignee | - | 
| 10 - 2nd Friday | **The last day to submit MRs for review** <br><br>MRs must include documentation and testing to be ready to merge <br><br>No MRs are to be merged on Fridays | **Milestone is roughly final** <br><br>Milestone Planner distributes issues to team members, with the appropriate considerations and preferences |
| 13 - 2nd Monday | **Last day of Milestone** <br><br>Ready MRs can be merged | - |
| 14 - 2nd Tuesday | **Meeting Day** <br><br> All unfinished issues either need to be removed from milestones or rolled to the next | **Milestone Planning** <br><br> Scheduled DE meeting with a tactical discussion of the work to be completed next Milestone. Stakeholders and submitters are updated with what will or wont be added to the next milestone. |

The short-term goal of this process is to improve our ability to plan and estimate work through better understanding of our velocity.
In order to successfully evaluate how we're performing against the plan, any issues not raised at the T+7 mark should not be moved until the next milestone begins.

The work of the data team generally falls into the following categories:
* Infrastructure
* Analytics
   * Central Team
   * Specialist Team
* Housekeeping

During the milestone planning process, we point issues.
Then we pull into the milestone the issues expected to be completed in the timeframe.
Points are a good measure of consistency, as milestone over milestone should share an average.
Then issues are prioritized according to these categories.

Issues are not assigned to individual members of the team, except where necessary, until someone is ready to work on it.
Work is not assigned and then managed into a milestone.
Every person works on the top priority issue for their job type.
As that issue is completed, they can pick up the next highest priority issue.
People will likely be working on no more than 2 issues at a time.

Given the power of the [Ivy Lee](https://jamesclear.com/ivy-lee) method, this allows the team to collectively work on priorities as opposed to creating a backlog for any given person.
As a tradeoff, this also means that every time a central analyst is introduced to a new data source their velocity may temporarily decrease as they come up to speed;
the overall benefit to the organization that any analyst can pick up any issue will compensate for this, though.
Learn [how the product managers groom issues](https://www.youtube.com/watch?v=es-SuhU_6Rc).

Data Engineers will work on Infrastructure issues.
Data Analysts, Central and sometimes Data Engineers work on general Analytics issues.
Data Analysts, <Specialty> work on <Specialty> analyses, e.g Growth, Finance, etc.

There is a demo of [what this proposal would look like in a board](https://gitlab.com/groups/gitlab-data/-/boards/1187725).

This approach has many benefits, including:
1. It helps ensure the highest priority projects are being completed
2. It can help leadership identify issues that are blocked
3. It provides leadership view into the work of the data team, including specialty analysts whose priorities are set from outside the data function
4. It encourages consistent [throughput](/handbook/engineering/management/throughput/) from team members
5. It makes clear to stakeholders where their ask is in priority
6. It helps alleviate the pressure of planning the next milestone, as issues are already ranked

### Issue Types

There are three *general* types of issues:
* Discovery
* Introducing a new data source
* Work

Not all issues will fall into one of these buckets but 85% should.

##### Discovery issues
Some issues may need a discovery period to understand requirements, gather feedback, or explore the work that needs to be done.
Discovery issues are usually 2 points.

##### Introducing a new data source
Introducing a new data source requires a *heavy lift* of understanding that new data source, mapping field names to logic, documenting those, and understanding what issues are being delivered.
Usually introducing a new data source is coupled with replicating an existing dashboard from the other data source.
This helps verify that numbers are accurate and the original data source and the data team's analysis are using the same definitions.

##### Work
This umbrella term helps capture:
* inbound requests from GitLab team-members that usually materialize into a dashboard
* housekeeping improvements/technical debt from the data team
* goals of the data team
* documentation notes

It is the responsibility of the assignee to be clear on what the scope of their issue is.
A well-defined issue has a clearly outlined problem statement. Complex or new issues may also include an outline (not all encompassing list) of what steps need to be taken.
If an issue is not well-scoped as its assigned, it is the responsibility of the assignee to understand how to scope that issue properly and approach the appropriate team members for guidance early in the milestone.

### Issue Pointing

**Issue pointing captures the complexity of an issue, not the time it takes to complete an issue. That is why pointing is independent of who the issue assignee is.**

* Refer to the table below for point values and what they represent.
* We size and point issues as a group.
* Effective pointing requires more fleshed out issues, but that requirement shouldn't keep people from creating issues.
* When pointing work that happens outside of the Data Team projects, add points to the issue in the relevant Data Team project and ensure issues are cross-linked.

| Weight | Description |
| ------ | ------ |
| Null | Meta and Discussions that don't result in an MR |
| 0 | Should not be used. |
| 1 | The simplest possible change including documentation changes. We are confident there will be no side effects. |
| 2 | A simple change (minimal code changes), where we understand all of the requirements. |
| 3 | A typical change, with understood requirements but some complicating factors|
| 5 | A more complex change. Requirements are *probably* understood or there might be dependencies outside the data-team. |
| 8 | A complex change, that will involve much of the codebase or will require lots of input from others to determine the requirements. |
| 13 | A significant change that has dependencies and we likely still don't understand all of the requirements. It's unlikely we would commit to this in a milestone, and the preference would be to further clarify requirements and/or break into smaller Issues. |

### Issue Labeling

Think of each of these groups of labels as ways of bucketing the work done. All issues should get the following classes of labels assigned to them:

* Who (Purple): Team for which work is primarily for (Data, Finance, Sales, etc.)
* What - Data or Tool
  * Data (Light Green): Data being touched (Salesforce, Zuora, Zendesk, Gitlab.com, etc.)
  * Tool (Light Blue) (Sisense, dbt, Stitch, Airflow, etc.)
* Where (Brown): Which part of the team performs the work (Analytics, Infrastructure, Housekeeping)
* How (Orange): Type of work (Documentation, Break-fix, Enhancement, Refactor, Testing, Review)

Optional labels that are useful to communicate state or other priority
* State (Red) (Won't Do, Blocked, Needs Consensus, etc.)
* Workflow Status (Workflow::Triage, Workflow::Ready, Workflow:: In Progress, Workflow:: Verification, Workflow:: Waiting)
* Inbound: For issues created by folks who are not on the data team; not for asks created by data team members on behalf of others

### Daily Standup

Members of the data team use Geekbot for our daily standups.
These are posted in [#data-daily](https://gitlab.slack.com/archives/CGG0VRJJ0/p1553619142000700).
When Geekbot asks, "What are you planning on working on today? Any blockers?" try answering with specific details, so that teammates can proactively unblock you.
Instead of "working on Salesforce stuff", consider "Adding Opportunity Owners for the `sfdc_opportunity_xf` model`."
There is no pressure to respond to Geekbot as soon as it messages you.
Give responses to Geekbot that truly communicate to your team what you're working on that day, so that your team can help you understand if some priority has shifted or there is additional context you may need.

### Merge Request Workflow

*Ideally*, your workflow should be as follows:
1. Confirm you have access to the analytics project. If not, request Developer access so you can create branches, merge requests, and issues.
1. Create an issue, open an existing issue, or assign yourself to an existing issue. The issue is assigned to the person(s) who will be doing the work.
1. Add appropriate labels to the issue (see above)
1. Open an MR from the issue using the "Create merge request" button. This automatically creates a unique branch based on the issue name. This marks the issue for closure once the MR is merged.
1. Push your work to the branch
1. Update the MR with an [appropriate template](https://gitlab.com/gitlab-data/analytics/-/tree/master/.gitlab%2Fmerge_request_templates). Our current templates are:
  * **dbt Model Changes** - used for any change involving dbt. Analysts will most often use this one
  * **add_manifest_tables** - for adding tables to pgp extract
  * **periscope** - for getting a Periscope dashboard reviewed
  * **python_changes** - for general changes to Python code
  * **All Other Changes** - for work that doesn't generally fall into these categories
1. Run any relevant jobs to the work being proposed
  * e.g. if you're working on dbt changes, run the job most appropriate for your changes. See the [dbt changes MR template checklist](https://gitlab.com/gitlab-data/analytics/blob/master/.gitlab/merge_request_templates/dbt%20Model%20Changes.md) for a list of jobs and their uses.
1. Document in the MR description what the purpose of the MR is, any additional changes that need to happen for the MR to be valid, and if it's a complicated MR, how you verified that the change works. See [this MR](https://gitlab.com/gitlab-data/analytics/merge_requests/658) for an example of good documentation. The goal is to make it easier for reviewers to understand what the MR is doing so it's as easy as possible to review.
1. Assign the MR to a peer to have it reviewed. If assigning to someone who can merge, either leave a comment asking for a review without merge, or you can simply leave the `WIP:` label.
  * Note that assigning someone an MR means action is required from them.
  * The peer reviewer should use the native approve button in the MR after they have completed their review and approve of the changes in the MR.
  * Adding someone as an approver is a way to tag them for an FYI. This is similar to doing `cc @user` in a comment.
  * After approval, the peer reviewer should send the MR back to the author to decide what needs to happen next. The reviewer should not be responsible for the final tasks. The author is responsible for finalizing the checklist, closing threads, removing WIP, and getting it in a merge-ready state.
1. Once it's ready for further review and merging, remove the `WIP:` label, mark the branch for deletion, mark squash commits, and assign to the project's maintainer. Ensure that the attached issue is appropriately labeled and pointed.

Other tips:
1. The Merge Request Workflow provides clear expectations; however, there is some wiggle room and freedom around certain steps as follows.
  * For simple changes, it is the MR author who should be responsible for closing the threads. If there is a complex change and the concern has been addressed, either the author or reviewer could resolve the threads if the reviewer approves.
1. Reviewers should have 48 hours to complete a review, so plan ahead with the end of the milestone.
1. When possible, questions/problems should be discussed with your reviewer before submitting the MR for review. Particularly for large changes, review time is the least efficient time to have to make meaningful changes to code, because you’ve already done most of the work!

### YouTube

We encourage everyone to record videos and post to GitLab Unfiltered. The [handbook page on YouTube](/handbook/communication/youtube/#post-everything) does an excellent job of telling why we should be doing this. If you're uploading a video for the data team, be sure to do the following extra steps:

* Add `data` as a video tag
* Add it to the [Data Team playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0KrRVTZY33WEHv8SjlA_-keI)
* Share the video in #data channel on slack

## <i class="fas fa-cubes fa-fw color-orange font-awesome" aria-hidden="true"></i>Our Data Stack

We use GitLab to operate and manage the analytics function.
Everything starts with an issue.
Changes are implemented via merge requests, including changes to our pipelines, extraction, loading, transformations, and parts of our analytics.

|Stage|Tool|
|:-|:-:|
|Extraction|Stitch, Fivetran, and Custom|
|Loading|Stitch, Fivetran, and Custom|
|Orchestration|Airflow|
|Storage|Snowflake|
|Transformations|dbt and Python scripts|
|Analysis| Sisense For Cloud Data Teams‎ |

## <i class="fas fa-exchange-alt fa-fw icon-color font-awesome" aria-hidden="true"></i>Extract and Load

We currently use [Stitch](https://www.stitchdata.com) and [Fivetran](https://fivetran.com/) for most of our data sources. These are off-the-shelf ELT tools that remove the responsibility of building, maintaining, or orchestrating the movement of data from some data sources into our Snowflake data warehouse. We run a full-refresh of all of our Stitch/Fivetran data sources at the same time that we rotate our security credentials (approx every 90 days). Prior to running a full refresh we will drop all of the tables.

| Data Source       | Pipeline  | Replication Frequency | [Quality Rating](/handbook/business-ops/data-team/data-quality/#extraction-data-quality) |
|-------------------|-----------|-----------------|-----------------|
| BambooHR          | Airflow   | 12 hour intervals for all time | 2 |
| CloudSQL Postgres | Stitch    |   | 2 |
| Customer DB       | Postgres_Pipeline   |   | 2 |
| Gitter            |           |  not updated |   |
| GitLab.com        | Postgres_Pipeline |  6 hour intervals | 2 |
| Google Analytics 360 | Fivetran | 6 hour intervals | 2 |
| Greenhouse        | Airflow (custom script) | Once per day | 2 |
| License DB        | Postgres_Pipeline   | 6 hour intervals | 2 |
| Marketo           |           | not updated |   |
| Netsuite          | Fivetran  | 6 hour intervals - Backfilled from January 1, 2013| 2 |
| Part of Product MRs | Airflow   | 1 day intervals | 1 |
| Salesforce (SFDC) | Stitch    | 1 hour intervals - Backfilled from January 1, 2013| 2 |
| SheetLoad         | SheetLoad | 24 hours | 2 |
| Snowplow          | Snowpipe  | Continuously loaded | 2 |
| Version DB        | Postgres_Pipeline   | 6 hour intervals | 2 |
| Zendesk           | Stitch    | 1 hour intervals - Backfilled from January 1, 2013| 2 |
| Zuora             | Stitch    | 30 minute intervals - Backfilled from January 1, 2013| 2 |

### SLOs (Service Level Objectives) by Data Source

This is the lag between real-time and the analysis displayed in the [data visualization tool](#visualization).

| Data Source       | SLO  |
|--------------------|-----------|
| BambooHR           | 1 day |
| Clearbit           | None |
| Airflow DB         | 9 hours |
| CI Stats DB        | None - Owned by [GitLab.com Infrastructure Team](/handbook/engineering/infrastructure/), intermittently unavailable |
| Customer DB        | None - Owned by [GitLab.com Infrastructure Team](/handbook/engineering/infrastructure/), intermittently unavailable |
| DiscoverOrg        | None |
| GitLab.com         | None - Owned by [GitLab.com Infrastructure Team](/handbook/engineering/infrastructure/), intermittently unavailable |
| GitLab Profiler DB | None - Owned by [GitLab.com Infrastructure Team](/handbook/engineering/infrastructure/), intermittently unavailable |
| Google Analytics 360  | 1 day | 
| Greenhouse         | 2 days |
| License DB         | None - Owned by [GitLab.com Infrastructure Team](/handbook/engineering/infrastructure/), intermittently unavailable |
| Marketo            | None |
| Netsuite           | 1 day |
| Salesforce (SFDC)  | 1 day|
| SheetLoad          | 2 days |
| Snowplow           | 1 day |
| Version DB         | None - Owned by [GitLab.com Infrastructure Team](/handbook/engineering/infrastructure/), intermittently unavailable |
| Zendesk            | 1 day |
| Zuora              | 1 day |


### Adding new Data Sources and Fields

Process for adding a new data source:
* Create a new issue in the Analytics project requesting for the data source to be added:
  * Document what tables and fields are required
  * Document the questions that this data will help answer
* Create an issue in the [Security project](https://gitlab.com/gitlab-com/gl-security/engineering/issues/) and cross-link to the Analytics issue.
  * Tag the Security team `gitlab-com/gl-security`

To add new fields to the BambooHR extract:

* Create a new issue in the Analytics project using the BambooHR template
* Gain approval from a Data Team Manager and the Compensation and Benefits Manager
* Once approved, assign to the Compensation and Benefits Manager and a Data Engineer who will verify the extract

### Data Team Access to Data Sources

In order to integrate new data sources into the data warehouse, specific members of the Data team will need admin-level access to data sources, both in the UI and through the API.
We need this admin-level access through the API in order to pull all the data needed to build the appropriately analyses and through the UI to compare the results of prepared analyses to the UI.

Sensitive data sources can be limited to no less than 1 data engineer and 1 data analyst having access to build the require reporting.
In some cases, it may only be 2 data engineers.
We will likely request an additional account for the automated extraction process.

Sensitive data is locked down through the security paradigms listed below;
Sisense will never have access to sensitive data, as Sisense does not have access to any data by default.
Sisense's access is always explicitly granted.


### Using SheetLoad

SheetLoad is the process by which a Google Sheets and CSVs from GCS or S3 can be ingested into the data warehouse.

Technical documentation on usage of sheetload can be found in the [readme] in the data team project(https://gitlab.com/gitlab-data/analytics/tree/master/extract/sheetload).

If you want to import a Google Sheet or CSV into the warehouse, please [make an issue](https://gitlab.com/gitlab-data/analytics/issues/new?issue%5Bassignee_id%5D=&issue%5Bmilestone_id%5D=) in the data team project using the "CSV or GSheets Data Upload" issue template. This template has detailed instructions depending on the type of data you want to import and what you may want to do with it.

#### Things to keep in mind about SheetLoad
{: #mind-about-sheetload}
We strongly encourage you to consider the source of the data when you want to move it into a spreadsheet. SheetLoad should primarily be used for data whose canonical source is a spreadsheet - i.e. Sales quotas. If there is a source of this data that is not a spreadsheet you should at least make an issue to get the data pulled automatically. However, if the spreadsheet is the SSOT for this data, then we can get it into the warehouse and modeled appropriately via dbt.

We do understand, though, that there are instances where a one-off analysis is needed based on some data in a spreadsheet and that you might need to join this to some other data already in the warehouse. We offer a "Boneyard" schema where you can upload the spreadsheet and it will be available for querying within Sisense. We call it Boneyard to highlight that this data is relevant only for an *ad hoc/one off* use case and will become stale within a relatively short period of time.

SheetLoad is designed to make the table in the database a mirror image of what is in the sheet from which it is loading. Whenever SheetLoad detects a change in the source sheet it will forcefully drop the database table and recreate it in the image of the updated spreadsheet. This means that if columns are added, changed, etc. it will all be reflected in the database.

Except for where absolutely not possible, it is best that the SheetLoad sheet import from the original Google Sheet directly using the `importrange` function. This allows you to leave the upstream sheet alone and while enabling you to format the sheetload version to be plain text. Any additional data type conversions or data cleanup can happen in the base dbt models. (This does not apply to the Boneyard.)

### Snowplow Infrastructure

Refer to the [Snowplow Infrastructure page](/handbook/business-ops/data-team/snowplow) for more information on our setup.


### Data Source Overviews
  * [Customer Success Dashboards](https://drive.google.com/open?id=1FsgvELNmQ0ADEC1hFEKhWNA1OnH-INOJ)
  * [Netsuite](https://www.youtube.com/watch?v=u2329sQrWDY)
    * [Netsuite and Campaign Data](https://drive.google.com/open?id=1KUMa8zICI9_jQDqdyN7mGSWSLdw97h5-)
  * [Version (pings)](https://drive.google.com/file/d/1S8lNyMdC3oXfCdWhY69Lx-tUVdL9SPFe/view)
    * Note that up until October 2019, the data team referred to the entire **version** data source as "pings". However, usage ping is only one subset of the version data source which is why we now use "version" or "version app" to refer to the version.gitlab.com *data source* and "usage data" or "usage pings" or "pings" to refer to the [specific usage data feature](https://docs.gitlab.com/ee/user/admin_area/settings/usage_statistics.html) of the version data source.
  * [Salesforce](https://youtu.be/KwG3ylzWWWo)
  * [Zendesk](https://drive.google.com/open?id=1oExE1ZM5IkXcq1hJIPouxlXSiafhRRua)

## <i class="fas fa-clock fa-fw color-orange font-awesome" aria-hidden="true"></i> Orchestration

We use Airflow on Kubernetes for our orchestration. Our specific setup/implementation can be found [here](https://gitlab.com/gitlab-data/data-image). Also see the [Data Infrastructure](/handbook/business-ops/data-team/data-infrastructure/) page for more information.

## <i class="fas fa-database fa-fw icon-color font-awesome" aria-hidden="true"></i> Data Warehouse

We currently use [Snowflake](https://docs.snowflake.net/manuals/index.html) as our data warehouse.

### Warehouse Access

To gain access to the data warehouse:
* Create an issue in the [access requests project](https://gitlab.com/gitlab-com/access-requests) documenting the level of access required.
* Do not request a shared account - each account must be tied to a user.
* We loosely follow the paradigm explained in [this blog post](https://blog.fishtownanalytics.com/how-we-configure-snowflake-fc13f1eb36c4) around permissioning users.

### Snowflake Permissions Paradigm

Goal: Mitigate risk of people having access to sensitive data.

We currently use [Meltano](https://meltano.com/)'s Permission Bot in to help manage permissions for Snowflake.
Documentation on the permission bot is in [the Meltano docs](https://meltano.com/docs/meltano-cli.html#meltano-permissions). Our configuration file for our Snowflake instance is stored in [this roles.yml file](https://gitlab.com/gitlab-data/analytics/blob/master/load/snowflake/roles.yml).

There are four things that we need to manage:
* databases - who has access to which ones
* roles
* user roles (mapped directly to users)
* warehouses

There are currently this many primary analyst roles in Snowflake:
* analyst_core
* analyst_engineering
* analyst_finance
* analyst_growth
* analyst_infrastructure
* analyst_marketing
* analyst_people
* analyst_sales
* analyst_sensitive

Analysts are assigned to relevant roles and are explicitly granted access to the schemas they need.

Two notes of the permission bot:
* things that exist but aren't in the file don't lead to errors
* it does not _delete_ objects when removing from the file - it will generate revoke commands

Common errors that are encountered:
* If there is a role referenced but not defined then it will error and the solution is to properly fix the config file
* If a role is defined in the spec but does not exist in Snowflake then it will error. The solution is to create the rle in Snowflake.

<div class="panel panel-success">
**Managing Roles for Snowflake**
{: .panel-heading}
<div class="panel-body">

Here are the proper steps for provisioning a new user and user role:
 
* Make sure we have an issue in the Gitlab Data Team project linking the original request with the `Provisioning` label applied
* Login to Snowflake and switch to `securityadmin` role
  * All roles should be under `securityadmin` ownership
* Copy the [`user_provision.sql`](https://gitlab.com/gitlab-data/analytics/-/blob/master/load/snowflake/user_provision.sql) script and replace the email, firstname, and lastname values in the initial block
* If a password is needed, use [Password Generator](https://passwordsgenerator.net/) to create one
  * Send username and password credentials to user with [One Time Secret](https://onetimesecret.com/) or via Slack
* Document in Snowflake config.yml permissions file
  * Add the user and user role you created
  * Assign the user role to new user
  * Assign any additional roles to user
* Ensure the user is assigned the application in Okta 
</div>
</div>

### Compute Resources

Compute resources in Snowflake are known as "warehouses".
To better track and monitor our credit consumption, we have created several warehouses depending on who is accessing the warehouse.
The names of the warehouse are appended with their size (`analyst_xs` for extra small)

* `admin` - This is for permission bot and other admin tasks
* `airflow_testing_l` - For testing Airflow locally
* `analyst_*` - These are for Data Analysts to use when querying the database or modeling data
* `engineer_*` - These are for Data Engineers and the Manager to use when querying the database or modeling data
* `fivetran_warehouse` - This is exclusively for Fivetran to use
* `gitlab_postgres` - This is for extraction jobs that pull from GitLab internal Postgres databases
* `loading` - This is for our Extract and Load jobs
* `merge_request_*` - These are scoped to GitLab CI for dbt jobs within a merge request
* `reporting` - This is for the BI tool for querying
* `stitch` - This is exclusively for Stitch to use
* `target_snowflake` - This is for the Meltano team to test their Snowflake loader
* `transforming_*` - These are for production dbt jobs

### Data Storage

We currently use two databases: `raw` and `analytics`. The former is for extracted and loaded data; the latter is for data that is ready for analysis (or getting there).

All database clones are wiped away every week.

#### Raw

* Raw may contain sensitive data, so permissions need to be carefully controlled
* Data is stored in different schemas based on the source
* User access can be controlled by schema and tables

#### Analytics

With the exception of the [`boneyard` schema](/handbook/business-ops/data-team/#mind-about-sheetload), all schemas are controlled by dbt. 
See the [dbt guide](/handbook/business-ops/data-team/dbt-guide) for more information.

### Timezones

All timestamp data in the warehouse should be stored in UTC. The [default timezone](https://docs.snowflake.net/manuals/sql-reference/parameters.html#timezone) for a Snowflake sessions is PT, but we have overridden this so that UTC is the default. This means that when `current_timestamp()` is queried, the result is returned in UTC.

[Stitch explicitly converts](https://www.stitchdata.com/docs/data-structure/snowflake-data-loading-behavior#%0A%0A%09%0A%09%09%09%09%09a-column-contains-timestamp-data%0A%0A%09%09%09%09%0A%0A%0A) timestamps to UTC. Fivetran does this as well (confirmed via support chat).

### Snapshots
{: #snapshots-definition}
[📊📚](/handbook/business-ops/data-team/documentation)

We use the term snapshots in multiple places throughout the data team handbook and the term can be confusing depending on the context. Snapshots as defined by the dictionary is "a record of the contents of a storage location or data file at a given time". We strive to use this definition whenever we use the word. 

#### dbt 

The most common usage is in reference to [dbt snapshots](https://docs.getdbt.com/docs/snapshots). When dbt snapshots is run, it takes the state of the data based on a query specified by the user and updates a table that contains the full history of the state of the data. It has `valid_to` and `valid_from` fields indicating the time period for which that particular snapshot is valid. See the [dbt snapshots](/handbook/business-ops/data-team/dbt-guide/#snapshots) section in our dbt guide for more technical information.

The tables generated and maintained by dbt snapshots are the raw historical snapshot tables. We will build downstream models on top of these raw historical snapshots for further querying. The [snapshots folder](https://gitlab.com/gitlab-data/analytics/tree/master/transform/snowflake-dbt/snapshots) is where we store the dbt models. One common model we may build is one that generate a single entry (i.e. a single snapshot) for a given day; this is useful when there are multiple snapshots taken in a 24 hour period. We also will build models to return the most current snapshot from the raw historical table.

#### Other uses

Our Greenhouse data can be thought of as a snapshot. We get a daily database dump provided by Greenhouse that we load into Snowflake. If we start taking dbt snapshots of these tables then we would be creating historical snapshots of the Greenhouse data.

The extracts we do for some [yaml files](https://gitlab.com/gitlab-data/analytics/tree/master/extract/gitlab_data_yaml) and for BambooHR can also be thought of as snapshots. This extraction works by taking the full file/table and storing it in its own, timestamped row in the warehouse. This means we have historical snapshots for these files/tables but these are not the same kind of snapshot as dbt. We'd have to do additional transformations to get the same `valid_to` and `valid_from` behavior.

#### Language

* Snapshot - The state of data at a specific point in time
* Take a snapshot - Run the job that takes the state of the data currently and stores it. Can be used in the dbt context. Not recommended to reference our yaml extract jobs - these would be "run the extract".
* Historical snapshots - A table that contains data for a given source table at multiple points in time. Most commonly used to reference dbt-generated snapshot tables. Can also be used to reference the yaml extract tables.
* Latest snapshot - The most current state of the data we have stored. For dbt snapshots these are the records that have null for the `valid_to`. For BambooHR and yaml extracts these correspond to the last time the extraction job was run. For Greenhouse raw, this represents the data as it is in the warehouse. Were we to start taking snapshots of the Greenhouse data the speaker would have to clarify if they mean the raw table or the latest record in the historical snapshots table.

### Backups

For an extra layer of robustness, we backup data from the warehouse into GCS (Google Cloud Storage). We execute the jobs using a dbt's [`run-operation`](https://docs.getdbt.com/docs/using-operations) capabilities. Currently, we backup all of our snapshots daily and retain them for a period of 1 month. We implemented the basic instructions outlined in [this Calogica blog post](https://calogica.com/sql/snowflake/dbt/2019/09/09/snowflake-backup-s3.html).

## <i class="fas fa-cogs fa-fw icon-color font-awesome" aria-hidden="true"></i>Transformation

We use [dbt](https://www.getdbt.com/) for all of our transformations. 
See our [dbt guide](/handbook/business-ops/data-team/dbt-guide) for more details on why and how we use this tool.

## <i class="fas fa-chart-bar fa-fw icon-color font-awesome" aria-hidden="true"></i>Visualization

We use [Sisense](https://www.periscopedata.com) as our Data Visualization and Business Intelligence tool. To request access, please follow submit an [access request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=New%20Access%20Request).

#### Meta Analyses for the Data Team

* [Sisense Usage! 📈](https://app.periscopedata.com/app/gitlab/410320/)
* [Sisense Account Optimization 💪](https://app.periscopedata.com/app/gitlab/410321/)
* [Sisense Account Maintenance 🗑️](https://app.periscopedata.com/app/gitlab/410322/)
* [dbt Event Logging](https://app.periscopedata.com/app/gitlab/420622/)
* [Snowflake Spend ️❄](https://app.periscopedata.com/app/gitlab/443349/)

## <i class="fas fa-user-lock fa-fw color-orange font-awesome" aria-hidden="true"></i>Security

### Passwords

Per GitLab's password policy, we rotate service accounts that authenticate only via passwords every 90 days. A record of systems changed and where those passwords were updated is kept in [this Google Sheet](https://docs.google.com/spreadsheets/d/17T89cBIDLkMUa3rIw1GxS-QWFL7kjeLj2rCQGZLEpyA/edit?usp=sharing).

We also rotate Snowflake user passwords the first Sunday of every 3rd month of the year (January, April, July, October) via the [Snowflake Password Reset DAG](https://gitlab.com/gitlab-data/analytics/blob/master/dags/general/snowflake_password_reset.py).

## Data Learning and Resources

### Powered by GitLab Team Members 

* [How Data Teams Do More With Less By Adopting Software Engineering Best Practices - Thomas's talk at the 2018 DataEngConf in NYC](https://www.youtube.com/watch?v=eu623QBwakc)
  * [Slides from a similar talk by Taylor at the 2019 Music City Tech Conference in Nashville](https://docs.google.com/presentation/d/1oSdej0y7o5d4DKlyykmTEMbokr7sRIxMkFmw6Z8a270/edit?usp=sharing)
* [Locally Optimistic AMA: August 2019 with Taylor Murphy](https://www.youtube.com/watch?v=iT1uRdyXfd8)
* [4 Examples of the power of open source analytics](/blog/2019/04/15/open-source-analytics/)
* [Deploying your first dbt project with GitLab CI](https://www.youtube.com/watch?v=-XBIIY2pFpc&feature=youtu.be&t=1305)
* [DataOps in a Cloud Native World](https://www.youtube.com/watch?v=PLe9sovhtGA&list=PLFGfElNsQthaaqEAb6ceZvYnZgzSM50Kg&index=9&t=0s)
* [The Three Levels of Data Analysis- A Framework for Assessing Data Organization Maturity](/blog/2019/11/04/three-levels-data-analysis/)
* [How to Implement DataOps using GitLab](https://www.youtube.com/watch?v=GSEwkL5ZRNs)
* [Lessons learned managing the GitLab Data team](/blog/2020/02/10/lessons-learned-as-data-team-manager/)
* [Views on Vue Podcast with Jacob Schatz and Taylor Murphy](https://devchat.tv/views-on-vue/vov-030-how-we-use-vue-in-data-science-with-jacob-schatz-taylor-murphy-gitlab-team/)
* [How to do DataOps with GitLab - Customer Call](https://chorus.ai/meeting/702422?tab=summary&call=31D048F239B04C28A5E25208A104BFD6) (GitLab Internal)
* [GitLab for ML - Customer Call](https://chorus.ai/meeting/747939?call=08C9A333A729435CB2954FFDE3556BC0) (GitLab Internal)

### Recommended Reading, Listening, Watching

* [The AI Hierarchy of Needs](https://hackernoon.com/the-ai-hierarchy-of-needs-18f111fcc007)
* [Data Meta Metrics](https://caitlinhudon.com/2017/11/14/data-meta-metrics/)
* [Engineers Shouldn’t Write ETL](https://multithreaded.stitchfix.com/blog/2016/03/16/engineers-shouldnt-write-etl/)
* [The Startup Founder’s Guide to Analytics](https://thinkgrowth.org/the-startup-founders-guide-to-analytics-1d2176f20ac1)
* [Functional Data Engineering — a modern paradigm for batch data processing](https://medium.com/@maximebeauchemin/functional-data-engineering-a-modern-paradigm-for-batch-data-processing-2327ec32c42a)
* [Keep it SQL Stupid, a talk by Connor McArthur of Fishtown Analytics at DataEngConf SF '18 explaining dbt](https://www.youtube.com/watch?v=9VNh11qSfAo)
* [DevOps for AI](https://www.youtube.com/watch?v=HwZlGQuCTj4)
* [What Can Data Scientists Learn from DevOps](https://redmonk.com/dberkholz/2012/11/06/what-can-data-scientists-learn-from-devops/)
* [One Analyst's Guide for Going from Good to Great](https://blog.fishtownanalytics.com/one-analysts-guide-for-going-from-good-to-great-6697e67e37d9)
* The Value of Data: [Part 1](https://www.codingvc.com/the-value-of-data-part-1-using-data-as-a-competitive-advantage), [Part 2](https://www.codingvc.com/the-value-of-data-part-2-building-valuable-datasets), [Part 3](https://www.codingvc.com/the-value-of-data-part-3-data-business-models)
* [Building a Data Practice](https://www.locallyoptimistic.com/post/building-a-data-practice/)
* [Does my Startup Data Team Need a Data Engineer](https://blog.fishtownanalytics.com/does-my-startup-data-team-need-a-data-engineer-b6f4d68d7da9)
* [Data Science is different now](https://veekaybee.github.io/2019/02/13/data-science-is-different/) (Note: this is why GitLab doesn't have a Data Scientist yet.)
* [Why You Don't Need Data Scientists](https://medium.com/@kurtcagle/why-you-dont-need-data-scientists-a9654cc9f0e4)
* [Resources Written by dbt Community Members](https://discourse.getdbt.com/t/resources-written-by-community-members/276)
* [Is your company too dumb to be data-driven?](https://towardsdatascience.com/is-your-company-too-dumb-to-be-data-driven-696932d597c3)
* [What does "self-serve" analytics mean to you?](https://discourse.getdbt.com/t/what-does-self-serve-in-analytics-mean-to-you/712/5)
* [Models for integrating data science teams within organizations](https://medium.com/@djpardis/models-for-integrating-data-science-teams-within-organizations-7c5afa032ebd)
* [Building a Mature Analytics Workflow](https://blog.fishtownanalytics.com/building-a-mature-analytics-workflow/) (Note: this explains the "Analytics is a subfield of software engineering" premise.)
* [DataOps playlist on YouTube](https://www.youtube.com/playlist?list=PLVbsAdgZXvtyy6HVKCP0HChjCcq2oW3eK)

### Data Newsletters
- [Algos & Ethics](https://algosandethics.substack.com)
- [Calogica](https://calogica.com/signup)
- [The Carpentries](https://carpentries.topicbox.com/latest)
- [DataEng Weekly](http://dataengweekly.com/)
- [Data Elixir](https://dataelixir.com/)
- [Data is Plural](https://tinyletter.com/data-is-plural)
- [Data Science Roundup Newsletter](http://roundup.fishtownanalytics.com/)
- [Data Science Weekly](https://www.datascienceweekly.org/)
- [Lantrns Analytics (Product Analytics)](https://www.lantrns.co/product-analytics-newsletter/)
- [Music and Tech](https://angelddaz.substack.com)
- [Normcore Tech](https://vicki.substack.com)
- [NumLock News](https://numlock.substack.com)
- [One Shot Learning](https://buttondown.email/oneshotlearning)
- [SF Data](http://weekly.sfdata.io/)


### Data Blogs
- [Airbnb](https://airbnb.io)
- [Ask Good Questions](https://askgoodquestions.blog/)
- [Buffer Blog](https://data.buffer.com)
- [Calogica](https://calogica.com/blog)
- [Fishtown Analytics Blog](https://blog.fishtownanalytics.com)
- [Go Data Driven](https://blog.godatadriven.com)
- [MBA Mondays](https://avc.com/archive/#mba_mondays_archive)
- [Mode Analytics Blog](https://blog.modeanalytics.com/)
- [Multithreaded](https://multithreaded.stitchfix.com/)
- [Sisense Data Blog](https://www.periscopedata.com/blog)
- [Silota](http://www.silota.com/docs/recipes/)
- [Wes McKinney Blog](http://wesmckinney.com/archives.html)
- [Data Ops](https://medium.com/data-ops)
- [Retina AI Blog](https://retina.ai/blog/)
- [StitchFix Algorithms Blog](https://multithreaded.stitchfix.com/algorithms/blog/)
- [Five Thirty Eight](https://data.fivethirtyeight.com/)
- [Data.gov](https://www.data.gov/)

### Data Visualization Resources
- [Storytelling with Data](http://storytellingwithdata.com/)
- [Data Revelations](https://www.datarevelations.com/)
- [Eager Eyes](https://eagereyes.org/)
- [FiveThirtyEight's DataLab](https://fivethirtyeight.com/features/)
- [Flowing Data](https://flowingdata.com/)
- [From Data to Viz](https://www.data-to-viz.com/)
- [Gravy Anecdote](http://gravyanecdote.com/)
- [JunkCharts](https://junkcharts.typepad.com/)
- [Make a Powerful Point](http://makeapowerfulpoint.com/)
- [Makeover Monday](http://www.makeovermonday.co.uk)
- [Perceptual Edge](https://perceptualedge.com/)
- [PolicyViz](https://policyviz.com/)
- [The Functional Art](http://www.thefunctionalart.com/)
- [The Pudding](https://pudding.cool/)
- [Visualising Data](http://www.visualisingdata.com/)
- [VizWiz](http://www.vizwiz.com/)
- [WTF Visualizations](http://viz.wtf/)

### Data Slack Communities
- [Data Viz Society](https://datavizsociety.slack.com)
- [Data Science Community](https://dscommunity.slack.com)
- [dbt](https://slack.getdbt.com)
- [Great Expectations](https://greatexpectations.io/slack)
- [Locally Optimistic](https://www.locallyoptimistic.com/community/)
- [Measure](ttps://docs.google.com/forms/d/e/1FAIpQLSdyAxOcI8z1EEiJDW4sGln-1GK9eJV8Y86eljX-uSlole0Vtg/viewform?c=0&w=1)
- [Meltano](https://join.slack.com/t/meltano/shared_invite/enQtNTM2NjEzNDY2MDgyLWI1N2EyZjA1N2FiNDBlNDE2OTg4YmI1N2I3OWVjOWI2MzIyYmJmMDQwMTY2MmUwZjNkMTBiYzhiZTI2M2IxMDc)
- [Open Data Community](https://opendatacommunity.slack.com)
- [Pachyderm](http://slack.pachyderm.io)
- [PyCarolinas](https://pycarolinas.slack.com/join/shared_invite/enQtNjI4NTY0MzM5MDc5LWE2ZjI3YmFkNTAzOTM2NmYyMWUwMmYzZGFkYTY2ZjdkZWFmZDg0YzE0MjQzMzMzMzVhOWUwN2I3MTQwMTllMjY)
- [R for Data Analysis](https://r-data-team.slack.com)
- [Software Engineering Daily](http://softwaredaily.herokuapp.com)
- [The Data School](https://thedataschool.slack.com)

### Technical Learning Resources
- [Chris Albon](https://chrisalbon.com/#postgresql)
- [Mode SQL Tutorial](https://mode.com/sql-tutorial/introduction-to-sql/)
- [dbt Tutorial](https://tutorial.getdbt.com/tutorial/setting-up)
- [Elements of Data Science](https://allendowney.github.io/ElementsOfDataScience/)
- [Machine Learning Resources](https://drive.google.com/drive/folders/1sOXWW-FujwKU2T-auG7KPR9h6xqDRx0z?usp=sharing) (GitLab Internal)
- [Codecademy](https://www.codecademy.com/learn/learn-sql)
- [DataQuest](https://www.dataquest.io/course/sql-fundamentals/)
- [Khan Academy](https://www.khanacademy.org/computing/computer-programming/sql)
- [HackerRank (Exercises)](https://www.hackerrank.com/domains/sql?filters%5Bstatus%5D%5B%5D=unsolved&badge_type=sql)
- [Udacity](https://www.udacity.com/course/intro-to-relational-databases--ud197)
- [Stanford University Mini-Courses](https://lagunita.stanford.edu/courses/DB/2014/SelfPaced/about)
- [The Data School by Chartio](https://dataschool.com/learn/inroduction-to-teaching-others-sql)
- [W3Schools](https://www.w3schools.com/sql/default.asp)

## <i class="fas fa-users fa-fw color-orange font-awesome" aria-hidden="true"></i>Team Roles

### Triager

The data team has a triager who is responsible for:
*  addressing `dbt run` and `dbt test` failures
*  labeling and asking initial questions on created issues 
    - Add the `Workflow::Triage` label
    - Add additional [labels](/handbook/business-ops/data-team/#issue-labeling)
    - Assign it to the appropriate Manager, Data for prioritization
*  guiding and responding to questions from GitLab Team-member
*  maintaining the KPI Index page by creating an issue with any outstanding concerns (broken links, missing KPI definitions, charts vs links, etc) and assigning it to the appropriate stakeholders to correct as soon as possible. 

Having a dedicated triager on the team helps address the bystander affect.
This is **not** an on-call position.
This role just names a clear owner.
Through clear ownership, we create room for everyone else on the team to spend most of the day around deep work.
The triager is encouraged to plan their day for the kind of work that can be accomplished successfully with this additional demand on time.

**The triager is not expected to know the answer to all the questions.
They should pull in other team members who have more knowledge in the subject matter area to pass on the conversation after understanding the issue.**
Document any issues you stumble upon and learn about to help disseminate knowledge amongst all team members.

#### Slack channels to monitor for triaging

* #data: this channel is where GitLabbers outside of the data team submit questions and inquiries. Questions often pertain to Sisense dashboards, technical questions around using SQL and Sisense, or general requests for analyses and reports.
   * Most of the requests that come in the #data channel can be solved by:
       * pointing folks to an appropriate dashboard; or
       * guiding them to create an issue in the right place.
   * It's important that folks feel acknowledged and that their questions are being addressed by the data team.
* #data-triage: this channel is where issues submitted from GitLabbers outside of the Data Team are triaged.
   * **Issue triaging**
Many issues that come into the data team project from other GitLab team members need additional info and/or context in order to be understood,
estimated, and prioritized.
It is the triager's priority to ask those questions.
This will help folks feel like their asks are not just going to the void and are being taken seriously by the data team.
It also help surface issues sooner, rather than later.

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/Hu_zDh0Av7M" frameborder="0" allowfullscreen="true"> </iframe>
</figure>


* #dbt-runs: this channel is where `dbt run` and `dbt test` failures are triaged.
   * **dbt run and test failures**
Occasionally, `dbt run` and `dbt test`  produce failures.
Many of the these failures are due to upstream data quality problems that need to be addressed.
     * `dbt run` failures indicate the model did not run and maintained its previous state and data composition. These failures are not common and it is not feasible to maintain a list of common `dbt run` failures. Please follow the general checklist located at the top of the below referenced README file to debug `dbt run` errors. 
     * `dbt test` failures indicate the model ran, but there are some records in the model that have data quality issues and require research and follow-up. Please follow the checklists in the below referenced README file to debug `dbt test` failures. Some tests have a severity setting of `warn` and not `fail`. If `warn` is configured, then dbt will log a warning for any failing tests, but the job will still be pass (assuming no failures). This configuration is useful for tests in which a failure does not imply that action is required. Warnings do not need to be triaged.
   * Most `dbt test` failures are documented in the [dbt tests README](https://gitlab.com/gitlab-data/analytics/blob/master/transform/snowflake-dbt/tests/README.md).
If you stumble upon one that isn't documented, be sure to document it to make it easier to address in the future.
The end result is not necessarily the resolution of the failing model in `dbt run` and `dbt test`; 
**however, the model should be taken to a `running` state and the problems documented in an issue.**
This is important because:
      1. Airflow only shows the last 50 lines of logs in Slack and we don't want to risk missing another issue; and 
      2. We reduce the noise for all team members this way, while things are actively worked to be resolved. 
If you see that there are multiple errors, you may need to ping someone with Airflow access to get the full logs. 
   * When creating an issue from a pipeline failure, add the `triage` label so that the next person on triage duty can easily find if the failure is new or not, and avoid issue duplication. Any created issues should also be posted to the `dbt-runs` slack channel by the triaging team member for quick review by the following triager. 


**Triage schedule**
The data team has implemented a triagle schedule that takes advantage of folks native timezones. The [Data Team's Google Calendar](https://calendar.google.com/calendar?cid=Z2l0bGFiLmNvbV9kN2RsNDU3ZnJyOHA1OHBuM2s2M2VidW84b0Bncm91cC5jYWxlbmRhci5nb29nbGUuY29t) is the source of truth for the triage schedule.
A team member who is off, on vacation, or working on a high priority project is responsible for finding coverage and communicating to the team who is taking over their coverage;
this should be updated on the [Data Team's Google Calendar](https://calendar.google.com/calendar?cid=Z2l0bGFiLmNvbV9kN2RsNDU3ZnJyOHA1OHBuM2s2M2VidW84b0Bncm91cC5jYWxlbmRhci5nb29nbGUuY29t).

| UTC day | Team member |
| ------ | ------ |
| Sunday | Primary: @ken_aguilar / Backup: @kathleentam  | 
| Monday | Primary: @ken_aguilar / Backup: @derekatwood | 
| Tuesday | @msendal (CET) / @m_walker (MST) |
| Wednesday | Alternating: @mpeychet / @eli_kastelein |
| Thursday | Primary: @jeanpeguero / Backup: @iweeks |
| Friday | Primary: @jeanpeguero / Backup: @derekatwood  |

### Reviewer 
All GitLab data team members can, and are encouraged to, perform code review on merge requests of colleagues and community contributors. 
If you want to review merge requests, you can wait until someone assigns you one, but you are also more than welcome to browse the list of open merge requests and leave any feedback or questions you may have.

Note that while all team members can review all merge requests, the ability to *accept* merge requests is restricted to maintainers.

### Codeowner
Code ownership is a [feature of GitLab](https://gitlab.com/help/user/project/code_owners) that links a project member to specific folders and files in a project. It is meant to answer the questions "who can I ask about this code?" and "who should review changes to this code?".

Becoming a code owner is part of the journey to becoming a project maintainer. If you are the sole creator of a file, say a new dbt model set, you will be the de facto code owner for those files. If you wish to expand your ownership purview, follow these steps:

1. Create an MR to the [CODEOWNERS file](https://gitlab.com/gitlab-data/analytics/blob/master/CODEOWNERS) with the ownership change you wish to make
1. Work with the other code owners that already cover the area you wish to join to pair with them on at least 5 MRs that alter the code you wish to be responsible for
  * The MRs should not reflect only small changes to the code base, but also architectural ones and ones that create a fully functioning addition. It may take more than 5 MRs for this criteria to be reached
  * You will be the primary reviewer for all MR's assigned to the code owner
  * You will review the MR's as if you had the power to merge
  * Once you feel the MR is ready and you would have merged it, assign it to the code owner and comment that you would have merged the MR
  * The code owner will do a follow up review if necessary and either merge the MR or assign it to a maintainer for you
  * Document the MR in the original MR you created
1. Once the 5 MR threshold has been reached, the code owner will work with the applicant's manager to make a decision
1. If denied, close the MR and work with your manager for a period of no less than 3 months before applying again
1. If approved, assign the MR to a maintainer to merge. You will automatically be added to the Code Owner approval list once merged

### Maintainer
A maintainer in any of the data team projects is not synonymous with any job title. 
Here, the data team takes from the precedent set forward by the engineering division on [the responsibilities of a maintainer](/handbook/engineering/workflow/code-review/#maintainer). 
Every data team project has at least one maintainer, but most have multiple, and some projects (like Analytics) have separate maintainers for dbt and orchestration.

#### How to become a data team maintainer 

We have guidelines for maintainership, but no concrete rules.
Maintainers should have an advanced understanding of the GitLab Data projects codebases. 
Prior to applying for maintainership of a project, a person should gain a good feel for the codebase, expertise in one or more domains, and deep understanding of our coding standards. You're probably ready to become a maintainer when both of these statements feel true:

1. The MRs you've reviewed consistently make it through maintainer review without significant additionally required changes
1. The MRs you've created consistently make it through reviewer and maintainer review without significant required changes

If those subjective requirements are satisfied, this is the process to add yourself as a maintainer:

1. Create an issue in the relevant project with the title "Add <user> as project maintainer"
1. Add documentation to the issue for the following:
  * Explain why you are ready to take on the maintainer responsibility
  * Explain the scope of your maintainership (entire project, dbt, python, etc.)
  * Recent MR's that you have created and reviewed that you believe show your readiness
1. Once the issue is created, tag a maintainer who you'd like to be paired with for a formal review
1. The maintainer will have you pair with them on at least 10 merge requests
  * The MRs should show a diversity of scope, including architectural changes as well as complete, fully functioning feature releases with changes across many files and directories. 
  * You will be the primary reviewer for these 10 MRs
  * You will review the MR's as if you had the power to merge
  * Once you feel the MR is ready and you would have merged it, assign it to the maintainer and comment that you would have merged the MR
  * The maintainer will do a follow up review if necessary and merge the MR for you
  * Document the MR in the issue you created
1. Once the 10 MR threshold has been reached, the maintainer will work with the applicant's manager to make a decision
1. If denied, close the issue and work with your manager for a period of no less than 3 months before applying again
1. If approved, create a MR to add the maintainership to your team page entry
1. Assign the MR to your manager and mention the existing maintainers of the relevant project (Infrastructure, Analytics, etc) and area (dbt, Airflow, etc.).
1. If the existing maintainers of the relevant group e.g., dbt, do not have significant objections, and if at least half of them agree that the reviewer is indeed ready, we've got ourselves a new maintainer!
1. An owner of the project will increase your privilege on the project

### Job Descriptions
#### Data Analyst
[Job Family](/job-families/finance/data-analyst/){:.btn .btn-purple}

#### Data Engineer
[Job Family](/job-families/finance/data-engineer/){:.btn .btn-purple}

#### Manager
[Job Family](/job-families/finance/manager-data){:.btn .btn-purple}

#### Director of Data and Analytics
[Job Family](/job-families/finance/dir-data-and-analytics){:.btn .btn-purple}


<!-- EXTRA STYLES APPLIED FOR THIS PAGE ONLY -->

<style>
.purple {
  color: rgb(107,79,187) !important;
}
.orange {
  color:rgb(252,109,38) !important;
}
.md-page h2 i.icon-color {
  color: rgb(107,79,187)
}
.md-page h2:nth-of-type(even) i.icon-color{
  color:rgb(252,109,38);
}
.font-awesome {
  font-size: .70em;
  vertical-align: middle;
  padding-bottom: 5px;
}
.btn-purple {
  color: rgb(107,79,187);
  background-color: #fff;
  border-color: #403366;
}
.btn-purple:hover {
  color: #fff;
  background-color: rgb(107,79,187);
  border-color: #403366;
}
.btn-purple-inv {
  color: #fff;
  background-color: rgb(107,79,187);
  border-color: #403366;
}
.btn-purple-inv:hover {
  color: rgb(107,79,187);
  background-color: #fff;
  border-color: #403366;
}
.btn-orange {
  color: rgb(252,109,38);
  background-color: #fff;
  border-color: rgb(226,67,41);
}
.btn-orange:hover {
  color: #fff;
  background-color: rgb(252,109,38);
  border-color: rgb(226,67,41);
}
.product.thumbnail img {
  display: block;
  max-width: 50%;
  margin: 20px auto;
}
.thumbnail img {
  display: block;
  max-width: 30%;
  margin: 20px auto;
}
.caption h4 {
  text-align: center;
}
.mkt-box {
  padding-bottom: 10px;
  padding-top: 10px;
  cursor: pointer;
}
.mkt-box:hover {
  /*border-radius: 5px;*/
  box-shadow:0 1px 5px rgba(0,0,0,0.3), 0 0 2px rgba(0,0,0,0.1) inset;
}
.mkt-row {
  padding-top: 20px;
  padding-bottom: 5px;
}
.mkt-row a:focus {
  outline: none;
}
.modal-header h2 {
  margin-top: 0;
}
.modal-footer p {
  margin-bottom: 0;
}
.center {
  text-align: center;
  display: block;
  margin-right: auto;
  margin-left: auto;
}
.description {
  color: #999;
}
.extra-space {
  margin-bottom: 5px;
}
.alert-purple {
  color: rgb(107,79,187);
  background-color: #fff;
  border-color: rgba(107,79,187,.5);
}
ul.toc-list-icons {
  list-style-type: none;
  padding-left: 25px;
}
ul.toc-list-icons li ul {
  padding-left: 25px;
}
ul.toc-list-icons {
  list-style-type: none;
  padding-left: 25px;
}
ul.toc-list-icons li ul {
  padding-left: 35px;
}
ul.toc-list-icons li i,
ul.toc-list-icons li ul li i {
  padding-right: 15px;
  color: rgb(107,79,187);
}
ul.toc-list-icons li:nth-of-type(even) i {
  color:rgb(252,109,38);
}
ul.toc-list-icons li ul li i.slack {
  color: rgb(224,23,101);
}
ul.toc-list-icons li ul li i.email {
  color: rgb(192,0,0);
}
</style>
