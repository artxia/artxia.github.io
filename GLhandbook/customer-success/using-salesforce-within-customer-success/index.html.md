---
layout: handbook-page-toc
title: "Using Salesforce within Customer Success"
---

# Using Salesforce within Customer Success
{:.no_toc}

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

- Using Salesforce within Customer Success *(Current)*
- [Account Onboarding](/handbook/customer-success/tam/onboarding/)
- [Technical Account Manager Summary](/handbook/customer-success/tam/)
- [Account Triage](/handbook/customer-success/tam/triage/)
- [Account Engagement](/handbook/customer-success/tam/engagement/)
- [Gemstones](/handbook/customer-success/tam/gemstones/)

On an account view in Salesforce, there is a Customer Success section, with the following fields:

* Health Score - A field to record the overall [customer health](/tam/health-scores)
* GitLab Customer Success Project - Where you enter the URL of the project created using the template described above
* Customer Slack Channel - A field to record Slack channel(s) used for internal and external customer collaboration. If a channel is internal, make sure it follows the naming convention `#a_<customer-name>-internal` per [Communication Chat](/handbook/communication/chat/#account-channels-a_)
* Solutions Architect - The Solutions Architect aligned with the account
* Technical Account Manager	- The Technical Account Manager aligned with the account

## Salesforce Objects

Salesforce operates using a series of objects. Standard objects are objects that are included with Salesforce. Common business objects like Account, Contact, Lead, and Opportunity are all standard objects.

Custom objects are objects that you create to store information that’s specific to your company or industry. For GitLab, we have created four custom objects that are specific to Customer Success. These are POV's, PS EngagementS (PSE's), EBR's, and Onboarding objects. We can link these custom objects to accounts and opportunities, and create automations such as allowing us to auto-populate specific fields and notify users when a task needs to be completed.

### Onboarding objects

