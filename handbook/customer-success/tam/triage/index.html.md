---
layout: handbook-page-toc
title: "Account Triage"
---

# Technical Account Management Handbook
{:.no_toc}

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

- [Technical Account Manager Summary](/handbook/customer-success/tam/)
- [CS Top 10](/handbook/customer-success/tam/cs-top-10/)
- [Capturing Customer Interest in GitLab Issues](/handbook/customer-success/tam/customer-issue-interest/)
- [Executive Business Reviews (EBRs)](/handbook/customer-success/tam/ebr/)
- [Account Engagement](/handbook/customer-success/tam/engagement/)
- [Escalation Process](/handbook/customer-success/tam/escalations/)
- [Gemstones](/handbook/customer-success/tam/gemstones/)
- [Customer Health Scores](/handbook/customer-success/tam/health-scores/)
- [Account Onboarding](/handbook/customer-success/tam/onboarding/)
- [Customer Renewal Tracking](/handbook/customer-success/tam/renewals/)
- [Account Triage](/handbook/customer-success/tam/triage/) *(Current)*

### Related Pages

- [Using Salesforce within Customer Success](/handbook/customer-success/using-salesforce-within-customer-success/)
- [Responsibility Matrix and Transitions](/handbook/customer-success/#responsibility-matrix-and-transitions/)
- [Customer Success & Market Segmentation](/handbook/customer-success/#customer-success--market-segmentation/)
- [Customer Success Vision](/handbook/customer-success/vision/)
- [Support handbook](/handbook/support/)
- [Sales handbook](/handbook/sales/)

---

# Account Triaging

In order to prevent customer churn and improve retention of our customers, we have an [Account Triage](https://gitlab.com/gitlab-com/customer-success/account-triage) project in GitLab.

## Account Triage Project

#### What is an "At Risk" Account?

If an account is in an Amber or Red state, it is deemed as "At Risk" and requires a "swarm" around it in order to save it and bring it back into a Yellow/Green healthy state. [Scroll down](/handbook/customer-success/tam/triage/#health-scores) to review the criteria for adding the correct health score to an account.

When a customer falls into Red, immediately create an issue in the [Account Triage](https://gitlab.com/gitlab-com/customer-success/account-triage) project and add the Red label. Follow the process below to get urgent attention added to the account. You must ensure that your Leader and/or the Customer Success Director is included in this issue.

If you are worried about a Green or a Yellow account and think it might be Amber, create an issue in the project and review it with the Technical Account Management team on the next Customer Emergency Room Weekly Triage call (explained below).

All Technical Account Manager's meet weekly to review the issue board for current "at risk" account activity. The meeting is a peer review of new at risk accounts to make sure activities are followed up on and owned across the business and is also a chance to discuss tactics/strategies on those accounts in case anything different should be done.

The triage team also needs to check the [TAM Regional Dashboard](https://gitlab.my.salesforce.com/01Z4M000000slMT) to ensure that all Amber and Red accounts have indeed been added to the board. This should be a five minute check. Also, make sure that all issues in the project have the correct health score according to Salesforce. If the scores do not match, reach out to the Technical Account Manager or Account Owner if there is no Technical Account Manager to find out why and then work with them to rectify it.

This project is for Amber and Red accounts. As mentioned above, if you have an account that is Yellow or Green, and feel that you need help and support on that account from the rest of the team and your leaders then you may add an issue on the triage board for that account. Please make sure you are able to attend the next Customer ER call. Once you have reviewed the account's health with the team on the call, you can assign it to the appropriate health score both on the issue and in Salesforce.

When an account is added to the issue board, assign it with a 'triage team', which should include:
* Account Owner
* Technical Account Manager
* Technical Account Management Leader
* Manager of Customer Experience and/or Director of Customer Success
* Regional Sales Manager for Account if appropriate
* Solutions Architect where appropriate
* Professional Services Engineer where appropriate
* Executive Sponsor (probably the account owner's RD, but could be VP of Engineering for example, depending on the problems the customer is having)
* Product Manager(s) where appropriate

This team will have responsibility for managing the account as a team until renewal point. It is NOT the responsibility of the people present on the Customer ER call to own these issues, it is yours. Make sure you keep your issues updated every week with the steps you have taken to try and pull the account back into a healthy state.

The team will also review the [TAM Regional Dashboard](https://gitlab.my.salesforce.com/01Z4M000000slMT) to review the accounts that _do not_ have a Technical Account Manager that are due for renewal within the next 90 days. You can use the dashboard to filter by region and ARR but for the purpose of the Customer Emergency Room call, the focus is on Large accounts. 

The objective here is to try and retain customers, and reduce churn while balancing that with the demands of the rest of the business. For example, if a customer is at risk over a feature that needs to be built, that cost on engineering/product time needs to be balanced with the commercial attractiveness of the customer. For that reason it is a good idea for a representative of the product team to also attend the review meetings, as required.

Having such a process in place ensures we are being proactive about managing our churn risk. It also means gaining visibility of potential churn in advance. If there are commonalities to churn risk customers, that will also help with visibility and prioritisation of any work required — or of any other problems.

If you move an account to Green or Yellow from Amber or Red, close it on the triage board. Make sure you close it AND add the label so we can see the history in the issue.

This project/process is a work in progress and can always be improved. If you have suggestions on how to improve it, please leave add your thoughts to [this issue](https://gitlab.com/gitlab-com/customer-success/tam/issues/80).

## Issue Template:

After creating an issue in the [Account Triage](https://gitlab.com/gitlab-com/customer-success/account-triage) project, it will be created with a default template requiring the following information for the description:

**Salesforce URL**

* Enter the URL of the customer's Salesforce record.

**Customer Success Plan URL**

* Include the URL of the GitLab customer project created during [Account Engagement](/handbook/customer-success/tam/engagement/)

**Contract Renewal Date**

* Include the date for which the customer contract is set to next renew with GitLab based on the Salesforce record.

**Reason for Health Score**

* Using the Health Scoring Criteria, provide justification for why the account is in a Amber or Red state.

With the description populated, the milestone should be assigned to the quarterly milestone that the next contract renewal date falls on.  The due date field is managed by the newly assigned Account Manager / Technical Account Manager as a method for tracking next steps and engagement with an account.


## Labels:

#### Health Scoring Guidelines

Each of these considerations below are to help TAMs assess the health of their customers. When a TAM runs into a tricky situation, they should bring it up with their manager in their 1:1 meeting. This is a mix of art and science — some customers may be a blend of multiple categories. To help, see the example below.

**Customer Health Scoring - Examples**

The examples below are meant to be somewhat difficult if evaluated only on the attributes provided. The TAM should rely also on their past customer conversations, SAL/AE dialogues, and other qualitative factors. These are good exercises for the TAM to work through with their manager.

__Enterprise Customer__
Fictitious company Acme Inc. has the following attributes:
* Onboarding customer
* Low user adoption (Amber)
* Lack of identified GitLab use cases (Yellow)
* Show up late to cadence calls (Yellow)
* Are not interested in [EBRs](/handbook/customer-success/tam/ebr) (?)

This customer could likely be scored as Yellow.

__Commercial Customer__
Captain Barnacle's Custom Paints is a fictitious company with the following attributes:
* Customer for 3+ years
* Interested in upgrading (Green)
* Lost our original GitLab champion (Amber)
* 2 releases behind (Amber)
* AE mentioned during their last call that they recently achieved a desired use case (Green)
* Active user base

This customer could likely be scored as Green or Yellow.


**Red**

* They’ve told us they are downgrading/cancelling.
* No communication.
* Limited or no access to executive sponsors.

**Amber**

* Low user adoption.
* Lack of response to us and/ or we haven’t done much discovery.
* Complains about the company (responsiveness, feature turnaround, missed priorities in direction).
* Loss of our GitLab champion.
* Original GitLab use-cases not achieved.
* Customer doesn't know what success looks like or it is ill-defined.
* At least two major releases behind.
* Frequently don't show up or are late to scheduled cadence calls.
* Raises more than 15 tickets a month.
* Customer was acquired and parent company uses competitor.
* Negative NPS scores.

**Yellow**

* We don’t have much info about how they are using GitLab.
* Don’t have the right contacts for each key person.
* Lack of clearly defined GitLab use-cases.
* Only one primary stakeholder.
* At least one major release behind.
* Doesn't raise any tickets or contribute to any issues.
* Occasionally doesn't show up or are late to scheduled cadence calls.
* Raises more than 10 tickets a month.
* Neutral NPS scores.

**Green**

* Successful GitLab use-cases.
* Using the full GitLab DevOps lifecycle.
* Regular communication and positive relationship.
* Healthy user adoption rate.
* Regularly show interest and utilisation in new features.
* At least two successful [EBRs](/handbook/customer-success/tam/ebr) every year.
* Always show up to regular cadence calls and communicates when they can't.
* They are interested in upgrading.
* Up to date on releases.
* Raises between 1 and 5 tickets a month and regularly contributes to issues.
* Regularly provides feedback on how to improve GitLab.
* Positive NPS scores.


#### Triage Labels for at risk (~red) accounts

* ~E&A
* ~E&U
* ~U&A
* ~U&U

See [Churn Classification](https://sixteenventures.com/churn-classification) for more info on these labels.

#### Workflow labels

* ~New

Every new issue will have the ~New label. Use the "Colours" board as your main view when viewing issues via an issue board. Once you have reviewed the issue, remove the ~New label.

### Region Labels

* ~US-WEST
* ~US-EAST
* ~EMEA
* ~APAC
* ~LATAM

There is also a region board for your viewing pleasure.
