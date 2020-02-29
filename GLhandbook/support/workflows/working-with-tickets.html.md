---
layout: handbook-page-toc
title: Working with Tickets
category: Handling tickets
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Working with tickets

### Ticket Statuses

|  **Status** | **Meaning** | **Notes** |
| --- | --- | --- |
|  New | The ticket has just been opened and has had no replies. |  |
|  Open | The ticket has had one or more replies, and the customer is waiting on GitLab Support to provide the next reply. |  |
|  Pending | The ticket has been replied to and is waiting on the customer to provide additional information. | After 3 days in "Pending", a customer will receive a further response reminding them that the ticket exists. If there are no responses after a total of 7 days, the ticket will be moved to Solved. |
|  On-Hold | GitLab support is working on the ticket and may be waiting for information from another team | Placing a ticket on-hold will assign it to the engineer. After 3 days the ticket will move back to open status, requiring an update to the customer. On-hold is transparent to the customer (they see the status as 'Open') so there is no need to inform the customer that the ticket is being put on-hold. It's the engineer's responsibility to ensure timely replies or set the ticket back to 'Open' if they are no longer working on it. Setting a ticket to 'on-hold' while working on the ticket can be useful as it takes it out of the main queue, thus saving other engineers from wasting time reading the ticket. |
|  Solved | The ticket has been solved | A customer who replies to a Solved ticket will re-open it. |
|  Closed | The ticket is archived | A customer who replies to a Closed ticket will open a new ticket with a note that relates the new case to the closed ticket. |

### Services and support

For an overview of the support we provide to customers and GitLab.com users, please see the general [support page](/support/). What follows is a more detailed description of the levels of service.

**Response time indicates the maximum first reply wait time.**

We strive to answer tickets faster than the SLA requires. The higher in the list a channel is, the sooner it should be answered.