The Onboarding object is the way for the Customer Success team to track and manage the customer onboarding experience. If and when an Onboarding object was not automatically created (and should have been), use the [instructions below](#creating-a-new-customer-onboarding-object-manually) to manually create one.

* When an account moved from Gemstone 5 or 6 to Gemstone 1-4 a new onboarding object is created.
* The purchase date field is auto-populated with the close date from the opportunity.
* The object and account will be automatically associated with one another.

A key purpose is measuring the three Time to Value metrics (definitions are covered under Fields). These will be used as a primary gauge for assessing the quality of customer onboarding.

1. [Time to Engage](#fields)
1. [Time to First Value](#fields)
1. [Time to Onboard (Days of Onboarding)](#fields)

##### Fields

* Customer Onboarding Name
* Opportunity (manually populated)
* Purchase date (date field, automatically populated, editable)
* First Reach-out (date field, manually populated, editable)
* Infrastructure Ready (date field, manually populated, editable)
* Onboarding Start Date (date field, manually populated, editable)
* Onboarding Finish Date (date field, manually populated, editable)
* First Value Date (date field, manually populated, editable) - date when a minimum of 20 users are active on Production Environment
* Onboarding Status (picklist) - Not started (default), Scheduled, In Progress, On Hold, Completed
* Time to Engage (calculation: Purchase Date - First Reach-out)
* Days of Onboarding (calculation: Onboarding Start Date - Onboarding Finish Date)
* Time to First Value (calculation: Purchase Date - First Value Date)
* Onboarding Notes (text field)
* Onboarding Challenges / Highlights (text field)
* Success Plan (manually populated link to GitLab Onboarding issue)

#### Compulsory fields after status is set to Completed

* Onboarding experience survey sent? y/N checkbox
* Onboarding experience survey results received? y/N checkbox
* Onboarding experience score (picklist of 1-5) (decided by TAM if no survey results received)

#### GitLab Team Fields

These are important to fill out so we can historically track who assisted with onboarding the customer. This is not pulled from the account metadata as the account metadata may change but these people should always be historically recorded.

### Creating a new Customer Onboarding object manually

1. In Salesforce, click the Customer Onboarding tab (click the ‘+’ to view all tabs if not visible on the top-right)
2. Click the New button to create a New Customer Onboarding record
3. Enter in the following information and click Save once completed:
    * Customer Onboarding Name
    * Account
    * Owner (Technical Account Manager)
    * Purchase Date
    * Onboarding Start Date
    * Greenfield?

### Updating Object During Onboarding

The Customer Onboarding object shouldn't be updated _only_ at the start and completion; update it at each milestone to measure Results, Iterate for short feedback loops, and Collaborate. Small changes are easier than attempting to remember all the details at completion. It also enables reporting on early metrics without waiting for the entire Onboarding process to be finalized.

### Completing the Customer Onboarding object

The TAM owner will be expected to finalize this Onboarding record through completion with the customer; this will result in a few additional values that must be populated:

* Ensure all date fields are accurately filled
* Complete any Onboarding Notes and Onboarding Challenges/Highlights
* Onboarding Finish Date
* Onboarding Status: mark `Completed`

#### Gemstone Automations

##### This is how the Gemstone for an account is calculated:

```
if >5000 users   
OR Ultimate AND >2000 users
OR >500k iACV
= diamond

else if >2500 users
OR Ultimate AND >1000 users
OR >250k iACV
= pearl

else if >1000 users
OR >100k in iACV
= sapphire

else if >500 users
OR >50k in iACV
= ruby

else
= quartz
```

Please visit [this page](/handbook/customer-success/tam/gemstones/) for more information on Gemstones.

### Executive Business Review (EBR) objects

[EBR](/handbook/customer-success/tam/ebr) objects allow the Technical Account Managers to track and measure the success of Executive Business Reviews held (or not held) with customers each year.

In order to appropriately track and create Executive Business Review Objects please follow the instructions below:

#### Creating the first EBR for an account

* If it is the first EBR for an account you can navigate to the EBR Tab. This can be located on the either the 'Sales' or the 'Service' App within Salesforce
* If you would like to schedule an EBR with a GitLab E-Group member, please review and follow the [Meeting request requirements](/handbook/eba/#meeting-request-requirements) page
* On the top of the list shown, you click on the 'New' button. This will enable you to create the new EBR object where you can provide the following. `Executive Business Review Name` is the name that you give this EBR. Select the `EBR Date` that the EBR is scheduled to occur on.

Note: If the EBR Date changes, please see below for handling this situation in order relate the EBR to the appropriate account. This is done using the search functionality provided by the `Account` field. `EBR Status` should be set to either 'Not Started' or 'Scheduled' depending on the current state of the EBR. All other fields should be left alone. Please refer to the section below on if you should link the EBR to any Opportunities.

#### Creating successive EBR's

In order to create any successive EBR's (anything besides the first EBR), use the 'New' button. Each customer has different needs and timing, so one customer may want a quarterly cadence while another wants semi-annually.

<!--* In order to create any successive EBR's (anything besides the first EBR), DO NOT us the 'New' button as this will cause errors with tracking. Instead, after the completion, cancellation or declined invite of an EBR, update the `EBR Outcome` to the appropriate value. This will automatically create the next EBR for the account 90 days after the `EBR Date` for the current EBR (ensuring that there is one EBR per quarter).

A number of fields will also auto populate making the creation process of new EBR's much more efficient. -->

#### Tracking the performance of EBR's

* There are currently two picklist fields in order to provide tracking for EBR's:
    * `EBR Status` - This field shows the scheduling status of the EBR. This should be used to help monitor workflow (Scheduled vs Not Started) and also to track cancellations and declined EBR's as well as completed EBR's that were actually held.
    * `EBR Outcome` - This field tracks the overall success of the EBR with the default set to `Incomplete`. This field should only be updated once the EBR is held OR after a cancellation or declined EBR. This tracks what the  Technical Account Manager believes was the outcome of the EBR (or if it was declined or Cancelled).
* `Declined` vs `Cancelled` - The main difference between a Declined EBR and a Cancelled EBR is dependent on how it is handled.

For example, if a customer pushes to only have two EBR's a year, then two of the EBR's each year should be labeled as Declined. If an EBR is successfully scheduled but then for whatever reason the customer or GitLab has to cancel the EBR, then this value should be chosen.

Handling EBR Date Changes:
* If the `EBR Date` is changed and is still planned to occur within the same fiscal quarter that it was originally planned to take place, simply update the `EBR Date` field to the new scheduled date.
* If the `EBR Date` is changed to a date that is in the next fiscal quarter please treat it as if that EBR was declined. Update the `EBR Status` and the `EBR Outcome` field to `Declined` and save the EBR. Please review the section above on creating successive EBR's for an account.  

#### Linking EBR's to Opportunities:
* Although all EBR's can be associated to an Opportunity, not all EBR's necessarily need to be associated to an opportunity. Only the four latest EBR's should be related to an upcoming opportunity.

For example, If there is an upcoming opportunity in Q4 2019 then the only EBR's that should be related to this Opportunity should be the following EBR's, Q1-2019-EBR, Q2-2019-EBR, Q3-2019-EBR & Q4-2019-EBR (Assuming that the Q4 EBR took place before the opportunity close date).

* To link an Opportunity to and EBR use the "New EBR-Opportunity Associations" Button that is located above the "EBR-Opportunity Associations" related list. This is done on either the Opportunity you would like to associate the EBR with, or the EBR that you want to associate with the Opportunity.

Scroll down to find the "EBR-Opportunity Associations" related list on the layout and click on "New EBR-Opportunity Associations" Button. From there, search and select the appropriate Opportunity and EBR that need to be associated with one another and save the record.

### Professional Services Engagements (PSE) objects

PSE objects in Salesforce are used to track the progress of our PSE's that are agreed upon with our customers. These PSE's describe the professional services that Gitlab will deliver to our client. As this is related to a billable service that we are extending to our clients all PSE's must be related to an appropriate Opportunity and an Account. For a walkthrough, see the GitLab Unfiltered [PS Engagement Object video](https://www.youtube.com/watch?v=IDvfHYLk7_Y&feature=youtu.be)

The Opportunity that each PSE is associated with will contain information relevant to the Opportunity (Amount, IACV etc.) while the PSE itself will house notes, details and monitor the progress of the PSE (Go Live Date, Kick Off Date etc.). If a client would like to move forward with many professional services at once then all of these services would be encapsulated and related through one Opportunity and one PSE.

If an existing client, who previously purchased professional services from Gitlab, would like to purchase addition professional services, then a new Opportunity and PSE would be created in Salesforce. Review our section in the [handbook](/handbook/sales/#when-to-create-an-opportunity) about creating new opportunities if you have any questions around the Opportunity creation process.  

In order to track the contacts that are associated with a PSE, we utilize the PSE-Contact Association list. This can be accessed by navigating to the PSE page layout and locating the PSE-Contact Association related list. From there you can create a new association by looking up the contact that is associated with this PSE. Multiple contacts can be associated with a single PSE.

##### Fields

**PS Team**
* Owner - the owner or overseer of the project
* Project Team - the planned team for the project

**PS Info**
* PS Engagement Name - the unique identifier for the project
* Engagement Type - whether the project is fixed, time based, etc.
* Opportunity - link to the related PS Opportunity
* Opportunity Amount - the booked amount (from the PS Opportunity)
* Success Criteria - the pre-defined criteria for what success will look like at the end of this engagement
* Sertifi EContract - link to the Sertifi contract
* Status - the current project status
   * Backlog - waiting for the customer
   * Initiation - in kick off or planning stages
   * In Progress - the project is being worked on
   * Closure - waiting for customer signature or finalizing paperwork but the services have been rendered
   * Completed - the project is 100%, all items have been signed-off, and this PS Engagement object is complete
* SOW Link - link to the SOW
* Collaboration Project - link to the GitLab collaboration project
* % Complete - the PS engineer's estimate on the project's completion
* General Notes - free-form text for notes about the project

**Project Tracking**
* Scoped Hours - hours scoped during the SOW
* Hours Consumed - billable hours consumed to date
* Remaining Project Hours - Remaining hours of the project
* Hours Updated Date - the date when Hours Consumed was last updated

**PSE Approval**
* Approved - PS management has signed off that the project can begin
* Approver - the Salesforce user who ticked the `Approved` box
* Passive acceptance language in SOW? - does the SOW contain passive acceptance language to complete the SOW?
* Signed Acceptance from Customer - confirmation GitLab has signed approval from the customer to begin the project
* Passive acceptanced used for sign off? - did we use passive acceptance to complete the SOW?


**Project Timeline**
* Kick Off Date - the date the project planning and scheduling began
* Expected Start Date - the anticipated date when the technical portion of the project should begin
* Expected Completion Date - the anticipated date when the project should be completed
* Expected Project Length - anticipated project length, `Expected Start Date` - `Expected Completion Date`
* Actual Project Start Date - when work actually began for the customer
* Completed Date - the actual completed date
* Actual Project Length - actual project length, `Actual Start Date` - `Completed Date`

#### Kicking Off the PS Engagement Object
When starting the PS Engagement, the following fields must be filled out:

* Approved By
* Actual Project Start Date
* Expected Completion Date
* Opportunity (automatically populated)
* Scoped Hours
* Success Criteria
* Sertifi Contract
* PS Engagement Link
* Collaboration Project
* Signed Acceptance from Customer

##### Approved By
When the PSE object has been approved, the following are reviewed to ensure accuracy and proper execution of the SOW:

* PS management team has reviewed the SOW
* GitLab Legal has reviewed the contract, if applicable
* The SOW contract explicitly states if the customer does not sign off within 5 days, it is automatically assumed completed

#### Updating the PS Engagement Object
The PS Engagement Object should be updated on a frequent basis. When it is updated, the following fields should be updated for the benefit of various stakeholders:

* Status
* Hours Consumed
* Hours Updated Date
* % Complete
* If applicable, update General Notes and/or other areas

#### Completing the PS Engagement Object
When completing the PS Engagement Object, review all fields in the PS Engagement to ensure accuracy and completeness. Salesforce validation rules are set up to ensure the fields are complete before marking Status as `Complete`. As a general rule, ask the following questions:

* Are the dates accurate?
* Did we achieve the Success Criteria?
* Are all links (PS Engagement Link, Collaboration Project, etc.) correct?
* Are all required docs signed off by GitLab and the customer?
* Are all remaining fields completed and ready for review by Professional Services, Finance, and Leadership?

Once the above questions have been reviewed, the PS Engagement can be marked `Completed` which will trigger certain events in Salesforce for the various stakeholders.

### Proof of Value (POV) objects

Please visit [this page](/handbook/sales/POV/) for POV documentation.

## Salesforce - Customer Success Automations

### New Zendesk Ticket Notifications

For all new Zendesk tickets that are created, the Technical Account Manager and Account Owner for the account that the ticket is associated with will receive an email notification alerting them of a new ticket. This currently is a one time notification that only occurs when the Zendesk ticket is first created in Salesforce.

### Tracking Emails within Salesforce

Anyone communicating with a customer via email should ensure their emails are being tracked within Salesforce in the account's activity history. To do this:

1. Log in to [Salesforce](https://gitlab.my.salesforce.com/home/home.jsp)
1. Click your name at the top right
1. Click "My Settings"
1. Click "Email" on the left sidebar
1. Click "My Email to Salesforce"
1. Save the email address it provides next to "Your Email to Salesforce address"

Any time you email a customer, bcc your "email to Salesforce address" on the email so that it is tracked within Salesforce.

Two alternatives exist:
1. If you have an [Outreach](/handbook/business-ops/tech-stack/#outreachio) account which is linked to your GitLab email address and your Salesforce account, your emails will automatically sync with Salesforce
1. If you do not have outreach, then consider the [Salesforce Chrome plugin](/handbook/sales/#salesforce-lightning-for-gmail) to easily log customer-related emails

### Logging Calls within Salesforce

There are two options:
1. If you have Chorus and Zoom, you can use the Chorus integration to automatically log calls in Salesforce
1. You can manually log calls

#### Manually Logging Calls, Emails, and Workshops in Salesforce

1. Go to the Account, Opportunity, or Contact
   1. Choose Opportunity if your touchpoint is specific to that deal (e.g., a renewal or sale)
   1. Choose Account if it's a general outreach or ongoing customer
1. Click Log a call
1. Record type: Task and then hit Continue
1. Update fields:
1. Subject (what was the call about?)
   1. Type should be Call*
    1. Activity Disposition: did you leave a message? Did you get the correct contact?
    1. Activity Source: Call
    1. Contact: if not already added, add the Contact.
    1. Account: if not already added, add the Account.

##### Best Practices on Logging Calls
1. You can change the Type to be Email or Workshop if you want to manually log an email, or to record a workshop event
1. When you Log a Call, you can attach it to the Account, Contact, and Opportunity if you want — you'll do that on the data input page
1. You _can_ create a follow-up task if you want, but aren't required to when logging a call.

### Building Reports in Salesforce

It's best practice to use an existing report rather than to create a new one, keeping it clean. If you're unsure, ask your Operations team. Building Salesforce reports can feel daunting, but here are a few tips. If you'd rather, you can watch a video on [Report Builder](https://www.youtube.com/watch?v=7_LkmrhKf2g).

1. Go to Reports in Salesforce
1. Click "New Report"
1. Choose a "Report Type"
   1. Tip: Typically, you'll want to choose Account (if you want to examine Salesforce Accounts) or Opportunity (if you want to report on open/closed Opportunities)
   1. Tip: "Report Type" is selecting the group of fields you want to use (e.g., Opportunity: all data related to the Opportunity)
1. Report structure:
   1. Show: choose which Accounts/Opportunities to show (typically you want to select "all")
   2. Date field: choose a date to filter results. You can always choose "All Time"
   3. Add filters (white box): you can filter using any fields on the left side
   4. Preview: You can drag any fields as a new column. For instance, you can add Account Name, Account Owner, and Technical Account Manager/Solutions Architect
1. Once complete, either hit "Save" or "Run Report" to preview your report. If you run it, you can hit Save on the next page.
1. No matter what, make sure you save it in a folder that others can also access for transparency
1. Congrats! You're done.   
