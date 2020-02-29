---
layout: handbook-page-toc
title: Zendesk Organizations Overview
category: Zendesk
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# Organizations

## How organizations are created?

Organizations in Zendesk are created automatically through our Salesforce and Zendesk integration. This integration allows agents to see a customer's full Salesforce Profile within a live ticket in Zendesk. You can read more about what information we send to Salesforce and what fields are populated with information from Zendesk in the [Support Ops handbook page](https://about.gitlab.com/handbook/support/support-ops/#salesforce---zendesk-sync).

## Organizations with outdated information

If you notice an organization in Zendesk contains outdated information or the information doesn't match what Salesforce is displaying, we might need to manually trigger a sync of that particular organization to update the information. In order to do so, you need to login to Zendesk and Salesforce:

- In Zendesk, update the `Salesforce ID` to match the Salesforce ID of the account you want to sync with. Also, make sure that the 'Domain' for the organization in Zendesk is properly formatted and doesn't include any special characters.

- In Salesforce, check that the `Zendesk Support Organization ID` matches the `Zendesk Organization ID` in Zendesk. The `Zendesk Organization ID` can be found in the link when you open an organization. Example: https://gitlab.zendesk.com/agent/organizations/361092349520/tickets where the `Zendesk Organization ID` is `361092349520`. You also have to make sure that the `Zendesk Support Organization Name` in SFDC matches the `Zendesk Organization name`.

Once you have checked this information, you can force a manual sync by changing any fields within Salesforce (you can change the Support Level from Gold to Silver). This will trigger the sync and update the information in Zendesk within seconds. You have to make sure to return the values that you change to their original values and trigger another sync if necessary to update the information in Zendesk. More information regarding this topic can be found in our [Associating tickets with the needs-org tag with appropriate organizations](https://about.gitlab.com/handbook/support/workflows/associating_needs_org_tickets_with_orgs.html#organization-exists-in-sfdc-but-service-level-does-not-match-zendesk) page.

## Shared Organizations

You have the option of allowing all of the members in an organization to see each other's tickets. This is referred to as a shared organization. Read more about this process in the [Support Engineer Ops page](https://about.gitlab.com/handbook/support/support-ops/#shared-organizations-in-zendesk) 

## Adding users to organizations

To add a user to an organization, you can do it through the end-user's profile as explained in this [Zendesk article](https://support.zendesk.com/hc/en-us/articles/203661976-Creating-managing-and-using-organizations#topic_wyj_dse_bc). Make sure that the request to add a new user to an organization always comes from the Account Administrator or an official party. Always make sure to check with the Technical Account Manager or Account Owner before adding new members to an organization, especially if the users you are adding aren't using a company email.
