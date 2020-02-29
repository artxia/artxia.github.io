---
layout: handbook-page-toc
title: "Customer Reference Program"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Customer reference program at GitLab

The goal of the Customer Reference Program is to provide opportunities for customers to share their story on how GitLab has helped them overcome the challenges, blockers and pain points within their organizations. The Reference Program Managers work as a conduit to help connect customers with opportunities by balancing customer requests with company demands. By providing a single point for outreach to customers, the CRP team prevents customer burnout, sales team burnout, and ensures a diversity of customer stories are shared publicly. 

##Who we are
Team of Experienced Customer Reference Professionals who are focused on building relationships within GitLab and with customers.  
The team gathers and builds information and relationships with the purpose of distilling these impactful insights into action. 

#Strategic driver of the Customer Reference Program
To manage our customer reference relationships like the precious resources they are to the maximum, quantified & qualified benefit for both customers and GitLab. 



##Goals of the Gitlab Customer Reference Program
- **Credibility** -Reinforce our credibility as an end-to-end DevOps solution partner.
- **Shorten the sales cycle** - Having our advocates involved with sharing their story with potential sales, analysts and the marketplace can help potential sales close sooner
- **Increase Revenue** - A successful Customer Reference Program helps increase revenue by attracting new clients and increasing retention rates.
- **Customer Advocacy** - Encourage our customers to share their success stories with others who are learning about or evaluating GitLab.

### Customer Reference Types
Some examples of the types of assets we'd use as customer references once we have approval from the customer:
* Logo (The ability to name a company as a customer and use their logo in our marketing materials)
* Live sales reference (both calls and possible in-person)
* Website content
  * Case studies
  * Blog posts
  * Videos
  * Podcasts
  * Usage quotes
