---
layout: handbook-page-toc
title: "Customer Health Scores"
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
- [Customer Health Scores](/handbook/customer-success/tam/health-scores/) *(Current)*
- [Account Onboarding](/handbook/customer-success/tam/onboarding/)
- [Customer Renewal Tracking](/handbook/customer-success/tam/renewals/)
- [Account Triage](/handbook/customer-success/tam/triage/)

### Related Pages

- [Using Salesforce within Customer Success](/handbook/customer-success/using-salesforce-within-customer-success/)
- [Responsibility Matrix and Transitions](/handbook/customer-success/#responsibility-matrix-and-transitions/)
- [Customer Success & Market Segmentation](/handbook/customer-success/#customer-success--market-segmentation/)
- [Customer Success Vision](/handbook/customer-success/vision/)
- [Support handbook](/handbook/support/)
- [Sales handbook](/handbook/sales/)

---

# Customer Health Scores

In order to manage customers at scale we must have a consistent way of keeping track of customer details including the current “health” of the customer.  The health of a customer is affected by many different factors including product usage, support interactions, internal budgets, and TAM communication.  

The current health of a customer is also directly related to the customer’s journey with GitLab.  Because of this, customer health and the running communication notes between a TAM and the customer should be closely linked.  Since the primary location for recording customer health scores is in Salesforce, the running call notes should also be available in this location. For additional information, watch a short (private- [watch as GitLab Unfiltered](https://www.youtube.com/watch?v=LKZ23pRfpBg) ) video on [updating Customer Health](https://www.youtube.com/watch?v=2j8ACuQksEo&feature=youtu.be&hd=1) and review the [Customer Health Dashboard](https://gitlab.my.salesforce.com/01Z4M000000skuA).

See [Health Scoring Criteria](/handbook/customer-success/tam/triage/#health-scoring-criteria).

# Meeting Notes

Meeting/call notes are the running notes for the TAM’s regular interaction with the client.  The call notes should at least cover the following topics:

 * Updates on action items from the TAM
 * New updates from the customer
   * Architectural changes
   * New deployments
   * Product feedback
 * A review of any open support tickets in Zendesk
 * Q&A
 * Current customer health from a business and operational standpoint

At the end of each customer call any changes to customer health should be reflected in the appropriate Salesforce field.  If the Customer Health Score drops below Yellow an issue must be created in the Account Triage Project, see details here.

Call notes should be saved in Google Drive (here) following this format:

```/Sales/Customers & Prospects/A/Acme/Acme - Meeting Notes```

A link to this document should appear in the “Health Score Reasons” field in Salesforce.

See an example meeting notes [here](https://docs.google.com/document/d/1dAcHBqoRTY6qqSw27VQstCCnk5Fxc2oIsbpKs014h3g).

The rationale for saving call notes in this manner is as follows:

 * Call notes frequently contain sensitive information and are for the internal sales team and management to review.
 * Call notes are tightly linked to the Health Score and should be available in the same “pane of glass” as the Health Score.
 * A folder structure allows non-Customer Success executives and support staff to easily locate the notes in the case of an escalation.
 * The naming convention “&lt;customer&gt; - Meeting Notes” allows for fast searching using Google Cloud Search for Work (https://cloudsearch.google.com/)

# Determining Customer Health

Refer back to the [Health Scoring Criteria](https://about.gitlab.com/handbook/customer-success/tam/triage/#health-scoring-criteria) for details on what each health score is intended to represent.  Some common things to look out for during regular meetings are:

 * **Utilization of the product.**  Is it just being used for a single facet of the GitLab experience?
 * **High number of “important” feature requests.**  Is the customer trying to make GitLab work just like another legacy piece of software in their environment?  A review of the GitLab workflow and best practices may be in order.
 * **High number of support requests.**  Is the customer struggling to keep GitLab operational or performant?  An architecture review should be considered.
 * **Missing cadence calls.**  Missing cadence calls could be a sign that GitLab is being deprioritized, work with your SAL to schedule a [EBR](/handbook/customer-success/tam/ebr) or higher level discussion to evaluate the customer’s health.
 * **Failure to upgrade.**  Is the customer more than a major release behind?  Work with the customer to explain the new features and security updates of the current version of GitLab and address any internal technical limitations that have prevented upgrades.  Develop an upgrade plan with the customer if appropriate.

# Customer Cadence

Customer cadence calls should be scheduled weekly during the customer onboarding phase and at least monthly otherwise.  Health scores should be updated at the end of each cadence call if there is a change. The `Customer Health Score Date` will automatically update if the `Customer Health Score` is changed, otherwise TAMs should update the date field so the broader team to know customer health is current.