The SLAs described in [GitLab Support Service Levels](/support/#gitlab-support-service-levels) are based on ticket priority which can be set manually by support agents. See [setting ticket priority](/handbook/support/workflows/setting_ticket_priority.html)

### Slack premium high priority notification

We use a webhook to get Slack notifications when a high priority premium ticket arrives.
It is posted on the `#support_self-managed` or `#support_gitlab-com` Slack channel.  If you answer the ticket put either a `:eyes:` or `:heavy_check_mark:` emoji to let other support engineers know if you're reading or have responded to the ticket.

If you're not sure how to answer the ticket start a thread under the ticket and tag other support engineers to join the discussion.

### Handling large files

Zendesk has a [maximum attachment size](https://support.zendesk.com/hc/en-us/articles/235860287-What-is-the-maximum-attachment-size-I-can-include-in-ticket-comments-) of 20MB _per file_. Zendesk will not allow us to increase this limit any further.

If you need a customer to share a larger file than this, then see [Provide large files to GitLab support](/support/providing-large-files.html) for more info on how.

### Filling out fields on tickets

Depending on the queue you are working on and the form the ticket belongs to, you might need to fill out some ticket fields manually. Those fields help us capture important data that will help us improve the customer experience. As a high percentage of our tickets are solved/closed automatically through our workflows, it is important to make sure that before you submit your response to a ticket, you check that all required (*) fields and relevant non-required fields have been filled out. 

### Linking relevant Support discussion in a ZenDesk internal note

When using Slack to work with others or communicate internally regarding a Support ticket, please link any relevant Slack threads in an internal note on the ZenDesk ticket. 

## SLA Workflow

Our SLA workflow relies on end-users who submit tickets belonging to an organization and that organization having a GitLab Plan. Organization information is automatically added to Zendesk via a Salesforce Integration. We sync all records with Account Type equal to `Customer` from Salesforce to Zendesk. The information we get from Salesforce includes but it is not limited to: Account Owner, Technical Account Manager, GitLab Plan and Salesforce ID. Organizations should never be created manually in Zendesk as that can cause our sync to be ineffective.  If you think an Account in Salesforce doesn't have an equivalent Organization in Zendesk, please let the Support Operations Specialist know so a manual sync can be run.

### GitLab.com & GitHost Views

GitLab.com Support team members should work on tickets following these views in order:

1. GitHost (Support Engineers only)
1. GitLab.com views (Subscribers, Free)

Within a view, tickets should be prioritized based on the SLA time until breach.

### Self-Managed Views

Tickets should be picked up in the following order to make sure that SLAs are not breached (maximum SLA wait time exceeded) or (if breached) are addressed as soon as possible, and customers receive the proper level of service:

1. About to breach Premium tickets (breaches within 2 hours)
1. About to breach Starter tickets (breaches within 2 hours)
1. Breached Premium tickets
1. Breached Starter tickets
1. High priority Premium tickets
1. High priority Starter tickets
1. Medium priority Premium tickets
1. Medium priority Starter tickets
1. Low priority Premium tickets
1. Low priority Starter tickets

This would not apply to those working specialized roles, such as [FRT Hawk](support-modes-of-work.html#first-response-time-hawk) or [SLA Hawk](support-modes-of-work.html#sla-hawk).

#### Non-Support Views

1. Security
1. Upgrades, Renewals & AR (refunds)

### Hot Queue: How GitLab Manages Ticket Assignments

Traditional Support teams often use an "assignment" model, where an agent is assigned a ticket and guides the ticket through to completion. If they are stuck, they can re-assign this ticket to another agent to pick up and try and complete. At GitLab though, we take advantage of our global support team and use a system dubbed "Hot Queuing". This system means that we all work from one global queue and it's expected that multiple agents will work together on most issues. This allows us to do the following:

- Keep tickets moving forward 24/7.
- Expose team members to more issues, so more learning is happening.
- Provide faster responses to customers, since tickets are not hidden away in an agent's personal queue and "bound" to an agent's workday.
- Everyone has an accurate overview of the support load.

#### When Should Tickets be Assigned?

There are times in the support process that an agent may need to assign the ticket to themselves:

- If you are going to take the ticket to a call/screenshare, take it out of the queue by assigning the ticket to yourself. After the call, if the ticket is still on-going, feel free to unassign yourself so that everyone can continue to move it forward.
- If you've established an understanding with the customer that **you** will see this through. There are times where we want this, and agents have full discretion to do it, but these cases should be few and far between. Be aware of SLAs if you do this!

#### What if I Can't Answer a Ticket?

If you see a ticket in the queue that you are not able to answer, you should:

- Make an internal note with your initial gut feelings as to where the issue might be.
- CC yourself so you can follow along as the ticket progresses.
- If you know that agents will need logs or version information, feel free to start the ball rolling with a simple response asking for it.
- Consider asking about the ticket in slack to see if others can help.
- Consider asking a more experienced colleague, or take a look at the [Team page](/company/team/) to find someone who can help you.

With the hot queue, we all work together and no one should be scared to start a ticket.

### What if Someone is Working on a Ticket that I’d Like to Work On?

If another agent is looking at a ticket that you’re interested in working on, keep in mind:

- If an agent is looking at a ticket, that doesn’t always indicate that they are actively working on the ticket.
- If an agent has a blue circle around their picture, it usually indicates that they are replying on the ticket. However, this can be a false positive.

If another agent is looking at a ticket that you would like to work on:

- Contact that agent via Slack to see if they are actively working on a ticket.
- If they are, ask to pair on the ticket, or offer any information and questions that you have.
- If they don’t respond, go ahead and work on the ticket (bias for action).

If you are working on a ticket, and need some time to research, indicate your involvement by:

- Leaving a note with your action plan and by what time you will respond.
- Be mindful of the remaining time in the SLA. If you aren't feeling confident that you can deliver within the SLA time, reach out to another engineer to pair on it.

### Zendesk SLA settings and Breach Alerts

SLAs are set as Business Rules within Zendesk. For more information, please refer to the specific [Zendesk](/handbook/support/workflows/zendesk_admin.html) page.

We have a slack integration that will notify us for self-managed, if a Premium ticket will breach within an hour, and for GitLab.com, if a Premium ticket will breach within 2 hours. If you see one of these, start a thread and consider this a _small emergency_. If you need help, draw the attention of other support engineers by tagging them, and work to move the ticket forward.

If a customer's reply is the last one in the ticket, do not set it to any status silently (except for Solved), because the breach clock will continue to run and the ticket may breach silently.

Instead, send a confirmation, greeting, or other message, while also changing the status.

#### Using on-hold status

You should use the On-hold status when it is necessary to do some internal work, e.g. reproduce a complex bug, discuss something with developers
or wait for a session scheduled with a customer. When setting the status to On-hold it will be automatically assigned to you by the trigger [`Automatically assign on-hold ticket to an agent who put it to the on-hold status`](https://gitlab.zendesk.com/agent/admin/triggers/360033242313).
If you think that it should be assigned to someone else (e.g. session is scheduled for another engineer), feel free to re-assign it. Tickets without assignee will be automatically reopened by the trigger
[`Automatically reopen on-hold tickets without assignee`](https://gitlab.zendesk.com/agent/admin/triggers/360028981853). Tickets in on-hold status _with_ an assignee will be automatically reopened in 4 days by the automation [`Reopen on-hold tickets after 4 days`](https://gitlab.zendesk.com/agent/admin/automations/360028978393).

If a customer's reply is the last one in the ticket, do not set it to the On-hold status silently due to the same reasons as stated above in the
[Zendesk SLA settings and Breach Alerts](#zendesk-sla-settings-and-breach-alerts) section. Instead, reply to the ticket while also changing the status.

#### Merging tickets

If you're merging two customer tickets that are related and it's not 100% obvious to the customer, be sure to send a message letting them know why you're merging them. If you don't, it often causes confusion and they open follow ups asking why it was closed without comment.

Additionally, when [merging tickets](https://support.zendesk.com/hc/en-us/articles/203690916-Merging-tickets), leave `Requester can see this comment` unchecked in the ticket that's being merged into (the second ticket from the top) in order to maintain the SLA. If the merge comment is made public it, Zendesk will consider it a response and will remove the SLA.

#### Removing information from tickets

We ask customers to send us logs and other files that are crucial in helping us solve the problems they are experiencing. If a customer requests deletion of information shared in a support ticket, if we suspect sensitive information was accidentally shared, ask a Support manager to delete the files using the [`Ticket Redaction`](https://www.zendesk.com/apps/support/ticket-redaction/) app. Only Zendesk administrators have access to this app.

To delete text or attachments from a ticket:

1. Go to the ticket in question and on the right hand nav bar, scroll down until you are able to locate the Ticket Redaction app. 
2. In the text box, enter a string of text or source image URL you wish to redact.
3. If you wish to remove an attachment, you can click on the `Redact Attachment` button and choose the attachment you would like to remove. 
