---
layout: handbook-page-toc
title: "Sales Order Processing"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Creating Accounts, Contacts, Opportunities, and Quotes in Salesforce

### Step 1 - Create an Account

1. Click on the Accounts tab
1. Click on New button to Create Account
1. Select either Standard or Channel record Type. Each record type will have a different Account layout based on our engagement.
1. Standard Record Type should be used for all non-reseller partner accounts.
1. Channel Record Type should be used for all authorized and non authorized reseller  accounts.
1. On the Create Account Screen
    1. Enter all mandatory fields 
    1. Populate the "Domain" field with the suffix of the customers email address - like `gitlab.com` (needed for identifying customers and leads)
    1. Click on Save – Account is created
1. Include detailed information regarding the Account including full (legal name), address, and other requested details on the Account template

### Step 2 - Create a Contact

1. Create Contacts, by clicking on the new contact button
1. Make sure to add in the full name, title, phone number and address for any contacts associated with the quote (Bill To and Sold To)
    **Note** Not including accurate information may result in delays of Opportunties being processed and/or closed
 

### Trade Compliance (Export / Import) and Visual Compliance Tool in SalesForce

1.  Why is Trade (Export / Import) compliance important
    1. Not complying could be detrimental to the United States and other countries GitLab operates in
	1. IT’S THE LAW!
	1. Not complying could result in fines or penalties for GitLab and/or GitLabbers
	1. Non-compliance could result in the inability to sell to federal customers, lose the trust of our customers, partners and investors and result in fines or jail time for officers and offenders
