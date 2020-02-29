---
layout: handbook-page-toc
title: "Business Systems: Portal Analysis, Integrations, and Flow"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Contact

* [Business Systems Analyst \| Jamie Carey](/job-families/finance/business-system-analyst/)
* [Product Manager, Fulfillment | Amanda Rueda](/job-families/product/product-manager/)

| [Growth Group](https://about.gitlab.com/direction/#growth-groups) | Request Type |
|:------:|:-------:|
| [Acquisition](https://about.gitlab.com/direction/acquisition/) | new biz |
| [Conversion](https://about.gitlab.com/direction/conversion/) | trials |
| [Expansion](https://about.gitlab.com/direction/expansion/) | How do I?, upgrades |
| [Fulfillment](https://about.gitlab.com/direction/fulfillment/) | purchasing issues/requests, customers portal usage, subscription management |
| [Retention](https://about.gitlab.com/direction/retention/) | renewal, getting started, license, user management |

## The Customer Portal
aka the portal, the customers' app

The customer portal is a GitLab created and managed application: there are three related applications: customers.gitlab.com, version.gitlab.com, and license.gitlab.com.

Additionally, there are two other points of sale online: via the [AWS marketplace](https://aws.amazon.com/marketplace/seller-profile?id=9657c703-ca56-4b54-b029-9ded0fadd970) and [GOV.UK Digital Marketplace](https://www.digitalmarketplace.service.gov.uk/g-cloud/services/526446644571793).

## Enterprise Application Ecosystem

The customer portal integrates with many of our other tools.
We use the label `EntApp Ecosystem` to alert other teams to what we are working on that could affect the data or operations of another team.

##### EntApp Ecosystem Boards

* [gitlab-com](https://gitlab.com/groups/gitlab-com/-/boards/1553398?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=EntApp%20Ecosystem)
* [gitlab-org](https://gitlab.com/groups/gitlab-org/-/boards/1553395?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=EntApp%20Ecosystem)

##### Team Boards

* [Sales Systems](https://gitlab.com/groups/gitlab-com/-/boards/1117318?label_name[]=SalesSystems)
* [Growth Team](https://gitlab.com/groups/gitlab-org/-/boards/1370834?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=devops%3A%3Agrowth)

##### Relevant Repos

* [Salesforce](https://gitlab.com/gitlab-com/sales-team/field-operations/salesforce-src)
* [Zendesk](https://gitlab.com/gitlab-com/support/support-ops)
* [Customers app](https://gitlab.com/gitlab-org/customers-gitlab-com)
* [Version app](https://gitlab.com/gitlab-services/version-gitlab-com)
* [License app](https://gitlab.com/gitlab-com/license-gitlab-com)

## Defined Technology Approach

##### Sales

Directly Responsible Individual James Harrison
- Clear, consistent workflows for Sales to be trained on new business and renewals.
- Clear, consistent processes on how to get self-service support or Sales support.
- Resolve: Salesforce to Zendesk synchronization problems.

##### Product

Directly Responsible Individuals  Amanda Rueda and Michael Karampalas
- Customers and Sales to be provided witheasy to read format of known bugs that are affecting the portal, what is the workaround, how to ask for the workaround to be applied to them, and what the timeline to fix is.
This should be created by Product and maintained by both Product and Support.
- Improvements to the portal’s user interface, user experience, and backend processes and integrations.
- Provide regular and clear updates to the Sales and Customer Success organizations about work in progress and upcoming work that has an impact on those customer facing organizations.

##### Support

Directly Responsible Individual Jason Coyler
- Support, triage and work the Zendesk License and Renewal queue.
- Provide feedback to teams that intersect with the portal.
- Document known bugs and workarounds in appropriate locations as identified by Product.
- Participate in single lane channel identified by Sales to request help from Support.
- Work with Sales Ops to resolve Salesforce synchronization problems.
- Create: “Support” contacts on accounts.

##### Business Operations

Directly Responsible Individual Jamie Carey
- With Business System Specialist, provide support to Sales, Support, and Product in creating interdepartmental feedback loops, workflows, and processes.
- Continue to monitor and illuminate gaps.
- Document the relationship between the customer portal and the product for Docs and Sales to provide to the customer during onboarding.
- Work with Product, Sales, and Support on a unified list of product features and functionality in prioritized order for Product.
- Work with Billing on adding dunning features into Zuora (ie notices to customer on expired credit cards on file).

## High Level Setup

##### Some Documentation

*  [video of custom setup](https://drive.google.com/drive/folders/1kfCEQM6XYGWYxq3Ke4TNvtmDR-46erVD)
*  [Security's Compliance Diagram](https://gitlab.com/gitlab-com/gl-security/compliance/compliance/blob/master/PCI/customers.gitlab.com_data_flow_diagram_-_New_Business.pdf)
*  [Growth Team's Portal Diagram](https://app.mural.co/t/gitlab2474/m/gitlab2474/1569500330861/8f9fd73826c42ad809d51be886db27494da91353)
*  [.com renewal flow Diagram](https://whimsical.com/S4r7nuRFgQ5kZKaZisZcoQ)
*  [Trade Compliance](/handbook/business-ops/trade-compliance/)
*  [Sales flow](https://drive.google.com/file/d/1nkJrsXewy1G9llV9-8k2EhineU2hyoDJ/view?usp=sharing)

### Customer Flow

<div class="center">
<div style="width: 640px; height: 480px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:640px; height:480px" src="https://www.lucidchart.com/documents/embeddedchart/d5593761-efdf-43a0-bfe5-717d787404d7" id="_OtpjB8oRZGk"></iframe></div>
</div>

### System Integrations

Important to know

* [READ ME customer portal repo](https://gitlab.com/gitlab-org/customers-gitlab-com#subscription-portal-app)
* API should send country codes ISO 2 from portal to SFDC and Marketo

<div class="center">
<div style="width: 640px; height: 480px; margin: 10px; position: relative;"><iframe allowfullscreen frameborder="0" style="width:640px; height:480px" src="https://www.lucidchart.com/documents/embeddedchart/b5a0e4b3-ff40-4685-8d21-3109696c8f64" id="0.tpYZzq.lbI"></iframe></div>
</div>

### Zuora and Salesforce

<img src="/handbook/business-ops/images/zuoraSFDC1.png" class="full-width">

##### Zuora details

* Communication Profiles: 
    * New accounts are set to `Default Profile`
    * `Silent Profile` is used temporarily when the customer should not receive notifications

## Change Management

##### Adding new SKUs

* When a new SKU is added, the Fulfillment team [must be notified thirty (30) days in advance](https://gitlab.com/gitlab-org/customers-gitlab-com/issues) with the requirements so that they can prepare the customer applications.
* When the SFDC sandbox is refreshed, the Fulfillment team is notified and the SFDC sandbox is reintegrated with the Zuora sandbox.

## Definitions of users

##### Self-managed EE

- a license holder is someone who pays for a GitLab license and manages the payments for a self-managed installation. [EULA](https://customers.gitlab.com/admin/eula), [TOU](https://about.gitlab.com/terms), [FOSS LICENSE](https://gitlab.com/gitlab-org/gitlab/blob/master/LICENSE), [EE LICENSE](https://gitlab.com/gitlab-org/gitlab/blob/master/ee/LICENSE)
- a self-managed admin is someone who manages the installation and users of a self-managed installation. [FOSS LICENSE](https://gitlab.com/gitlab-org/gitlab/blob/master/LICENSE), https://gitlab.com/gitlab-org/gitlab/blob/master/ee/LICENSE
- a self-managed user is someone who uses a self-managed installation. [FOSS LICENSE](https://gitlab.com/gitlab-org/gitlab/blob/master/LICENSE), https://gitlab.com/gitlab-org/gitlab/blob/master/ee/LICENSE

##### Dotcom

- a dotcom subscriber is someone who pays for dotcom. [EULA](https://customers.gitlab.com/admin/eula), [TOU](https://about.gitlab.com/terms)
- a dotcom user are people who can be assigned to seats that a dotcom subscriber is paying for. [TOU](https://about.gitlab.com/terms)

##### Self-managed FOSS

- a self-managed admin is someone who manages the installation and users of a self-managed installation. [FOSS LICENSE](https://gitlab.com/gitlab-org/gitlab/blob/master/LICENSE)
- a self-managed user is someone who uses a self-managed installation. [FOSS LICENSE](https://gitlab.com/gitlab-org/gitlab/blob/master/LICENSE)

## Related Documentation and Links: Licensing, Billing, Transactions

* [Customer Portal: General Issues](https://gitlab.com/gitlab-com/business-ops/bizops-bsa/general-analysis/issues/8)
* [Issue: Analysis: Licenses & Terms](https://gitlab.com/gitlab-com/business-ops/bizops-bsa/general-analysis/issues/6)
* [EULAs/TOS: As-Is + To-Be](https://gitlab.com/gitlab-com/business-ops/bizops-bsa/general-analysis/issues/3)
* [Licenses/Self Managed: As-Is + To-Be](https://gitlab.com/gitlab-com/business-ops/bizops-bsa/general-analysis/issues/4)
* [Troubleshooting: True Ups, Licenses + EULAs](/handbook/business-ops/business_systems/portal/troubleshooting/)
* [Troubleshooting subscription and licensing problems](/handbook/support/workflows/license_troubleshooting.html)
* [License documentation](https://docs.gitlab.com/ee/user/admin_area/license.html)
* [Customer Portal: Admin internal documentation](/handbook/internal-docs/customers-admin/)
* [Epic: Analysis: License and Billing Queue](https://gitlab.com/groups/gitlab-com/business-ops/bizops-bsa/-/epics/6)

## Licensing and Renewals (L&R) Queue in Zendesk

The customer portal intersects with Support, Billing, Sales, and Product primarily.
Tickets come into the L&R queue in Zendesk generally three ways, generally prioritized as low:
   - by emailing renewals@gitlab.com
   - by [opening a support ticket](https://support.gitlab.com/hc/en-us/requests/new?ticket_form_id=334487) and selecting `Help with my license`
   - by filling out the form on the [Renewals page](https://about.gitlab.com/renewals/)
The L&R Queue is a separate queue of Zendesk tickets that fall outside of the scope of customer product support; it's handled by Support by triaging the issue and rerouting the tickets to the appropriate team.
   * **Passing to Sales:** Pass tickets relating to IACV to Sales via cc to Sales in reply to ticket which sends an email to both customer and account owner. If an account is associated with the ticket, there's a ticket object in SFDC.
It's then Sales's responsibility to continue the customer interaction and the BSS closes the Zendesk ticket.
   * **Passing to Sales:** If a ticket comes in and Support is unable to determine the account owner or the inquiry is related to new business, they reach out to the SFDC chatter group `ZD-newbusiness` where the SDR Regional leads for EMEA, APAC and AMER/LATAM provide an answer.
Then Support cc's that person on the ticket and closes in Zendesk.
      * Regional Leads for SDRs: 
         *  AMER/LATAM - Mona Elliot
         *  APAC - Jay Thomas-Burrows
         *  EMEA - Elsje Smart
* **Passing to Billing:** The mechanism to pass tickets to the Billing team is to open the ticket, then change the field `form` from the value `Upgrades, Renewals & AR (refunds)` to `Accounts Receivable/Refunds`.
This puts the ticket into the Billing Team's queue which they then manage.

## Notifications

##### Notification Emails
Emails notifications are sent through Mailgun

* Reseller Notification: this email is delivered from the customers portal after the customer accepts the EULA.
   - [HAML/HTML](https://gitlab.com/gitlab-org/customers-gitlab-com/blob/5e50769b1ef64f9002ecf9b59dbba5cc24031733/app/views/customer_mailer/reseller_notification_license_sent.html.haml#L1)
   - [Text](https://gitlab.com/gitlab-org/customers-gitlab-com/blob/5e50769b1ef64f9002ecf9b59dbba5cc24031733/app/views/customer_mailer/reseller_notification_license_sent.text.erb#L3)

* Customer - Accept Terms Request: this email is delivered from the customers' portal when the EULA is required to be accepted before delivering the license.
   - [HAML/HTML](https://gitlab.com/gitlab-org/customers-gitlab-com/blob/3248ac5978678b6920d7cb755be288e312fda8aa/app/views/customer_mailer/accept_terms_request.html.haml#L1)
   - [Text](https://gitlab.com/gitlab-org/customers-gitlab-com/blob/3248ac5978678b6920d7cb755be288e312fda8aa/app/views/customer_mailer/accept_terms_request.text.erb#L4)

* Customer - License Email: this email is delivered from the license app after the license is created following the EULA acceptance.
   - [HAML/HTML](https://gitlab.com/gitlab-org/license-gitlab-com/blob/12dffa87b8b1c092b7abebc63a7aaae61528f68f/app/views/customer_mailer/license_email.html.haml#L1)
   - [Text](https://gitlab.com/gitlab-org/license-gitlab-com/blob/f8e7e146b10319640176e1cedf395c5a83c325bd/app/views/customer_mailer/license_email.text.erb#L1)