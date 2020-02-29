---
layout: handbook-page-toc
title: "Go-To-Market Technical Documentation"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## How to use this documentation

The Documentation below is organized by Feature, each section will have the relevent inputs and outputs as well as references to the logic that processes the input and outputs.

---

## Territory Success Planning

**Business Process this supports:** [Territory Success Planning](/handbook/sales/field-operations/sales-operations/go-to-market/#territory-success-planning-tsp)

**Overview:** The goal of TSP is to keep a set of staging fields constantly update to date from a variety of data sources, then at given intervals copy these vales to the "Actual" set of fields for general use. This allows for us to contantly receive changes but only apply those changes in a control fashion at given intervals. This also allows us to easily track exceptions. Note: This project was orginally referred to as ATAM, which is why the API names of the fields reference that instead of TSP.

**Logic Locations:** [AccountJob.cls](https://gitlab.com/gitlab-com/sales-team/field-operations/salesforce-src/blob/master/force-app/main/default/classes/AccountJob.cls)
Code Units:
* getHighestEmployeesInFamily
* stampATAMAddressFields

**Inputs:** DataFox, DiscoverOrg, Manually Entered Address & Employee Data, Account Parenting Hierarchy

**Outputs:** Here is the outline between of two sets of fields we are setting on the Account object. Staging(TSP / ATAM) are set nightly via APEX job. Actuals are set at given intervals found in the business documentation.

| **Data Name**     | **Actual - Field API Name**                  | **TSP - Field API Name**        |
|---------------|--------------------------------------------|-----------------------------|
| Owner         | Owner                                      | ATAM_Approved_Next_Owner__c |
| Owner Role    | Owner.Role                                 | ATAM_Next_Owner_Role__c     |
| Owner Team    | Account_Owner_Team__c                      | ATAM_Next_Owner_Team__c     |
| Max Employees | TBD                                        | JB_Max_Family_Employees__c  |
| Sales Segment | Ultimate_Parent_Sales_Segment_Employees__c | JB_Test_Sales_Segment__c    |
| Region        | Region__c                                  | ATAM_Region__c              |
| Sub-Region    | Sub_Region__c                              | ATAM_Sub_Region__c          |
| Area          | Account_Area_ADMIN_USE_ONLY__c             | ATAM_Area__c                |
| Territory     | Account_Territory__c                       | ATAM_Territory__c           |
| Country       | TBD                                        | ATAM_Address_Country__c     |
| State         | TBD                                        | ATAM_Address_State__c       |
| City          | TBD                                        | ATAM_Address_City__c        |
| Street        | TBD                                        | ATAM_Address_Street__c      |
| Postal Code   | TBD                                        | ATAM_Address_Postal_Code__c |

## Salesforce Record Sharing And Visibility Settings 

**Business Process this supports:** Security and compliance requierments for federal customers

**Overview:** The goal of our record sharing settings in Salesforce is so that the Public Sector Team and approved supporting functions can view public sector records. A Public Sector recrod is considered any record in Salesforce that is owned by the Public Sector team. This is acchomplished by the use of sharing rules and groups within Salesforce. If a record is owned by a member of thePublic Sector Group then that record is only shared and visible to other members of the Public Sector Group. If the record is owned by anyone other then a member of the public sector group, then that record is visible to all internal users within our Salesforce Instance. Membership to these applicable groups is controlled by System Administrators and Sales Operations.  

**Logic Locations:** 
* [Salesforce Object Sharing Settings](https://gitlab.my.salesforce.com/p/own/OrgSharingDetail?setupid=SecuritySharing&retURL=%2Fui%2Fsetup%2FSetup%3Fsetupid%3DSecurity)
* [Public Groups in Salesforce](https://gitlab.my.salesforce.com/p/own/OrgPublicGroupsPage/d?setupid=PublicGroups&retURL=%2Fui%2Fsetup%2FSetup%3Fsetupid%3DUsers)

## Quote Approval System

**Business Process this supports:** Discount Approvals

**Overview:** According to the [Deal Approval Matrix](https://docs.google.com/document/d/1-CH-uH_zr0qaVaV1QbmVZ1rF669DsaUeq9w-q1QiKPE/edit) Quotes must have discounts approved by different management levels depending on discount percentage and term length. To achieve this, we have written automation to stamp a quote with each potential approver, revised the code that determines which approvals are required, and revised the actual approval process in Salesforce.

**Quote Management Stamp** When a Quote is inserted, get the owner of the related Opportunity. Then, find the manager of the owner and the manager of the manger for each manager, five mangers down. Record the first active Regional Director, Area Sales Manager, and Vice President on the Quote. These lookup fields will be used in the Approval Process, if needed.

**Quote Approval Code** This is a table of the Quote (API Name: zqu__Quote__c) fields that trigger quoteApprovals to recalculate and what must happen to them.

|**Field API Name**|    **What Must Happen**|
|----|----|
|Rate_Plan_Count__c|Change|
|zqu__Previewed_TCV__c|Change|
|zqu__Previewed_SubTotal__c|Change|
|zqu__Previewed_Discount__c|Change|
|Non_Standard_Contract_Terms__c|Change|
|Reseller_PO_Status__c|Change|
|zqu__PaymentTerm__c|Change|
|zqu__Previewed_Total__c|Change|
|zqu__Previewed_Discount__c|Change|
|Quote_Amendment_Last_Modified_Date__c|Change|
|zqu__InitialTerm__c|Change|
|zqu__RenewalTerm__c|Change|
|X_Trigger_Quote_Approval_Check__c|Become true|

If any of these events happen, all "Required_Approvals" fields (Required_Approvals_From_CEO__c, Required_Approvals_From_CFO__c, Required_Approvals_From_CRO__c, Required_Approvals_From_CS__c, Required_Approvals_From_Legal__c, Required_Approvals_From_VP_of_Channel__c, Required_Approvals_From_VP_of_Sales_RD__c, Required_Approvals_From_RD__c, Required_Approvals_From_ASM__c) are cleared. These are the rich text area fields that show which management levels need to approve the Quote on the page layouts.
Then, all relevant Quote Rate Plan Charges (API Name: zqu__QuoteRatePlanCharge__c) related to the Quote are queried, these are what hold the term, product, and discount information we need to determine what approvals are required. Following the [Deal Approval Matrix](https://docs.google.com/document/d/1-CH-uH_zr0qaVaV1QbmVZ1rF669DsaUeq9w-q1QiKPE/edit), we determine what level of management the Quote Rate Plan Charge needs and stamp the correct "Required_Approvals" fields with the discount percentage, type, and term. Similar logic is then run for any Quote Rate Plan Charges related to Professional Services products.
Finally, the Quote's Approval_Stage__c field records whether it needs approval, doesn't need approval, or has been approved.

**Quote Approval Process**
This utilizes Salesforce's built-in Approval Process functionality.
We have two Approval Processes for Zuora Quotes, the first for undiscounted, and the other for ones with discounts.
The Quote must be submitted using the "Submit for Approval" button on the page layout to enter the correct Approval Process.
* Undiscounted Approval Process
    * If the Quote's Approval Stage is "Approvals Not Required" or null, the Approval Stage is updated to "In Review" and the Owner of the Quote is emailed confirming submission for approval. Then, if there are any Special Terms and Notes or has been flagged as Requires Deal Desk Review, a member of the Deal Desk team must approve. If neither of those are true, the deal auto-approves. Upon approval, the Owner of the Quote is emailed to inform them of the approval and the Approval Stage is updated to "Approved". If the Quote is rejected, the Approval Stage is set to "Rejected" and the Owner is emailed informing them.
* Discounted Approval Process
    * If the Quote's Approval Stage is "Approvals Required" or "Rejected", the Approval Stage is updated to "In Review" and the Owner of the Quote is emailed confirming the submission for approval. Then, based on the "Required_Approvals" fields, the Quote waits for approval by the people in that step. Once all approvals are acquired, the Approval Stage is set to "Approved" and the Owner of the Quote is emailed. If any step rejects, the Approval Stage is set to "Rejected" and the Owner is emailed as well.

**Logic Locations:**
* [ZuoraQuoteClass.cls](https://gitlab.com/gitlab-com/sales-team/field-operations/salesforce-src/-/blob/master/force-app/main/default/classes/ZuoraQuoteClass.cls)
Code Unit:
    * stampManagerStack
* [ZuoraQuoteClass.cls](https://gitlab.com/gitlab-com/sales-team/field-operations/salesforce-src/-/blob/master/force-app/main/default/classes/ZuoraQuoteClass.cls)
Code Unit:
    * quoteApprovals
* [Salesforce Approval Process Setup](https://gitlab.lightning.force.com/lightning/setup/ApprovalProcesses/home)
Manage Approval Process For:
    * Quote (Installed Package: Zuora Quotes)