1. For more information on Trade Compliance see [Trade Compliance (Export/Import Control)](/handbook/people-group/code-of-conduct/#trade-compliance-exportimport-control) on the [Code of Business Conduct & Ethics and GitLab People Policy Directory page](/handbook/people-group/code-of-conduct/).
1. GitLab uses a third party tool called “Visual Compliance” that is connected to our GitLab SalesForce account
1. This tool checks Account information against various databases to ensure no matches, Accounts are checked repeatedly to ensure GitLab's continued compliance

1. VISUAL COMPLIANCE STEPS
    1. STEP 1: The Account information is pulled into Visual Compliance when an Opportunity, or other action, is requested for that Account. 
    1. STEP 2: The information is automatically reviewed for non-compliance / issues with the Account
    1. STEP 3: If the Account information provides NO MATCHES, Visual Compliance will CLEAR the Account
        1. NOTE: Visual Compliance will update SFDC every 15 minutes
    1. STEP 4: If the Account information provides a ‘hit’, meaning it matches some element of information from a regulation or restriction, a GitLab legal member will manually review the Account
        *NOTE: GitLab legal reviews these accounts at 09:00, 12:00, 5:00 (CENTRAL TIME)
    1. STEP 5: If the Account is approved, the GitLab legal member will CLEAR the Account, and Visual Compliance will update (every 15 minutes)
        *NOTE: If GitLab legal finds an issue with the Account they will alert the Sales Team to the Account being ‘locked’ and will work to verify next steps. 

1. WHAT SHOULD SALES DO?
    1. STEP 1: The more accurate information in the Account--THE BETTER! Meaning, provide the full company name, company address, and contact name(s). Partial information will result in ‘hits’ and delay the process
    1. STEP 2: If you receive the below error when attempting to update an Account: 
        *(i) Check if the Visual Compliance Section [of the Account] says “Pending”-- Wait 15-30 minutes for the system to run its initial check and update. However, if Visual Compliance finds a potential ‘hit’ it will be cleared per the below
        *(ii) If the Visual Compliance Section [of the Account] says  “Yellow” or“Red”-- The legal team is manually reviewing the Account to ensure compliance. This is done three (3) times a day and will automatically update the Account--check back in on the Account during the same day
        *(iii) If the Account requires immediate action (i.e., to close a deal), open a Chatter message in the Account and message “@legal”--upon receipt the Legal team will immediately review and update in Visual Compliance--change should update in 15-30 minutes
    1. STEP 3: Once the Visual Compliance Section is updated, all Account functionality will return and you may proceed
    
### How to process Customer requested "Vendor Setup Forms"
* From time to time a Customer may request that GitLab complete a Vendor Setup document. This is generally required for procurement groups to add a new vendor to their system(s).
* The Sales Team member is responsible for completing such forms by following the below steps:
1. Complete as much of the form as possible. Much of this information is publicly available in the GitLab handbook. Helpful information can be found on the [Company Information](https://gitlab.com/gitlab-com/finance/wikis/company-information) page and on the final page of any direct order form generated via a Zuora quote;
2. Engage deal desk (via Cases in SFDC) only for any information that is not available in the GitLab handbook;
3. With respect to any legal terms, deal desk will engage GitLab legal for review and approval;
Note: GitLab will not agree to any additional terms in a Vendor Setup Form. The parties will have all the applicable terms related to the products and services we offer in, (a) the Order Form agreed to between the parties, and/or (b) a definitive agreement that is executed by GitLab and the prospect/customer.
4. Vendor Setup Forms that require signature must follow the standard Signature Process (See [Obtain Signature](/handbook/business-ops/order-processing/#obtain-signatures) process below).
Note: Sales Team Members are **NOT** authorized to sign any document, contract and/or Agreement.      

### Step 3 -  Create an Opportunity

1. Please see the [Creating a New Business Opportunity](/handbook/business-ops/resources/#how-to-create-an-opportunity) section for an overview on how to create opportunities based on new vs. growth.
1. Select the Opportunity Record Type. Like Accounts, the options are Standard and Channel.
   * Standard should be selected when engaged in a Sales opportunity.
   * Channel should be selected when engaged in a Reseller opportunity (attempting to sign a reseller partner in a new territory, not Sales opportunities where resellers are involved).
1. Enter all the required fields based on your business process and click on Save Button
       **Note** Not including accurate information may result in delays of Opportunties being processed and/or closed

### Step 4 - ZQuotes – New QUOTE

This is the process to create a quote. If you want to clone an existing quote, please see the Cloning an Existing Quote section.

#### Entering Quote Details

1. Click on New Quote button within the opportunity
1. Enter all details and click on Next and select products to complete the Quote creation process
1. All the fields marked in red are mandatory fields, below are fields description
1. Valid Date – Date until when Quote is valid; This is auto set to 30 days from today’s date
1. Quote Template – click on the button to select the Quote template
   * If you are selling a GitLab.com subscription where the prospect/customer is requiring an SLA for the hosted offering, please make sure to use the template that includes the SaaS Addendum. For example, if selling to a customer, you would normally use **New Quote V2.5**. However, if you need the SLA, you would select **New Quote V2.5 (w/ SaaS Addendum)**.
1. Non Standard Contract Terms - select all items in this multi-select picklist that are relevant for this quote
2. Submitter Comments - This is an open text field and will be shared with [quote approvers](/handbook/business-ops/order-processing/#quote-approval). Please provide context around this quote and all details that any approver should know. 
1. Bill To contact  - Click on the vlookup button to enter the Bill To contact information. This will bring up a pop-up window that will list all the contact that were created during Step 2 of the process. Bill To person would be the contact to whom the bill will be sent
1. Sold To Contact - Click on the vlookup button to enter the Sold To contact information. This will bring up a pop-up window that will list all the contact that were created during Step 2 of the process. Sold To person would be the contact to whom the product was sold. For GitLab.com deals, please make sure that the Sold To Email is the same as the email used on the GitLab.com account.
1. Invoice Owner - This field will only be used incase of creating a Quote created for a End Customer that involves a Partner; Please see [Creating a Quote for Partner Section](/handbook/business-ops/#reseller-opportunities)
1. Invoice Owner Contact - is the person at the Invoice Owner who will receive the invoice.
1. Note that the GitLab entity information will be populated via the following rules. This table is based on the [ISO-2 billing country code](http://www.nationsonline.org/oneworld/country_code_list.htm) of the direct customer or reseller we are delivering invoices to:

| **Entity**      |**Direct / Unauthorized Reseller** | **Authorized Reseller**
|-------      |---------- |  ---- |
|BV (Netherlands)         | NL | Not AU, DE, UK, or US |
|GmbH (Germany)       | DE | DE |
|Ltd (United Kingdom)          | UK | UK |
|Inc (United States)          | Not AU, NL, DE, or UK | US|
|Pty Ltd (Australia)          | Not NL, DE, UK, or US | AU |



* For example:
  * a direct customer or unauthorized reseller in the Netherlands (NL) will be billed out of GitLab BV; Germany from GitLab GmbH; United Kingdom from GitLab Ltd; any direct customer outside these countries will be billed from GitLab Inc.
  * an authorized reseller based on Germany will be billed from GitLab GmbH; United Kingdom from GitLab Ltd; United States from GitLab Inc; any resellers based outside these countries will be billed out of GitLab BV.

1. Payment Method - refers to the type of payment the customer is using for paying this Quote/Subscription. Payment Methods currently defined are as follows:
   *  Credit Card
   *  ACH
   *  Check
   *  Wire Transfer
1. Currency - only USD is available.
1. Click Thru EULA - Set to `Yes` only when using a Reseller template and it's a new subscription or an add-on. This is used when an agreement has not been signed; A use case being a product (EE) is sold through a partner
1. Start Date -  Specify the date on which this subscription, or contract, is effective. This date becomes the Contract Effective Date of the subscription in Zuora. Note: Customers can purchase in advance of the subscription Start Date. In this case, when the Quote is pushed to Z-billing the license generated will be encrypted with the future Start Date and will not function until then.
1. Subscription Term Type:
 * By default set as Termed
1. Initial Term and Renewal Term - Specify initial term and the renewal term in months
1. Auto Renew - it is checked by Default; However for all quotes when they are saved the auto-renew is turned off.
1. Tax Exempt - Need to check with client to make sure they are tax exempt and load tax exempt certificate into their account in SFDC.
1. Tax Exempt - If tax exempt click yes on drop down menu and add additional notes if needed.
1. Tax/VAT ID field - adding a valid VAT ID is required for tax compliance of cross-country transactions to European Union countries. These are when we bill from GitLab Inc to any EU country, from GitLab BV to any other EU country except the Netherlands, from GitLab Ltd to any other EU country except the UK, from GitLab GmbH to any other EU country except Germany. **Note there is an [automation rule](https://gitlab.my.salesforce.com/01Q4M000000oVDi) in Salesforce that automatically populates the contents of a Quotes `VAT ID` from a quotes `VAT/Tax ID` - If you attempt to update the VAT ID and it is overwritten please [chatter for support](/handbook/sales/field-operations/sales-operations/#how-to-communicate-with-us) on the related opportunity**
1. Special Terms and Notes - Enter any additional notes that is not specified by the above settings.
1. Click on Next to make the product selection

#### Selecting Products

1. In the 'Edit Products and Charges' screen, click 'Select'.
1. Select either 'Add Base Products' or 'Add Add On Products'. Starter, Premium, Ultimate, or the GitLab.com plans are considered Base Products, while Professional Services and True Ups are considered Add On Products.
2. Locate the product you'd like to add to the Quote.
3. Click 'Select Plan'. If there are no options, click on 'Add'.
1. Go the term length (one, two, three, etc) and click '+Select'. It should say 'Added' if you've successfully added the rate plan. If not, reselect the rate plan.
2. Go to the bottom right and click 'Next'.
3. If you were adding a base product, you will be prompted to select Add On Product.
4. Repeat steps 3 - 5 to select add on products.
5. Once done, click 'Next.'
6. One the next screen, you will see a summary of the products you've selected in the previous steps. The columns in yellow are editable.
1. In the Discount field, enter the discount in percentage (%) you wish to apply. This will automatically update the Effective Price field.
1. Conversely, if you wish to apply a specific price to a product, enter the price in the Effective Price field. This will update the Discount (%) field.
2. Enter the quantity.
1. Once you've entered the final numbers, click anywhere on the screen to update the totals on the quote.
1. Repeat this step for each product you've selected.
1. If you need to add additional products to the quote, click "+Add Product" button and repeat the steps of adding a product and rate plan.
1. After you've completed adding all products to a quote, click Next Button and you will be taken back to the Quote record detail screen.
1. Once the quote has been created, you can modify it or delete it.
2. Before sending the quote out to the client though you must first have your [quote approved](#quote-approval) 

##### Sending a "DRAFT" proposal to a Client/Prospect Before it Has Been Approved

If you would like to send a draft proposal to a client/prospect before it has been approved in the following step, you may do so. Please note that the draft proposal will have differences from the standard quote template.

*  Draft watermark will be visible on the template
*  No references to legal terms
*  No signature block

To generate a draft proposal:

1. Go to the quote and select one of three draft proposals, based on the transaction type of the quote
2. Click on the "General PDF Draft" button


### Step 5 - Submitting a Quote for Discount and Terms Approval

#### Quote Approval 
Prior to generating a standard (non-draft) quote to deliver to a client or prospect in Word or PDF format, all quotes must be approved. The following steps outline the process for how to correctly submit a quote for approval. This approval flow follows the criteria in [our matrix](https://docs.google.com/document/d/1-CH-uH_zr0qaVaV1QbmVZ1rF669DsaUeq9w-q1QiKPE/edit#heading=h.ag75fqu12pf0) for approvers. Please review this matrix so you are aware of all the scenarios as well as any potential fields that you may have to fill out on the quote. To watch training videos on various scenarios that you may encounter when submitting a quote for review or after it is reviewed please refer to our training videos below. 
1.  Navigate to the quote that you would like to submit for approval. Ensure that all of the relvant information is filled out on the quote. 
2.  Make sure to include the `Submitted Comments` on the quote before you submit for discount and terms approval. Please provide as much detail as to why you are requesting discounts or other terms that require approval.
2.  You will be able to see who the required approvers are on the quote prior to submitting the quote and why they are required.
3.  Once you are sure that the quote has the correct info on it click the the `Submit for Approval` button on the quote screen. 
4.  Your quote has now been submitted for approval. If it needs any approvals you can monitor who needs to approve it on the quote in the section `Required Quote Approvals`
5.  If Quote approvals are not rolled out for you team/region/segment you will be notified to move forward with approvals via a window in Salesforce

#### Training Videos
* In order to view these training videos you must switch your youtube viewer profile so that you are logged into Gitlab Unfiltered. You can switch your user profile by clicking on your profile photo in the top right corner, selecting `Switch account` and selecting Gitlab Unfiltered.   
  
1.  [Simple Quote Approvals](https://youtu.be/XZXyv-6CInk)
2.  [Standard Quote Approvals](https://youtu.be/RppeHssnazs)
3.  [Complex Quote Approvals](https://youtu.be/J49vQe4DGOs)  
  
##### Quote Approvers
According to [our matrix](https://docs.google.com/document/d/1-CH-uH_zr0qaVaV1QbmVZ1rF669DsaUeq9w-q1QiKPE/edit#heading=h.ag75fqu12pf0) for approvers there are a number of reasons that you may be involved in approving an opportunity. Please make sure that you are familiar with the scenarios that you may be involved with.
*  To review how you can approve or reject quotes please watch this [training on youtube](https://youtu.be/T47h4VNTRWU) - Please see the bullet in [Training Videos](#training-videos) on how to access this training video
*  Once a user submits a quote for approval it follows the order of approvers as stated in our approvers matrix.
*  When you are required to review a quote and are the current team member who should review a quote you will be notified by email. In the email you will find the details as to why your approval, who any previous approvers were as well as a link directly to the quote.
*  Once you have reviewed the quote you can either approve or reject any quote in one of two ways: 
   1.  You can reply directly in the email that you received by following the instruction in the email as to if you approve or reject the quote. You must follow this format when replying to an email: 
        * `APPROVE`, `APPROVED`, `YES`, `REJECT`, `REJECTED`, or `NO` must the first line of the email message. Any other terms in the first line of the reply will result in an error.
        * You can enter comments, but they must be on the second line of your response. 
        * If you combine the first and second lines into a single line in your response, this will result in an error.

   2.  You can approve or reject the quote directly within salesforce on the bottom of the quote page under `Approval History`
* If you are going to be unavailable to review and approve quotes (PTO, at a conference etc.) please coordinate with the appropriate team members to ensure that there will still be someone who can review quotes while you are unavailable. 
   

### Step 6 – Generate Quote as PDF

1. Once a [quote has been approved](#quote-approval), go back to the quote and click `Generate PDF Doc`. The document will be saved as an attachment in the Notes and Attachments section in the opportunity record. Note that the ability to generate a Word Doc has been restricted to the Deal Desk team.
2. All requests for custom language or Order Form edits must meet the standards listed in [our matrix](https://docs.google.com/document/d/1-CH-uH_zr0qaVaV1QbmVZ1rF669DsaUeq9w-q1QiKPE/edit#heading=h.ag75fqu12pf0). To request edits to an Order Form, tag @Sales-Support in chatter with the request and Deal Desk will evaluate the request and execute the edits via Word doc after necessary approvals are received.
3. The default template for all transaction types (new, amendment, or renewals) will be the direct (non-channel) quotes that do not show $0 line items. If you want to select a different template, click the search icon next to the Quote Template field and select the desired template. A description of each template will be visible next to each template.

### Process for Agreement Terms Negotiations (when applicable) and Contacting Legal

If the Opportunity meets the dollar thresholds:
  * Greater than $25,000 (USD) Opportunity to review edits on GitLab Agreement template(s)
  * Greater than $100,000 (USD) Opportunity to review Customer template / agreement version(s)
The Sales Team Member will follow the below workflows to make requests for, (i) editable version(s) of GitLab Templates, (ii) engagement of contract negotiations, and (iii) assistance on general questions related to a Customer / Opportunity.

A presentation overview of the process to engage GitLab Legal can be found [**HERE**](https://docs.google.com/presentation/d/1lesWNvPAFd1B3RuCgKsqQlE85ZEwLuE01QpVAKPhQKw/edit#slide=id.g5d6196cc9d_2_0)

A video tutorial can be found [**HERE**](https://www.youtube.com/watch?v=CIWdsqRX7E0&amp=&feature=youtu.be)

You may contact Legal directly in Slack via #Legal

#### Request editable version of GitLab Template:  

At Customer Account, OR, Opportunity:
1. Click "Legal Request" (located at the top of Account and Opportunity SFDC layout)
2. For "**Type of Legal Request**" select "**Request for GitLab Agreement Template**"
3. For "**Type of Contract**" select the Template desired. For example, for a Non-Dislclosure Agreement request, select "NDA"
4. For "**Contract Source**" select "**GitLab Contract Template**"
5. Add any additional notes that may be helpful for GitLab Contract Manager / Legal and hit "SAVE"
6. The information provided will open a "Case", which will automatically be assigned to a Contract Manager / Legal Member
7. The Contract Manager / Legal Member will attach the requested template and tag the requesting Sales Team Member
8. The Sales Team Member will take the template version and provide to the Customer
  * NOTE: Sales Team Members are responsible for communication(s) with Customers. This includes providing back GitLab templates and negotiated terms.

**At this time, the Contract Request Case will be marked as "Closed". Follow the below steps to initiate "Contract Review" of the Customer edits.**

#### Request for GitLab review of Customer edits to GitLab Template, OR, Review of Customer Agreement Template

On Customer Account, OR, Opportunity:
1. Click "**Legal Request**" (located at the top of Account and Opportunity SFDC layout)
2. For "**Type of Legal Request**" select "Contract Review"
3. For "**Type of Contract**" select the type of Agreement / Template being negotiated. For example, for a Non-Dislclosure Agreement request, select "NDA"
4. For "**Contract Source**" select the applicable Agreement / Template Source
  * For edits to a GitLab Agreement / Template select "**GitLab Contract Template**". NOTE: Be sure the Opportunity size is above $25,000 (USD)
  * To request GitLab to edit a Customer Agreement / Template select "**Customer Contract Template**". NOTE: Be sure the Opportunity size is above $100,000 (USD)
5. Add any additional notes that may be helpful for GitLab Contract Manager / Legal and hit "SAVE"
6. The information provided will open a "Case", which will automatically be assigned to a Contract Manager / Legal Member
7. The Contract Manager / Legal Member will review the Agreement / Template and attach updated red-lines
  * The Sales Team member will be alerted (via SFDC Chatter) to the Agreement being updated and ready to be sent to customer
8. If another round of edits are necessary, the Sales Team member will attach the Customer provided red-lines and tag (via SFDC Chatter) the Contract Manager / Legal Member assigned
9. The same steps will repeat until an executable version is reached. At which point, the Contract Request Case will be closed.  
10. The Sales Team Member will follow the steps found at ["Obtain Signatures"](handbook/business-ops/order-processing/#obtain-signatures) and attach the fully executed version to the Customer Account. 
NOTE: The above process may be used to also engage Contract Managers / Legal Members to add non-standard language to Order Forms

**All communications, and versions of Agreements, should be kept in the Contract Request Case**

#### General questions related to a Customer:  

On Customer Account, OR, Opportunity:
1. Click "Legal Request" (located at the top of Account and Opportunity SFDC layout)
2. Provide the question in the "NOTES" Section and hit "SAVE"
3. The information provided will open a "Case", which will automatically be assigned to a Contract Manager / Legal Member
4. The Contract Manager / Legal Member will review the question and provide an answer in the case comments and tag the requesting Sales Team Member via SFDC Chatter
5. Once the question is addressed, the Case will be closed by the Contract Manager. 


#### Obtain Signatures

All contracts / Agreements that require GitLab countersignature will be digitally stamped by a GitLab Contract Manager or legal representative. This is done to ensure and signify that the document has been reviewed and vetted by GitLab legal, and may be signed. 

**Receiving a stamped contract / Agreement**
* Once GitLab and the customer / prospect reach executable terms, the Contract Manager or legal representative will provide a final "Clean" version. This will be in PDF format and include a digital stamp below the GitLab signature line/block which indicates, (i) the name of the GitLab legal member that approved, and (ii) the date of approval.
* If a final agreement has been reached, the Sales Team Member should ensure the contract / Agreement includes the stamp (mentioned above). If a stamp is not included, please contact the contract manger or legal representative involved on the negotiation. Upon being notified of the need for a digital stamp, the Contract Manager or legal representative will respond and attach promptly. 
* Contracts / Agreement without a digital stamp indicating approval by a GitLab Contract Manager or legal representative will be rejected and not signed.

NOTE: In very few circumstances, a Customer may refuse to use a PDF with GitLab Legal stamp for signature, due to their electronic signature tool(s). If this is the case, please supply the Agreement to be signed, and notify the individual(s) with signatory authority with the following information: (I) Overview that the Customer toolset prohibits the use of our GitLab Legal stamp, and (II) A link to the SFDC Case where the Contract / Agreement was negotiated. With this information, the GitLab individuals with signatory authority will be able to compare the requested version for execution, and the latest version approved by Legal in the case.

The signatory Authorization Matrix can be found here: https://about.gitlab.com/handbook/finance/authorization-matrix/  

**Process for Signature**
Once negotiations are completed, and the digital stamp has been affixed to the final version of the contract / Agreement: 
1. Change the status of the contract, in SFDC, to 'Approved to Sign'; and 
2. [stage the contract](https://faq.hellosign.com/hc/en-us/articles/205830938-How-do-I-request-a-signature-) in HelloSign for signatures; 
3. Send to the Customer and cc' our CFO (Paul Machle).

### Uploading Contracts in Salesforce 

All fully executed Customer agreements must be uploaded in SalesForce under the applicable Account, in the Google Docs, Notes & Attachments Section. 
*   Contracts **should not** be stored in the ‘Activity History’ or Chatter section in SalesForce. 
*   Contracts stored under the Account should be labelled appropriately with, (i) Agreement name, and (ii) Date executed.


### Referencing Customized Customer Agreements in Quote 
 
If GitLab agrees to customized terms with a customer, all quotes, SOWs, POs, etc. must reference those customized terms and *not* the GitLab standard terms listed on our website.
 
To update the terms of a quote, follow these steps:
1. Delete the reference in the quote to GitLab’s URL terms.  
2. Replace the reference with the following language - “By accepting this Quote, you and the Entity that you represent (collectively, “Customer”) unconditionally agree to be bound by and a party to the GitLab Subscription Terms executed between Customer and GitLab on mm/dd/yyyy.”
3. Insert the date that the customized agreement was signed.

### Step 7 – Send for Signature via Sertifi

1. Within the ZQuote object, click Sertifi E-Sign button near the top of page.
1. 1st signer will be auto-populated with the bill to contact. You can change if needed by clicking on the search icon next to the contact name field.
1. You will now be asked to attach the Quote PDF.  Under the drop down for Related Notes and Attachments. Select the quote for signature and click send for signature.
1. Once the prospect/customer has signed, you will receive an email with the signed quote as an attachment. The signed document will also be added to the Notes and Attachments section of the Opportunity.

#### Filing the Executed Contract

After both parties have signed the contract, complete these steps:

1. Upload the fully executed pdf to the contract page;
2. Edit the `Contract Status` field to show “Active”;
3. Input the ‘Contract Start Date` and fill in the `Contract Term (months)` field, if applicable. The End Date will auto-fill based on the number you enter. Do not put the end date in the Termination Date field.
4. Copy and paste the terms that have capture fields from the executed contract into the fields. Then, change the drop-down named "Term Capture" to "Complete". If you run into problems, you can change the field to "Started" and then request help by sending a chatter message at @Contracts.

#### Quote Metrics

The following quote metrics are available:

 * MRR (Monthly Recurring Revenue) - Monthly recurring revenue (MRR) calculates subscription recurring fees normalized to a monthly value.
 * Delta MRR - Delta of the total MRRs between the original subscription and the amendment.
 * TCV (Total Contract Value) - Total contract value (TCV) calculates the total recurring charges over the lifetime of a subscription.
 * Delta TCV - Delta of the TCVs between the original subscription and the amendment.
 * Sub-total - The quote subtotal for the specified billing periods, excluding discount charges and taxes.
 * Discount - The sum of all discount charges for the specified billing periods.
 * Tax - The tax calculated for the specified billing periods.
 * Total - The quote total for the specified billing periods, including discount charges and taxes.

### Step 8 – Submitting an Opportunity for Deal Desk Approval

#### Before You Submit an Opportunity for Deal Desk Approval

The following is a list of required documents/processes needed before you submit an opportunity for approval:

####  Direct Deals that do not involve resellers
1. Prospect/Client paid via Credit Card through the web portal- In this scenario the applicbale GitLab terms are agreed upon at the time of the purchase.

**FOR ALL DIRECT PURCHASES (OTHER THAN WEB PORTAL AS STATED ABOVE) AN ORDER FORM MUST BE CREATED AND SIGNATURE IS REQUIRED. ORDER FORMS WITHOUT SIGNATURE WILL REQUIRE ADDITIONAL APPROVAL & REVIEW, INCLUDING OF CUSTOMER PURCHASE ORDER(S), WHICH MAY CAUSE ADDITIONAL TIME IN OPPORTUNITY CLOSURE. GITLAB FIRMLY REQUIRES ORDER FORMS TO BE EXECUTED, OTHERWISE, THE BELOW STEPS MUST BE FOLLOWED**

1. An Order Form (which includes a Quote No.) is required in order to confirm products purchased, # of seats, term, and pricing. An Order Form is also needed to confirm the Prospect/Client agrees to the terms and conditions referenced in the Order Form.
  * Discuss with customers / prospects, from on the onset, that signature will be required.
  * If the parties agreed to non-standard, negotiated terms, the URL to our standard terms and privacy policy should be deleted and replaced with the following: "This Order Form is governed by the terms and conditions of the [NAME OF AGREEMENT] dated [MM/DD/YYYY] between the parties ("Agreement"). Customer has been deemed to have "Accepted" the terms of this Agreement upon the earlier of, (i) executing this Order Form, (ii) reference of this Order Form Quote No within a purchase order or similar document, or (iii) the use of any GitLab software.
  * If an Order Form is executed by the Customer, GitLab review of a submitted purchase order will be minimal, the purchase order must include: a) the correct GitLab entity, b) the Quote No. found within the applicable Order Form, c) payment terms matching the Order Form, and d) line item descriptions that match the Order Form. 
2. In rare circumstances, where a Prospect/Client is unwilling to sign the Order Form, the Sales Team Member must attach to the Opportunity: 
    - Reason(s) why the Customer is refusing to execute the Order Form; and
    - Documentation (i.e., email thread) of the customer refusal
3. If the Customer's purchase order **DOES NOT** include any legal or finance terms, as determined and approved by GitLab finance and legal, and includes a) the correct GitLab entity, b) the Quote No. found within the applicable Order Form, c) payment terms matching the Order Form, and d) line item descriptions that match the Order Form (without signature block), GitLab may accept the Order Form and purchase order without changes.   
4. If the Customer's purchase order **DOES** include any legal or finance terms, as determined and approved by GitLab finance and legal, the Sales Team Member will be guided to direct the customer to either:
   * Remove all references to such terms found within the purchase order; and/or
   * Insert the following language into the supplied PO: "Notwithstanding any of purchaser's standard terms and conditions set forth or referenced herein, this PO is governed by the GitLab Subscription Agreement, GitLab Professional Services Terms (as applicable) or other such software license and/or services agreement negotiated by the parties"
   * The purchase order in either instance (3&4) must also include: a) the correct GitLab entity, b) the Quote No. found within the applicable Order Form, c) payment terms matching the Order Form, d) line item descriptions that match the Order Form (without signature block)
5. Direct Deals without an executed Order Form that do not meet the standards listed above (Sections 2-4) will be rejected.  
 

####  Authorized Reseller Opportunities that involve an Authorized Reseller purchasing to resell to an End User

1. Authorized Reseller must sign an Authorized Reseller Order Form. This will include reference to the executed Agreement between the parties, and in the event there is no executed Agreement, then the Fulfillment Reseller Agreement (located here:https://about.gitlab.com/terms/#reseller) will govern. 
2. Clickthrough EULA must be delivered and accepted by the End User. Please attach a Note to the Notes and Attachments section with a confirmation link or email.
3. If the End User has previously accepted a EULA, then we can use it as the governing terms [with respect to the End User] for this purchase.  In such a case go to our [EULA Request Server](https://customers.gitlab.com/admin/eula_request) and find the ```Token``` and ```Accepted At``` from the customer's previous EULA. Then insert the following into the quote: *"By accepting this quote, you, and the entity that you represent (collectively, “Customer”) unconditionally agree to be bound by the terms agreed to in EULA ```Token``` previously accepted on ```Accepted At```."*


####  Fulfillment Reseller Opportunities that involve a Fulfillment Reseller purchasing to resell to an End User

1. The Sales Team member must create (and provide to the Reseller) a Fulfillment Reseller Order Form, that DOES NOT include a signature block. This Order Form template will include reference to the Fulfillment Reseller Agreement (located here:https://about.gitlab.com/terms/#reseller)
2. GitLab will accept the Fulfillment Order Form without signature, and the Reseller PO, PROVIDED THAT: 
   * The Order Form includes the correct reference to the Fulfillment Reseller Agreement and other terms; and 
   * The PO received is issued to the correct GitLab entity and references the applicable Order Form Quote No. which includes, Quote ID, products, # of users, term, and pricing of the subscription(s).  
3. Clickthrough EULA must be delivered and accepted by the End User. Please attach a Note to the Notes and Attachments section with a confirmation link or email.
4. If the End User has previously accepted a EULA, then we can use it as the governing terms [with respect to the End User] for this purchase.  In such a case go to our [EULA Request Server](https://customers.gitlab.com/admin/eula_request) and find the ```Token``` and ```Accepted At``` from the customer's previous EULA. Then insert the following into the quote: *"By accepting this quote, you, and the entity that you represent (collectively, “Customer”) unconditionally agree to be bound by the terms agreed to in EULA ```Token``` previously accepted on ```Accepted At```."*



####  Required fields in Salesforce before submitting for approval

1. On the Account record:
  * Industry
  * Complete Billing and Shipping Address
  * In the Special Terms field, add any non-standard terms related to the subscription (ramps, special pricing), support (non-standard SLAs), finance (special billing/payment terms), or legal.
1. On the Opportunity record:
  * Go to the Contact Roles related list and add a Primary Contact. Ideally, you'll add Contact Roles much earlier in the sales cycle.
  * If the opportunity involved a partner, meaning partner will get credit for the opportunity, please click new in the partner section and add partner. There should only be one partner selected for each opportunity.
  * Add the Competitor(s). Note that this is only required for New Business; it is not required for Renewals or Add On Business.
  * Make sure your Close Date is for the date you are submitting the opportunity for approval.
  * Provide the Closed Won Details- a few sentences on highlighting why we won the deal (pricing, packages, feature set, etc.) should do.
  * Once these steps are completed, save the record and submit the opportunity for approval.
1. On the Contract record:
  * Attach any signed agreements, POs, and quotes as an attachment to the **contract** record in Salesforce.com.

#### Submitting an Opportunity for Deal Desk Approval

1.  **To submit the opportunity for approval and closure, the Sales Rep should click on the “Submit for Approval” button on the opportunity.** 
    *  The opportunity page will then display “edit” mode. Click Save. 
    *  Common errors when submitting an opportunity for approval:
        *  Approval Status. The Approval Status should not already say “Approved.” If the opportunity was already approved, the opportunity should not be submitted for approval.
    *  Once submitted, the opportunity’s stage will update to “7- Closing,"" the opportunity record will become locked, and the Approval Status will read "In Progress."
    *  Recalling Approval: 
        *  To unlock the opportunity to make changes, recall the approval submission by scrolling down to Approval History and clicking “Recall Approval Request.” Once you’ve made your changes, resubmit the opportunity for approval. You will receive a confirmation email once the opportunity has been submitted for approval.
2.  **Deal Desk + Finance Approval Workflow**
    *  **Deal Desk Review** is initiated. It is unnecessary to chatter Sales Ops after you submit an opportunity. A Deal Desk Analyst will assign themselves to review the deal via the “Deal Desk Analyst” opportunity field.
    *  **Deal Desk Approval:** If Deal Desk approves the opportunity based on the criteria above, the “Approval Status” field will update to “Deal Desk Approved.” The opportunity will remain in stage “7- Closing,” but will route to the Billing team for Finance approval. 
    *  **Deal Desk Rejection:** If Deal Desk rejects the opportunity based on the criteria above, the “Approval Status” field will update to “Rejected” and the opportunity will unlock. The opportunity will revert to stage “6- Awaiting Signature.” A rejection email will be sent to the Sales Rep with rejection comments and/or instructions. After taking the appropriate action(s) outlined in the rejection comments, the Sales Rep should re-submit the opportunity for approval. 
    *  **Finance Approval**: Once Deal Desk has reviewed and approved the transaction, Finance will review. If the opportunity is approved by Finance, the stage will update to “Closed Won” and the deal is officially booked. An approval email will be sent to the opportunity owner and Slack message will appear in the “wins” channel and the "wins-key-deals" channel where applicable.
    *  **Finance Rejection:** Once Deal Desk has reviewed and approved the transaction, Finance may reject the opportunity. If Finance rejects the opportunity, the stage will remain in “7- Closing” and both the Sales Rep and Deal Desk Analyst will receive an alert email containing the rejection reason. The Sales Rep should work with the Deal Desk Analyst to rectify the issues that led to Finance rejection. Once the issues are resolved, the Deal Desk Analyst will approve the deal once more to submit it to Finance for final approval.



### Deal Desk Approval Process

The Deal Desk will review the following data points once an opportunity has been submitted for approval:

1. There is a signed quote or a PO attached to the opportunity Notes and Attachments section.
1. If an SLA or MSA has been issued, it must be attached to the opportunity, approved, and countersigned.
1. Complete and accurate Bill To and Sold To Information on the order form. Any blank values will be rejected.
1. Start Date confirmation- start dates may be in the past because quote was never updated or took time to sign.
1. Correct template is used for direct vs. authorized vs. unauthorized resellers. This is especially important if a EULA must be delivered.
1. If a PO is issued:
    * The Amount on the PO and the Quote must match.
    * The entity on the PO should match the correct entity of the quote.
    * The correct Quote ID must appear on the PO for reseller deals only. If the client/prospect is not going to sign the order form and if the PO contains terms and conditions (or a link to terms and conditions), you must also include the effective date of the governing MSA or EULA onto the PO.
    * The PO must appear in the `Purchase Order` field on the Quote object.
    * All PO terms must be approved by Legal or CFO for each opportunity.
1. For reseller quotes, the opportunity and quote should be created under the end-customer account, NOT the reseller account. The reseller should be listed as the Invoice Owner and the reseller's billing contact should be listed as the Invoice Owner Contact.
1. Discounts:
    * Check discount level as per the [Discount Approval Matrix](https://docs.google.com/document/d/1-8TG8YLAQB-465mFLYnX3wkB6C6-0aI1A4CzdfjpacU/edit#heading=h.gajbwmoww16e).
    * Were the discount approvals documented via Chatter?
    * Future discounts greater than initial discount. This should be checked upon quote creation, but should be pre-approved by CRO or RD.
1. Correct GitLab Entity
    * For customers subject to switch to new entity, Add Ons should be on the original entity.
    * Upon renewal, customer will then be migrated to new entity.
1. Review for any revenue recognition terms.
1. Ensure that the quote does not list any future products as this impacts revenue recognition.
1. Any exceptions to standard start/end dates.
1. If the opportunity is for training or professional services a detailed cost estimate must be included as an object in the opportunity record. 
    * Professional services that are associated with a SKU do not require a cost estimate. Any discounted services (including zero values) require specific approval according to the discount authority matrix.

### Deal Desk Approval Process - FY21 Additions

In addition to the above, starting in FY21 Deal Desk will review the below items before approving any deal:

**1. SalesForce Data Points**

*   Account Ownership
*   Opportunity Ownership
*   Financial Fields [Amount, Renewal Amount, Renewal ACV, iACV]
*   Compensation Fields [User Segment (O), Account Owner Team (O), Owner Team (O), SA Team - Xactly]

**2. Professional Services Opportunities**

*   In scenarios where an SOW contains multiple billable events, payable at the time the event takes place (i.e. invoice schedule based on completion of services at different times), multiple opportunities will be created based on the dates of the services. This ensures that invoicing can be done correctly.
*   A Professional Services SKU may be used in conjunction with a subscription product SKU on a single quote/opportunity in cases where an SOW is not required. 
*   A Professional Services quote reflecting a signed SOW will be created using the GitLab Service Package SKU.
  
**3. New Business Opportunities for Existing Billing Accounts**

*   Deal Desk will check if the Sold To Contact on the quote matches the current Sold To Contact on the Zuora Billing Account. 
    *   If the contact does match, Deal Desk will paste the Billing Account ID into the Billing Account ID field on the quote object.
    *   If the contact does not match, Deal Desk will ensure that the Billing Account ID is blank on the quote to drive creation of a new Billing Account.

**4. Revenue Recognition Issues**

*   Deal Desk must tag the Revenue Recognition team to review opportunities in the following scenarios:
    *   Where there are multiple line items for the same product (i.e. 100 Starter licenses at 0% discount and 50 Starter licenses at 10% discount)
    *   Professional Services sku used on the same quote as a subscription product SKU
    *   Any discounted Professional Services SKU
    *   Tiered Pricing
    *   Guest or Reporter Access SKU(s) in addition to a standard subscription product SKU on the same quote
    *   The usage of any free SKU


### Step 8 – Sending the Quote to Zuora

1. Once the opportunity has been approved, the Deal Desk will receive an email from Salesforce to push the Quote to Zuora.
2. The immediate task will be to click on Send to Zuora button. This will complete a few actions:
    - First it will create the subscription in Zuora.
    - Second, it will create the Billing Account.
    - Lastly, it will prepare the system to send an invoice to the customer (this is completed by the Finance team).
2. To send a quote to Zuora, go to the Quote and click on the Send to Zuora button.
3. Review the customer and product details.
4. Click Submit.
5. If Click Through EULA is "Yes", the EULA will be delivered to the sold to email address for new customers. For existing customers, the EULA is delivered to the previous email that received the original EULA. Note that EULAs will be delivered in the following scenarios:
    - Invoice Owner is a reseller and it's for a new subscription or an add-on
    - Quote Template contains "No Signature"

## Post-Closed Won Account and Opportunity Reassignments

Once an opportunity is approved and marked as Closed Won, certain actions occur:

1. Depending on the Sales Segmentation, the account and/or future renewal opportunity may be assigned to a new team member:
  * If Sales Segmentation is SMB, then the account and renewal opportunity will be assigned to the regional SMB Customer Advocate.
  * If Sales Segmentation is Mid-Market, then the account and renewal opportunity will be assigned to the Mid-Market Account Manager by Region.
  * If Sales Segmentation is Large or Strategic, then the renewal opportunity will be assigned to the current Account Owner.
  * Please note the following exceptions to these assignments, regardless of Sales Segmentation:
      * If the Account Manager field is populated, the renewal opportunity and account will be reassigned to this user.
      * If the Account Owner is a Partner User, the renewal opportunity and account will remain with the Partner.
      * If the Customer is a Federal government account, the renewal opportunity and account will remain with the current Account Owner.
1. If the customer agrees to be a reference, please complete the following steps:
  * In the Referenceable Customer field on the account page, change the picklist value to "Yes".
  * Select all the Reference Types they are willing to offer (please see the next section for an explanation of the Reference Types).
  * Enter any Reference Comments related to the customer's willingness to be a reference.
  * Also go to the contact object who agreed to be a reference and under the field "role" please select "reference - investors and prospects".
  * If customer agrees to speak with product marketing about how they use GitLab, please email product marketing manager.
1. If the customer declines to be a reference in any way, please note that we cannot mention them in any external conversations with prospects or investors. Please make sure to add notes in the Reference Notes field on why the customer declined.
1. Once the opportunity is closed won, the field "type" on the account object will change to "Customer".
1. Create an add-on or Existing Account (new division) opportunity if there has been one identified by you at this time.

**Customer Support Levels**

Depending on the products purchased, the customer will receive certain level of support.
1. If a customer has purchased:
   *  Ultimate, Premium, or legacy Premium Support add on, they will receive "Premium" support.
   *  Starter or legacy Enterprise Edition packages, they will receive "Basic" support.
   *  Legacy Standard or Plus customers will receive a "Custom" support package.
   *  GitLab.com customers will receive support that corresponds to their package (eg, Gold Plan customers receive Gold support).
   *  Organization on a free Ultimate or Gold Plan for EDU or OSS will be on a "Community" support. If they paid for support, they will be on plan based on their package.

If a customer is overdue on an outstanding balance, the Finance team will mark their support as "Hold". This will sync to Zendesk and support will not respond to their support requests until the "Hold" has been lifted.


**Reference Types:**

* Homepage: The customer allows GitLab to use their logo on the GitLab homepage. Please obtain an image file with their logo, or gain customer acceptance of a logo to be used on the GitLab website.
* Customer Story: The customer allows GitLab to share their story and use case with prospects and investors.
* Case Study: The customer allows GitLab's marketing team to draft content highlighting their business challenges and how GitLab solved those challenges.
* Verbal Reference: The customer agrees to speak with either investors or prospective customers on their experience with GitLab.

### Cloning an Existing Quote

If you'd like to save time by cloning an existing quote, you can do so by doing the following:

1. On the Quote Detail page of the quote you want to clone, click Clone Quote.
2. On the Quote Clone Configuration page, select the following options:
    * Clone Products: Select to clone the products associated with the quote. This option only applies to the New Subscription quotes. Ensure that the products associated with the quote are maintained in the current version of the product catalog.
    * Maintain Quote: Select to be directed to the first step in the Quote Wizard flow that allows you to edit the newly cloned quote. The flows are configured based on the quote type, i.e., New Subscription, Amendment, and Renewal, in the Quote Wizard Settings.
5. Click Next.
    * If you selected the Maintain Quote option, you are redirected to the first step in the Quote Wizard of the newly cloned quote.
    * If you did not select the Maintain Quote option, you are redirected to the Quote Detail page of the newly cloned quote.
8. Please note that you cannot clone the products on an amendment (add-on or renewal quote.)

### Using the Primary Quote Checkbox

If you create multiple quotes for a single opportunity (EEP vs. EES, single year vs. multi-year, etc.), you can select one of the quotes as the "primary", which  will push the details of that quote to the opportunity. Once you select a different quote as primary, the details of the opportunity are overwritten with the new primary quote's details (amount, initial term, start date, and related quote).

### Opportunity Values and Fields

The following fields are populated via a series of workflows or calculations from an associated quote or subscription in Zuora to the Opportunity object in Salesforce. For more information on some of the following values and how they are defined, please see the [GitLab Metrics](/handbook/finance/operating-metrics/) of the handbook.

1. Annual Contract Value (ACV) is the value of first twelve months of a subscription. This field is calculated by the Opportunity Term and the MRR fields on the Opportunity. Here are the calculations: If the Opportunity Term is greater than 12 months, the ACV will be the `12 * MRR`; otherwise the ACV will be `Opportunity Term * MRR`.
2. Renewal ACV is manually populated at this time and takes all renewing opportunities and sums the ACV of these opportunities. For example, there are two opportunities (a new opportunity at 7,800 ACV and an add-on at 3,900 ACV). The Renewal ACV for the renewal opportunity will be 11,700.
3. Incremental ACV is `ACV - Renewal ACV`. This value can be negative if the customer is planning to renew at a lower ACV than the previous subscription.
4. Upside IACV is the potential value of an opportunity where the client/prospect might be interested in a higher-tier package or deploying to more users. For example, if you have a client/prospect that is interested in 1,000 Premium seats or 1,000 Ultimate seats, you will have 1,000 * $228 ($228,000) for the Incremental ACV but could have 1,000 * $1188 ($1,188,000) as the Upside IACV.
5. Swing Deal is a checkbox. If this field is checked, it means that this opportunity has a chance to close in the current period.
5. Opportunity Term is a value that is captured based on certain scenarios:
   * Single Quote
      * For New Business with a single quote, this field will be populated via the `Initial Term` field on the Quote object.
      * For Renewals with a single quote, this value will be populated via the `Renewal Term` field on the Quote object.
      * For Add-On Business with a single quote, this value will be populated via a formula that takes the `Term End Date - Start Date`. Any partial month will automatically be rounded up to the next month (2 months 1 day will automatically round up to 3 months).
   * Multiple Quotes: If there are multiple quotes, the values from the `Primary Quote` (Quote) will be pushed to the opportunity. If there is not a primary quote, this values can be manually entered.
   * No Quotes
      * Sales-Assisted - All Types: If there are no quotes, the value will be null and can be manually entered.
      * Web Direct - New Business or Renewal: This value will be hardcoded with `12` months since all web direct opportunities are 1 year in length.
      * Web Direct - Add On Business: This value will take the `End Date` (Subscription) `- Start Date` (opportunity created date).
5. MRR (Monthly Recurring Revenue) is a value that is captured based on certain scenarios:
   * Single Quote
      * For New Business or Renewals with a single quote, this value will be populated via the `MRR` field on the Quote object.
      * For Add-On Business with a single quote, this value will be populated via `Delta MRR` field on the Quote object.
      * Multiple Quotes: If there are multiple quotes, the values from the `Primary Quote` will be pushed to the opportunity. If there is not a primary quote, this values can be manually entered.
   * No Quotes
      * Sales-Assisted: If there are no quotes, the value will be null and can be manually entered.
      * Web Direct- New Business or Renewal: MRR will be the `Amount/12`
6. Start Date varies by type and is captured based on certain scenarios:
   * Single Quote: for all types of business with a single quote, this field will be populated via the `Start Date` field. For new business or renewal, this will be the date that the new or renewal subscription starts, respectively. For Add-On Business, this will be the start date of the amendment.
   * Multiple Quotes: If there are multiple quotes, the values from the `Primary Quote` will be pushed to the opportunity. If there is not a primary quote, this values can be manually entered.
   * No Quotes
      * Sales-Assisted: If there are no quotes, the value will be null and can be manually entered.
      * Web Direct- New Business or Add-On Business: For new web direct purchases, the `Start Date` will be the `Created Date` of the opportunity
      * Web Direct- Renewal: For web direct renewals, the `Start Date` will be the `Term End Date` + 1 of the subscription.
6. End Date is a value that is captured based on certain scenarios:
   * Single Quote
      * For New Business or Renewals, this field will be populated via a workflow that will take the End Date from the `Start Date + Opportunity Term`.
      * For Add-On Business, this field will be populated via the `Term End Date` on the Quote object.
   * Multiple Quotes: If there are multiple quotes, the values from the `Primary Quote` will be pushed to the opportunity. If there is not a primary quote, this values can be manually entered.
   * No Quotes
      * Sales-Assisted: If there are no quotes, the value will be null and can be manually entered.
      * Web Direct- New Business and Renewals: Since all web direct purchases are for 12 months, the End Date will be calculated taking the `Start Date + 12 months`
      * Web Direct- Add-On Business: End Date will be taken from the `Term End Date` on the Subscription object.

If a quote is sent to Zuora, the values from the Quote will overwrite any values on the opportunity, regardless of whether the quote is primary or not. If there are discrepancies between any of the values, such as the MRR, Amount, or Start and End Dates, please contact Finance or Sales Operations to resolve. We will either need to make amendments to the subscription or manually override the value in the Opportunity.

### How to Handle Duplicate Accounts and Opportunities from Web Direct Purchases

In some cases, a prospect or customer that is currently engaged with an AE on an opportunity might be proactive and sign up online via the web portal. If this occurs, then a duplicate Account, Opportunity, and Contact could be created. In the event that a duplicate record is created, please do the following to resolve as we want to keep the original lead source, activity history, and other information from the original opportunity:

1. Go to the original opportunity owned by the sales rep.
2. In Chatter, send a note to the SDR Manager and @sales-ops that this opportunity should be updated to Closed Won. Also, provide a link to the web direct opportunity.
3. Sales Ops or the SDR Manager will do the following on the web direct opportunity:
   * Remove the `Sales Accepted Date` and `Sales Qualified Date`, but only if these dates are for the current month. **Please do not update if this is in the past since this opportunity was already counted as an SAO or SQO for a previous period.** If either the Close Date, Sales Accepted Date or Sales Qualified Date are from a previous month, we must create a refund opportunity, which is described below.
   * Change the Stage from `Closed Won` to `10-Duplicate` (if you do not perform the first step, you will run into a validation rule).
4. Now go to the original opportunity worked by the Sales Rep.
   * Change the Stage to `Closed Won`.
   * Change the `Start Date`, `End Date`, and `Opportunity Term` to match the values from the web direct opportunity.
   * Make sure the `IACV`, `ACV`, and `Amount` values are the same.
   * Save the record.
5. If the web direct opportunity resulted in a duplicate accounts, please do the following:
   * Open both accounts in multiple tabs. 
   * Make sure the account name is the same for both opps.
   * Go to the Account Home tab in Salesforce and merge the accounts.
   * When selecting the values on the final account, make sure to select the values for MRR, count of active subscriptions, support level, and other subscription related values from the account associated to the web direct opportunity. This information is being pulled from the Subscriptions, which only exist on the account from the web direct opp.
   * Merge the accounts.
   * Chatter @deal-desk to update the CRM ID in Zuora so that the connection between these systems remains in tact.

If the prospect is still a Lead record that has not converted into an Account, please complete the following steps:

1. Go to the Lead record and convert it into an account, contact, and opportunity as you normally would any qualified opportunity.
1. Then follow Steps 1-4 in the previous section.

### Closing Deals for GitLab.com

* The Sold To contact should match the email used on the GL.com account.
* The customer then needs to reset their password on the subscription portal.
* Once they are logged in the portal, the customer can click on the `Update` button of the subscription card.
* The customer needs to pick one of their Groups that were fetched from GL.com and proceed to update the subscription.
* Finally, the customer should then be able to see the right plan for their group on their GL.com account.

### Closing Deals for GitHost

 * Confirm with client the best contact for installation, the type of plan, and how many paid users will be needed, then create quote.
 * When the quote is created, the system will automatically add the GitHost Subscription Terms to the quote in addition to the GitLab EE Subscription Terms.
 * Once quote is singed, send to zbilling
 * Once sent to zbilling there will be an automated email that goes out to support@gitlab.com alerting the support team to contact the client to connect their GitLab EE license key with the GitHost instance
 * A second email will be sent to the client with the GitLab EE license key and the process will be complete

### Closing Deals for Educational Institutions receiving educational pricing

 * The customer should purchase a license as normal through Zuora, except that the number of users purchased should only include non-student users (as described in [Educational Pricing](/pricing/licensing-faq/)).
 * After the customer purchases the license, the account executive then manually creates and sends a license that includes the total number of users, where `total # of users = students + non-students`.

### View and download invoices in Salesforce

 As soon as an invoice is generated, the sales rep can view and download it as a PDF in Salesforce. Scroll to the bottom within the Salesforce-Account and click on the invoice number under "Invoices". Then on the bottom of the invoice view, click "Invoice PDF".

 A paid invoice will have a zeroed Balance and positive Payment Amount.

## Returning Customer Creation Process(Upgrade/Renewals/Cancellations)

1. Create an Opportunity for an [Add-on or Renewal](/handbook/sales/#opportunity-types). If a cancellation, click on Opportunity they want to cancel.
1. Click on New Quote button within the opportunity.
1. Since this is a returning customer, sales rep will see a screen showing the current subscription.
1. This screen determines that this customer is already established in Zuora and will allow the sales rep to perform on the 4 actions.

### Updating Subscription for the account

1. Amend existing subscription for this billing account
2. Renew existing subscription for this billing account
3. Cancel existing subscription for this billing account

#### New Subscription for the account

1. This will allow the Sales rep to create a [new subscription](/handbook/sales/#opportunity-types) for the existing billing account.
1. Clicking on Next will take the sales rep thru the same Quoting flow that was seen the new Quote creation process

#### Amend existing subscription for the billing account

1. This process is used to perform any [upgrade to a subscription plan or add-on of additional seats t same subscription](/handbook/sales/#opportunity-types)on an existing subscription.
1. Choosing “Amend existing subscription for billing account”, will allow sales rep to perform amendment to an existing subscription.(Upgrades)
1. Clicking on the this radio button will list all subscriptions that are tied to the customer
1. Click to choose the subscription for performing an Amendment and hit on Next button

Note: In the case of multiple, back-to-back amendments/add-ons affecting the same subscription, the first amendment/add-on opportunity must be Closed Won (and the quote must be sent to Zuora) prior to the creation of an additional amendment/add-on. If an amendment/add-on is created prior to the closing of a previous amendment/add-on to the same subscription, Zuora will combine the delta amount for both quotes into the second amendment quote's subtotal, resulting in an incorrect order form.

#### Cancel existing subscription for the billing account

1. This process is used to cancel an existing subscription. (Note that if a customer purchases seats for the wrong billing account, please see the next section.)
1. Click on Opportunity to cancel.
1. Click on New Quote
1. Since this is a returning customer, sales rep will see a screen showing the current subscription.
1. Choosing “Cancel existing subscription for billing account”,
1. Clicking on the this radio button will list all subscriptions that are tied to the customer
1. Click the subscription for performing a cancellation and hit on Next button
1. Select cancellation date and click Next Button.

#### Cancel an erroneous subscription for the billing account

1. This process is used to cancel an erroneous subscription.
1. For example, a customer may purchase additional seats or products via the web portal which was originally intended as on add-on to an existing subscription.
1. Provide Finance or Sales Operations with the erroneously created Zuora Subscription ID, invoice number and the correct Zuora Subscription ID.
1. Finance will cancel the subscription and either refund the invoice (if a credit card purchase) or cancel the invoice (if check or other payment method).
1. Finance will then amend the correct Zuora Subscription ID and will either charge the card on file or send the invoice via email.

### Changing the Sold To or Bill To Contact

If the customer wishes to change the contacts for either the license (Sold To Contact) or the invoice (Bill To Contact), then:

1. Add the new recipient as a Contact to the Account;
2. Choose the new Contact for the Sold/Bill To Contact;
3. On the Quote Detail screen, select 'Update Zuora Account Details'.

### Zuora Supporting 4 types of Amendments 

1. Terms and Conditions amendment – The sales rep will be able to change the terms and conditions of an existing subscription;
1. Remove product Amendment – The sales rep will be able to perform a Remove a product Amendment;
 * In this case, sales rep will have to Set the Start date (Contract effective date in Zuora terms) when the remove product amendment should happen
 * Click on Next
 * This will take them to the product selector page and displays the original product that was purchased within the subscription
 * Sales rep can now remove the product
1. Add product Amendment – Sales rep can add a new product from the product selector page
1. Update Product Amendment – Sales rep can update the existing product of the existing selected product
 * Note: Do not change the Terms and conditions unless you are performing a terms and conditions amendment(except for start date).
       Let's take an example - Let's say a customer once to add more seats to their license.
       1. Set the start date
       1. Change the quantity field to reflect the new total number of seats
         * Hit on Save
1. If you want to change the Payment Terms on an add on quote, you must contact the Billing Team to make this change as Zuora does not allow this value to be changed from within Salesfore. Zuora assumes the same payment term used for the original opportunity will be used for the amendment. However, Billing can change this in Zuora if needed.

Once on the Quote Summary, will click on generate PDF to generate a Quote PDF
Send it to the customer - only if there is no record of a signed quote. If customer purchased online, they agreed to our terms and condition, so no need to have them sign a quote. It is ideal though.
Upon Sign-off, or existing signed quote, click on the Send to Z-billing button to send the Quote over to Zuora

#### Renew existing subscription for the billing account

1. This process is used to perform Renewal on an existing subscription; this is only created if the AUTO RENEW Flag is set to “NO” for a subscription initially.
1. Choosing “Renew existing subscription for billing account”, will allow sales rep to perform Renewal to an existing subscription;
1. Clicking on the this radio button will list all subscriptions that are tied to the customer
1. Clicking on next will take the sales to the Create Renewal Quote page
1. Sales rep will select the renewal Quote Template from the list
1. Enter the Renewal term in months
1. Will hit on Next
1. Skip the product selector page, unless want to update the QTY or want to add a new product
 * if they are adding more seats, change the quantity field to reflect the new total number of seats
1. Once on the Quote Summary, will click on generate PDF to generate a Quote PDF
1. Send it to the customer, via Sertifi button within Zquote screen
1. Upon Sign-off will click on the Send to Z-billing button to send the Quote over to Zuora
1. Close Won the opportunity

#### Renew existing subscription with a "true-up" for the billing account

1. This process is used to perform a Renewal on an existing subscription and to add a one time charge for true up; this is only created if the AUTO RENEW Flag is set to “NO” for a subscription initially.
1. Choosing “Renew existing subscription for billing account”, will allow sales rep to perform Renewal to an existing subscription;
1. Clicking on the this radio button will list all subscriptions that are tied to the customer
1. Clicking on next will take the sales to the Create Renewal Quote page
1. Sales rep will select the renewal Quote Template from the list
1. Enter the Renewal term in months
1. Will hit on Next
1. On the product selector page, add the true up product
 * enter the number of seats they will true-up. Add in the price of the seat, 100% of price they paid.
1. Next, update their current subscription to reflect the new total number of seats they will be renewing for which will be equal or greater than the amount they had with their subscription plus the true up amount.
1. Once on the Quote Summary, will click on generate PDF to generate a Quote PDF
1. Send it to the customer, via Sertifi button within Zquote screen
1. Upon Sign-off will click on the Send to Z-billing button to send the Quote over to Zuora
1. Close Won the opportunity

#### Amendments with Two Different Prices on the Same Product

If you are amending an existing subscription with an old product (eg, GitLab Starter) at the previous rate ($39) but are adding additional seats at the new rate ($48), you will need to add a second line item on the quote for the new rate plan (Starter). For example, you have a customer currently with 50 seats at $39, and you'd like to add another 50 seats at $48, your quote will look like this:
 * GitLab Starter, quantity: 50, unit price: $39, total price: $1,950.
 * Starter - 1 Year, quantity: 50, unit price $48, total price: $2,400.

#### Provisioning Licenses for Subscriptions with Two Different Prices for the Same Product

Once this opportunity is Closed Won via the approval process, you will send the quote to Zuora to create the subscription and invoice. However, since the licensing application only looks at one line item as the quantity for provisioning, it will not take the actual number of licenses that the customer purchased. If use the previous scenario as an example, although the customer purchased 100 seats, they will only be provisioned 50 seats. You will need to create a new license in the license server for the appropriate number of seats. If you aren't familiar with how to create a license manually, please contact Sales Operations.


### Subscription Types and Opportunity Type Validation Rules

The following Subscription Types (New, Renewal, Amendment) must match the corresponding Opportunity Types (New, Renewal, Add On) in Salesforce:

* New Subscription = New Business
* Amendment = Add On Business
* Renewal = Renewal Business

If you attempt to create a `New Subscription` when the Opportunity Type is `Add On Business` or `Renewal`, Salesforce will reject your request unless you obtain approval from Finance or Sales Operations. A major reason for this is because of churn considerations, as creating a new subscription instead of amending the existing subscription will cause this subscription to count towards our churned metrics. With approval, Sales Ops and Finance are made aware of the special circumstance and can make any adjustments needed to ensure the transaction will not count as churn.


### Assistance with Quotes

If your quote contains any of the following special circumstances, or if you have questions regarding basic quotes, you are encouraged to send a Chatter message to "@deal-desk" on the Account or Opportunity record. Please provide as much detail as possible, including links to relevant records, dates, user counts, and other useful information.
* **Contract resets:** If the customer wishes to reset their terms in the middle of their term (for example, they want to upgrade, but want to reset their term for another 12 months), you will need create a new subscription. In this case, the Subscription Type will be 'New' while the Opportunity Type will be 'Renewal'.
* **Co-term of multiple subscriptions:** If the customer has multiple groups and wishes to consolidate their subscriptions, an "Amendment" may be created against a "Renewal Business" opportunity.
* **Splitting out a single subscription**. Conversely, there may be times when a customer needs to split their single subscription into multiple subscriptions. When this occurs, the Subscription Type and Opportunity Type will be 'Renewal'.
* **Ramped Pricing:** If the prospect or customer would like to employ a ramped pricing schedule where they may want to increase their user count over time. Two examples of ramped schedules include:
  * Year 1 will be for 100 users and year 2 will be for 200 users.
  * Year 1 will be $45 per user per year and year 2 will be $48 per user per year.

### Co-Terming

Co-terming is when a customer wants to align two or more subscriptions with different end dates.

Example:

Customer has 2 subscriptions for Premium.

* Subscription 1 = 100 seats, expiring 2018-06-30
* Subscription 2 = 50 seats, expiring 2018-12-31

The most likely scenario is to co-term into the subscription ending last:

* On the renewal opportunity for subscription 1, create an amendment quote for subscription 2;
* The start date for the amendment will be 2018-07-01;
* Add 100 seats to the existing 50 and close as usual;

The other scenario is co-terming into the subscription ending first:

This requires two steps: first combining the subscriptions, then cancelling the leftover one.

* Create a new opportunity, with a quote amending subscription 1;
* The start date will remain unchanged, e.g. 2018-04-01;
* Add 50 seats to the existing 100 and close as usual;
* Once closed, create a new opportunity to cancel subscription 2 on the day before the start date of the previous quote e.g. 2018-03-31;


#### Tracking Churned Subscriptions and Opportunities

The following events will trigger require the Churn Information to be completed on the opportunity record:

* An opportunity has been submitted for approval with a negative amount. This signifies either a credit or refund of a subscription was requested by a customer and processed by an Account Executive or Account Manager.
* A renewal opportunity has been won, but has a negative IACV. This signifies that the customer has downgraded. Sales Operations and Finance will reach out to the opportunity owner to understand the nature of the churn.
* A renewal opportunity has been lost. This signifies that the customer did not renew their subscription. Sales Operations and Finance will reach out to the opportunity owner to understand why the customer did not wish to renew.The following information will be captured:

When one of the above conditions are met, the user is responsible for entering the following details on the Churn Information of the opportunity record:
* Churn Type will capture the nature of the downgrade/non-renewal:
  * **Credit** is used when a customer will receive a refund to their account. This mostly happens when a customer resets their subscription term and the unused portion of their subscription is credited back to them.
  * **Edition Downgrade** is used when a customer downgrades to a lower paid package (from Premium to Starter). If a customer is downgrading from any paid packages to the Community Edition, this would be considered a Non-Renewal as they are no longer a paying customer.
  * **Non-Renewal** is used when a customer requests to cancel their subscription upon renewal, either to the Community Edition or to a competitor. Note that we have increased the grace period after the end of a subscription before we consider it as an official non-renewal from 15 days to 75 days. Any subscription that has not been resolved after 75 days must closed as a lost renewal. However, should that customer return at any point in the future, it will be considered a renewal, and we will merely have a gap in our revenue recognition for that customer.
  * * **Removed Product** should be used when a customer removes a product from their subscription.
  * **Price Per User Downgrade** is used when a customer renews with the same product, but the per unit price is discounted.
  * **Seat Reduction** is used when a customer reduces the number of seats from the previous year at renewal.
  * **Termination** should be used when a customer cancels their subscription mid-term.
* Churn ACV: The annual contract value that was lost.
* Churn Month: The month that the churn occurred. This should be the Close Date.
* Churn Notes: Open text field to capture any additional notes regarding the churn. If the customer has provided specific reasons for churn, please enter them into this field. Please try to find out the underlying reason for the decrease in ACV. If they are reducing the number of users, did they not realize adoption? Did some users move to a different solution? Did they overbuy? If they are downgrading from one edition to another, are they not using the features in the higher edition? Do they feel the features do not justify the cost difference?


## Creating a Quote for an Authorized Reseller Partner

A reseller quote has a few different things than a regular quote:

* Before you generate a quote for an authorized reseller, make sure to go to the reseller's account record in Salesforce. In the Account Detail section, enter the Payment Term (30, 60, etc) that has been agreed upon between GitLab and the reseller. Make sure to only enter the numeric value and not "Net 30" or "Net 60". This value will appear in the Quote document in the Terms section.
* Quote Name Field: append “via reseller name” to the Quote name (i.e.: “Quote for Federal Reserve via ReleaseTEAM”)
* Quote Template: Needs to be a reseller template, such as "Reseller New Quote" or "Reseller Amendment Quote". Since resellers cannot accept terms for their customers, the reseller template contains different language around acceptance.
* Sold To Contact and Bill To Contact fields both need to be a person at the end customer. This is who will accept the EULA.
* Invoice Owner Field: This needs to be the resellers account. If you do not see the reseller listed, then you need to send the SFDC URL of the reseller’s billing contact to finance and for an Invoice Owner record to be created.
* Invoice Owner Contact: This is the Bill To Contact for the reseller. This is important as the Bill To Contact's account record will populate the GitLab entity, and all information related to that GitLab entity (Entity Name, Entity Contact Info, Entity Banking Information, and Entity Beneficiary Information).
* Click Through EULA required: Set this to Yes. This will cause a URL to be sent to the customer via email where they agree to our Terms and Conditions before getting their license key. This is important as a reseller cannot agree to terms on behalf of the end user.  Alternatively, the reseller could obtain a physical signature and send it to you.
* Discount: Authorized resellers all have pre-defined discounts depending upon the market they serve and the services they provide to GitLab.  GitHost is never discounted as our margin after paying Digital Ocean is very small.  We do not give discounts to fulfillment houses like SHI, Insights, or other resellers that are not authorized resellers. Reseller discounts can be found on the first page of the [Resellers List](https://docs.google.com/spreadsheets/d/1tQjPMRUuzsDR4mNj74aY-W8jBQH4u9h7PpEsw088Zx0/edit#gid=1395032632)
When in doubt please consult the reseller team.

## Using Customer Form Agreements and Negotiating GitLab's Standard Agreement
{: #CustomerFormAgreements}

Our experience shows that using a prospect's form agreement is expensive and, more importantly, time consuming. Deals in which we use the customer agreement take on average 60 days longer to close than if completing using our standard subscription agreement with changes as requested by customer counsel.  The arguments in favor of using our agreement are as follows:

1. Our agreement is an annual subscription agreement with a true-up whereas customer form agreements typically are based on paid up licenses.
1. We are an open source company and our agreement provides licenses for both the CE version of the product and the EE version as well as dealing with contributions of code from our customer.
1. We have non-standard but customer favorable warranty and acceptance provisions.

Despite the overwhelming arguments in favor of using the GitLab form some prospects insist on using their form agreement. GitLab will accommodate such requests with the following assumptions:

1. GitLab must have been selected as the solution of choice by the customer.
1. The deal must be in excess of $100,000.
1. The primary decision maker must indicate their willingness to facilitate the internal process in a manner that brings issues to closure within 30 days of negotiations. The decision maker must also acknowledge that they understand that the form agreement may require significant revisions based on what is described in the above section.
Items 1 and 3 above must be acknowledged in writing prior to proceeding with the contract markup.

GitLab will not accommodate changes to our standard forms for deals under $25,000. 

## Handling OSS and EDU Inquiries

With GitLab's announcement that our Ultimate and Gold packages will be free for Education institutions or organizations developing  open-source software projects, we are implementing the following process with the Community Advocacy team owning many steps in this program. The process from initial inquiry to delivering a license key will be as follows:

### Inquiry and Application Process (Leads)
1. The Community Advocate team will receive inquiries from interested organizations. These inquiries will initially be bulk uploaded into Salesforce. Eventually, these inquiries will be created manually as they come in via a web capture form, manual entry, or other sources (Contact Us, trade shows, etc).
2. If an existing lead is interested in taking part of the program, the lead must be reassigned to the Community Advocate user in Salesforce. When reassigning, be sure to notify the team by clicking the "Send Notification to New Owner" checkbox.
2. The Community Advocate team will search Salesforce for the lead record via email address. During the application process, First Name, Last Name, and Address information must be captured. We should also include notes on whether they are interested in Ultimate or Gold, and if they want support or not.

### Approved Applications and Opportunity Creation
1. When an application is approved, the Community Advocate team will convert the Lead into an Account, Contact, and Opportunity.
2. The opportunity name should be `CompanyName-Source Product NumberofUsers`, eg, "ABC University-Ultimate (EDU or OSS) 25" or "ABC University-Gold (EDU or OSS) 500 w/ Support"
3. Type is "New Business"
4. The Close Date should be a future date (as a general rule, it should be the date you expect the signed agreement from the organization). If you are unsure, you can set this date to the end of the current or next month.
5. Stage should be "0-Pending Acceptance"
6. Click Save.

### Quote Creation and Product Selection
1. To create a Quote for this organization, click on the "New Quote" button
2. Select the Account you'd like to associate to Quote to
3. Select "New Subscription for this Account"
4. Click "Next"
5. In the Quote Template, select "Ultimate or Gold Free (OSS Only)" for OSS organizations and "Ultimate or Gold Free (EDU Only)" for educational institutions (the difference between the templates is because of an additional addendum for EDU)
6. Click "Primary"
7. Add a Sold to and Bill To Contact
8. Enter the Start Date
9. Enter the Initial and Renewal Term of 12 months
10. Disable Auto-Renew
10. Uncheck "Click-through EULA required?"
11. If Tax Exempt and they want to purchase Support, make sure to ask for a Certificate ID so that there is not tax added to the Support cost. Not all organizations that opt for the free Ultimate or Gold will be tax exempt. If they are just signing up for  the free plan, there will be no tax so you can skip this step.
12. Click Next
13. Click on the Select pull down
14. Click "Add Base Products"
15. Look for either Ultimate or GitLab.com (Gold Plans are listed under this product)
16. Look for plan you'd like to add and click "Select Plan".
17. Click Save
18. Enter the Quantity (number of seats)
19. Click Submit

### Quote PDF Creation and Delivery
1. Click on the Generate PDF button. A new window will appear. Please wait until you receive confirmation that the Quote has been successfully created before closing the window, otherwise your quote PDF will not be created.
2. Go to the Sertifi eSign button
2. In the Email Invite Message, add a few sentence notes to the contact
3. Confirm the email the quote will be delivered to
4. Click Next
5. Go to the Related Notes and Attachments pull down and select your Quote
6. Please wait for the quote PDF to load. You will see a green box titled "Signature Documents Added". It is recommended you click on the "Preview/Prefill Document" link before you deliver the quote to the organization. You can verify the data on the order form is correct.
7. Send for Signature

### Opportunity Approval
1. You will receive a notification once the quote has been signed. Go to the opportunity in Salesforce
2. Confirm that the signed document is in the Notes and Attachments section of the Opportunity. If it is not, you can attach the document
3. Change the Stage to 6-Awaiting Signature
4. Click on the Submit for Approval button
5. You will receive an email if the opportunity was approved or rejected. If rejected, you will receive reasons why. Please resolve these issues and re-submit the opportunity for approval
6. If the opportunity was approved, it will automatically be changed to "Closed Won" and the Close Date will be updated to the date the opportunity was approved. Also, a renewal opportunity will be created.
7. The Deal Desk team will send the quote to Zuora. This will trigger the delivery of the license key to the organization.
8. Create a reminder to reach out to this customer in 11 months time to start the renewal process. This may require adding seats if their organization has grown.

## Using Cases in Salesforce

A Case is a question or feedback from a prospect or customer. While there are many ways that a customer can reach out to GitLab, the following are the only email addresses that will create a Case in Salesforce. If the Case submitter is an existing Contact in Salesforce, the case will be associated to both the Contact and Account record, and will be assigned to the Contact owner. If the Case submitter is not an existing Contact in Salesforce, please see below who the case will be assigned to.

* Sales@: this is an inquiry from a prospect requesting information on GitLab's services. These inquiries will create cases in Salesforce in the [SDR Queue](https://gitlab.my.salesforce.com/500?fcf=00B610000042ioq) and will be handled by the SDR Team. The inquiries are routed to the appropriate team per the rules outlined below. This email is in process of being deprecated.

#### New Business Inquiries

All new business inquiries will be handled by the SDR team. However, if an inquiry comes in for an account owned by an AE - Mid-Market or above or SAL, these will be treated similar to `Contact Us` requests and routed to the named account owner. Before the case is reassigned, the SDR will search Salesforce for a matching record:
  * If a matching record exists, both the Case and record will be reassigned to the SAL/AE - Mid-Market or above. The new owner will be notified upon reassignment.
  * If a record does not exist, the Case will be reassigned to the MMAE+/SAL and the new owner will be responsible for creating a LEAD record.

#### Existing Customer Inquiries

Existing customer inquiries should be routed based to the appropriate team based on the inquiry:

* Contact Us form is submitted where it is an existing customer inquiry;
* A case is created;
     * If the contact AND email address exist in SFDC, it will be assigned to the Account Owner;
     * If the contact AND email address does not exist in SFDC, it will be assigned to the Account Management Queue;

Working the Account Management Queue
* Work through any cases in your name and close once completed;
* To encourage all users to view this queue, Cases will not be directly assigned to the new user, but instead, two things should happen:
     * The account should be associated to the Case. This will then add the Account Owner field to the Case object.
     * This field will appear on the list view.
* If you see any in the queue that have an Account Owner, but have not yet been assigned, transfer them to the Account Owner and choose to Send Notification Email;

Each user will be responsible for checking Cases throughout the day to resolve their open cases.

* If finance related (refunds, invoice requests, payment method updates, remittance, etc), re-assign the case to Cristine or Anna;
* If support related, forward to support and close case;
* If missing license key, go to [license app](https://licences.gitlab.com) and re-send key;
* If bounces, you must contact the Account and find a new billing contact as the bounce is most likely coming from Zuora renewal notifications address to the Bill To email address. You will be responsible for updating the billing contact as part of renewing the customer.

Replying to CASES assigned to you:

* Using your GitLab Gmail account:
     * You will need to copy the Case Thread ID to both the subject AND body of the email.
     * You will still be responsible for closing the case.
* Using the Case Thread functionality
     * within the Case object using your GitLab Gmail as the From address.
     * You will need to keep renewals@gitlab.com in the “Additional To” field.
     * If you do not do this, the emails will not be associated to the Case Thread. However, if you send from your GitLab Gmail account, it will be associated as an activity in your Activity History as long as you have Outreach configured correctly.

For adding student users to an existing license key:
1. Request proof of purchase from educational institution for staff users, which will either be an invoice or the signed order form
1. Open the license app and duplicate the license adding the amount of extra seats for students
1. The new license is sent automatically, but the best practice is to attach license to a follow-up explainer email. (Also clarify that they are not entitled to Gitlab technical support)


#### Purchase Order (PO) Fulfillment from a Reseller

In some cases, a reseller may send a purchase order for order fulfillment. When this happens, the following steps will be taken by the SDR:
1. Search Salesforce for the related account and opportunity. Once found, the email will be forwarded to the opportunity owner.
1. Reassign the Case to the Opportunity Owner.
1. Go to the Type field and select `PO Delivery`.
1. Go to the Status field and select `Closed`.
1. Click Save.


### Accessing Cases

The primary ways to access Cases in Salesforce:

1. Cases display in a Cases related list on the Account, Contact, or Opportunity record. This is best when you are looking for Cases assigned to a specific Account or Contact.
2. You can go to the Cases tab in Salesforce, then select My Open Cases (or any other list view available). This is best when you are looking for Cases either assigned to you or your group. It is a good practice to review cases assigned to you at least a few times a day.
3. You can use the Console tab in Salesforce (if unavailable, it can be added by clicking on + to see All Tabs, and then selecting `Customize My Tabs`). This view allows you to view the Cases List and Content in the same window.

### Working Cases

1. You may be assigned a case that is not associated to a Contact or Account. This happens because the person who submitted the case is not an existing record in the system.
1. When this occurs, a best practice is to create the contact, then associate the Case to that contact.
1. Also, it is a best practice to associate the case to the Account, so that when you, or another team member access the account, the case will be visible to all team members.

### To work with Email-to-Case or On-Demand Email-to-Case emails

* Click Send An Email to send an email to a contact, another user, or any other email address.
* Click Reply to respond to an email. The email response automatically includes the email body as received from the customer. Enter your response and click Send.
* Click To All to respond to all participants on an email thread.
* The email address of the contact who created the case automatically appears in the To field, as long as the creator is an existing contact. To add more recipients, click Lookup icon to look up an address, or type or paste email addresses or names in the To field.
* When you enter an email address or name that matches one contact or user, the address appears as a button with the person’s name.
* To add several addresses at once, copy and paste them separated by spaces or commas. These email addresses appear as buttons, and, if they’re associated with a contact or user, show the contact’s name.
* When you enter an email address that matches multiple contacts or users, the address appears as a button. Clicking the button brings up a list of people associated with the email address so you can choose the one you want to associate with the message.
* If you need to copy other people on the message, click Add Cc or Add Bcc.
* By default, the email subject is the name of the case it’s related to. You can edit the subject if you need to.

* Click the subject of the email to view the email. From the email, you can reply to the sender, reply to everyone, forward the email, or delete it.
* While viewing an email, you can display a list of all the emails associated with the case by clicking Email Message List, and you can navigate to the case's other emails by clicking Next or Previous.
* While viewing an email, click Forward to forward it. The email automatically includes the email body as received from the customer. Optionally, enter text and click Send.

### Closing a Case

* Before closing a case, make sure that the account is associated with the case
* Choose the case reason before you close

## Process after you close a Premium Support Subscription

Once you close a deal that includes Premium Support, you need to:

1. On the account object in Salesforce, check the **Support Level** in the _GitLab Subscription Information_ section, so that it carries through to Zuora and Zendesk.
2. Notify the Customer Success team there is a new Premium support customer, by creating an issue on the [Customer Success](https://gitlab.com/groups/gitlab-com/customer-success/-/issues) project using the _Premium support onboarding_ template. Be sure to include all parts of the issue:
   - Name of organization
   - Domain name, and optionally named individuals that are most likely to submit support tickets
   - Link to the SalesForce record.
   - Mark the issue confidential!
   
## Eval users SKU creation

In order to have the Eval users SKU created:

1. Submit your request via an issue in the Finance issue tracker.
1. Submit to CFO, CRO and CEO for approval.
1. Once approved, submit to Accounting to create SKU in Zuora (Eval users SKU should not be added to the portal).
1. Once SKU is created, inform Sales Ops team to have the SKU created in SFDC and added to the current SKUs.

Eval users SKUs are subject to the discount authorization policy.

Booking:

1. All orders with mixed SKUs must be reviewed by revenue accounting for a fair value analysis prior to being sent to Zuora. Seek approval via chatter.
1. If fair value must be allocated differently than what will be on the invoice that value will be assigned on an order form and used for the entry to be pushed to Zuora. The fair value will also be used for assigning booking value (i.e. IACV, PCV, etc).

## Creating Order Forms for Add-ons to multi-year Subscriptions

Where annual payments were approved for multi-year subscriptions, the add-ons to these orders will be created for the whole duration of the subscription and should indicate the full payment, 
e.g.: 
1. 2020-07-01 - 2021-01-31 - 5700 USD (pro-rated)
1. 2021-01-31 - 2022-01-31 - 11400 USD (full)
1. 2022-01-31 - 2023-01-31 - 11400 USD (full)





