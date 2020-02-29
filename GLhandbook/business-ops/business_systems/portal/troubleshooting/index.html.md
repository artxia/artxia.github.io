---
layout: handbook-page-toc
title: "Troubleshooting: True Ups, Licenses + EULAs"
---
## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}


> * Please feel free to add more to this page
> * Join #smb_training_support on slack

## Important Links Internal
* [Board of issues that are bugs that affect the customer portal by milestone](https://gitlab.com/gitlab-org/customers-gitlab-com/-/boards/1418919?label_name[]=bug)
* GitLab Team Member (Internal Link) [Customer Portal](https://customers.gitlab.com/admins/sign_in)
    - if you need to get a login to the customers app, [open an access request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=Single%20Person%20Access%20Request) and remove all systems in the list except for the customers app row.
* GitLab Team Member (Internal Link) [License Application](https://license.gitlab.com/)
    - if you need to get a login to the license or version app, [open an access request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=Single%20Person%20Access%20Request) and remove all systems in the list except for the row for `GitLab DEV` which you will use to Oauth into the application. Make sure to save these credentials as distinct from your regular GitLab credentials.
* GitLab Team Member (Internal Link) [Version Application](https://version.gitlab.com/users/sign_in)
    - if you need to get a login to the license or version app, [open an access request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=Single%20Person%20Access%20Request) and remove all systems in the list except for the row for `GitLab DEV` which you will use to Oauth into the application. Make sure to save these credentials as distinct from your regular GitLab credentials.
* [Kyla's Quote Creation Videos](https://drive.google.com/drive/u/0/folders/1CAXWx2SSXbIIW5bmPv4Lahlv_VPYdJce)
* [Support: Common Licensing, Transaction and Billing Troubleshooting](/handbook/support/workflows/license_troubleshooting.html)
* [Sales Ops Renewal Doc - Sales Enablement 9.27](https://docs.google.com/document/d/15WKHS-LxE4c4BbZ4eNREwwH_n_DhX_Q2yzT0OYTNjh0/edit)
* [Submitting a quote](/handbook/business-ops/order-processing/#step-5---submitting-a-quote-for-discount-and-terms-approval)
* [Quote Approval instruction](/handbook/business-ops/order-processing/#quote-approval)
* [Good resource of helpful links from TAMs](https://gitlab.com/gitlab-com/account-management/commercial/triage/blob/master/LINKS.md)
* [How GitLab.com Subscriptions Work](https://about.gitlab.com/handbook/marketing/product-marketing/enablement/dotcom-subscriptions/)
* [Google doc with list of recent bugs/problems](https://docs.google.com/document/d/1OeAzXOZ0xnX-6_T2cyKRaJG1_3r5AOwRKSK2BcID00M/edit#heading=h.sm3p4ys0l14j)

## Important Links for Customers and Prospects
* Resources for Prospects who are trialing and need direction
   - [Get started with GitLab](https://docs.gitlab.com/ee/intro/)
   - [GitLab epics](https://docs.gitlab.com/ee/user/group/epics/)
* [Instructions on how to renew self-managed](/pricing/licensing-faq/#how-do-i-renew-my-subscription)
* [Customer Facing: Licensing, Renewing, and Subscription FAQ](/pricing/licensing-faq/)
* [Subscription Setup and Management (user facing)](https://docs.gitlab.com/ee/subscriptions/)

## True-Ups, Adding Seats, Users

### User Counts: True Ups, Add-ons, Users Over License

##### What is a True Up?
* [definition](/handbook/sales/#true-up)
* A true-up is a back payment for a customer going over their license count during the previous year.
We use the true-up model so that the license never becomes a barrier to adoption for the client.

##### What causes a true-up error?
We [currently charge 100%](/handbook/ceo/pricing/#true-up-pricing) for users added during the year of their subscription.
At renewal, it has become a common occurrence that our customers have miscalculated the number of true-up users required for their license.

The true-up must match the number of users over license data collected on their admin dashboard or else the license will fail to register.

Example: 

Customer purchased 10 users at the start of their subscription; during the year of their subscription, they had 12 total users in license, adding 2 additional.
Their admin dashboard would read 2 users over license.
At the time of their renewal, they will be responsible for paying for those 2 users over license in addition to however many users they want to renew for, and once paid for, those 2 users will be added to their new subscription license key.
If the true-up is not added or has the incorrect number of users over the license, the license key will not work.

The customer is always free to renew for as many users as they would like, even if this number is lower than the previous year; the true-up amount just needs to be paid for in full.

If a customer is having issues obtaining the number of licenses needed to purchase, you can [request a screenshot](https://about.gitlab.com/handbook/business-ops/business_systems/portal/troubleshooting/#screenshot-needed-for-users-over-license) from them or else access their usage ping data through the [version application](https://version.gitlab.com/).
If there is no data available through usage ping, we can conclude that the usage ping has not been enabled from the customer, and you will need to obtain this information manually.

##### Customer Question: Why is there a discrepancy between “Maximum Users” and “Users” on the admin dashboard? (self-managed)
The following users *do not* take up a license on self-managed:
- Guest users on Ultimate plans
- Blocked users who were blocked prior to the daily job which counts the users (hard to pin point this one)
- Users who are in the system but do not have access to any projects
- Support Bot
- Ghost Users

##### Customer Question: How do I add users to self-managed?
Communicate to customer
> - Navigate to the [customers app](http://customers.gitlab.com/admin) and sign in or reset the password if required
> - Go to `subscriptions`
> - Locate the subscriptions you wish to add more users to and click the button `Add more users`
> - Enter the total amount of users you wish to have (i.e. you have 50 but want to have 60, so you have to enter 60)
> - Click `Proceed to checkout` and finalize the purchase
> - You will receive amended license key afterward

## Licenses

##### What is a license?
* A license is only generated for self-managed customers or prospects.
* The license is generated by our license app and the customer will be emailed a license key.
* It is possible to generate license keys manually.
* If you need access to the license or the version applications, [open an access request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=Single%20Person%20Access%20Request) and remove all systems in the list except for the row `GitLab DEV (required for license and version access)`.
You will use the dev credentials to Oauth into the license and version apps using `login with GitLab` so make sure to save these credentials in a way to differentiate them from your other GitLab credentials.

##### What users **do not** affect counts towards license on self-managed? 
   - Guest users on Ultimate plans
   - Blocked users who were blocked prior to the daily job which counts the users (hard to pin point this one)
   - Users who are in the system but do not have access to any projects
   - Support Bot
   - Ghost Users

##### How to ask the customer for a screenshot needed for users over license
Communicate to the customer
> To help me provide better support for your renewal I'll need some more information, could you please provide a screenshot following the below instructions?
   > For Self Hosted
   > 1. Navigate to Admin Area
   > 1. Click `License` as it's shown [here](https://docs.gitlab.com/ee/user/admin_area/img/license_details.png) and send it to me
   > For .com/Saas
   > 1. Navigate to group settings
   > 1. Navigate to billing area
> If you can share the details found there under Maximum Users and Users over License, then I will be able to send a quote over to you.

##### How can I ask Support to resend a license?
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=license%20issue) using the `License Issue` template.

##### How do I change the license owner for self-managed instances with license.gitlab
> You can [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=license%20issue) and ask Support to do this.

From the license app
1. Navigate to the [license app](https://license.gitlab.com/)
1. Find the company account through the search option
1. Select their most recent license that needs to be sent
1. Scroll down to the bottom and select duplicate license
1. After duplicate license change the email address

From the customer portal
1. Navigate to the [customers app](http://customers.gitlab.com/admin)
1. Search company name
   - Click on the edit icon
   - Change the email (and name if applicable)
1. The customer needs to click on `Forgot Password` using the new email

##### When might a license be manually generated?
Licenses only apply to self managed.
*  In order to fix a problem/error: This would generally occur around a renewal after a customer tried to use the portal and entered in users counts that didn't match what the system expected.
*  In order for a customer on a subscription to trial Bronze or Silver
*  When a reseller has different discount rates for renewals and add-ons.
For this scenario, an order will be created with two lines of the same product but if a license gets automatically created in such case it will only be pulled for the first line of product and won't be complete so this requires manual license creation.
*  Licenses are sometimes generated manually when a customer has add-ons for multi-year deals.

##### Manually Generate License for a Trial or to Amend a True Up Problem
*Note: There are no license keys provided for GitLab.com subscriptions*

> You can [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=license%20issue) and ask Support to do this.

Generate Trial License:
1. Navigate to the [license app](https://license.gitlab.com/)
1. Type in customer name (exactly as it is in Salesforce) or use the domain name in their email address
1. When the license comes up, there might be one or there might be multiple 
    - Navigate to the most recent license based on `expires at` date
    - Click on the `Name`
    - Scroll down to `duplicate license`
    - Type in the correct number of users
    - Check the box indicating this is a trial 
    - Select the plan: make sure the `starts at` and `expires at` reflect the accurate dates for the trial *because we cannot retract a license* if you accidentally make the expiration date for a year from now they’ll have free access for a year
    - Add notes if you prefer
    - Click `Create License`
1. The license will automatically be sent to the email on file, and you can also download the license from that screen and send as an attachment to prospect directly.  

Generate License to Amend a True Up Problem (not for trial)
1. Navigate to the [license app](https://license.gitlab.com/)
1. Type in customer name (exactly as it is in Salesforce) or use the domain name in their email address
1. When the license comes up, there might be one or there might be multiple 
    - Navigate to the most recent license based on `expires at` date
    - Click on the `Name`
    - Scroll down to `duplicate license`
    - Type in the correct number of users or true-ups
    - Make sure the `starts at` and `expires at` dates are not changed
    - Add notes to give reference as to why you’re amending the license
    - Click `Create License`
1. The license will automatically be sent to the email on file, and you can also download the license from that screen and send as an attachment to prospect directly.

## Terms (EULAs/TOS/T&Cs)
##### Overview 
* End User License Agreement (EULA), Terms of Service (TOS), or Term & Conditions (T&Cs) will be referred to generally as "Terms" in this documentation. Terms are applicable to all customers and are required to be accepted before using Gitlab (self-managed or .com) even if it's a trial version.
**License files will not be sent until the customer accepts Terms.**
*  License Files are **only applicable to Self-Managed**

##### When are Terms required to be acknowledged?
* Customers who purchase through the portal are required to acknowledge Terms during the process of purchasing.
* Customers who purchase from Sales accept Terms when they sign the order form.
* Users who want to trial a product.

##### When do I send a EULA from Salesforce?
When do I set `Click Through EULA required` = `Yes`?
A click through EULA is used when a sales order hasn't been signed by the end customer-it must be a reseller deal that is new subscription or add-on only.

{::options parse_block_html="false" /}

<div class="center">
<div style="width: 960px; height: 720px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:960px; height:720px" src="https://www.lucidchart.com/documents/embeddedchart/e65bf3f2-cc8c-4a32-b38a-2f6966733550" id="GXuoxl-sJmj0"></iframe></div>
</div>

*  [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=EULA) for EULA problems
*  [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=license%20issue) for license problems

##### Who receives the EULA?
If `Click Through EULA` = `yes` and this is a new subscription or an add-on, the EULA will be delivered to the `sold to` email address which should be the end customer not the reseller, per [order processing instructions](/handbook/business-ops/order-processing/#step-8--sending-the-quote-to-zuora).

##### What is the difference between Terms (EULA/T&Cs/TOS) and a License?
* A *EULA (End User License Agreement)* or *T&Cs (Terms and Conditions)* are the legal agreements for the terms of use and privacy policy that customers and users must agree to before using our software.
You can read through them on our [company website.](https://about.gitlab.com/terms/)

* A *license* is a string of characters that is tied to the customer's subscription or trial that has a start and end date.
Without applying the license, the self managed software won't work as expected.
It is sent to the customer via email or available for download **after** Terms have been accepted.

> Note: The link for the customer to accept the EULA is until accepted.
After the customer accepts the EULA, the link is no longer valid.
The customer will see a 404 error if they attempt to access via EULA link after it's been accepted. 

* If the customer accepts the EULA but the license file is still not received, this is almost always an application error.
[Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=license%20issue) using the `License Issue` template.

##### How to check if a EULA has been sent? 
1. Navigate to the `Closed-Won` opportunity in Salesforce. 
2. Was this a `Reseller` opportunity that was `New Business` or `Add-On` opportunity?
If Yes, proceed to 3.
EULAs are not sent for `Renewal` opportunities.
3. Verify that the `Click Through EULA Required` dropdown was set to `Yes`.
If yes, the EULA has been sent to the customer.
The customer needs to accept the EULA before they will be sent the license.
To check where a license/EULA was sent, proceed to 4.
If this was set to `No`, the EULA was not sent.
[Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=EULA) to have a EULA resent. 
4. Navigate to the `Account Overview` page of the account that the opp is linked to.
In `Activity History` click `Show More`.
If the customer has accepted the EULA, there will be a logged activity on the close date of the opportunity titled `Your GitLab License File` - click on the link to see when and to whom the license file was sent.
The customer may need to check their junk/spam folders.
5. If there is no record of the license file in the Account Activity History, but the EULA checkbox was `Yes` on the quote object, then there was likely a system error.
[Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=EULA) to have a EULA resent.

##### How can I change who the EULA was sent to? 
Best practice is to ensure that the `Sold To` contact information is correct on the quote object before the opportunity closes.
If the contact was incorrect or the `Sold To` contact left the company and the EULA needs to be resent, [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=EULA) using the `EULA` template.

##### How do I resend a EULA? 
1. Review "How to Check if a EULA has been sent?" **before** contacting the support team. 
1. [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=EULA) using the `EULA` template.

## Trials

##### How do I request a trial for .com customer?
* Submit an issue using the `Plan Change Request` template here: https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues

##### How long do trials last? Where can I see the end date?
30 days, you can see the end date if a namespace is on a trial in the customer portal admin 

##### How do I request to extend a .com trial for a customer?
For trial extensions [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Trial%20Extension) using the `Trial Extension` template.

##### How do I request a Bronze or Silver trial for a customer?
1. [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Plan%20Change%20Request) using the `Plan Change Request` template. 
   - **NOTE**: It's not yet possible for users or GitLab employees to directly start a Bronze or Silver trial on a namespace.
   - If one is needed, have the user initiate a Gold trial and then open an issue per the above link using the `Plan Change Request` template to have the plan manually changed.
   Implementation of this feature is being discussed in [this issue](https://gitlab.com/gitlab-org/growth/engineering/issues/37).

##### Customer Question: how do I setup a gitlab.com trial?
Communicate to customer
> * Have you created a group?
> * If not, please do so; this documentation will help: https://docs.gitlab.com/ee/user/group/#create-a-new-group
> * When you've created a group try the trial again using the email associated with that group here: https://customers.gitlab.com/trials/new?gl_com=true
> * If you still run into an error please let me know and I'll have support manually upgrade your trial group.

##### Trial Users who need help
* Trial users are not entitled to access support unless they are sales assisted
* If a prospect working with Sales needs help they should email `trials@gitlab.zendesk.com` and there is no SLA

## Subscription or Plan Problems
##### My prospect is unable to apply a purchased subscription to their GitLab.com group
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Plan%20Change%20Request) using the `Plan Change Request` template.
   - **NOTE**: The issue is most likely that their group still has an active trial which must be expired manually first.
   - Open an issue using the above template to have that done.
   - This should only be necessary until an active trial is expired automatically when a subscription is applied to a namespace.
   - Keep an eye on [this issue](https://gitlab.com/gitlab-org/gitlab-ee/issues/12186) to track progress on the fix.

##### I want to change the plan of a GitLab.com user or group
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Plan%20Change%20Request) using the `Plan Change Request` template.

## Common Questions from Customers

##### Customer Question: Where can I track how many CI minutes I've used?
> For individuals on dotcom, go to the user settings and at the bottom you see `pipeline quotas` where it shows the usage.
> Group settings have a similar page, but they’ll see `Usage Quotas`.

##### Customer Question: I bought a subscription for my personal account, how can I apply it to my group?
*They just need to reassociate it with the group.*

Communicate to the customer:
> To do this: 
> - Log into: https://customers.gitlab.com/customers/sign_in using email **EMAIL**
> - Navigate to **Manage Purchases**
> - Select **Change linked group**
> - Select the desired group from the **This subscription is for dropdown**
> - Select Proceed to checkout

> Note, if there are more users associated with the group (including its subgroups and nested projects) than what is included in your subscription, you will be charged for the overage of users during this last step.

##### How do I upgrade a customer?
1. Navigate to customer’s account in [Salesforce](https://login.salesforce.com/).
1. Navigate to `opportunities` and click into most recent purchase: should be `renewal` or `new business`, *not add-on*
1. From the opportunity view, navigate and click `New Add On Opportunity`
   - This will create a new oppty for your upgrade
   - Name the oppty appropriately
   - From the new add-on oppty view click `New Quote`
   - [Amend subscription](/handbook/business-ops/order-processing/#amend-existing-subscription-for-the-billing-account)
      - add the new SKU
      - remove the old items
      - `Save`
      - Generate PDF

## Billing

##### Customer Question: I want to pay my sales assisted order by credit card, how do I do that?
Ask your customer to tag Billing Ops in Salesforce chatter on the opportunity with this request.

##### Customer Question: How can I initiate a refund or downgrade?
*If a customer requests to downgrade the product they are currently using, we are unable to process refunds within 45 days of purchase; however, we are able to downgrade their plan.*

A customer can initiate a refund themselves:

Communicate to the customer:
> You can get this charged reversed by reaching out directly to `AR@gitlab.com`
> 1. Add your invoice
> 1. Request a refund explaining that the second charge was an error purchase
> 1. You must do this within 45 days of your original purchase

> If you have additional questions, please let me know!

##### How do I initiate a refund or downgrade for a customer?
If a customer requests to downgrade the product they are currently using, we are unable to process refunds within 45 days of purchase; however, we are able to downgrade their plan.
You can initiate the refund for the customer:
   - Send an email to `ar@gitlab.com` to request a refund for the customer.
   - Include all subscription information and link to SFDC account record.

##### How does a customer pay with a credit card with a sales assisted order?
**Self-managed/self hosted**

Communicate to the customer
> * To finalize the order, please sign and date it on the second page and return all pages back to me.
> * Afterward, you will receive an automated email with the license key as well as the invoice and we will charge your credit card.

*Make sure they have added a credit card on the payment methods within the customers.gitlab.com portal.*

**.com/Saas**
Communicate to the customer
> To finalize the order, please sign and date it on the second page and return all pages back to me.
> Afterward, your group will be upgraded with new users and you will receive the invoice and we will charge your credit card.

**Make sure that the customer has created an account, *as well as a group*, in order for us to apply the subscription to their group appropriately.**

##### Customer Question: How can I do a wire transfer?
Communicate to the customer

**Self-managed:** 
      > To finalize the order, please sign and date it on the second page and return all pages back to me.
      > Afterward, you will receive an automated email with the license key as well as the invoice for the wire transfer.

**com:** 
      > Find the quote attached.
      > To finalize the order, please sign and date it on the second page and return all pages back to me.
   > Afterward, your group will be upgraded with new users and you will receive the invoice for the wire transfer.

*(No license file on .com.)*

##### Payment by credit card (new customer) e-Sertifi
1. Start within quote object *not* from opportunity page
1. Sertifi e-sign
   - Email invite message
   - Email addresss, click `next`
   - Click `related notes and attachments` and select correct quote
   - Click on `preview/prefill document`
1. Navigate on lefthand bar to `payment authorization without address`
1. Move box to right of signature field
1. `Save`
1. `Exit`
1. `send for signature`

*When they return the signed quote, no need to ping deal-desk on chatter.*

OR

*tag Billing Ops in chatter on the opportunity with this request*

## Quotes

##### What do the terms "Sold to" and "Bill to" mean on a quote? 
* `Sold To` email address is the on for which customers.gitlab.com account is generated and where the license key is sent to
* `Bill To` email address is the email address to which automatic message with the final invoice will be sent to only

##### Entity
All web direct orders are GitLab Inc.
However, say you have an upcoming renewal that will be sales assisted where the customer previously purchased web direct, if the customer is located in one of the countries where we have another entity (UK, Germany, Netherlands, Australia), the renewal quote must reflect the correct entity.
E.g. Customer in UK purchased web direct, at renewal (if sales assisted) the quote should reflect GitLab Ltd. (UK entity).
This is to make sure we ask for Tax ID or VAT ID which prevents a customer from paying tax or VAT charges.

The following image reflects how inside the quote object you can change the entity to US.
<img src="/handbook/business-ops/business_systems/portal/troubleshooting/entity.png" class="full-width">

## Checklists for quotes

##### Add-on opportunity quotes
- Do I have address on account?
- Do I have address on contact?
- What is the original entity and does it match on the add-on quote?
- Is the payment correct - CC or wire transfer?

##### Information required for normal quote
- Full company name
- Full company address
- Sold To Contact person title, name, surname, email address
- Bill To Contact person title, name, surname, email address
- Plan
- Number of users

##### Copy/paste for renewals
1. Screenshot of customer admin area
1. Sold To Contact first/last name, email address, mailing address
1. Bill To Contact person first/last name, email address, mailing address
1. Plan
1. Number of users

##### Information required for a reseller Quote
1. Reseller Name
1. Contact Name
1. Contact Email
1. Reseller Address
1. End User Company Name
1. Contact Name
1. Contact Email

## General Communications to Customers
##### Budget
Ask:
> Is there a budget that you are looking to stay within that we should be mindful when considering your use case?

## Documentation Needed
* What do I do when I get a report of a bug or a problem with the renewal or purchase process?
* What are the instructions to process a sales assisted wire transfer?