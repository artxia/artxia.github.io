---
layout: handbook-page-toc
title: Setting ticket priority
category: Zendesk
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Definitions
The [definitions of support impact](/support/#definitions-of-support-impact) are in the Statment of Support.

## Setting Ticket Priority

If a customer submits a ticket via the web ticket form, they can choose the starting priority of the ticket - this is the `Customer Priority` field you will see in Zendesk. On ticket creation a trigger sets the main `Priority` field (not visible to the customer) to match the `Customer Priority` choice. After ticket creation, changes to `Customer Priority` do not affect the `Priority` field or SLAs.

If a customer emails in a ticket it will get a `Priority` of 'Normal' (unless it is sent to the special emergency contact).

Manually setting a ticket's priority in the `Priority` field (not `Customer Priority`) in Zendesk will change the overall ticket [SLA](/handbook/support/support-engineering/working-with-tickets.html#sla), for both the first and next replies. This allows support to prioritize tickets and update the urgency during the life of the ticket (for example the initial request may be 'High' priority and then follow up questions may need 'Low' priority.) Customers don't receive automatic notifications upon priority change.

## Resetting Ticket Priority
Typically, FRT Hawks will set priority during ticket triage as part of the [FRT Process in Action](/handbook/support/workflows/support-modes-of-work.html#the-process-in-action). If it comes to pass that a ticket has an incorrect priority, feel free to reset the priority.

There is a Zendesk Macro `General::Changed priority` that includes language and links that will be helpful if you need to do this.

### Guidelines and Effects

Changing the priority in a ticket will change the SLA, because different priorities have shorter or longer SLAs. Please refer to the [guidelines and SLA listed in our statement of support](/support/#standard-support).
