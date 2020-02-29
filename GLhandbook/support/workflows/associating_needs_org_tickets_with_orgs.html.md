---
layout: handbook-page-toc
title: Associating needs-org tickets with appropriate organization
category: Zendesk
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Associating tickets with the `needs-org` tag with appropriate organizations
Occasionally tickets come in without an associated organization, which means that no SLA is applied.

Potential reasons this might occur:
- we've never seen anyone from the organization in ZD before (i.e. this is an organization's first ticket)
- the user is using a generic domain name that we cannot assign to a ZD organization (e.g. `@gmail.com`)
- the company has more than one division with a support level, but only a single email domain
- the user is writing from a domain name that doesn't match what we have in ZD (e.g. they're using a personal email address for a work-related issue)
- the user or organization has a trial license

It could equally be the case that a ZD organization was manually created and the SLA type is out of date / incorrect.
Many of the same principles apply here.

> Please avoid manually creating organizations. 

### Determining if this workflow applies
This workflow applies if:
- ZD is prompting you to create an organization
- The Tag `needs-org` is applied (implied by above)
- You have reason to believe that this ticket belongs to a customer
- The domain TLD is *not* a generic domain (e.g. `gmail.com`)

![ZD prompts for an org to be created](/images/handbook/support/zendesk_needs_org-create.png)

### Marking Free Users for GitLab.com

For GitLab.com, if a user cannot be identified as a customers, nor a [trial or prospect](#trials-and-prospects), then change the subscription dropdown to "Free user" and choose the appropriate "problem type".

#### Trials and Prospects

Note: Due to the type of subscription/license they receive, trial users often identify themselves as Ultimate or Gold customers. This form field does *not* need to be updated as SLA is tied to the ZD org.

When applicable, tickets should have one of the following tag (not both):

- **Trial** = user or organization that has taken out a trial, typically using the free trial form.
- **Prospect** = organization trialing GitLab that is sales assisted, also often referred to as a POC (proof of concept).

A long term solution is still being worked on, but in the short term, prospects are supposed to email Support using the email address provided to them or use the appropriate form field, which will automatically add the `prospect` tag.

Otherwise, prospects are identified manually either through form content, ticket content, or the sales rep posts about it in one of the Support Slack channels. In the last case, please *add* an internal note on the ticket.

You can manually add the appropriate tag to the ticket (using Apps > Tag Locker).

Once tagged, the ticket will move to the appropriate queue, and for prospects, with appropriate SLA. However, [trials do not receive support](/support/) (wording included in our "free user" macro), and prospect SLA is for guidance only.

##### Other ways to identify trials and prospects when necessary

While SFDC syncs organizations nightly to ZD, it does not include trial licenses because no organization account is created in SFDC, only a lead. So organizations on a trial will not show in ZD, and this workflow _does not_ apply and we should _not_ manually create these organizations.

To check if a customer is on a trial: In SFDC (see search instructions below), the `Initial Source` will likely say `Trial` (check that initial date is within the standard trial period).

For prospects, there will likely be an organization account with `Account Type` `Prospect`. However, the presence of an org with type prospect does *not* mean they receive pre-sales support.

For self-managed, you can double check for a license in the [license app](http://license.gitlab.com).

For GitLab.com, in the Customers Portal, trials are marked with an expiration date under the **Trials** column in the `GitLab Groups` Tab next to a namespace. If needed, also check the [dotcom-internal project](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues) for manual plan changes.

### Finding the existing organization in Zendesk

You may attempt to find the organization within Zendesk using the search functionality. Do note that TLDs don't necessarily correspond to company names, so you may need to search in SFDC to find the appropriate organization.

Also, note that users may be using generic mail providers you might not be familiar with, so the TLD on their email address may not correspond with their company at all. 

> When in doubt, check SFDC

![Selecting an organization in ZD](/images/handbook/support/zendesk_needs_org-finding-org.png)

### Finding the existing organization in SFDC

See: [Looking up customer account details in Salesforce](/handbook/support/workflows/looking_up_customer_account_details.html#within-salesforce)

#### Organization exists in SFDC but service level does not match Zendesk
At times, the organization exists in Zendesk but has the wrong service level. You can force a resync for the specific organization.

1. Ensure that the **Account** in SFDC says the organization is a `Customer`.
1. `Edit` the `Support Level` to something aside from the current level.
1. `Save`.
1. `Edit` the Account again to change the `Support Level` back to the original.
1. `Save`.

If you refresh the organization page in Zendesk, the proper service level should immediately be reflected. However, for existing tickets where the user was already associated with the organization, the appropriate tag will need to be added manually to the tickets.

### Finding the existing organization in [customers.gitlab.com](https://customers.gitlab.com)

See: [Looking up customer account details in customer.gitlab.com](/handbook/support/workflows/looking_up_customer_account_details.html#within-customersgitlabcom)

### Adding the domain (Zendesk Admins only)
> **Important**: Be extra careful here. If a large company has multiple subscriptions it may not be appropriate
to add the domain. You'll need to add individual customers to the appropriate organization (see below)

Once you've determined the appropriate domain to add and identified the correct ZD Organization, you can click 
the `Domains` field to add it.

![Filling in an organization domain in ZD](/images/handbook/support/zendesk_needs_org-adding-org.png)

### Adding a customer to an organization (All Zendesk Users)
If you don't have admin access on ZD, you can still make sure the proper SLA is applied by adding the user to the appropriate
organization.

1. Click on the customer's name in ZD
1. In the "Org" field type the organization name

![Adding a user to an existing organization](/images/handbook/support/zendesk_needs_org-add.png)

### Verifying that the ticket now has the proper SLA applied
Now that you've added the appropriate domain, head back to your original ticket and verify that it is associated with
the appropriate organization and SLA.

![Verifying SLA](/images/handbook/support/zendesk_needs_org-verifying-sla.png)

### Handling customers with expired licenses and updating info on SFDC side

If you see that the ticket still has no SLA after associating a user with an organization, it could mean that this
organization has some special status on Salesforce side. One of the edge cases - the organization is marked as
`Former Customer` and support level is set to `Expired`. In such case it is better to check with Sales if the
status is valid or not:

- open Salesforce and find the customer in question
- click `Show feed` button at the upper part of the page

![Salesforce show feed](/images/handbook/support/sfdc_show_feed.png)

- send a message there asking to clarify the customer's status and mention `@Sales-Support`,
they should be able to help with such cases

**Note:** the same workflow applies if you notice that customer-related information is not up-to-date on SFDC side
and you are not able to update it using our generic `Support Admin` account.


### Associated Trigers:
- [Add need-org tag](https://gitlab.zendesk.com/agent/admin/triggers/360001567348)
- [Remove need-org tag](https://gitlab.zendesk.com/agent/admin/triggers/360017109414)
