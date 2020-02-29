---
layout: handbook-page-toc
title: Internal Support for GitLab Team Members
---

## Internal Support for GitLab Team Members
{:.no_toc}

**Looking for technical support? Please visit the [Support Page](/support/) instead.**
{:.no_toc}

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## What does the Support Team do?

GitLab Support provides technical support to our Self-managed and GitLab.com customers for the GitLab product.

We are *not* internal IT Support, so we probably can't help you with your MacBook, 1Password or similar issues. (Check in with `#peopleops` for who to contact regarding these problems.)

If you're a customer (or advocating for a customer), you should take a look at the dedicated [Support Page](/support) that describes how to get in
contact with us.

Fellow GitLab team-members can reach out for help from the Support Team in various ways:


1. For general support questions ("Can GitLab do x?", "How do I do y with GitLab?") try:
   - posing your question on the `#questions` channel in Slack, so that everyone can contribute to an answer. If you're not getting an answer, try cross-posting in the [relevant support team channel](#support-chat-channels).
1. For longer term or larger scope questions, such as team process change, or data gathering requests, create a [support issue](https://gitlab.com/gitlab-com/support/support-team-meta/issues)
1. If customers or users have questions, advise them to contact support directly via the [support web form](https://support.gitlab.com).
1. As a last resort, ping the support team on one of the [support channels](#support-chat-channels).

### Support Issue Tracker

The [Support project](https://gitlab.com/gitlab-com/support/support-team-meta/issues) hosts an issue tracker meant to improve our workflow by reporting any problems that may arise in our tools or processes. It's also meant to propose and discuss ideas in general.

The issue tracker is open to the community and part of the `gitlab-com` group. It should not contain any sensitive information. Links to Zendesk or other references are encouraged.

### Support Chat Channels

The support channels are as follows:

- [#questions](https://gitlab.slack.com/messages/questions) - If your question is something that you think anyone in the company could answer or is valuable to the greater company to know, ask it here!
- [#zd-self-managed-feed](https://gitlab.slack.com/messages/C1CKSUTL5/) - Feed of all self-managed Zendesk ticket activities.
- [#zd-gitlab-com-feed](https://gitlab.slack.com/messages/CADGU8CG1/) - Feed of all GitLab.com Zendesk ticket activities.
- [#support-managers](https://gitlab.slack.com/messages/CBVAE1L48/) - This channel is specifically for support managers.
- [#support_self-managed](https://gitlab.slack.com/messages/support_self-managed/) - This channel is specifically for the self-managed support team. They handle self-managed production issues, triage bugs, and self-managed emergencies, among other things.
- [#support_gitlab-com](https://gitlab.slack.com/messages/C4XFU81LG/) - This channel is specifically for the GitLab.com support team. They handle GitLab.com account and subscription support and GitHost.
- [#githost](https://gitlab.slack.com/messages/githost/) - This channel handles monitoring for GitHost instances.

In order to attract support team's attention in Slack, you can use the team handles, mentioning multiple team members in a message or a thread where support is needed. Support team handles are:
- `@support-selfmanaged` - Self-managed support team members.
- `@support-dotcom` - GitLab.com support team members.
- `@supportmanagers` - Support director and managers.

## Internal Requests

### Requesting Support for Customers

If your customer has a support question, please direct them to open a ticket either through the [Support Portal](https://support.gitlab.com) or via an email to support@gitlab.com. The former is preferred. This ensures that, as a paid user, the customer is serviced by the team that is best equipped to assist them and holds us to the SLA appropriate for their subscription tier.

### Note on Zendesk and support@gitlab.com 

All internal requests to support should follow the guidelines set in the rest of this section. Please *do not* open requests directly through [Zendesk](https://support.gitlab.com) (the Support Portal) or by sending an email to support@gitlab.com.

### Note on Requesting Customer Information

According to our [privacy policies](/privacy/), the support team will not provide any information regarding customers, groups, projects, etc, that are not available publicly. This includes situations where a customer is requesting information about their own projects, groups, etc. If they are unable to authenticate, we cannot assume they are who they say they are. If they are locked out, please have them submit a ticket to the support team for assistance.

### 'Light Agent' Zendesk accounts available for all GitLab staff

All GitLab staff can request a 'Light Agent' account so that you can see customer tickets in Zendesk and leave notes for the Support team. These accounts are free. 

To request a Light Agent Zendesk account, please send an email to <mailto:gitlablightagent.5zjj2@zapiermail.com> - you'll receive an automated reply with the result of your request. **NOTE:** you must send your request from your GitLab Google / Gmail account. No other addresses will work. The Subject and Body fields of the email can be empty.

Once set up, you'll need to wait 24 hours for your account to be assigned Zendesk in Okta. Once Zendesk is assigned, you should be able to login to Zendesk by following this link: <https://gitlab.zendesk.com/agent>. 

You cannot send public replies to customers with a Light Agent account - if you need to do this, please submit a [new Access Request issue](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=Single%20Person%20Access%20Request) for a paid full agent account. 

[Read more information on Light Agent accounts from Zendesk](https://www.zendesk.com/company/collaboration-add-on-additional-features/)

### Common internal requests - all GitLab team-members

##### I want Gold for my work or personal account
- [Submit a request](https://docs.google.com/forms/d/e/1FAIpQLSddexI8VZTCiyxme1_7QtbQZ6WoIJRlHdaI2Gi6PD8Eti-DLQ/viewform). Your account(s) will be upgraded to the Gold tier within 30 minutes of submission.

Please note that Support is no longer handling these requests. If you require a group to be upgraded to Gold for work purposes, please [submit an access request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=Single%20Person%20Access%20Request).

##### I want to claim a dormant username
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Dormant%20Name%20Request) using the `Dormant Name Request` template.

##### I keep getting reCaptcha on an issue/MR on GitLab.com
- At the time it is happening, please drop us a message and link to the issue/MR in our Slack channel `#support_gitlab-com`. A team member will mark you as "ham", which override the reCaptcha requirement.

##### I need access to something
- Support doesn't handle these requests so you'll want to open a new [Access Request](https://gitlab.com/gitlab-com/access-requests/issues/new?issuable_template=New%20Access%20Request) issue.

##### I need Support to contact a user on GitLab's behalf
- If required, you can [request us to contact a user](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Contact%20Request). Typically, this is for the production team to notify actions taken on behalf of a user.

### Common internal requests - Sales Team / Technical Account Managers / Accounts Receivable

##### I want to extend or change the plan of a GitLab.com Trial
- For trial extensions [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Trial%20Extension) using the `Trial Extension` template. Support Engineers will handle the trial extensions for GitLab.com.

- To grant a Bronze or Silver trial [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Plan%20Change%20Request) using the `Plan Change Request` template. 

>**NOTE**: It's not yet possible for users or GitLab employees to directly start a Bronze or Silver trial on a namespace. If one is needed, have the user initiate a Gold trial and then open an issue per the above link using the `Plan Change Request` template to have the plan manually changed. Implementation of this feature is being discussed in [this issue](https://gitlab.com/gitlab-org/growth/engineering/issues/37).

##### I want to extend a trial for a Self-managed prospect
For trial extensions [open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Trial%20Extension) using the `Trial Extension` template. The Growth team will handle the trial extensions for self-managed.

##### My prospect is unable to apply a purchased subscription to their GitLab.com group
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Plan%20Change%20Request) using the `Plan Change Request` template.

>**NOTE**: The issue is most likely that their group still has an active trial which must be expired manually first. Open an issue using the above template to have that done. This should only be necessary until an active trial is expired automatically when a subscription is applied to a namespace. Keep an eye on [this issue](https://gitlab.com/gitlab-org/gitlab-ee/issues/12186) to track progress on the fix.

##### I want to change the plan of a GitLab.com user or group
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Plan%20Change%20Request) using the `Plan Change Request` template.

##### I want to see if a group name is free or able to be claimed for a potential customer
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Dormant%20Name%20Request) using the `Dormant Name Request` template.

>**NOTE**: Using another's trademark in a way that has nothing to do with the product or service for which the trademark was granted is not a violation of trademark policy. User and group names are provided on a first-come, first-served basis and may not be reserved. We can ask nicely to free an active namespace, but we won't take anything away. Your prospects desired group name may not be freeable.

##### I want to draw attention to an existing support ticket

It's important to understand that Support targets a 95% SLA acheievement KPI. This means that some tickets breaching is expected. Our SLA is for a _First Reply_ but we also internally track next reply. 
1. Review the SLA associated with the account and the amount of time left until a breach by logging into https://gitlab.zendesk.com with your GSuite credentials. (It's not typically necessary to escalate an issue that is hours away from a breach) If the ticket has had a first reply, then you are looking at an "internal breach".
1. Post a link to the ticket and a reason for why this ticket needs special attention into `#support-managers`. Feel free to tag `@supportmanagers`. When you do this, we ask that you go above and beyond to help. If something breached, it means we are probably stuck. Take a look at the ticket and try and call in a relevant department manager to help. Messages where you ask other groups for help will more likely get resolved sooner.
1. Understand that we'll do our best to prioritize appropriately taking into account all of the tickets in the queues - there may be more pressing items.

Please note that this guideline also applies to any issues outside of Zendesk as well, such as those created in `dotcom-internal`.

##### I want to know who is on-call today
- You can run `/chatops run oncall support` in `#support_self-managed` to see who is on-call. This will **not** page the on-call person. Alternatively, you can run that command in a direct message with `GitLab Chatops`.

##### I want to schedule a customer call for upgrade assistance 
- [Open an issue](https://gitlab.com/gitlab-com/support/support-team-meta/issues/new?issuable_template=Upgrade%20Assistance%20Request) using the `Upgrade Assistance` template.

##### I want to request that pipeline minutes be reset for a user or group

- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Pipeline%20Quota%20Reset%20Request) using the `Pipeline Quota Reset Request` template.

##### Users in an account I own would like more visibility into their organization's support tickets 

In some cases, certain organizations want all members of their organization to be able to see all of the support tickets that have been logged. In other cases, a particular user from the account would like to be able to see and respond to all tickets from their organization. If you'd like to enable this, please:

- [Open an issue](https://gitlab.com/gitlab-com/support/support-ops/support-ops-project/issues/new?issuable_template=Shared%20Organization%20Request) using the `Shared Organization Request` template

##### My customer wants to know how many total users they have in their group(s)

A member of the group with `Owner` permissions may visit the **Settings -> Billing** section of the group to see how many seats are in their subscription and how many are currently in use. They may also make use of the [GitLab Group Leader](https://gitlab.com/gitlab-com/support/toolbox/glgl) tool. Please note that it is currently not possible for users to download a report of their group user count and usage but there is an [open feature proposal](https://gitlab.com/gitlab-org/gitlab/issues/118479) suggesting that such functionality be implemented.


##### I need an EULA sent/resent
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=EULA) using the `EULA` template.

##### I need assistance with a License issue
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=license%20issue) using the `License Issue` template.

### Common internal requests - Legal
##### I need logs preserved pursuant to a subpoena or other formal legal request
- [Open an issue](https://gitlab.com/gitlab-com/support/dotcom/dotcom-internal/issues/new?issuable_template=Information%20Request) using the `Information Request` template.

##### I need to submit a DMCA request
- [Open an issue](https://gitlab.com/gitlab-com/gl-security/abuse/issues/new?issuable_template=dmca_meta_issue) using the `DMCA Meta Issue` template

