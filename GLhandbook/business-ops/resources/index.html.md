---
layout: handbook-page-toc
title: "Go to Market"
description: "Operations, Procedures, Documentation"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

----
{::options parse_block_html="true" /}

## Reaching the Teams (internally)
- Public Issue Tracker: A short list of the main, public issue trackers. For respective teams, there may be additional resources. Please use confidential issues for topics that should only be visible to team members at GitLab
    - [Sales](https://gitlab.com/gitlab-com/sales/issues/) - general sales related needs & issues
    - [Marketing](https://gitlab.com/gitlab-com/marketing) - All issues related to website, product, design, events, webcasts, lead routing, social media and community relations
    - [Customer Success SA Triage](https://gitlab.com/gitlab-com/customer-success/sa-triage-boards) - your go to place for technical pre-sales requests
- Slack: A short list of the primary Slack channels used by these respective teams
    - `#customer-success`
    - `#sdr_global`
    - `#mktgops`
    - `#it-ops`
    - `#lead-questions`
    - `#marketing-programs`
    - `#marketing`
    - `#outreach`
    - `#sales`
    - `#sfdc-users`


## Glossary

| Term | Definition |
| :--- | :--- |
| Accepted Lead | A lead a Sales Development Representative agrees to work until qualified in or qualified out |
| Account | An organization tracked in salesforce.com. An account can be a prospect, customer, former customer, integrator, reseller, or prospective reseller |
| AM | Account Manager |
| AE | Account Executive |
| APAC | Asia-Pacific |
| CS | Customer Success |
| EMEA | Europe, Middle East and Africa |
| EULA | End User Licence Agreement |
| High intent | an event, webcast, demo that is a strong indicator of purchase or evaluation |
| Holdover Account | Account ownership retained by someone other than the territory owner |
| Inquiry | an Inbound request or response to an outbound marketing effort |
| IQM | Initial Qualifying Meeting |
| LATAM | Latin America (includes all of Central & South America) |
| MQL | Marketo Qualified Lead - an inquiry that has been qualified through systematic means (e.g. through demographic/firmographic/behavior lead scoring) |
| MVC | [Minimum Viable Change](/handbook/product/#the-minimally-viable-change-mvc) (not Model View Controller)|
| NCSA | North, Central, South America (legacy region being phased out) |
| NORAM | North America |
| Qualified Lead | A lead a Sales Development Representative has qualified, converted to an opportunity and assigned to a Sales Representative (Stage `0-Pending Acceptance`) |
| RD | Regional Director |
| ROW | Rest of World |
| SAL | Strategic Account Leader |
| Sales Admin | Sales Administrator |
| Sales Serve | A sales method where a quota bearing member of the sales team closes the deal |
| [SAO] | Sales Accepted Opportunity - an opportunity Sales agrees to pursue following an Initial Qualifying Meeting |
| SDR | Sales Development Representative |
| Self Serve | A sales method where a customer purchases online through our web store |
| SLA | Service Level Agreement |
| [SCLAU] | Abbreviation for SAO (Sales Accepted Opportunity) Count Large and Up |
| SQO | Sales Qualified Opportunity |
| TAM | Technical Account Manager |
| TEDD | Technology, Engineering, Development and Design - used to estimate the maximum potential users of GitLab at a company |
| Won Opportunity | Contract signed to Purchase GitLab |

[SAO]: /handbook/business-ops/#criteria-for-sales-accepted-opportunity-sao
[SCLAU]: /handbook/business-ops/#glossary

## Customer Lifecycle

A customer lifecycle is a term used to track the different milestones prospective customers go through as they learn about GitLab and interact with our sales and marketing teams. Each subsequent milestone is a subset of the previous milestone, and represents a progression from not knowing GitLab to being a customer (and fan) of GitLab.

At the highest level of abstraction, we use the terms `lead`, `opportunity`, and `customer` to represent a person's progression towards becoming a customer of GitLab. Those three terms also correspond to record types in salesforce.com

Lead => Opportunity => Customer

However, there are more granular steps within the above milestones that are used to track the above process with more precision. They are tracked as follows:

| Funnel stage | Record Type | Status or Stage |
| :----------- | :---------- | :-------------- |
| Raw | [Lead or Contact] | Raw |
| Inquiry | [Lead or Contact] | Inquiry |
| Marketo Qualified Lead | [Lead or Contact] | MQL |
| Accepted Lead | [Lead or Contact] | Accepted |
| Qualifying | [Lead or Contact] | Qualifying |
| Qualified | [Lead or Contact] | Qualified (converted) |
| Pending Acceptance | [Opportunity] | 0 - Pending Acceptance |
| [Sales Accepted Opportunity] | [Opportunity] | 1 - Discovery |
| Sales Qualified Opportunity | [Opportunity] | 2 Scoping - 5 Negotiating |
| Customer | [Opportunity] | 6-Closed Won |

For the definition of the stage please click the record type link.

When going from Qualifying to Qualified Lead the lead is duplicated to an opportunity, and the lead is set to qualified and not being used anymore.

[Lead or Contact]: #lead--contact-statuses
[Opportunity]: #opportunity-stages
[Sales Accepted Opportunity]: #criteria-for-sales-accepted-opportunity-sao

Note: Our lifecycle is undergoing a revamp! See how things are progressing [here](https://gitlab.com/gitlab-com/marketing/marketing-operations/issues/298).

## SAL Sales Capacity
The following calculation is used to measure/plan for sales capacity.  This is a calculation only and should be used to set goals and plan.  Sales capacity is an individual metric that is based on several factors (lead source, tenure of salesperson, competitive landscape, geographic location, rep productivity) not included in the formula below:

* Days to close - 180 days
* Months to close - 6 months
* Win rate - 33%
* Months to lose - 3 months (half of months to close, expecting constant fallout)
* Months on average - 4 (33.3% times 6 and 66.7% of 3)
* Capacity Goal (active opportunities in [Stage 1-6](#customer-lifecycle)) - 40 opportunities
* [SCLAU](#glossary) per month - 10 (40 opportunities / 4 months)


## How tos & Setup

### Events (Conferences, Field Events, Owned Events)

Event details are owned by the Field Marketing Team with execution of system tracking, landing pages, reminders, and follow up completed by Marketing Program Managers.

#### Who to work with

* Event request for sponsorship - Field Marketing Manager (see guidelines to request sponsorship [here](/handbook/marketing/revenue-marketing/field-marketing/#suggesting-we-sponsor-an-event))
* Booth duty and any day-of organization - Field Marketing Manager
* Landing page creation - Marketing Program Manager (with Web Developer/Designer)
* Design assets for event landing page & promotion - Marketing Program Manager (with Designer)
* SFDC & Marketo program creation - Marketing Programs Manager
* Registration confirmation email - Marketing Programs Manager
* Lead list data cleanup and organization of notes - Field Marketing Manager (MOps to help with large corporate events)
* Mass invitation, reminder and follow up email blasts to our marketing database - Marketing Programs Manager

#### How to do Step 1 cleanup of lead lists before passing to MktgOPS

[List cleaning instructions](/handbook/marketing/marketing-operations/list-import/#import-cleaning-template) have been moved to the Import page under Marketing Operations. 

### Webcasts

Webcasts are an excellent tool used by Sales, Marketing and Customer Success to communicate with prospects, customers and partners.

*  [Who to work with](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/virtual-events/#who-to-work-with)
*  [Best Practices](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/virtual-events/webcast/#best-practices)
*  [Speaker Approval](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/virtual-events/webcast/#speaker-approval)
*  [Tips for Speakers](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/virtual-events/webcast/#tips-for-speakers)
*  [Logistical Setup](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/virtual-events/webcast/#logistical-set-up)
*  [Routing](#lead-routing)

## Requesting an Email

To request an email, create an issue in [Digital Marketing Programs project](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/issues/new?issuable_template=Email-Request-mpm), using the `Email-Request-mpm.md` issue template. Be as complete as possible providing all requested detail related to the email, goal, target audience and any other pertinent details. Please review the `Email Review Protocol` section below for more detail. 

Email requests should be submitted **no less than** 72 hours* before intended send date so the new request can be added into the responsible Marketing Program Manager's (MPM) and for select cases (see email review protocol below) into Content team's workflow. The responsible MPM will be determined by type of email requested, [see division of duties](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/#responsibilities).

All links in email sends, going to about.gitlab.com will need to be appended with utm parameters, following the nomenclature outlined in this [document](https://docs.google.com/spreadsheets/d/12jm8q13e3-JNDbJ5-DBJbSAGprLamrilWIBka875gDI/edit#gid=0). This is the way we track and give attribution to emails.

Below are the information from the issue template that will need to be filled out before the MPM will create the email in the appropriate system:

- **Sender Name**: Typically we use GitLab Team for most outgoing communications; for Security Alerts we use GitLab Security. Choosing a name that is consistent with the type and/or content of email being sent is important, if unsure make a note and we will make recommendation.
- **Sender Email Address**: What email address should be used?
- **Approvers**: All approvers must be listed on the email request. At least one individual who will receive the replies to the email must be listed an as approver. For example, if the email is coming from security@, someone who will receive replies to the email should be listed as one of the approvers. See approval table below.
- **Subject Line**: 50 character max is preferred (30-40 characters for mobile devices)
- **Email Body Copy**: Can be a text snippet within issue, clearly identified comment on issue or attach a Google Doc with copy. The copy must be approved before requesting the email.
- **Target Date to Send Email**: at a minimum a few days notice is preferred because we need to balancing the number of emails being sent to our database so they are not perceived (or marked) as spam; however, a simple email can be turned in a few hours if absolutely necessary
- **Recipient List**: Emails can be sent to one of the [existing segments](/handbook/marketing/marketing-operations/marketo#geographic-dma-list ) or a recipient list can be provided as a .csv file
    -  Audience should be appropriately segmented and tokens selected for personalization (if applicable) 
    -  All subscribers are selected list are opted-in to receive your message
    -  If supplying a .csv file, the file must include the following fields:  Email address, First Name (or Full Name)
    -  If personalizing the email to reference a specific project or page, that field must be included in the .csv file and clearly marked using the same terminology used in the email copy. The email copy must clearly identify {{Project}} or {{Page}} where the applicable personalization should be inserted.

**Urgent security emails are exempt from this SLA.*

### Types of email requests

- **Marketing Emails**: Marketing emails are designed to generate leads. The request process outlined is used for ad-hoc marketing emails (not events, webcasts, integrated campaigns, etc as these all have a separate established process). These emails are sent through Marketo using the marketing database or [existing segments](/handbook/marketing/marketing-operations/marketo/#geographic-dma-list).
- **Terms of Service or Privacy Policy Updates**: Terms of Service or Privacy Policy emails are sent to the user base and are not marketing-related. These emails are sent through MailChimp and may require additional approvals, based on the content or number of recipients.
- **Support emails**: Support emails are typically sent to a subset of impacted users and are not marketing-related. These emails are sent through MailChimp.
- **Security emails**: Security emails are sent either to the entire user base or a subset of users and are not marketing-related. They are often urgent, but in the case of the monthly security release, they are scheduled. The monthly security release email is sent through Marketo. Urgent notifications are typically sent through MailChimp.
 
### Approvals and notifications for email requests

Marketing related ad-hoc emails are sent at the discretion of the MPM team.

Terms of Service or Privacy Policy updates that impact all users must be announced on the company meeting, in the `#company-announcements` and `#community-advocates` Slack channels, and approved according to the table below prior to submitting the Email Request.

Support and Security emails sent to a small subset of users should be announced in `#community-advocates` and `#support-managers` Slack channels, and mentioned in `#company-announcements` if relevant.

The approval table below applies to non-Marketing emails.

|  **Users to be contacted** | **Approval by** |
| --- | --- |
|  <1,000 | reply-to owner |
|  1,001-4,999 | PR, reply-to owner, community advocate |
|  5,000-499,999 | PR, reply-to owner, community advocate, director+ in originating department |
|  500,000+ | PR, reply-to owner, community advocate, director+ in originating department, e-group member |

### Email review protocol

All MPMs and reviewers should adhere to the following protocol for every marketing email that is sent to ensure brand consistency and quality in our email program. 

#### Goals & Audience

*  Goal of the campaign is clearly defined with 1 main CTA
    *  If part of a nurture series, each email has main CTA with a main CTA for the entire series
*  Success of the campaign is defined with measurable KPIs
*  Personalization added (if applicable)
*  All suppressions have been applied
*  Subscribers are opted-in
*  All SPAM and privacy laws are being recognized (GDPR, CAN-SPAM, CASL, etc.)
*  We will send event and webcast invite emails to those who are in our database. Accounts with open opportunities in **late stages 4-6** will not be included in the email send. We do this because we know it takes many marketing touches to help bring an opportunity to closure.

*Note: If you would like additional people to receive a test email prior to sending it out, please specify that in the request template and refer them to this protocol for reviewing the email.*

#### Envelope

*  From address and name are recognizable as the business
*  Subject line
    *  Descriptive, clear, and concise
    *  Length: Less than 50 characters (aim for 30-40 for mobile devices)
    *  No obvious spammy words (if in doubt, use Litmus to test)
    *  Personalization added where applicable
*  Preview/preheader text
    *  Length: depends on the email client but anywhere from 40-90 characters
    *  Descriptive, clear, and concise

#### Body

*  Any content pulled from a template is replaced with main message
*  Only relevant content is included. Follow our brand guidelines for [tone of voice](/handbook/marketing/corporate-marketing/#tone-of-voice) when evaluating copy. Put yourself in the subscriber’s shoes. Ask the question, “What’s in it for me?”
*  The main call-to-action is descriptive, clear, and ties directly back to the campaign goal(s)
*  Company contact information with physical address is included
*  No grammar or spelling issues
*  Unsubscribe link is visible and works

#### Design

*  Message renders properly across desktop, mobile, and tablet views
*  Message renders properly across main email clients (use Litmus to determine top email clients used by subscribers)
*  Calls-to-action are easily identified and interact with
*  All links work and are being tracked appropriately (UTMs applied where needed)
*  Any dynamic content or personalization included merges properly
*  Images work and have descriptive ALT text
*  Tracking and analytics are in place and work
*  Font and colors are matched or closely matched to our [brand guidelines](/handbook/marketing/corporate-marketing/#brand-guidelines)

### Internal Email List

There is an internal email list, called `INTERNAL - Email Send List` in Marketo that will be included on every outbound email that is sent. If you are a team member and wish to be included on every email that is sent, please post a request to the `#marketing-programs` slack channel and the MPMs will review. To avoid skewing email results (particularly on smaller sends), this list will be kept to a minimum.

If you are an internal team member and wish to subscribe to a segment or segments please subscribe through the [preference center](/company/preference-center/) and you will only be included in those dedicated email sends.

## Record Management

### MQL Definition
A Marketo Qualified Lead is a lead that has reached a certain threshold, we have determined to be 90 points accumulated, based on demographic, firmographic and/or behavioral information. The "MQL score" defined below is comprised of various actions and/or profile data that are weighted with positive or negative point values.
Any record with a `Person Score` greater than or equal to 50 points will be inserted into the routing flow. Using LeanData every time a `Person Score` is updated, LeanData will run a check to see if the record needs to be processed through the flow.

### MQL Scoring Model
The overall model is based on a 100 point system. Positive and negative points are assigned to a record based on their demographic and firmographic information, and their behavior and/or engagement with GitLab marketing.

The MQL scoring model below is correct as of 30 September 2018. Additional changes are being made and the following will be updated over time.

#### MQL = 90 pts
{:.no_toc}

##### Positive Point Values
{:.no_toc}
  * 100pts
     * Completes self-hosted or SaaS trial request form^
     * Completes a Contact form
     * Completes a Professional Services Request form
     * Completes a Public Sector Request form
  * 90 pts
     * Fill out [high intent](#glossary) content form related to Force Management 
     * Attends [high intent](#glossary) live webcast, livestream or demo
  * 50 pts
     * Title contains “VP, Manager, Director, Senior, or Head”
     * Visits Enterprise trial page but doesn’t complete form
  * 45 pts
     * Watches high intent on-demand webcast, livestream or demo
  * 40 pts
     * `Follow Up Requested` in Conference/Field Event/Speaking Session campaign - manual process when lists are uploaded
     * Attends Live in-person/Owned Event - manual process when lists are uploaded
  * 30 pts
     * `Visited Booth` in Conference/Field Event campaign - manual process when lists are uploaded
     * `Attended` in Speaking Session Event campaign - manual process when lists are uploaded
     * Downloads any gated asset
  * 15 pts
     * Registers for any livestream, webcast or demo
     * Attends low intent live webcast
     * Watches low intent on-demand webcast
  * 10 pts
     * Opts into Newsletter
     * Opts into Security Newsletter
     * Opts into webcast emails
     * Opts into live event/conference emails
     * Visits about.gitlab.com/pricing page
     * Visits about.gitlab.com/features page
  * 5 pts
     * Valid company email
  * 2 pts
     * Visits about.gitlab.com/installation page

##### Negative Point Values
{:.no_toc}
  * -5 pts
     * Email is @ “gmail, hotmail, yahoo, aol” (or other free-domained email)
  * -10 pts
     * Title is “blank, numerical, developer, engineer”
  * -25 pts
     * Email unsubscribe
     * Multiple career page visits in 7 days

^In-product trial requests for SaaS and self-hosted are applied using batch method that runs daily at 6a Pacific time.


### Segmentation
Sales Segmentation is based on `Total Employee` count of the `Global Account`. If a `Global Account` has a lower segment than any of its child accounts, the `Global Account` will adopt the largest sales segment of any of its child accounts.
  * `Large` = 2,000+ total employees
  * `Mid-Market` = 100-1,999 total employees
  * `SMB` (Small Business) = 0-99 total employees

`Total Employee` count is based on the number of employees that our data tools return for that account **as determined in the [sales segment review process time period](#Sales-Segment-Review-Process)**. We use a hierarchy structure to determine what the number of employees is for the account. The hierarchy of our data tools on *Accounts* as they relate to the `Total Employee` count is shown below.

1. DataFox.......(Default Value)
2. DiscoverOrg...(Only used if DataFox Employee Count field is blank)

LinkedIn/Websites are not designated data sources. If a prospect communicates a different employee size from DataFox/DiscoverOrg that conflicts with segmentation of what is determined by DataFox/DiscoverOrg then SalesOPS should be notified via chatter on the record. Admins have the ability to override the `Number of Employees` and bypass this hierarchy but only during our [sales segment review process](#Sales-Segment-Review-Process). 


#### Sales Segment and Hierarchy Review Process
In order to address issues when it is believed that the `Total Employee` count is incorrect the Sales Ops team on a Yearly schedule(Fiscal Q4) will review accounts where individuals think that the segment is incorrect as well as any account that has had their number of employees changed (according to our data sources). Reviews for updates to the `Total Employee` count field that do not result in a change of segment will not be reviewed.

For an individual to submit an account for review as it relates to the number of employees at the account they must fill out the following two fields on an accounts:
* `Number of Employees: Manual - User` - This is a number field that you think the number of employees should be
* `Number of Employees: Manual Source -User` - This is a URL field that links to where the above information was found

For an individual to submit an account for review as it relates to the hierarchy and final address of the account they must fill out the following four fields on an account:
*  `Account Zip - Manual - User` - This is a text field to be populated with Global Account HQ's Zip
*  `Account State - Manual - User` - This is a text field to be populated with Global Account HQ's State
*  `Account Country - Manual - User` - This is a text field to be populated with Global Account HQ's Country
*  `Account Address - Manual Source - User` - This is a URL field that links to where the above information was found

Examples of valid sources include but are not limited to financial filings, newspaper articles, reports directly from the company. As a rule LinkedIn is not accepted as a valid source. During the Sales Ops review period it is at the discretion of the Sales Ops team to have the `Total Employee` count updated or to have it remain the same.

If the number of employees, according to our sources based on our hierarchy as described in [Segmentation](#Segmentation), has changed the Sales Ops team will automatically update the accounts segment and resulting ownership at the completion of the review process. 

While the review process occurs over the course of Q4 the results of the process will not be put into place or enforced until the begining of Q1 (or as announced by the Sales Ops team)


### Region/Vertical
  * **VP Commercial Sales** (Mid-Market & Small Business): Ryan O'Nell
  * **[Europe, Middle East and Africa](#emea)**: Mike Pyle, VP of Enterprise Sales (interim)
  * **[Asia Pacific](#apac)**: Anthony McMahon, Regional Director
  * **[North America - US East](#us-east)**: Mark Rogge, Regional Director
  * **[North America - US West](#us-west)**: Haydn Mackay, Regional Director
  * **[Public Sector](#public-sector)**: Paul Almeida, Director of Federal Sales

### Territories

[Territory tables](/handbook/sales/territories) are maintained within the Sales Handbook. Both maps & written tables are kept up to date with all pairings and territory assignments. Our LeanData routing workflows and SFDC reports are based on these tables.

The Location of each account used to determine its Sales Territory is determined by a combination of 3rd party data systems (Datafox, DiscoverOrg) and manual overrides. This address is stored in "Account - Territory" on the Account object in SalesForce. This field inherits data from other fields in the following priority: 1. Admin Manual Override (if present) 2. Datafox 3. DiscoverOrg 4. Shipping Address 5. Billing Address. 


### Account Ownership Rules of Engagement

1. **Source of Data**: The data source priority order for `Employee` count, `Address`, `Industry` and `Corporate Hierarchy` will be Datafox, DiscoverOrg, Linkedin; otherwise <blank> or `[[unknown]]` until resolved through manual research.  Any disputes must follow the Final Decision Escalation Process below. These data points are locked in during [the sales segment review process](#sales-segment-review-process) 
1. **Account Ownership**: Will be determined by the **Sales** `Segment`, `Address` and `Corporate Hierarchy` and all children accounts, regardless of physical location. All of the accounts will be owned by the *Global Account* owner unless it is either a Named Account (see point 3) or it has been agreed upon by both reps and their managers that the customer is best serviced by the *Territory* rep (see point 13).
1. **Named Account**: Defined as an account that is owned by a sales rep regardless of corporate headquarters. A sales rep will own no more than 30 named accounts.
1. **Transfer of Named Accounts**: A transfer and ownership time frame of a Named Account should be agreed upon by both sales reps and their managers.
1. **Open Opportunities of Transferred Accounts**: Any open opportunity on an account subject to transfer to the *global account* owner will remain with the original owner for a period of no more than 180 days after opportunity creation. No later than the 120 day mark, the original owner can request an extension and must provide sufficient evidence that the deal will close within the next 90 days. If the evidence is insufficient, the *global account* owner can request that the opportunity be transferred immediately. The are two reports that track holdover opportunities: [New Business/Add Ons](https://gitlab.my.salesforce.com/00O61000004hitu) and [Renewals](https://gitlab.my.salesforce.com/00O61000004hmUy). These reports should be reviewed weekly by new account owners expecting to receive a holdover opportunity that has stalled or existing opportunity owners whose opportunities may be subject to transfer to the new account owner.
1. **Reassigning to a Territory Rep**: The *global account* owner can reassign any child account to a *territory rep* if it is determined that the client/prospect would be best serviced by a local rep. To do this, please Chatter the *territory rep* and provide an explanation on the transfer. Please review point 12 'Considerations for Transferring an Account to a Local Rep'.
1. **Requesting Reassignment**: A *territory rep* can request reassignment of a child account if they feel that the client/prospect would be best serviced by a territory rep as opposed to the *global account owner*. To do this, the *territory rep* must Chatter the *global account* owner and provide an explanation, (please see point 12, “Considerations for Transferring an Account to a Local Rep”). It is at the discretion of the *global account* owner to keep or reassign the account, but they must provide a compelling and explicit reason why a *territory* account should be managed globally. If the *territory rep* does not agree with the decision, it can be discussed by their respective managers.
1. **Parent/Child Segmentation**: All Accounts in a hierarchy will adopt the MAX Segmentation of any account in the hierarchy.
1. **Changes to Ultimate Parent Details**: In the event of a merger or acquisition, or any other changes that impact the ownership of an account, such as a move of headquarters to another territory, either the *global account* owner or *territory* sales rep should submit the updated information in accordance with [the sales segment review process](#sales-segment-review-process), who will then initiate a review of all affected accounts. A transition plan (if needed) should be agreed upon by all reps and their managers.
1.  **Exceptions**:
    1. **Spirit of Collaboration**: All requests and or actions must adhere to the Gitlab Value of “Collaboration” and proactively communicate the inquiry and/or intent to all parties affected.
    1. **Indisputable** (not including Employee Count): reps must provide evidence and Sales Ops will render ruling; otherwise escalates to Final Decision Escalation Process.
    1. **Newly updated accounts**: will be reviewed in the annual review process as this impacts TAM and quota assignment.  Holdover of an active deal will be dealt with on a case-by-case basis following the Final Decision Escalation Process.
    1. **Stand-alone Child Account**: can be considered if the Child Account clearly has their own buying authority and purchasing process. For example:
        1. Private Equity or Holding Company : Child Accounts
        1. Government Holding Entity : Child Entity
        1. HQ : Franchises or Consultants (Note: Franchises do not count towards HQ Total Employee Count)
1. **Final Decision**: In all situations where an agreement between the reps, ASM/RDs and/or VPs cannot be reached; CRO will determine final ruling.
1. **Ownership**: All Lead, Contacts and Accounts are to be owned by the owner of the Account (RD/SAL/AE) [per the handbook](#record-ownership). **NOTE: Working a deal does not mean ownership.**
1. **Considerations for Transferring an Account to a Local Rep**: If the decision-making power, end users, PO and Terms (or a majority combination) are confined to the child account, the Ultimate Parent owner should hand off the Lead to the appropriate Territory owner as this would be in the best interests of the customer and for GitLab.



### Website
Since an accounts `Website` is a key data point in determining [the accounts segment](#segmentation) and [the accounts address](#account-ownership-rules-of-engagement) and thus the resulting territory and ownership, the website on an account in salesforce is a required field on the layout. In the event that the account is linked to an individual that uses a free email domain (or other similar cases) than the value of `[Blank]` should be used as the value for the accounts website.



### Initial Source
`Initial Source` is first "known" touch attribution or when a website visitor becomes a known name in our database, once set it should never be changed or overwritten. For this reason Salesforce is set up so that you are unable to update both the `Initial Source` and `Lead Source` fields. If merging records, keep the `Initial Source` that is oldest (or set first). When creating Lead/Contact records and you are unsure what `Initial Source` should be used, ask in the `#lead-questions` Slack channel.

The values listed below are the only values currently supported. If you attempt to upload or import leads or contacts into Salesforce without one of these initial sources you will encounter a validation rule error. If you think that there needs to be a new Initial Source added to this list and into Salesforce please slack the appropriate team member(s) listed in the [Tech Stack](/handbook/business-ops/tech-stack-applications/#tech-stack-applications).

The `Initial Source` table below is current as of 9 October 2019.

Status in the table below means:
- Active = can be selected from picklist
- Inactive = cannot be selected from picklist, but a record may exist with this source

| Source                          | Definition and/or transition plan                                                                            | Status*  |
|:--------------------------------|:-------------------------------------------------------------------------------------------------------------|:---------|
| Advertisement                   | to be evaluated                                                                                              | Active   |
| AE Generated                    | Sourced by an Account Executive through networking or professional groups                                    | Active   |
| CE Download                     | Downloaded CE version of GitLab                                                                              | Active   |
| CE Usage Ping                   | Created from CE Usage Ping data                                                                              | Active   |
| CE Version Check                | to be evaluated                                                                                              | Inactive |
| Clearbit                        | transition to `Prospecting` -> sub field `Clearbit`                                                          | Active   |
| Conference                      | Stopped by our booth or received through event sponsorship                                                   | Active   |
| CORE Check-Up                   | will be activated for new records created by the Instance Review in-product                                  | Inactive |
| Datanyze                        | transition to `Prospecting` -> sub field `Datanyze`                                                          | Active   |
| Demo                            | Filled out form to watch demo of GitLab                                                                      | Active   |
| DiscoverOrg                     | transition to `Prospecting` -> sub field `DiscoverOrg`                                                       | Active   |
| Education                       | Filled out form applying to the Educational license program                                                  | Active   |
| EE Version Check                | to be evaluated                                                                                              | Inactive |
| Email Request                   | Used when an email was received through an alias (*will be deprecated*)                                      | Active   |
| Email Subscription              | Subscribed to our opt-in list either in preference center or various email capture field on GitLab website   | Active   |
| Employee Referral               | to be evaluated                                                                                              | Active   |
| Event partner                   | to be evaluated                                                                                              | Inactive |
| Field Event                     | Paid events we do not own but are active participant (Meetups, Breakfasts, Roadshows)                        | Active   |
| Gated Content - General         | Download an asset that does not fit into the other Gated Content categories                                  | Active   |
| Gated Content - eBook         | Download a digital asset categorized as an eBook                                 | Active   |
| Gated Content - Report          | Download a gated report                                                                                      | Active   |
| Gated Content - Video           | Watch a gated video asset                                                                                    | Active   |
| Gated Content - Whitepaper     | Download a white paper                                                                                       | Active   |
| Gemnasium                       | Previous a Gemnasium customer/prospect merged into our database when acquired                                | Active   |
| GitLab Hosted                   | GitLab Hosted customer/user                                                                                  | Active   |
| GitLab Subscription Portal      | Account created through the Subscription app (check for duplicates & merge record if found)                  | Inactive |
| GitLab.com                      | Registered for GitLab.com account                                                                            | Active   |
| Gitorious                       | Previous a Gitorios customer/prospect merged into our database                                               | Active   |
| gmail                           | unknown, to be deprecated                                                                                    | Inactive |
| InsideView                      | transition to `Prospecting` -> sub field `InsideView`                                                        | Inactive |
| Leadware                        | transition to `Prospecting` -> sub field `Leadware`                                                          | Active   |
| Legacy                          | to be evaluated                                                                                              | Active   |
| LinkedIn                        | transition to `Prospecting` -> sub field `LinkedIn`                                                          | Active   |
| Live Event                      | transition to correct category based on first event attended -> `Owned Event`; `Field Event` or `Conference` | Active   |
| MovingtoGitLab                  | to be evaluated                                                                                              | Inactive |
| Newsletter                      | to be evaluated                                                                                              | Active   |
| OnlineAd                        | to be evaluated                                                                                              | Inactive |
| OSS                             | Open Source Project records related to the OSS offer for free licensing                                      | Active   |
| Other                           | Should never be used but is a legacy source that will be deprecated                                          | Active   |
| Owned Event                     | Events that are created, owned, run by GitLab                                                                | Active   |
| Partner                         | GitLab partner sourced name either through their own prospecting and/or events                               | Active   |
| Promotion                       | to be evaluated                                                                                              | Active   |
| Prospecting                     | Account research and development prospecting work                                                           | Pending  |
| Prospecting - LeadIQ            | transition to `Prospecting` -> sub field `LeadIQ`                                                            | Active   |
| Public Relations                | to be evaluated                                                                                              | Active   |
| Referral                        | to be evaluated                                                                                              | Inactive |
| Registered                      | transition to correct event type source                                                                      | Inactive |
| Request - Contact               | Filled out contact request form on GitLab website                                                            | Active   |
| Request - Professional Services | Any type of request that comes in requesting to engage with our Customer Success team                        | Active   |
| Sales                           | to be evaluated                                                                                              | Inactive |
| SDR Generated                   | Sourced by an SDR through networking or professional groups                                                  | Active   |
| Security Newsletter             | Signed up for security alerts                                                                                | Active   |
| Seminar - Partner               | not actively used - transition to `Owned Event` or `Field Event`                                             | Active   |
| SocialMedia                     | to be evaluated                                                                                              | Inactive |
| Swag Store                      | to be evaluated                                                                                              | Inactive |
| Trial - Enterprise              | In-product or web request for self-hosted Enterprise license                                                 | Active   |
| Trial - GitLab.com              | In-product SaaS trial request                                                                                | Active   |
| Unknown                         | need to evaluate what records are in this status - it should never be used                                   | Inactive |
| Unsubscribe Form                | to be evaluated                                                                                              | Inactive |
| Web                             | transition to `Web Direct`                                                                                   | Active   |
| Web Chat                        | Engaged with us through website chat bot                                                                     | Active   |
| Web Direct                      | Created when purchase is made direct through the portal (check for duplicates & merge record if found)       | Active   |
| Webcast                         | Register for any online webcast (not incl `Demo`)                                                            | Active   |
| Word of Mouth                   | to be evaluated                                                                                              | Active   |
| Zoominfo                        | transition to `Prospecting` -> sub field `Zoominfo`                                                          | Inactive |


### Lead & Contact Statuses
The Lead & Contact objects in Salesforce have unified statuses with the following definitions. If you have questions about current status, please ask in #lead-questions channel on Slack.

| Status | Definition |
| :--- | :--- |
| Raw | Untouched brand new lead |
| Inquiry | Form submission, meeting @ trade show, content offer |
| MQL | Marketo Qualified through systematic means |
| Accepted | Actively working to get in touch with the lead/contact |
| Qualifying | In 2-way conversation with lead/contact |
| Qualified | Progressing to next step of sales funnel (typically OPP created & hand off to Sales team) |
| Unqualified | Contact information is not now or ever valid in future; Spam form fill-out |
| Nurture | Record is not ready for our services or buying conversation now, possibly later |
| Bad Data | Incorrect data - to potentially be researched to find correct data to contact by other means |
| Web Portal Purchase | Used when lead/contact completed a purchase through self-serve channel & duplicate record exists |

### Routing
Routing is determined by `Sales Segmentation`, `Region`, and `Global Account Ownership`. Routing through Lean Data when a record has no less than 30 points, this means that they have engaged with at least one piece of content or visited a high value page.

#### Routing & LeanData   

**LeanData** works within the Salesforce ecosystem and is the primary tool leveraged to manage all routing workflows. The Marketing Operations team is responsible for on-going management and customizations within LeanData. For more information see the [dedicated LeanData page](/handbook/marketing/marketing-operations/leandata).    

#### Contact Requests
All `Contact Us` requests must be followed up within **one (1) business day** Service Level Agreement (SLA) and follow up must be tracked as an activity on the record within Salesforce.

U.S. Public Sector: Routed to the U.S. Public Sector Inside Sales team.
- [GitLab Public Sector Rules of Engagement](/handbook/sales/public-sector/engaging-public-sector.html)

#### Professional Service Requests
`Professional Service Requests` are treated like a [`Contact Us` request](#contact-us-requests) and followed up within **one (1) business day** Service Level Agreement (SLA). Follow up must be tracked as an activity on the record within SFDC.

Requests submitted through the professional services page will be routed following `Global Account Ownership` rules. Notification of form submission will be sent to the Strategic Account Leader (SAL) and Sales Development Representative (SDR) as well as Customer Success manager. Initial response to form submission is the responsibility of the Account Owner (i.e. SAL).

#### Trial Requests
Trials can be requested through [web form](/free-trial/) or within product UI for both self-managed or SaaS. Default trial length is thirty (30) days, but can be manually extended by the GitLab team for both the SaaS and self-managed products. Trial extensions for the SaaS product use the [`plan_change_request` issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=plan_change_request) template found in the `dotcom` Group, `dotcom-internal` project. Extending self-managed trials requires access to the internal `Licensing App`.

#### Universities

##### United States
- **Public** University = [Public Sector team](/handbook/sales/territories#public-sector)
- **Private** University = Sales Development Representative (Enterprise or Commercial, based on `Sales Segment`)

##### Rest of the World
- **Any** University = appropriate regional Sales Development Representative


### Record Ownership
Contacts on accounts owned by a member of the Field Sales Team (RD/SAL/AE/AM), will be owned by the named Account Owner (i.e both the Account and Contact ownership will match). When an SDR is assigned to an Account to support and assist with outreach, the SDR will be added in the `SDR Assigned` lookup field to the account in Salesforce. This field then populates down to the related Contact records. Only SDRs are able to edit the `SDR Assigned` field and if there is a need to mass update the `SDR Assigned` on many accounts then the SDR should reach out to a member of the Sales Ops Team for support. 

Records, both `LEAD` and `CONTACT`, need to be synced to Outreach to ensure email activity is properly mapped back to `Activity History` in SFDC. The owner of the record in SFDC **does not** need to match the owner in Outreach.

#### Record Ownership and Record Visibility
In order to meet compliance standards our SFDC instance uses a private model. This private model allows for some records to be visible by all Gitlabbers who use Salesforce while other recrods may not be visible to them. Currently this is in place as it pertains to records owned by the Public Sector team. All salesforce records (leads, contacts, accounts, opportunities etc.) owned by the Public Sector team are only visibily to other members of the public sector team and a group of supporting staff who have been reviewed and permitted to view the these records. All other records (owned by non-public sector team members) maintain their standard visibility levels.

This is important as it relates to inbound records or accounts in a sales reps name. If you believe you have been incorrectly assigned a record that should belong to the public sector team member please coordinate with your manager, the sales-ops team or a member of the public sector team to review the record.

### Changing Ownership in Salesforce

#### Changing Account Ownership in Salesforce
Everyone in Salesforce has **some** ability to change the ownership of accounts. When accounts have their owners changed, by anyone other then an admin, there will be an email notification go out to both the previous account owner and the new account owner. This is to allow individuals to change ownership of accounts if they think they should belong to them. If there are any questions in regards to who should own an account Sales Ops will assist in that decision and you can mention @sales-ops in salesforce. It's also important that just because a user can change the owner of an account does not mean that they should own the account. Please refer to the criteria for reassigning accounts and our account territories for more information.

*  Criteria for Reassigning Accounts
*  The account must have its address in the account owners territory. If the account has a parent account or the parent account also has a parent account the address that determines the final owner of the account is the address of the ultimate parent. This address follows our data hierarchy - with Datafox being our primary source of data (Link to come)
*  The account must also have a matching sales segmentation that the owner should be working. Any Account adopts the highest sales segment that exists within an account hierarchy. Segment is determined by our data hierarchy - with Datafox being our primary source of data (Link to come)
*  Any owner of an account must follow our guidelines for [Record Ownership](#record-ownership)

1.  Any account owner can reassign their own account to someone else
2.  Any RD can reassign any account
3.  Any Team Lead can reassign any account that is located within their region
4.  Anyone can reassign any account as long as the following criteria is met
    A.  The account does not have a parent account
    B.  The account is located in the same region as the individual transferring ownership of the account
    C.  Datafox has enriched the number of employees on the account
    D.  The sales segment of the account is the same as the segment that the user is working on (SALs/Large,AEs/Mid-Market)
5.  Any Admin can reassign any account

#### Changing Contact Ownership in Salesforce
Everyone is able to change the owner of a contact as long as they are either changing the Contact Owner to match the Account Owner or they are the current Contact owner. Since all contacts are to be owned by the owner of the contacts account this should address all needs to update contact ownership.

#### Changing Lead Ownership in Salesforce
Lead ownership follows the same rules as contact ownership - whoever owns the account also owns all of the leads. However since leads are not directly tied to Accounts someone looking to update the ownership of a lead should match the leads data points with our rules related to [Global Account Ownership](#global-account-ownership), [Named Account Ownership](#named-account-ownership) as well as [Territory Account Ownership](#territory-account-ownership). Regional Directors, Team Leads and Admins can all change the ownership of any lead.

#### Default Ownership 
*  In the event that Ops encounters that there is not enough information to assign a record to a specific user in Salesforce it is to be assigned to the default user: [`Sales Admin`](https://gitlab.my.salesforce.com/00561000000mpHT?noredirect=1&isUserEntityOverride=1). **This user should only be used by ADMINS. Non-Admins should not be reassigning records to this user**. Before assigning to this user, admins should do their best to assign records to the actual users within Salesforce. If you are unsure of who to assign it to please coordinate with the SalesOps Team. This is also only a temporary solution until we have a more scalable solution in place that will reassign records to individuals who can and will actually be able to to work recrods. 

### Record Creation in Salesforce
ACCOUNT/CONTACT records in Salesforce are created in a number of ways - [list imports](#list-imports), [mass creation screen flows](#mass-create-contact-on-opportunities-with-contact-roles), field event booth scans, research, networking, webcasts, content downloads. Ideally all ACCOUNTS exist in Salesforce and team members are only creating CONTACT records; however, if a connection is made at an event and follow up needs to be done *prior* to official event list upload occurs team members should do the following:
   - Search Salesforce to be sure ACCOUNT does not already exist **AND** search using the person's email address to ensure duplicate record is not created
   - Record **does not** exist:
        - Create `Standard` ACCOUNT type - required fields are `Account Name` & `Account Type`
        - Create `Standard` CONTACT type - required fields are `Last Name`, `Account Name` (use lookup tool to find ACCOUNT just created) & `Initial Source` (i.e. where is this name coming from `Conference` = Field Event, `SDR Generated` or `AE Generated` = regular networking event, etc)
        - Be accurate where the name is collect from, `Unknown` is **not** acceptable.
        - The `Initial Source` on a CONTACT record *does not* equal `Source` on an opportunity. Refer to [`Initial Source`](#initial-source) for guidance on why this is important.
   - Record **does** exist:
        - If LEAD or CONTACT is unowned or "owned by Sales Admin, James Harrison or Chad Malchow", this record is adoptable by anyone - change `Record Owner` to your name
        - If LEAD or CONTACT is owned by SDR team member, **before** reaching out Chatter on the record asking SDR to transfer ownership. Ownership *must* be transferred **before** reaching out to avoid confusion, cross-communication and/or multiple people reaching out to same contact.

When official event list import is completed the created ACCOUNT or CONTACT record will be appended with the additional data collected at the event. If there are any questions or you need assistance, please ping Marketing or Sales OPS in Slack `#sfdc-users` channel.

#### Best practices
1. Be as accurate with your data as possible. If you do not have a Contact `Phone` do not substitute the Account `Phone` - Leave it blank on the Contact record.
2. Search the database for duplicates before creating new records.
3. When merging records, retain the `Initial Source` of the record that was created first.


### Mass create contacts on opportunities with contact roles

This process is specific for the unique cases of creating totally new contacts for an account that also have to be associated with an opportunity. An example of when to use this process is when you meet a number of new contacts at an account during a demo for a specific opportunity. The process to create these contacts for that account and to have them related with that opportunity would be through the steps listed below or as demonstrated in this [video](https://drive.google.com/file/d/1iEO4dQUAfa4tkbEmip1Xne7-9Tg2nR6h/view?usp=sharing):

1. Navigate to the Opportunity record in Salesforce that these contacts should be associated with
2. Click on the button `New Contacts & Opp Contact Roles`
3. Follow the screen flow and instructions for creating all contacts and associating them with the opportunity, providing all required and known information
4. If there is additional information for any of the contacts that you have but you were not able to input the information via the screen flow, navigate to the contact(s) once the operation is complete and fill in any additional information you have for the contact(s)

It is important to note that by following this process that all contacts must meet the following criteria:
1. All of the contacts that are created are to be associated with both the account and opportunity for that opportunity record.
2. All of the contacts are net new and do not exist within Salesforce already - as either contacts or leads.
3. All of the contacts will be assigned a contact role on the opportunity.
4. There already is a primary contact, or one of the new contacts will be the primary contact on the opportunity.


#### List Imports

The [list import instructions & process](/handbook/marketing/marketing-operations/list-import/) has been moved to the Marketing Operations section of the handbook. 

#### Rules of Engagement

Named Accounts are owned and worked by the designated Strategic Account Leader (SAL) and the paired Sales Development Representative (SDR). This pairing owns all records (LEADS and CONTACTS) associated to a Named Account and any related Child accounts within SFDC. See [global ownership](#global-account-ownership) and [named account](#named-account-ownership) descriptions above.

Territories are assigned based on [Sales Segmentation](#segmentation) and routing for each type of inbound request is [listed above](#lead-routing).


LEAD/CONTACT Records with the `Initial Source` of `GitLab.com` are **not** to be engaged, prospected or targeted unless they have taken a handraising 'active' activity, such as `Trial - Enterprise`, `Trial - GitLab.com`, `Contact Us`, `Demo`, 'Webcast', 'Content' and/or engaged in `Web Chat`.

For information about GitLab's email policy and the types and number of emails we send, please see our [Email Communication Policy](/handbook/marketing/marketing-operations/index.html#email-communication-policy).

#### Active vs. Passive

`Initial Source` cannot be used to determine if a lead is 'active' or 'passive' since the Initial Source is set upon first touch attribution; therefore, looking at the `Last Interesting Moment` field is the primary field used to begin determining if a record is actively being worked. Reviewing the `Activity History` in Salesforce is another factor considered when evaluating 'active' or 'passive'.

A LEAD or CONTACT is considered 'Active' if they have taken an `Trial - Enterprise`, `Trial - GitLab.com`, attended a high intent live webcast or demo and/or engaged `Web Chat`, these are all handraising 'active' activities. These types of records are considered 'Active' for a minimum of 60 days from the date of the handraising activity. For example: the record is considered 'Active' for entire duration of EE trial, plus 30 days after `EE Trial End Date`.


## Campaigns
Campaigns are used to track efforts of marketing tactics - field events, webcasts, content downloads. The campaign types align with how marketing tracks spend and align the way records are tracked across three of our core systems (Marketo, Salesforce and Bizible) for consistent tracking. Leveraging campaign aligns our efforts across Marketing, Sales and Finance.
### System Set-up

#### Salesforce Campaigns
There are [**MASTER** Campaign templates](https://gitlab.my.salesforce.com/70161000000CnPg) created for each of the campaign types with the correct progression statuses pre-designed. When creating a new campaign, clone the template & modify the name to match the program/event. If you inadvertently set up the campaign using the wrong campaign type, you will need to update the member status (in advanced) and resync through Marketo. Marketing Ops can assist if needed.

SFDC template quick links (only available when logged in):
- [Cohort] (link to be added)
- [Conference](https://gitlab.my.salesforce.com/70161000000CnPH)
- [Field Event](https://gitlab.my.salesforce.com/70161000000CnPM)
- [Gated Content] (link to be added)
- [Geographic](https://gitlab.my.salesforce.com/7014M000001llpy)
- [Inbound Request](https://gitlab.my.salesforce.com/70161000000VwZW)
- [List Build](https://gitlab.my.salesforce.com/70161000000VwYO)
- [Owned Event](https://gitlab.my.salesforce.com/70161000000CnPR)
- [PathFactory Listener](https://gitlab.my.salesforce.com/7014M000001lmxy)
- [Referral Program] (link to be added)
- [Speaking Session](https://gitlab.my.salesforce.com/70161000000CnPW)
- [Trial](https://gitlab.my.salesforce.com/70161000000VwYT)
- [Virtual Sponsorship](https://gitlab.my.salesforce.com/70161000000CnP7)
- [Webcast](https://gitlab.my.salesforce.com/70161000000CnPb)


#### Marketo Programs

The Marketo programs for the corresponding campaign types have been prebuilt to include all the possible necessary smart campaigns, email programs, reminder emails and tokens that are to be leveraged in the building of the program.

Marketo program quick links (only available when logged in w/ `Marketing Activities` access):
- Programs to be added with links


### Campaign Type & Progression Status
A record can only progress **one-way** through a set of event statuses. A record *cannot* move backward though the statuses.

i.e. Record is put into `Registered` cannot be moved backward to `Waitlisted`


#### Cohort
A method of tracking a group (cohort) of targeted known records and/or records included in an ABM strategy. All touchpoints related to this specific campaign are excluded from Bizible tracking.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Nominated                 | ACCOUNTS/CONTACTS Sales has identified for inclusion that Marketing would otherwise be suppressing because of late-stage open opps &/or active sales cycle |        |
| Marketing List               | ACCOUNTS/CONTACTS Marketing has identified for inclusion based on the target audience, the "ABM list", demographic, etc.                    |          |
| Organic Engaged           | LEADS/CONTACTS added to the campaign through the listening campaigns that engage with the pages &/or assets for the integrated campaign that do not contain `utm_` params        | Yes      |


#### Conference
Any large event that we have paid to sponsor, have a booth/presence and are sending representatives from GitLab (example: AWS). This is tracked as an *offline* Bizible channel.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Invited                   | Invitation/Information about event sent by Sales/SDR                                  |          |
| Sales Nominated                 | Sales indicated record to receive triggered event email sent by Marketing             |          |
| Marketing Invited               | Marketing geo-targeted email                                                          |          |
| Meeting Requested               | Meeting set to occur at conference                                                    |          |
| Meeting No Show                 | Scheduled meeting at conference was cancelled or not attended                         |          |
| Meeting Attended                | Scheduled meeting at conference was attended                                          | Yes      |
| Visited Booth                   | Stopped by booth for any reason                                                       | Yes      |
| Follow Up Requested             | Requested additional details about GitLab to be sent post event                       | Yes      |

#### Field Event
This is an event that we have paid to participate in but do not own the registration or event hosting duties (example: Rancher event). This is tracked as an *offline* Bizible channel.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Invited                   | Invitation/Information about event sent by Sales/SDR                                  |          |
| Sales Nominated                 | Sales indicated record to receive triggered event email sent by Marketing             |          |
| Marketing Invited               | Marketing geo-targeted email                                                          |          |
| Waitlisted                      | Holding state if registration is full will be moved to `Registered` if space opens    |          |
| Registered                      | Registered for event                                                                  |          |
| No Show                         | Registered but did not attend event                                                   |          |
| Attended                        | Attended event                                                                        |          |
| Visited Booth                   | Stopped by booth for any reason                                                       | Yes      |
| Follow Up Requested             | Requested additional details about GitLab to be sent post event                       | Yes      |

#### Gated Content
White Paper or other content offer. This is tracked as an *online* Bizible channel.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Downloaded                      | Downloaded content                                                                    | Yes      |

#### Geographic  
We have specific geographic DMA lists that are used for field marketing and marketing programs to target event invitations. This is **not** tracked with Bizible touchpoints or channels. This campaign type is only used for visibility of our DMA lists - [click to see full list](/handbook/marketing/marketing-operations/marketo#geographic-dma-list) of DMAs available. 


| Member Status | Definition       | Success |
| :------------ | :-----------     | :------ |
| Member        | A record is a member of this DMA list | n/a this is a cohort campaign type not awarding touchpoints | n/a - this campaign type *does not* have a success metric |


#### Inbound Request
Any type of inbound request that requires follow up. This is tracked as an *online* Bizible channel.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Requested Contact               | Filled out Contact, Professional Services, Demo or Pricing Request                    | Yes      |


#### List Build
A static list built for ad hoc requests by the FMM or MPM team. This campaign type **does not** apply any touchpoints and is **not** tracked as a Bizible channel. 

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Nominated               | Any record proactively identified by Sales to be included in the campaign                    |        |
| Marketing List                       | Any record identified by targeting filters applied by Marketing Operations to build the initial list                                             |          |
| Organic Engaged               | Occasionally used when we are wanting to track & include any records engaging with specific marketing web pages                    | Yes      |


#### Owned Event
This is an event that we have created, own registration and arrange speaker/venue (example: Gary Gruver Roadshow). This is tracked as an *online* Bizible channel.


| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Invited                   | Invitation/Information about event sent by Sales/SDR                                  |          |
| Sales Nominated                 | Sales indicated record to receive triggered event email sent by Marketing             |          |
| Marketing Invited               | Marketing geo-targeted email                                                          |          |
| Waitlisted                      | Holding state if registration is full will be moved to `Registered` if space opens    |          |
| Registered                      | Registered for event                                                                  |          |
| No Show                         | Registered but did not attend event                                                   |          |
| Attended                        | Attended event                                                                        | Yes      |
| Follow Up Requested             | Requested additional details about GitLab to be sent post event                       | Yes      |


#### PathFactory Listener
This campaign type is used to track consumption of specific PathFactory assets. This is tracked as an *offline* Bizible Channel and touchpoint. Details related to types of assets being tracked can be found on the [Marketing Operations - PathFactory](/handbook/marketing/marketing-operations/pathfactory/#listening-campaigns) page. 

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Content Consumed                   | Status when the corresponding Marketo listener picks up the contents consumption.                                  | Yes         |



#### Referral Program
This campaign type is used for our third party prospecting vendors or meeting setting services (Like BAO, DoGood). This is tracked as an *offline* Bizible Channel and touchpoints.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Target List               | Identified as persona we want to speak with                    |          |
| Meeting Set               | Vendor has set & confirmed a meeting time                    |          |
| Meeting No Show               | Scheduled meeting was cancelled or not attended                    |          |
| Meeting Attended               | Scheduled meeting at conference was attended                     | Yes      |


#### Speaking Session
This campaign type can be part of a larger Field/Conference/Owned event but we track engagement interactions independently from the larger event to measure impact. It is something we can drive registration. It is for tracking attendance at our speaking engagements. This is tracked as an *offline* Bizible channel.


| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Invited                   | Invitation/Information about event sent by Sales/SDR                                  |          |
| Sales Nominated                 | Sales indicated record to receive triggered event email sent by Marketing             |          |
| Marketing Invited               | Marketing geo-targeted email                                                          |          |
| Registered                      | Registered or indicated attendance at the session                                     |          |
| No Show                         | Registered but did not attend event                                                   |          |
| Attended                        | Attended speaking session event                                                       | Yes      |
| Follow Up Requested             | Had conversation with speaker or requested additional details to be sent post event   | Yes      |


#### Trial
Track cohort of Trials for each product line (Self-hosted or SaaS) to see their influence. In-product trials are tracked as an **offline** Bizible touchpoint. Webform Self-hosted trials are an **online** Bizible touchpoint.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Target List               | LEAD or CONTACT record that has been identified for marketing campaign prospecting                    | Yes      |


#### Virtual Sponsorship
A virtual event that we sponsor and/or participate in that we do not own the registration but will generate a list of attendees, engagement and has on-demand content consumption post-live virtual event. This is tracked as an *offline* Bizible channel.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Invited                   | Invitation/Information about event sent by Sales/SDR                                  |          |
| Sales Nominated                 | Sales indicated record to receive triggered event email sent by Marketing             |          |
| Marketing Invited               | Marketing targeted email                                                              |          |
| Waitlisted                      | Holding state if registration is full will be moved to `Registered` if space opens    |          |
| Registered                      | Registered for event                                                                  |          |
| No Show                         | Registered but did not attend event                                                   |          |
| Attended                        | Attended event                                                                        |          |
| Visited Booth                   | Stopped by booth for any reason                                                       | Yes      |
| Follow Up Requested             | Requested additional details about GitLab to be sent post event                       | Yes      |
| Attended On-demand              | Watched/consumed the presentation materials post-event on-demand                      | Yes      |

#### Webcast
Any webcast that is held by GitLab or a sponsored webcast with a partner. This is tracked as an *online* Bizible channel.

| Member Status                   | Definition                                                                            | Success  |
|:--------------------------------|:--------------------------------------------------------------------------------------|:---------|
| No Action                       | default starting position for all records                                             |          |
| Sales Invited                   | Invitation/Information about event sent by Sales/SDR                                  |          |
| Sales Nominated                 | Sales indicated record to receive triggered event email sent by Marketing             |          |
| Marketing Invited               | Marketing geo-targeted email                                                          |          |
| Registered                      | Registered through online form                                                        |          |
| No Show                         | Registered but did not attend live webcast                                            |          |
| Attended                        | Attended the live webcast                                                             | Yes      |
| Attended On-demand              | Watched the recorded webcast                                                          | Yes      |


## Opportunities

### Criteria for Sales Accepted Opportunity (SAO)

The following criteria are **required** for all SAOs:
An Opportunity is deemed a Sales Accepted Opportunity (SAO) when the Opportunity is moved from Stage `0-Pending Acceptance` to `1-Discovery` by the Strategic Account Leader.

The following criteria is required for an SDR to submit an opportunity to sales:

**Authority**
The prospect being met is directly involved in a project or team related to the potential purchase of GitLab within this buying group, either as an evaluator, decision maker, technical buyer, or *influencer.
*If the “influencer” is not directly involved (i.e. is related to a "decision maker" in another group/division or someone who is not directly tied to the opportunity at hand) the SDR will continue to own the opportunity and will seek to set-up the next meeting with a key contact in the buying group (leaving 0-pending status until date/referral is confirmed), updating the current opportunity with the new directly-involved point of contact in the buying group once it's acquired.

**Initiative**
An initiative the company is working on has been identified and GitLab can potentially help the initiative. Identified by either a business problem (i.e too many tools), strategic direction or modernization interest (impetus to change).

**Fit**
The following fields have been obtained:
* Current DevOps or software development lifecycle tools (from conversation or credible data source)
* Expected entry point use case (e.g. SCM or CI)
* Potential seats of the first opportunity (if this is a new account or buying group)

**Timing**
After the initial qualifying meeting with the account leader/executive, there must be a next step that is set to occur within a *60 day timeframe. (*If next step isn’t within a 60 day timeframe, the opportunity remains in stage 0 and in SDR ownership to nurture until the next step is actualized.)

_**SDR best practice:**_
Ask prospect about their environment, what they develop software for etc. to try build a picture of the company and how we will be able to help them.
Share relevant resources with the point of contact.
Add other potential influencers/buyers from that company into our database and the Outreach cadence in an effort to build more momentum within that organization.

_**Before the IQM with the account leader/executive, the SDR will also aim to gather:**_
* SaaS vs. Self Hosted
* Potential Future Seats in the Buying Group
* Total Seats Available Estimate at the company

_**Post IQM:**_
Opportunities in `1-Discovery` stage are accepted and owned by the account leader/executive. The account leader/executive is responsible for the progression, activities, engaging other resources, and converting this early engagement to a mutual win. The Sales account leader/excutive is responsible for taking the next step within 60 days, or reverting the opportunity back to SDR ownership or disqualifying the SAO if ultimately there is no opportunity. Managers should be able to use the 'NEXT STEP DATE' field to determine if the IQM has taken place but opportunity has not been moved to new stage. Opportunities should be moved to new stage within 48 hours of IQM.


### How to create an Opportunity
An OPPORTUNITY can be created in Salesforce a) when converting a LEAD to CONTACT; b) from a CONTACT. **All opportunities** should be created with a Stage = `00-Pre Opportunity` regardless of how you create the OPPORTUNITY. Once the initial setup is complete, the [OPPORTUNITY Stage](#opportunity-stages) can updated based on the criteria below.

#### Creating a New Business Opportunity from CONTACT record
{:.no_toc}
1. On CONTACT record, click the `New Opportunity` button. Required fields are:
     * Opportunity Name - using [Opportunity Naming Convention](#opportunity-naming-convention)
     * Account Name = This should NOT need to be changed as it pulls from the CONTACT object
     * Type = `New Business`
     * Initial Source = DO NOT CHANGE
     * Close Date = if no time frame defined, **SDR** set close date rolling 9-months
     * Stage = `00-Pre Opportunity` - starting stage for ALL opportunities
     * Add as much detail on the OPPORTUNITY record as you can.
     * Click `SAVE`
2. Scroll down OPPORTUNITY record to the `Contact Roles` section, **click** `New`. CONTACTS associated to the ACCOUNT will be listed (up to 50 records). You must select a CONTACT as **Primary** and define the `Role`.
     * If you do not define a **Primary** CONTACT marketing attribution & activity influence on the OPPORTUNITY will not be accurately captured.
3. Change the OPPORTUNITY Owner to the `Account Owner` (i.e. SAL/AM). Click `Save`.
4. Within the OPPORTUNITY record, click the `Initial Qualifying Meeting` button. Enter the required fields (Start/End dates, Type) and update the description field with any notes the SAL/AM should have and review *before* taking the scheduled meeting.
     * Fill in the `Related to` section for BOTH the CONTACT and the OPPORTUNITY
     * Change the `Assigned to` field to the OPPORTUNITY owner
     * Click `Save`
5. Update the OPPORTUNITY Stage from `00-Pre Opportunity` to the correct stage -> normally `0-Pending Acceptance`.
6. Update the 'NEXT STEP DATE FIELD' with the date of the next action step (most often an IQM).
7. Enter in 'NEXT STEPS' with details that correlate to the NEXT STEP DATE FIELD.

#### Creating a New Business Opportunity from LEAD record
{:.no_toc}
1. On LEAD record, fill out the required qualification questions, add additional notes to the optional sections if gathered AND update to `Lead Status` = `Qualified`. Click **`Save`**.
2. Click the `Convert` button:
     * Change `Record Owner` to the Account Owner (based on [Global Ownership rules](#global-account-ownership))
     * Check the "Send Email to the Owner" box
     * Lookup the correct `Account Name` - if unsure assign OPPORTUNITY to the "Parent" account
     * Opportunity Name - using [Opportunity Naming Convention](#opportunity-naming-convention)
     * Click `CONVERT`
          * If CONTACT record exists, associate converted LEAD to existing CONTACT. *Do not create duplicate if possible*
3. The OPPORTUNITY will need to be updated with the following:
     * Click `Edit`
     * Type = `New Business`
     * Initial Source = DO NOT CHANGE
     * Close Date = if no time frame defined, **SDR** set close date rolling 9-months
     * Add as much detail on the OPPORTUNITY record as you can.
     * Click `SAVE`
4. Scroll down OPPORTUNITY record to the `Contact Roles` section, the converted LEAD will automatically be set as **"Primary"**. Click `Edit` and define the `Role`.
     * Add any additional CONTACTS and define their `Role` that need to be associated with the OPPORTUNITY
     * Opportunities must have a **Primary** CONTACT defined so marketing attribution & activity influence is accurately captured.
Change the OPPORTUNITY Owner to the `Account Owner` (i.e. SAL/AM). Click `Save`.
5. Within the OPPORTUNITY record, click the `Initial Qualifying Meeting` button. Enter the required fields (Start/End dates, Type) and update the description field with any notes the SAL/AM should have and review *before* taking the scheduled meeting.
     * Fill in the `Related to` section for BOTH the CONTACT and the OPPORTUNITY
     * Change the `Assigned to` field to the OPPORTUNITY owner
6. Update the OPPORTUNITY Stage from `00-Pre Opportunity` to the correct stage -> normally `0-Pending Acceptance`.
7. Update the 'NEXT STEP DATE FIELD' with the date of the next action step (most often an IQM).
8. Enter in 'NEXT STEPS' with details that correlate to the NEXT STEP DATE FIELD.

#### Creating an Add-on Opportunity
{:.no_toc}
An `Add-On` OPPORTUNITY will inherit information from the *original* `New Business` OPPORTUNITY. The steps to create an `Add-on` OPPORTUNITY varies slightly from the instructions above because this type of OPPORTUNITY is created from the `New Business` OPPORTUNITY **not** from a converted LEAD or CONTACT.

This creates a parent-child relationship between the *original* `New Business` OPPORTUNITY and the `Add-on` OPPORTUNITY.

1. Navigate to the *original* `New Business` OPPORTUNITY (this will become the "parent" opp).
     * Example: If you are selling additional seats to an existing subscription - you should go to the original `New Business` OPPORTUNITY.
2. Click the `New Add-on Opportunity` button.
3. **UPDATE** the OPPORTUNITY Name - see the [Opportunity Naming Convention] guidelines
4. Define:
     * `Initial Source` = see the [definition table](#initial-source) to choose the most correct source. It is important to be accurate as this does impact reporting and marketing attribution.
     * Close Date = if no timeframe defined input close date on a rolling 9-months.
     * Stage = All opportunities start as `00-Pre-Opportunity`
5. Add any additional details on the OPPORTUNITY record
6. Click `Save`

Within the parent-child OPPORTUNITY hierarchy some information will pass from the parent (`New Business`) to the child (`Add-on`). This information will be used in our reporting and analysis to track add-on business OPPORTUNITIES to their `Initial Source` and contributing team members.

There are additional validation rules that are presently in effect:
- The **Parent** OPPORTUNITY must either be a `New Business` or `Renewal` OPPORTUNITY.
- A **Parent** OPPORTUNITY *cannot* be another `Add-on` OPPORTUNITY
- All sales-assisted non-portal `Add-on` OPPORTUNITIES **must** have a parent opportunity.

#### Creating an Upside IACV Opportunity
{:.no_toc}
An `Upside IACV` OPPORTUNITY will inherit information from the *original* OPPORTUNITY. The steps to create an `Upside IACV` OPPORTUNITY varies slightly from the instructions above because this type of OPPORTUNITY is created from the OPPORTUNITY **not** from a converted LEAD or CONTACT. An `Upside IACV` OPPORTUNITY has a minimal amount of fields as it's only for tracking the potential upside amount.

This creates a parent-child relationship between the *original* OPPORTUNITY and the `Upside IACV` OPPORTUNITY.

1. Navigate to the *original* OPPORTUNITY (this will become the "parent" opp).
2. Click the `Upside IACV` button.
3. **UPDATE** the OPPORTUNITY Name - see the [Opportunity Naming Convention] guidelines
4. Define:
     * Close Date = if no timeframe defined input close date on a rolling 9-months.
     * Amount = the upside value in addition to the Parent OPPORTUNITY value. If Parent OPPORTUNITY amount is $100,000 and total OPPORTUNITY amount potential is $150,000, then the Upside IACV amount is $50,000
6. Click `Save`

When the PARENT OPPORTUNITY is changed to "Closed Won" or "Closed Lost," please update the stage of the UPSIDE IACV OPPORTUNITY to "Duplicate." In order to save this change, you must also enter the PARENT OPPORTUNITY name in the "Duplicate Opportunity" field on the UPSIDE IACV OPPORTUNITY. 

Note: Upside IACV opportunities exist for tracking purposes only. All final IACV (including any won upside IACV) will be attributed to the PARENT OPPORTUNITY. 

#### Creating a Professional Services Opportunity
{:.no_toc}
A `Professional Services` OPPORTUNITY will be used to cover any integration, consulting, training or other service that a Sales rep will sell to a prospect/client and needs or wants to be invoiced separately. To invoice separately a new quote and opportunity must be created.
A full list of professional services can be found [here](/handbook/customer-success/professional-services-engineering/offerings/).

1. Navigate to the *original* OPPORTUNITY (this will become the "parent" opp).
2. Click the "New PS Opportunity" button and fill out the following:
     * OPPORTUNITY Name = will already be set correctly; do not change
     * Type = do not change it will populate from parent OPPORTUNITY
     * Initial Source = do not change it will populate from parent OPPORTUNITY
     * Close Date = if no timeframe defined input close date on a rolling 9-months.
     * Stage = All opportunities start as `00-Pre-Opportunity`
     * Professional Services Value (ProServe Value) = enter dollar value, which is defined as the total value of all consulting, training, integration, or other professional services as outlined in the Statement of Work.
     * ACV = **do not populate** an automated workflow will fill this information
     * Amount = **do not populate** an automated workflow will fill this information
     * Professional Services Description, Project Scope, Task Schedule and Key Assumption fields = these will push to the Statement of Work when a PDF is generated from Zuora.
     * Verify the `Professional Services` OPPORTUNITY has the *original* OPPORTUNITY in the `Parent Opportunity` field. If this is not a validation rule error will occur while attempting to save the OPPORTUNITY.
3. Click `Save`
4. To create a quote, see the ['Creating Accounts, Contacts, Opportunities and Quotes'](/handbook/sales/#creating-accounts-contacts-opportunities-and-quotes-in-salesforce) and begin with Step 4. Here is a [video](https://drive.google.com/file/d/142csIZyrzIfSJOSJkIAK6d9c1JwTO_Rq/view?usp=sharing) that hightlights the process.

### Tracking Sales Qualified Source in the Opportunity

Sales Qualified Source is dimension used when analyzing pipeline creation, lead conversion, sales cycles, and conversion rates. Sales Qualified Source may be different from the Lead Source of an Opportunity, which captures the original source (event, campaign, etc). For example, if a prospect originates from a trial (lead source), that prospect can be qualified by a SDR, Account Executive, Channel Partner, or the Web (sales qualified source).

The logic for the Sales Qualified Source is as follows:

2. If the Sales Development Representative field (Opportunity) is populated, regardless of opportunity owner, the Sales Qualified Source is "SDR Generated"
3. If the Sales Development Representative fields are NULL and the opportunity owner is:
   * a Regional Director, Account Executive, or Account Manager, the Sales Qualified Source is "AE Generated"
   * a GitLab team-member that is not a Regional Director, Account Executive, or Account Manager, the Sales Qualified Source is "Other"
   * an authorized reseller, the Sales Qualified Source is "Channel Generated"
   * the Sales Admin, the Sales Qualified Source is "Web Direct Generated"

### Reseller Opportunities

Opportunities utilizing a reseller require slightly different data:

* Lead/Contact:
The partner record should be converted to their company channel type account. The end user record should be converted to the end user standard account type.

* Opportunity Name:
If the partner is an authorized reseller, rename the opportunity with the partner’s nick-name in front, then a dash.  For instance; if it is a Perforce deal, the opportunity name should start with P4 - (whatever your opportunity name is)  This is important for the workflow that solicits updates from the reseller.

* Account Name:
It is important that opportunities using a reseller are created on the END CUSTOMER’s account, and not the reseller’s account.  The account name on an opportunity is never a reseller.  Resellers do not buy licenses; they purchase them on the behalf of an end customer.  For instance, the account name field on an opportunity should never be SHI.

* Opportunity Owner:
The AE/SAL/Channel Manager who is working the deal with the reseller

* Deal Registrant:
The reseller who registered the deal.

* Associating Contact Roles:
After creating the opportunity, click “New” in the contact section to associate contacts with the opportunity.
 - The primary contact should always be a contact at the end user’s account and not a contact at the reseller.  This is important as resellers come and go, and if we do not capture the contact at the end user account, we will not be able to sell to this account if the reseller ends their relationship with us or with the end account.
 - A reseller contact (say, the sales rep at ReleaseTEAM) can, and should be added to the opportunity with the role of Influencer.  NOTE: A contact that works for a reseller should never be added to an end user account.  For instance an employee of SoftwareOne should be a contact of the SoftwareOne account only, and not the Boeing account.

* Associating Partners to an Opportunity:
After creating the opportunity, click “New” in the Partners section to associate the reseller with the opportunity.
 - You can associate multiple partners with an opportunity if there is more than one reseller involved in the opportunity. This is not uncommon for government opportunities, or opportunities where the customer is asking multiple fulfillment houses (like SHI and SoftwareOne) to fulfill the order.
 - Unofficial resellers should never be marked primary
 - If there are any authorised resellers associated, at least 1 must be marked as primary
    - In order of precedence this would be:
        - The deal registrant (`Deal Registrar` field in SFDC, This should be confirmed with the appropriate channel manager)
        - The deal fulfiller (i.e.: The one issuing the PO)
        - The distributor

* Opportunity Team List:
Add the reseller user to the Opportunity team list with the role of “Reseller” or else they cannot see the opportunity.

### Opportunity Naming Convention

Opportunities for subscriptions will use the following guidelines:

- **New Business**: [Quantity]
   - [Name of Company]- [Quantity] [Edition]
   - Example: Acme, Inc- 50 Starter

- **Add-On Business (seats only)**:
   - [Name of Company]- Add [Quantity] [Product]
   - Example: Acme, Inc- Add 25 Starter

- **Add-On Business (Upgrade from Starter to Premium)**:
   - [Name of Company]- Upgrade to Ultimate
   - Example: Acme, Inc- Upgrade to Ultimate

- **Renewal Business (no changes)**:
   - [Name of Company]- [Quantity] [Product] Renewal [MM/YY]
   - Example: Acme, Inc- 50 Premium Renewal 01/17

- **Renewal Business + Add On Business (seats)**:
   - [Name of Company]- [Quantity] [Product] Renewal [MM/YY]+ Add [Quantity]
   - Example: Acme, Inc- 50 Premium Renewal 01/17 + Add 25

- **Renewal Business + Upgrade**:
   - [Name of Company]- [Quantity] Upgrade to Premium + Renewal [MM/YY]
   - Example: Acme, Inc- 50 Upgrade to Premium + Renewal 01/17

- **Professional Services**:
   - [Name of Company]- Professional Services [MM/YY]
   - Example: Acme, Inc- Professional Services 06/18

- **Refunds**:
   - [Original Opportunity Name] - REFUND
   - Example: Acme, Inc- 50 Upgrade to Premium + Renewal 01/17 - REFUND

## Opportunity Types

There are three things that can be new or existing:

- Account (organization)
- Subscription (linked to a GitLab instance)
- Amount (dollars paid for the subscription)

That gives 4 types of opportunities:

1. New account (new account, new subscription, new amount) This type should be used for any new subscription who signs up either through the sales team or via the web portal. Paid training also falls under this type if the organization does not have an enterprise license.  This should be marked as New Business.
1. New subscription (existing account, new subscription, new amount) If an existing account is purchasing a new license for another GitLab instance, this will be New Business.
1. Add On Business (existing account, existing subscription, new amount) This type should be used for any incremental/upsell business sold into an existing subscription division mid-term, meaning not at renewal. This may be additional seats for their subscription or an upgrade to their plan. If an existing account is adding a new subscription, this would be new business, not an add-on.
1. Renewal (existing subscription, existing subscription, existing amount) This type should be used for an existing account renewing their license with GitLab. Renewals can have their value increased, decreased, or stay the same.  We capture incremental annual contract value growth/loss as a field in Salesforce.com. Renewal business can be a negative amount if renewed at less than the previous dollars paid for the subscription (renewal rate). Only the part that is more or less than the old amount is IACV, the rest is part of the renewal opportunity.
 * In the event that the customer wants to reset their contract, this would be considered a renewal.  For example, a customer starts January 1st for 12 months, but wants to reset starting April 1st for another 12 month term.

**New business** is the combination of new account and new subscription


### Opportunity Stages

To help move sales through the sales process, [here](https://docs.google.com/document/d/1ag7YY9aJ93j0CRZb-DrbfgH3vmHprTEdjG7l3O57xEk/edit) is a list of questions to ask at each stage

**00-Pre Opportunity**- This stage should be used when an opportunity does not meet our opportunity criteria. However, there is a potential for business, and it should be tracked for possible business.
* What to Complete in This Stage:
  * Schedule discovery call with prospect to determine if there is an opportunity to pursue; or
  * If there is no opportunity then the stage would be updated to 0-Unqualified.
* Creating an Opportunity in this stage from Contacts
  * If you are qualifying a contact for a new business opportunity open an opportunity in this stage and use the qualifications questions in the qualification section on the opportunity while qualifying the contacts.
  * "Convert" Opportunities from this stage to **0-Pending Acceptance** when the opportunity meets [our criteria for an opportunity](#criteria-for-sales-accepted-opportunity-sao)
  * Follow [our process](#how-to-create-an-opportunity) on creating opportunities from a contact record.

**0-Pending Acceptance**: This is the initial stage once an opportunity is created.
* What to Complete in This Stage:
  * For SDR sourced opportunities, the opportunity meets [Sales Accepted Opportunity criteria](#criteria-for-sales-accepted-opportunity-sao).
  * The SDR has scheduled a call via Google Calendar, sent invites, created an event on the account object, named the event: GitLab Introductory Meeting - {{Account Name}}
  * Once it is confirmed that the opportunity meets our Sales Accepted Opportunity criteria, the SAL or AE should move the opportunity to the next stage. The date the opportunity moves from this to the next stage in the sales cycle will populate the `Sales Accepted Date` field on the opportunity record.
  * If the details on the opportunity do not meet our Sales Accepted Opportunity criteria, the SAL or AE should move the opportunity to an `8-Unqualified` stage (this is the only time an opportunity can move into `8-Unqualified` stage).
  * All Opps that are sales assisted must first enter this stage before they can be moved further in the pipeline. If they do not enter this stage at some point you will encounter a validation rule error.

**1-Discovery**: Uncover as much intelligence about the project as you can, which will be confirmed at later stages throughout the sales cycle.
* What to Complete in This Stage:
  * Begin filling out [MEDDPICC](/handbook/sales/#capturing-meddpic-questions-for-deeper-qualification)
  * Send Plan Letter/Recap Email to Attendees- [Example](https://docs.google.com/document/d/16Gurj_MVREmKoqXTdB1F0OQ3eyq1gzbTNU8LNHHuoEM/edit)
  * Scheduled Scoping Call
  * Provide an estimate for the `Expected Number of Users`  and the `Expected Product` for the Opportunity. This information is used to help the customer success team to predict their future workload as well as to help them with their hiring plans.
  * Should the opportunity progress from `1-Discovery` to the next stage (not 7-Closed Lost or 9-Duplicate), it will be considered a `Sales Qualified Opportunity`. The following values are entered once the opportunity progresses from this stage:
     * `Sales Qualified` is True.
     * `Sales Qualified Date` is the date the opportunity moves from this stage to the next open or won stage.
     * `Initial IACV` captures the value in the `Incremental ACV` field. `Initial IACV` is a snapshot field that will not change, even when the `Incremental ACV` field is updated and will be used for `Deal Size` analysis.

**2-Scoping**: Uncover business challenges/objectives, the competitive landscape, realizing fit.
* What to Complete in This Stage:
  * Complete a Demo (Optional)
  * Schedule a Technical Evaluation Call
  * Confirm and collect new [MEDDPICC](/handbook/sales/#capturing-meddpic-questions-for-deeper-qualification) information.

**3-Technical Evaluation**: Confirming technical requirements. A proof-of-concept (POC) might occur at this stage. This is also the stage to confirm information before a proposal is delivered.
* What to Complete in This Stage:
  *  Enter POC Notes and POC Success Criteria (if applicable) and enter into the POC Notes and POC Success Criteria fields related to the opportunity.
  *  Confirm *Technical Requirements, POC Scope*
  *  Confirm *Technical Win/POC Success*
  *  Confirm and collect new [MEDDPICC](/handbook/sales/#capturing-meddpic-questions-for-deeper-qualification) information.

**4-Proposal**: Business and technical challenges and been uncovered and resolved. A proposal is drafted and delivered to the prospect.
* What to Complete in This Stage:
  * Confirm Bill to Information (who will receive the invoices), Sold to Information (who will receive the license key). You should also confirm whether or not the customer will issue a PO, and whether there is a vendor registration form required by the customer.
  * Deliver formal contract to the prospect with complete bill to and sold to information. Remember that quotes with incomplete or incorrect information will be rejected by Deal Desk.
  * An MSA may be delivered separately
  * Clear understanding of purchase/contract review process and a close plan (actions to be taken, named of people to complete actions and dates for each action) documented in the Purchasing Plan field.

**5-Negotiating**: The prospect or customer has received the proposal and is in contract negotiations.
* What to Complete in This Stage:
  * Agreement on business terms
  * All proposals should include the standard GitLab [Terms](/terms/)
  * Determine if customer will be referenceable when the opportunity closes. If the answer is:
       * "Yes" update the `Referenceable Customer` section on the Account object with appropriate reference information
       * "No" the discussion of being a reference can be revisited at a later date
  * Modifications will not be accepted to the standard terms for any opportunity that is less than $25k, or for Starter edition.
  * If the above threshold is met, requests for modifications to the standard terms should be sent to Legal through SalesForce, using Chatter at the Parent Account level, following the process found [here](/handbook/business-ops/order-processing/#process-for-agreement-terms-negotiations-when-applicable).
  * If the Account is seeking to use their own paper, requests will only be entertained if the opportunity is greater than $100k, and the request should be sent through SalesForce, at the Parent Account level, following the process found [here](/handbook/business-ops/order-processing/#CustomerFormAgreements).

**6-Awaiting Signature**: The prospect or customer has verbally agreed to the terms and conditions outlined in the proposal and has submitted for signature.
* What to Complete in This Stage:
  * Received signed order form, which signals agreement of all pricing and legal terms.
  * Obtain a purchase order, if applicable.
  * Work with GitLab AR to deliver any tax and/or complete any vendor registration processes.
  * Ensure all relevant documents, MSA, PO, and other forms uploaded to SFDC in the Notes and Attachments section of the opportunity record.
  * EULA (End User Licence Agreement) has been accepted by end-user organization (if applicable).
  * If this is a large/strategic account, or if IACV is +$12,000, enter `Closed Won Details` summarizing why we won the opportunity.
  * Subscription created in Zuora.
  * Opportunity has been submitted for Finance approval.

**7-Closed Won**: Congratulations!! The terms have been agreed to by both parties and the quote has been approved by Finance.
* What to Complete in This Stage:
  * Introduce Customer Success/Account Management (if applicable)
  * Set a calendar reminder for 30 day follow up
  * If applicable, initiate Customer Onboarding or Premium Support onboarding

**8-Closed Lost**: An opportunity was lost and the prospect/customer has decided not to pursue the purchase of GitLab.
* What to Complete in This Stage:
  * Select all applicable Closed Lost Reasons
     * If the loss is due to Competitive Loss, you are required to select the competitor(s) from the opportunity's `Competitor` field
     * If the loss is due to Product Maturity, you are required to select the product stage(s) from the opportunity's `Product Maturity: Product Line` field.
  * In the `Closed Lost Detail`, enter as much detail as you can as to why we lost the deal. For example:
     * If they selected a competitor, why? Was it due to features or pricing?
     * If decided not to move forward with a project, what were the reasons? Did they not understand the value? Was there not a compelling event or reason?
     * Again, please be as thorough as you can as this information will prove valuable as we learn from these experiences.
  * Please note that for new business deals where the opportunity is with a Large/Strategic account OR the Incremental Annual Contract Value (IACV) is equal or greater than USD 12,000, then a notification will be sent to the [#lost-deals](https://gitlab.slack.com/messages/C8RP2BBA7) Slack channel.
  * Uncover a time for follow up (incumbent solution contract expiration date)
  * Note that if an opportunity is dead/stalled, mark the Stage as 8-Closed Lost. Should the prospect/customer re-engage before 30 days, you can reopen this opportunity. However, if they re-engage beyond 30 days, you will need to create a new opportunity.
  * If the `Closed Lost Reason` is "Merged into another opportunity" please link this closed opportunity to the opportunity you are merging it into by using the `Merged Opportunity` lookup field. Otherwise, you will encounter a validation rule error.

**9-Unqualified**: An opportunity was never qualified.
* What to Complete in This Stage:
  * Update Reason for Closed Lost and add any pertinent notes as to why the opportunity was not qualified.
  * A notification will be sent to SDR Team Lead and a feedback session should be scheduled between AE and Team Lead.

**10-Duplicate**: A duplicate opportunity exists in the system. This usually happens when a web direct opportunity is won when an existing opportunity already exists in Salesforce. Another reason could be multiple renewals created for the same opportunity. This stage **should not** be used when disqualifying an opportunity or if it is discovered at some point after acceptance that the opportunity is really part of a larger initiative. If the opportunity was accepted, it cannot be marked as a duplicate. Instead, you must mark the opportunity as `8-Closed Lost` and select the appropriate reason. Possible selections could include "Consolidating order - part of another subscription" or "Merged into another opportunity" as reasons why a duplicate opportunity may have been created.
*  What to Complete in this stage:
  *  Move the Opportunity into this stage
  *  Fill out the lookup field `Duplicate Opportunity` with the opportunity that this opportunity is a duplicate of. If this field is not populated you will encounter a validation rule error.

#### Opportunity Stage Movement Considerations
Note that once you qualify an opportunity via our standard qualification process, you cannot revert an opportunity back to the following stages: `00-Pre Opportunity`, `0-Pending Acceptance`, or `9-Unqualified`. If you need to revert an opportunity you've previously qualified to one of these stages, please contact Sales Operations and we can determine why the opportunity (once qualified) is no longer qualified.

#### Reverting an Opportunity to a Previous Stage
If a previously met criteria has become unmet, you are required to revert back to the latest stage where all activities were completed. For example, if a prospect had previously signed off on GitLab from a technical standpoint, requested a quote and has begun contract negotiations, you would set the opportunity to `5-Negotiating`. However, if at any point during the negotiations, additional technical questions or requirements arise that result in a re-evaluation of GitLab's technical capabilities, you would revert the opportunity back to `3-Technical Evaluation`. After the opportunity has once again met the stage completion criteria, you are able to move the opportunity to either `4-Proposal` if a new order form was created as a result of the additional technical requirements, or back to `5-Negotiating` if no changes were made to the original order form.

### Locking Opportunities as a result of their "At Risk" potential
In order to be in compliance with US Regulations there is a need to screen opportunities against known individuals and organizations with whom we are not allowed to do business. In order to comply with these regulations, opportunities are screened when they are created through a third party application, Visual Compliance. Visual Compliance is a dynamic screening tool that constantly compares our account information with those sanctioned parties listed on various Denied Party Lists.  Visual Compliance will screen new information and will monitor existing information to ensure the integrity and legality of the parties with whom we do business. The more **accurate** information in the Account--the better! Partial information may trigger a false ‘hit’ and cause delays.  Please provide the full company name, company address, country and contact name(s).

If you receive an error referencing export when attempting to update an Account:
(i) Check if the Visual Compliance Section of the Account says “Pending”-- Wait 15-30 minutes for the system to run its initial check and update.
(ii) If the Visual Compliance Section of the Account says  “Yellow” or“Red”-- The legal team is manually reviewing the Account to ensure compliance. Manual reviews of hits are conducted three (3) times a day.  Changes by Legal will automatically update the Account, although updates may take 15-30 minutes to sync.
 - If the status has been updated to “Clear”, the order will process and account functionality will resume.
 - If the status is updated to “Escalate”, there is a concern with either the company itself or there is an attempt to sell in an embargoed country.  Escalated orders will not process.
(iii) If the Account requires immediate attention (i.e., to close a deal), open a Chatter message in the Account and message “@legal”.  Upon receipt of a request, the Legal team can review and update in Visual Compliance.  Please understand that if Legal finds a problem, the flag and the account will remain locked down.

### Executive Account Sponsorship Program
This program adds a member of e-group to be a dedicated part of the sales Account Team on a specific account.  The exec will maintain direct relationships with people at the account and participate in both remote and in-person meetings as appropriate. 

Goal: Leverage our executive team to ensure great customer experience and direct two-way connection with GitLab and executive visibility into a small number of high-value customers.  This is intended to both support the customers to be successful and to provide insights to ensure GitLab is sucessful.  Examples of executive sponsor responsibilities may include (and not limited to) participation in quarterly account planning meetings, communications with the customer as well as helping to facilitate internal conversations & resources where necessary.  

Very few accounts will have named sponsors; execs are still available as needed:
1. Only a small number of accounts can have exec sponsorship, so there is no guarantee for any account to necessarily have an assigned exec sponsor
2. Even though most accounts will not have an assigned exec sponsor, the exec team is available to support an engage all customers as needed.

Accounts are selected for and matched to an executive sponsor:
1. Total accounts with named sponsors: 10
2. Accounts may be nominated by Sales VPs and Confirmed by CRO after agreement with the named sponsor.
3. Sponsored accounts typically represent deep product utilization, large opportunity, and/or a broad vision for success and engagement with GitLab.

Example activities for sponsors:
1. SAL Exec briefing & initial Zoom w/customer exec champion
2. Quarterly Account Review Meetings
3. Two in-person meetings with account / yr
4. 1 year on the account

Process: 
1. Executive sponsors are to be involved in accounts *with and without* active opportunities. 
1. Once approved, Sales Operations will update the "Executive Sponsor" field.
1. Executive Sponsored Accounts can be referenced here: https://gitlab.my.salesforce.com/00O4M000004e2Ma 

## Types of Accounts

### Accounts Created in Salesforce utilizing CE Usage Ping Data
The [CE Usage ping](https://docs.gitlab.com/ee/user/admin_area/settings/usage_statistics.html) provides GitLab with some limited insight into how end users are utilizing the platform. The raw information is cleaned, enriched and then pushed to SFDC as an Account by the Data Team.

If there is not an existing account match in Salesforce, a new account record will be created with the following information populated:

| SFDC Field | Default Value |
|---|---|
| Account Name |  |
| Account Source | `CE Download` |
| Number of Employees |  |
| Billing Street |  |
| Billing City |  |
| Billing Zip |  |
| Billing Country |  |
| Account Type | `Prospect - CE User` |
| Account Website |  |
| Industry | Populated by Clearbit (since been deprecated) |
| Active CE Users | Populated by Usage Ping |
| CE Instances | Populated by Usage Ping |
| Account Owner | Sales Admin by Default |
| Using CE | Checked True |

**Process**
1. Sales Team members can use this data to proactively identify `Prospect - CE User` accounts that fit their target segment(s). Accounts owned by `Sales Admin` can be adopted by a Sales Team member changing ownership in Salesforce. The adoption of any `Sales Admin` owned records will trigger an email alert that is sent to the Account Research Specialist for transparency and awareness of what account records have been claimed.
2. The Account Research Specialist will be responsible for reviewing the `Prospect - CE User` accounts on a regular basis to determine additional account records that should be worked either by a Sales Team member or Outbound SDR.
3. When an account record has been identified for follow up, the Account Research Specialist will work with the appropriate Regional Director (RD) to determine Outbound SDR assignment based on work load and available capacity.
4. The assigned Outbound SDR will work the `Prospect - CE User` account the same as any other known `CE User` account leveraging the tools at their disposal (DiscoverOrg, LinkedIn Sales Navigator, etc) to add contacts to the account record and populate the firmographic profile of the account.

## Reporting

### Marketing Reports

The Online Growth team is in charge of updating reports and dashboards for marketing meetings. Our key metric is pipe-to-spend.  Pipe compared to marketing spend shows how effective our marketing is in filling the pipeline. This report will include all pipe, not just large and up, and is better than cost per lead as it will account for each type of lead in our hybrid sales model and show the value of leads in larger organizations as they generate more pipe. More information on pipe-to-spend as a marketing metric can be found in [Salesforce](https://success.salesforce.com/ideaView?id=087300000006thQ) and [Marketo](https://blog.marketo.com/2012/08/my-favourite-marketing-metric.html). Currently we are using the Full Path revenue model to show all Touchpoints in a path.

Marketing metrics sources are here:
- [Pipe](https://gitlab.my.salesforce.com/00O61000004IgAu) used to account for pipeline using Full Path model. This will be divided by spend. The SST for pipe-to-spend will be in Looker.
- Sales Pipeline dashboard - will add once new data visual tool onboarded
- [Web Traffic by source](https://analytics.google.com/analytics/web/#report/acquisition-channels/a37019925w65271535p67064032/)
- [Online Growth Web Metrics Dashboard](https://datastudio.google.com/open/1lSOfaMEBPVpFtLCpFuzvV3I_DfRdtngB)
- [SCLAU Dashboard](https://gitlab.my.salesforce.com/01Z61000000Qbm2)

### Report on SCLAU Opportunity Creation

An area of focus is to create Sales Accepted Opportunities ([SAO]) in the [large and up sales segment](#segmentation) - we call this type of opportunity a [SCLAU]. For visibility into performance in these market segments we use a [Large and Up Opportunity Performance dashboard](https://gitlab.my.salesforce.com/01Z61000000J0h1) in salesforce.com. The dashboard tracks the [pending acceptance](#customer-lifecycle/) opportunities, [SAO](#customer-lifecycle/), and [SQO](#customer-lifecycle/).

The dashboard analyzes opportunity measures by the dimensions `initial source type`, [sales segmentation](#segmentation) and [sales qualification source](/handbook/sales/#tracking-sales-qualified-source-in-the-opportunity). We set our demand generation targets based on SAO count in large and up segments ([SCLAU]) by `initial source type` and `sales qualification source` as follows:

- SDR Generated - opportunity is created by SDR prospecting. Sales qualification source is `SDR Generated`.
- AE Generated, Marketing assisted - opportunity is created by an AE or SAL and is associated with a contact that has responded to one or more marketing programs. Sales qualification source is `AE generated` and `Initial source` is not `AE Generated`.
- AE Generated, Cold calling - opportunity is created by an AE or SAL but is not associated with any contacts that have responded to marketing programs. Sales qualification source is `AE generated` and `Initial source` is `AE Generated`.


#### Using Bizible Fields in Salesforce to Report Attribution
 In 4Q18, we are making updates to the Bizible Channel rules, but currently, these channels and subchannels are pulled into Salesforce and can be further filtered by using `medium` for those channels with overlap or with `Ad Campaign name` to search for specific UTMs or campaigns:

| Bizible Online Channel or subchannel | Type of marketing |SFDC Marketing Channel-path |
|---|---|---|
|`CPC`|Google Adwords or other Paid Search|CPC.Adwords|
|`Display`|Display ads in Doubleclick, Terminus, etc|Display|
|`Paid Social`|Ads in Facebook or LinkedIn |Paid Social.[Name of site]|
|`Organic`|Organic search|Marketing Site.Organic|
|`Other`|Not specifically defined |[Name of channel].Other|
|`Partners`|Google or events|	Marketing Site.Web Direct|
|`Email`|Nurture, Newsletter, Outreach emails|Email.[Name of email type]|
|`Field Event`|From Field event, will show Salesforce campaign as touchpoint source|Email.[Field Event]|
|`Conference`|From conference, will show Salesforce campaign as touchpoint source|Conference|
|`Social`|Any referral from any defined social media site| Social.[Name of site]|
|`Sponsorship`|Paid sponsorships, Display, and Demand gen as well as Terminus|Sponsorship|
|`Web Direct`|Unknown or direct (NOTE: this is not the same as Web direct/self-serve in SFDC, this is a Web referral where the original source was not captured)|Marketing Site.Web Direct|
|`Web Referral`|Referral from any site not otherwise defined|Marketing Site.Web Referral|