* Event speakers (At industry, third-party and company events)
* References for analysts and press
* Quotes (can be attributable with approval or anonymous)
* Anecdotes (short "snackable" stories, can be attributable with approval or anonymous) Read [GitLab's customer anecdotes](#customer-anecdotes).

### Creating new issue for Customer Reference Program
To create a new issue around the Customer Reference Program, open an issue on the [Customer Reference Program Board](https://gitlab.com/groups/gitlab-com/marketing/-/boards/927283?&label_name[]=Customer%20Reference%20Program).
Make sure it has the label *Customer Reference Program*. Feel free to add any applicable labels around the request. Assign to Reference Program Manager as needed.

### Customer Case Studies
The most recent customer case studies are found on the [GitLab customer's page.](/customers/)
When we build case studies, we need to have quantifiable metrics and business value to help describe how GitLab helped a customer achieve a significant business result.  Below are a sample of KPIs / dimensions we need to find in a good case study.

**Speed**
* Improved cycle time - the time it takes for an idea to reach production.
* More frequent deploys -  related to cycle time, but easier to measure

**Savings**
* Reduced IT spend - We reduced budget by x.   Or we saved $ with GitLab
* Improved efficiency - We shipped more features in the same time…

**Business Value**
* Increased revenue

**Better / Quality**
* Reduced defects / errors
* Reduced security issues/vulnerability
* Decrease of customer support calls

If a proposed customer case study doesn't have at least one metric to include, then we consider working with the account team to help identify a solid metric before building the case study.

#### Common Interview questions
Interview Questions: (Select the questions we should ask)

**Why GitLab**
- [ ] What insights do you have that might make a good case study today?
- [ ] Describe what your organization does, how the software is used, and how your team helps solve business challenges.
- [ ] What problem were you trying to solve when you were looking at GitLab?
- [ ] What was your process before using GitLab?
- [ ] Why did you choose to replace your current tooling?
- [ ] What were the negative consequences of your previous environment?
- [ ] What would have happened if you hadn't replaced your tooling
- [ ] How was this problem affecting you?
- [ ] What products were you using before using GitLab?
- [ ] What were the required capabilities you were looking for?
- [ ] Why did you choose GitLab?

**What if**
- [ ] What would have happened if you hadn't selected GitLab?

**Feedback on GitLab**
- [ ] How did GitLab solve those problems you were suffering from?
- [ ] Which teams are using GitLab?
- [ ] What do users say about GitLab?

**Impact of GitLab**
- [ ] What are the positive business outcomes of introducing GitLab?
- [ ] Has GitLab simplified workflow?
- [ ] How has GitLab enabled cross-functional relationships?
- [ ] How has it helped modernize architecture?
- [ ] What are some initial successes resulting from moving to GitLab?
- [ ] Can you share any larger successes?
- [ ] What does your current workflow look like?
- [ ] What other tools do you have plugged into GitLab?
- [ ] Are you using AWS, GCP, Azure?
- [ ] Can you describe how your deployments look?
- [ ] How does GitLab plug into your cloud environment?
- [ ] Are you using security testing features?

**Metrics of GitLab**
- [ ] Do you have any metrics available?
- [ ] How has GitLab impacted your cycle time?
- [ ] Have you measured throughput/Lead time? Can you give a before and after?
- [ ] What does your deployment frequency look like?
- [ ] Has there been an impact on change failure rate?
- [ ] Is your MTTR (mean time to resolution) improved?
- [ ] What percentage of your releases are now on time and on budget?
- [ ] Are you catching bugs earlier? Are you catching bugs that would have previously been missed?
- [ ] What percentage of your code is now scanned?
- [ ] What percentage of critical security vulnerabilities that previously escaped development have been caught?
- [ ] Has GitLab helped you achieve the KPIs you set out to solve?



#### Publishing to the website

1.	Start by opening a public issue and an Merge Request in the www-gitlab-com project.
2. Create a `.yml` file in `/data/case_studies` directory under Marketing site repo (www-gitlab-com project). This can be accomplished in the Web IDE.
3.	Keep the name of file same as company name (this is not mandatory but it is easier to manage), for eg; if company name is "Foobar", create a file as `/data/case_studies/foobar.yml`.
4.	Once created, add contents of the file using the sample Case Study template, or by scraping the content from an existing case study, and then update the values of each property based on case study details, remember, do NOT change property names.
5. Add images to the same MR. This ensures they show up in the preview app. To accomplish this, stay in your MR and on the left rail open the selected file. Upload the file to the specific directory by hovering over the file and selecting upload file. The Cover image needs to be a .jpg and put in 'source/image/blogimage' directory. The company logo needs to be a color .SVG image and is placed in the 'source/image/case_study_logos' directory. 
6.	In the Web IDE, you can view generated Case Study page in the generated App under the URL, for eg; http://localhost:4567/customers/foobar.
7. Once the case study is ready to publish, remove the WIP label from your MR and ask an approved publisher to post. 

### Customer references collection

Our written customer case studies are found on the [/customers page](https://about.gitlab.com/customers/)
Our video customer case studies are found on the YouTube site on [this playlist](https://www.youtube.com/playlist?list=PLFGfElNsQthZ__Rq59rec-EMgKsLuNjJE)

To initiate a formal case study process, follow the process listed [here](/handbook/marketing/corporate-marketing/content/case-studies/)

### Reference Program Process
Adding a new reference customer (Note the process is currently different for SALs)
** Commercial and SMB process**
    1. AE nominates customer for the program to Customer Reference Manager by adding an issue to the [Customer Reference Program Board](https://gitlab.com/groups/gitlab-com/marketing/-/boards/927283?&label_name[]=Customer%20Reference%20Program)
    2. CRM - AE briefing <br>
Key info needed:
		- Industry / Vertical
		- Region/Geo
    - Tier (core, starter, premium, ultimate)
    - [GitLab Use Case](/handbook/use-cases/)
    - Customer Segment (strategic, large, smb)
    - Deployment size (licenses)
    - Customer Story (why GitLab, key metrics, etc)
    - Who did we beat?<br>
 	 3. AE Introduces CRM to customer
		- Describe the Customer Reference program
    - Describe the types of reference activities and gauge their interest
		- Gauge their interest participation level
   4.  CRM updates Referenceable customer field in SFDC with information 

**SAL Process**
   1. SAL nominates champion from the contact record from the button at the top of SFDC
   2. SAL fills out the GitLab version customer is using, stages the customer is using and any information about the tech stack
   3. CRM team is notified of nomination in SFDC
   4. If additional information is needed, CRM team will outreach to SAL

### Sample Interview Questions/topics for Customer joining the Reference Program
    * What led you to GitLab, what problems were you trying to solve?
    * Why did you choose GitLab and what other tools were you using or considering?
    * What has been your experience with GitLab?  
    * How did you make the business case for GitLab and what metrics have you seen improve?
    * What have you heard from the GitLab users, what was the adoption curve like?
    * What has been the most unexpected success you have experienced? Adoption rates? Improved speed?

### Requesting a Reference for a sales call
**Commercial and SMB process**
   1. AE submits an issue on the [Customer Reference Board](https://gitlab.com/groups/gitlab-com/marketing/-/boards/927283?&label_name[]=Customer%20Reference%20Program) with the label "Customer Reference Checks".
   2. CRM reaches out to AE for additional information and with recommended sales references

**SAL process**
   1. SAL selects "Find a reference" button from the selected opportunity
   2. Filter to find the most appropriate reference for your needs. 
   3. Fill out required information and include any customer forms that may be required. 
   4. Hit submit and wait for the approval for the call from the champion's account owner

### Requesting a Reference for an event
**Local Field Marketing event**
   1. Please open an issue on the [Customer Reference Board](https://gitlab.com/groups/gitlab-com/marketing/-/boards/927283?&label_name[]=Customer%20Reference%20Program) with the label "Customer Speaking Requests" a miminum of 45 days before the event. 
   2. Please send a slack notifaction to the regional [Customer Reference Manager](https://about.gitlab.com/handbook/marketing/product-marketing/customer-reference-program/#which-customer-reference-team-member-should-i-contact)  with a link to the issue. 
   3. CRM will pull a SFDC report of customers in billing city/state/area to view an applicable pool of speakers as well as a report in Reference Edge.
   4. CRM will create a table from the report in the issue listing AE/SAL and customer accounts. CRM will tag any additional AEs/SALs in the issue. 
   5. CRM will work with AEs/SALs to identify customer stories (if known).
   6. CRM coordinate with Field Marketing to refine the speaker pool. 
   7. CRM and AE/SALs will reach out with speaking request to customers giving customers a minimum of 30 days before the event to respond. 
   8. If customer accepts, introduction to field manager is coordinated. 
   9. If customer outreach is unsuccessful, CRM will coordinate with Field Marketing on internal alternatives. 

Note: If travel is required for a customer speaker, it is covered by field marketing. 

**Partner/Alliance Associated event**
   1. Please open an issue on the [Customer Reference Board](https://gitlab.com/groups/gitlab-com/marketing/-/boards/927283?&label_name[]=Customer%20Reference%20Program) with the label "Customer Speaking Requests" a miminum of 65 days before the event. Ideally 90 days.
   2. Please send a slack notifaction to the regional [Customer Reference Manager](https://about.gitlab.com/handbook/marketing/product-marketing/customer-reference-program/#which-customer-reference-team-member-should-i-contact)  with a link to the issue. 
   3. In the issue, please identify Partner/Alliance organization and anticipated outcome.
   4. Requestor to identify tier of customer requested. (Enterprise, Commercial, SMB)
   5. Customer Reference Manager identifies pool of proposed customers with Reference Edge, SFDC, and Alliance customer stories.
   6. CRM distributes pool to requestor and works with them to identify a short list of customers to request.
   7. CRM reaches out to appointed SALs/AEs of customers to verify timing of request.
   8. CMR or SAL/AE outreach to customer a minimum of 60 days before the event. 
   9. If customer accepts, introduction to the alliance manager is coordinated. 
   9. If customer outreach is unsuccessful, CRM will coordinate on internal alternatives.

Note: If travel is required for a customer speaker, it is covered by different parts of the org. (Determined on a per request basis.)


### Requesting a customer for analysts
**Requesting a confidential request (Customer not named in report)**
   1. Analyst Relations team adds label "Customer Speaking Requests" to the report as soon as issue is opened.
   2. Analyst Relations team adds a slack message with the issue in the "Customer_References" Channel.
   3. Customer Reference Team will work with Analyst Relations manager to narrow down the pool of potential customers based on used stages etc. 
   4. CRM to review previous customer references for the specific report. CRM to identify 1 speaker to show growth and maturity of product to speak for report again. 
   5. CRM to outreach to SAL/AEs for customers to get approval to speak for report. 
   6. CRM to outreach to customer for request to speak for report. 

### Customer Logo Permission Form
**Purpose: To reflect our customer base we use customer logos to promote organizations that are using GitLab** 

Customer logos appear on our website and other marketing and promotional materials. To respect the intellectual property of companies that use our product, we request a signed permission form to use their logo. To request logo usage from a customer, please send the [Logo permission form](https://drive.google.com/open?id=1oCRUFM4cjOTHU8DhfSBr6uO_sTYURAGo) to the appropriate member of the customer organization. 
   1. Once we have received back the signed logo form, send the form to the Customer Reference Team.
   2. The Customer Reference Team will attach the signed form to the account on SFDC.
   3. The Customer Reference Team will add the customer to the Reference Edge software with logo usage selected. 
   4. The Customer Reference Team will then add the logo to the customer approved locations (including website and or promotional presentations.)


### GitLab Customer Advisory Board
**Purpose:** To help foster DevOps transformation and adoption we are establishing a Customer Advisory Board, where we focus on sharing DevOps best practices and lessons learned with each other. We believe that transparency and sharing  is a key way to help encourage the success of DevOps transformations.  The GitLab customer advisory board is intended to be home to learning and collaboration so we can all experience success through DevOps transformation.

**Members** Executives/Champions for DevOps within their organizations

**Frequency:**  We meet virtually the first Wednesday of the month at 11 a.m. Eastern

**Membership:** Approximately 15 - 20 customers, GitLab

**Meeting Recordings** Meetings are recorded for internal and member use. Members can seek these recordings by emailing CAB@gitlab.com

**Recurring Content** We will frequently ask for GitLab Product Managers to join to [present the vision for their assigned DevOps stage](/product/#customer-advisory-board-meetings).
When doing so we will distribute a recorded video of their [stage direction](/handbook/product/product-management/process/#section-and-stage-direction) in advance.

**Meeting Schedule**

***Kickoff Meeting-September 5, 2018***
- Member introductions-9 members in attendance
- Group goals  
- Top DevOps challenges

***GitLab Road Map review-September 26, 2018***
- Member introductions- 7 members in attendance
- Road Map review
- Within Depth, what is holding you back the most from adopting existing features/capabilities?
- Within Breadth, what are you most excited about?
- Within Roles, what are you most excited about?

***GitLab Plan review-October 17, 2018***
- Member introductions- 8 members in attendance
- Review of Plan Roadmap
- Customer Sharing

***GitLab Create review-November 7, 2018***
- Member introductions
- Customer Sharing
- Review of Create

***GitLab Release review-December 5, 2018***
- Member introductions
- Review of Release
- Year-end check up and member discussion

***GitLab Manage review - January 9, 2019***
- Member introductions - 11 members in attendance
- Review and feedback around Manage
- Customer Sharing

***GitLab Geo review-February 6, 2019***
- Member introductions
- Customer Sharing
- Review of Geo

***GitLab Configure review- March 6, 2019***
- Member introductions
- Customer Sharing
- Review of Configure

***In-Person CAB Meeting- April 18-19, 2019***
- Yankee Stadium
- Bronx, New York
- Number of attending customers - 17

***GitLab In-Person CAB Review -May 1, 2019
- Member introductions
- Review of In-Person Customer meeting
- Discussion around future of CAB and project to work on together

***GitLab Verify direction update - June 5, 2019***
- Member introductions - 11 members in attendance
- Review of Verify direction
- Customer Sharing

***GitLab Product Roadmap review - July 10, 2019***
- Member introductions -
- Stage discussion
- Customer Sharing

*** GitLab Product Roadmap Review - August 7, 2019***
- Member introductions
- Stage discussion
- Customer Sharing

***GitLab Product Roadmap Review - September 4, 2019***
- Member introductions
- Stage discussion
- Customer Sharing

***GitLab In-Person CAB Meeting - October 15 & 16, 2019***
- Space Needle
- Seattle, Washington



### GitLab Special Interest Group

***Purpose:*** We are forming Special Interest Groups to foster specific and focused discussions about how to apply DevOps practices and GitLab capabilities in specific domains such as planning, development,  CI/CD, security, etc. These Special Interest Groups will encourage sharing and collaboration of DevOps best practices and lessons learned between users and GitLab.

We believe that transparency and sharing is a key way to help us all learn and improve how we deliver for our customers. GitLab special interest groups are intended to be home to learning and collaboration.

***Members*** Technical utilizers and advocates of GitLab

***Frequency:***  We will try to meet virtually every 6 to 8 weeks

***Membership:*** Approximately 8-15 users, GitLab Product Manager





### Customer Anecdotes
Customer anecdotes are short, "snackable" customer stories. These can be used on a call or in a meeting to share a point about GitLab by validating it with the customer story. An anecdote can be a summary of a formal, attributable case study or just an anonymous story from a conversation you had with a customer. It's important to keep customers anonymous unless we have explicit approval to use their name.

#### Remove the complexity of multi-tool environments

A communications company recently shared how they built their technology stack. "GitLab checks so many boxes for us that we don't need other tools." The company then explained they they are operating with a team of 2 people because GitLab makes the environment so simple. They said another organization would probably have to employ 15 people to accomplish what they can.

#### Administrative overhead

We hosted a dinner for customers and prospects to mingle with each other and share stories. When the topic of managing the DevOps toolchain came up, the Head of Risk at a large US bank mentioned that she had a team of 20 to keep SDLC tools running in her org. A GitLab customer, the managing director of a product group for a global investment management corporation said, "this is going to break your heart, but I have 1 guy that spends 25% time to keep GitLab up and going for my team of 1500 devs."

#### Deliver value faster

Pinterest is not a GitLab customer, but uses Kubernetes together with Jenkins. Because there's no [native kubernetes integration](/solutions/kubernetes/) for Jenkins they needed to dedicate a [team of 4 spending 6 months](https://kubernetes.io/case-studies/pinterest/) to build a custom system to control access management and allow teams to self-serve builds. This is functionality that comes out of the box on day one with GitLab.

#### Adoption at an incredible pace

A large enterprise in the software space is a recent GitLab Premium customer wanting to replace Perforce. They predicted that it would take them 3 years to hit 6K active users. But, the developer experience was so superior that they ended up hitting 6K active users in only 8 months.

#### Security is at the center

A publishing firm is utilizing GitLab best of breed CI/CD functionality and with upcoming product advancements they have informed us that GitLab is a mission critical application for them. They also chose GitLab over the competition because security is currently the biggest aspect they want to improve on internally.

#### Removing the wait

A financial services company recently stated that their teams went from two week releases to six times per day using GitLab. They are able to release this quickly because they do not need to wait for infrastructure.

#### No babysitter required

An online gaming development house has a team of 9 looking after its toolstack for SDLC. GitLab is one of the tools in the stack, but is self-sufficient enough that they only deal with it every six months.

#### Providing happiness everyday

A large media company recently stated that GitLab is the best architected application they have ever used. According to this company, "This product is a joy to use. We cannot believe how much incremental value you crank out with each release."



### Customer Case Studies

#### [Ticketmaster - 15x faster build time](/blog/2017/06/07/continous-integration-ticketmaster/)
Ticketmaster is a global event ticketing leader with one of the world's top five e-commerce sites, getting almost 27 million monthly unique visitors. Ticketmaster was using Jenkins for continuous integration. Weighed down by plug-ins and legacy development, their pipeline was taking 2 hours to complete. After getting stuck late on a friday night waiting for the build to complete, their ops team began exploring other options. They were able to run their pipeline on GitLab CI/CD in 8 minutes for a 15x increase.

#### [Axway - 26x faster release cycles](/customers/axway/)
Axway, is a global enterprise software company with over €300 million in yearly revenue. Axway wanted to adopt DevOps practices but their legacy Subversion toolchain was blocking them. By moving from Subversion to Git using GitLab as their Source Code Management (SCM) solution they were able to implement DevOps integrating GitLab into tools like JIRA, for issue management and Jenkins for continuous integration. They increased deployments from once-a-year to every two weeks.

#### [Paessler - 120X increased QA efficiency](/customers/paessler/)
Paessler AG provides the award-winning PRTG Network Monitoring software used by over 150,000 IT administrators in more than 170 countries. QA engineers were manually testing software with a routine set of tasking taking an hour to complete. By implementing GitLab pipelines they were able to automate QA tasks requiring only 3 minutes of effort for a 120x efficiency increase.

#### [Equinix - increased DevOps agility](/customers/equinix/)
Equinix is a leading global data center company. Their client-side development teams are responsible for building software products and business critical applications,  increase development speed, self-serviceability, and ship fixes and features quickly. Equinix needed a version control and continuous integration tool for distributed workflows to support globally distributed development teams.

#### [Other customer case studies](/customers/)

### Which customer reference team member should I contact?

  - Listed below are areas of responsibility within the Customer Reference team:

    - [Kim](/company/team/#kimlock), Customer Reference Manager
    - [Fiona](/company/team/#fokeeffe), EMEA Customer Reference Manager
    - [Colin](/company/team/#colinwfletcher), Manager, Market Research and Customer Insights
    - [Ashish](/company/team/#kuthiala), Director PMM
