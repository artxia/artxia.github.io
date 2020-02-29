---
layout: handbook-page-toc
title: "Selling Professional Services"
---
# Selling Professional Services
{:.no_toc}

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

You can also [watch the sales enablement session](/handbook/customer-success/professional-services-engineering/sales-enablement) about how to sell services.

## Basic Workflow for selling Professional Services

There are 4 main steps for selling Professional Services:
* Step 1: Identify the right service
* Step 2: Create the opportunity in SFDC
* Step 3: Create the SOW
* Step 4: Close the opportunity

### Step 1: Identify the right service

1. SAL/ISR identifies Standard Service SKU that best meets needs of customer from the Full Product Catalog list with assistance from SA as needed
1. SAL/ISR reviews the standard services description, duration, and pricing with customer and confirms no customizations are needed with assistance from SA as needed

### Step 2: Create the opportunity in SFDC

SAL/ISR creates opportunity using "Professional Services" opportunity record type

* If the Standard Services SKU meets the customer's needs, follow Step 2A.
* If the Standard Services SKU does not meet the customer's needs, follow Step 2B.

#### Step 2A: Standard SKU workflow

1. SAL/ISR adds the standard SKU to the opportunity from product catalog in Zoura
1. SAL/ISR proceeds to Step 3A to create a standard services SOW

#### Step 2B: Custom Services workflow

SAL/ISR requests SA to follows the process for creating a Custom Services SOW in Step 3B

### Step 3: Create and add the SOW

Follow Step 3A for Standard Services, or Step 3B for Custom Services.

#### Step 3A: Create and add a Standard Services SOW

1. SAL/ISR uses SKU SOW template to create copy of SOW in Google Docs and sends to customer for review
1. SAL/ISR adds SKU SOW to the opportunity

#### Step 3B: Create a Custom Services SOW

SA follows the Custom Services SOW workflow below

### Step 4: Close the opportunity
1. SAL/ISR obtains signatures from customer
1. SAL/ISR moves the opportunity to Closed Won status

## Custom Services SOW workflow

Generally, this workflow involves using the GitLab SOW Calculator for creation of the baseline SoW and issue by the Solutions Architect (SA). The SA then engages the PS team to get scoping questions defined and answered.  After that, the SoW is finalized by the PS team and approved by the director of Professional Services.

The GitLab PS team is responsible for maintaining the [GitLab SOW Calculator](https://services-calculator.gitlab.io). The PS team also maintains the SOW template located [at this internal link](https://docs.google.com/document/d/1X8_EiX8kgJdpaVlydbTJg5pn4RXeDvYOIyok2G1A69I/edit)

### Overview

1. SA: Create baseline SoW from Services Calculator
1. SA: Add details to issue around customer requirements
1. SA & PSE: Conduct detailed scoping call with the customer
1. PSE: Develop Custom SoW and pricing for customer
1. Account team: Deliver SoW to the customer, add to the Salesforce (SFDC) opportunity
1. Send for signature (just like software terms)
1. When Closed Won PS team will assign engineer and service delivery will start typically with 4 weeks lead time

### Detailed Process

1. Sales and account team to introduce early in discussions.
1. The SA can do basic scoping and use the [calculator](/handbook/customer-success/professional-services-engineering/selling/#services-calculator) for an estimate.
  - This should be a good estimate to secure budget.
1. Customer should execute Subscription Agreement AND Consulting Services Agreement.
1. The SA can use the [custom SoW scoping details](/handbook/customer-success/professional-services-engineering/scoping/) page to help drive the conversation and uncover required capabilities for the custom SoW.
1. The SA will create the SoW from the [calculator](/handbook/customer-success/professional-services-engineering/selling/#services-calculator), scoping the project and estimating both schedule and cost for the SoW. 
1. The calculator automatically creates an approval issue on the [SoW Proposal Approval board](https://gitlab.com/groups/gitlab-com/customer-success/professional-services-group/-/boards/1353982?&label_name[]=Services%20Calculator).
1. SA: Check and add any more details to the issue created on the SoW Proposal Approval board.
1. SA: Fill out any additional scoping details. Ensure the issue is assigned to a Solutions Manager for review, and move it to the `proposal::Scoping` step.
1. SA & PSE: Conduct more detailed scoping call (only when needed) to [prepare SoW](/handbook/customer-success/professional-services-engineering/#statement-of-work-creation).
1. If there are additional scoping questions needed to scope the engagement, Professional Services Engineering will inform the account team within three (3) business days of this call.
1. Once all scoping questions are complete, move the SoW to the `proposal::Writing` step.
1. Once written, move the SoW to the `proposal::Cost Estimate` step where a Manager of Professional Services will provide a [cost estimate](/handbook/customer-success/vision/#professional-services-standard-cost) used to calculate the expected margin for the project. It will be completed and ready for the account team review within one (1) business week.
1. Move the SoW to the `proposal::ReadyForApproval` step.
1. The SoW is approved by the Senior Director of Professional Services or VP of Customer Success.
1. Move the SoW to the `proposal::Approved` step. Assign the issue to the SA for delivery to the customer via the account team.

## FAQ

#### Do we have set SKUs I can use?

Yes - for off the shelf items, we have [SKUs](/handbook/customer-success/professional-services-engineering/#professional-services-skus).

#### What are our daily or hourly rates?

We do not currently have an hourly or daily rate.  Nor do we plan to have an hourly rate.  Just as with GitLab support, the mission of our Professional Service group is not to bill hours, but to achieve success for our Customers.  So just as we don't offer support by the call or by the hour, we do not offer Professional Services by the day or the hour.

In the future, we may have a daily rate or a daily rate for on-site support.  However, we currently do not for the same reasons listed above.

#### What if the customer only wants training?

If the customer is an EE customer, we can offer training.  However, training will need to be scoped out by the Customer Success department before quoting a price.  The account executive will also be required to provide the use case for the need for just training.

Example use case might be:

Customer is under license utilization and we need to prevent churn, help expand usage into additional groups and other business units.

#### What options exist for CE Customers?

GitLab CE is ideal for personal projects or small groups with minimal user management and workflow control needs.  Because these groups don't typically need a lot of focus on scaled implementation or training, we currently do not offer implementation, integration or training services to our CE customers.  Many of our [partners](/resellers/) offer such services.  However, we find that many customers who have been running a CE instance and are looking to transition to a scaled implementation of GitLab may require a [Discovery Engagement](#discovery-engagement) to determine the customer's long-term needs.

If a customer is upgrading from CE to EE, Professional Services should be engaged to scope out the requirements for the transition if the customer will need services in the transition.
