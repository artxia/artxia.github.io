---
layout: handbook-page-toc
title: "Community advocacy tools"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Zendesk instance

![Mentions in Zendesk](/images/handbook/marketing/community-relations/zendesk.jpg){: .shadow}

The Community Advocates team use a [dedicated Zendesk instance](https://gitlab-community.zendesk.com/) to centralize the management of mentions in the [social response channels](/handbook/marketing/community-relations/community-advocacy/#community-response-channels).

The majority of the response channels' mentions are routed to Zendesk via automation. Generally through Zapier or a native Zendesk integration.

Each mention is then converted into a ticket and filtered into a [View](#zendesk-views), ordered by channel priority. As part of their daily workflow, Community Advocates process each one of these views and manage the ticket lifecycle.

A typical ticket lifecycle is as follows:

1. A wider community member mentions GitLab in one of our [social response channels](/handbook/marketing/community-relations/community-advocacy/#community-response-channels)
1. The social response automation routes the mention to Zendesk and converts it into a ticket.
1. The ticket appears in one of the [View](#zendesk-views) as New
1. A Community Advocate scans through the views by priority or expertise, and opens the ticket
1. The Community Advocate decides the type of response. Typically, this will be either replying on the social channel, [involving experts] or marking the ticket as NOOP (no action required).
1. After the action for the ticket has been taken, the ticket will be closed by the Community Advocate, either manually or via a [macro](#zendesk-macros).

### Zendesk subscription

After [a discussion with the GitLab Support team](https://gitlab.com/gitlab-com/support/support-team-meta/issues/1583), it was concluded that for the specific Advocate workflows and metrics it would be best to keep the [Community Relations Zendesk instance](https://gitlab-community.zendesk.com/) separate from the [Support team's Zendesk instance](https://support.gitlab.com).

The Community Relations instance runs on a [Professional Zendesk Support](https://www.zendesk.com/product/pricing/#support_pricing) subscription, with one seat per Advocate plus an extra seat for the team manager.

### Zendesk access

Zendesk access is provided for every Community Advocate and their manager via the Zendesk admin. Once access is set up, Advocates can log in as "Agent" via SSO and their GitLab Google Suite account.

## Zendesk views

### View limits workaround

![Views in Zendesk](/images/handbook/marketing/community-relations/zendesk-views.jpg){: .shadow}

There is a [limit on the number of views](https://support.zendesk.com/hc/en-us/articles/231732128) that can be displayed on the main "Views" panel on Zendesk, regardless of the type of subscription:

- 12 shared views
- 8 personal views

If the number of views exceeds these limits, the additional views are moved to the `Settings > Views` panel. As the Community Advocates make use of the shared views feature, and as the number of response channels already exceeds the limit of 12, this poses a hindrance on ticket visibility and effectivity.

As a workaround, the team has decided to standardize the personal views for each Advocate, thus effectively increasing the number of visible Views to 20. If the number of response channels exceed the count of 20, an alternative approach could be to consolidate some of the existing views –a practice already followed where it makes sense (e.g. E-mail view).

The workaround is based on two steps: creating a shared view, which then every advocate can clone as a personal view.

To create a new shared view:

1. Navigate to `Settings > Views`
1. Click on the `Add view` button or clone an existing shared view
1. Set up or modify the filter conditions if necessary
1. On `Available for`, choose `All agents`
1. Inform the rest of the team about the availability of the new view  

To create a personal view from a shared view:

1. Navigate to `Settings > Views`
1. In the views list, hover over the right hand side of view you want to clone
1. Click on the ellipsis to open the context menu
1. Choose `Clone` 
1. Do not modify the filter conditions
1. On `Available for`, choose `Me only`  

## Zendesk macros

A macro is similiar to an email template, but consists of one or more actions that modify the values of a ticket's fields. Macros are applied to tickets manually by Advocates. For example, we use macros for mentions or questions requests that we can answer with a single, standard response. Please keep in mind, though, that the goal is to personalize each response as much as possible.

Macros can perform the following tasks:

* Add comment text
* Update ticket fields
* Add or remove ticket tags
* Add CCs
* Change the assignee
* Set the ticket subject
* Add attachments to ticket comments

### Creating macros

There are two types of macros: personal macros (created by an agent or administrator for their own use) and shared macros (created by an administrator  with permission for multiple users).

Please make sure to focus on creating shared macros since we want to keep all the info transparent and available to the whole team.

#### Creating personal macros

Although only administrators can create the macros that are shared by all Community Advocates, Advocates can also create personal macros for their own use. A personal macro is only visible to and can only be used or modified by the creator. 

1. Click the **Admin** icon in the sidebar, then select **Macros**.
1. Click the **All shared macros** drop-down menu and select **Personal macros**.
1. Click the **Add macro** button.
1. Enter the macro name, and add actions for your macro as described in Building macro action statements.
1. Click **Create**.

#### Creating shared macros

Administrators (and agents in custom roles with permission) can create macros that are shared by all Zendesk Support agents or macros that are shared by only agents in a specific group. Administrators can also create personal macros for their own use.

A personal macro is only visible to and can only be used or modified by the creator. Administrators can create shared macros, and can modify all shared macros, regardless of who created them.

1. Click the **Admin icon** in the sidebar, then select **Macros**.
1. Click the **Add macro** button.
1. Enter a **Macro name.**
1. (Optional) Enter a **Description.**
1. Select an option from the Available for menu:
    * **All agents**, available to all agents.
    * **Agents in group**, available only to agents in the group specified. A drop-down menu to choose the group appears when you select this option.
    * **Me only**, available only to you.
1. Under **Actions**, use the drop-down menus to add actions for your macro as described in Building macro action statements.
    * If you choose the Comment/description macro action, and you have rich text formatting enabled, you can add formatting and inline images and you can add attachments to your macro comments.
1. Click **Create**.

### Applying macros

You can manually apply one or more macros to a ticket at once. Just as you can make bulk updates to many tickets at once, you can also apply a macro to more than one ticket using your views.

A typical use case is a ticket that contains more than one question or issue, let's say two in this example. You might have set up two macros that both insert a comment into a ticket to answer each issue separately. By applying each macro to the ticket, you add two comments and address both issues in a single response.

1. In a ticket , click the **Apply macro** button in the bottom toolbar.
1. Typically, your five most commonly used macros from the past week appear at the top of the macros list.
    * You can select one of these, begin typing the name of the macro, or scroll through the list to find the one you want to use.
1. The actions defined in the macro will be applied. If the macro updated the ticket comment, you can edit the text before submitting the ticket.
1. To apply another macro, click **Apply macro** again and select another macro.

### Previewing macros

There is an option to view a description of a macro, and preview the update it will make to a ticket, before applying it.

1. In a ticket, click the **Apply macro** button in the bottom toolbar.
1. Scroll through the list to locate the macro you want to use.
1. Hover your cursor over the macro to display its description tooltip.
    * If the macro does not have a description, the tooltip does not appear.
1. If the description matches the macro you want to apply, click on it to use it.

### Current macro stack descriptions

| Macro Name | Macro Description |
|---|---|
| Country block feedback | Use when tagging feedback related to the China/Russia country block. Applies tag `country-block`, assigns the ticket to you, and changes ticket status to `solved`.|
| Crowdin | Use to track Crowdin notifications. Applies `crowdin` tag, assigns the ticket to you, and changes ticket status to `solved`. |
| Deleted | Use when comment or post was deleted or removed. Assigns the ticket to you and changes ticket status to `solved`.|
| Email::AntiSales| Use to reject sale offer. Applies plain text template to email. Assigns the ticket to you and changes ticket status to `solved`.|
| Email::CommunityWriters| Use for outreach/requests for involvement in Community Writers program. Applies plain text template to email. Applies `guest-post` tag, assigns the ticket to you, and changes ticket status to `solved`. |
| Email::Sponsorship | Use for sponsorship requests. Applies plain text template to email and `sponsorship` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Expert Responded | Use to track responses from GitLab experts to community members via their personal social accounts. Applies `expert-responded` tag and changes ticket status to `solved`. |
| Feedback | Tag something as feedback. Applies the `feedback` tag. |
| License | Use to track Education and OSS license distribution. Applies `license` tag, assigns the ticket to you, and changes ticket status to `solved`. |
| Mention | Use on Twitter and Reddit tickets when no further action is required. Applies the `mention` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Monitoring | Use when you're keeping something open to monitor. Assigns the ticket to you, and changes ticket status to `on-hold`. |
| No-op | Used on HackerNews tickets to indicate no response required, mention only. Applies the `no-op` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Non-English | Can be applied to any ticket view. Applies `non-english` tag, assigns the ticket to you, and changes ticket status to `solved`. |
| Non-Profit Application | Used to track applications to the Education program by Non-Profit groups that are not universities. Applies `non-profit` tag, assigns the ticket to you, and changes ticket status to `solved`. |
| Printfection Update | Used to tag order update emails from Printfection. Applies `printfection-update` and changes ticket status to `solved`. |
| Reddit::Follow-Up | Use when you respond on Reddit and are waiting for user to follow-up. Assigns the ticket to you, and changes ticket status to `pending`. |
| Reddit::Responded | Use when you have responded, and no follow-up is required via Reddit. Assigns the ticket to you and changes ticket status to `solved`. |
| Removed | Use when the mention of GitLab is removed by author.  Applies the `removed` tag, assigns the ticket to you, and changes ticket status to `solved`. |
| StackOverflow::Insufficient Information | Use when the StackOverflow post has insufficient information. Assigns the ticket to you and changes ticket status to `solved`. |
| StackOverflow::Responded | Use when you respond to the question/thread. Assigns the ticket to you and changes ticket status to `solved`. |
| StackOverflow::Solved | Use when the question has been answered. Assigns the ticket to you and changes ticket status to `solved`. | 
| StackOverflow::Unrelated/Non-Specific | Use when the question is unrelated or not specific to GitLab. Assigns the ticket to you and changes ticket status to `solved`. |
| Tag as education | Applies the `education` tag. |
| Tag as merchandise | Applies the `merchandise` tag. |
| Tag as open source | Applies the `oss` tag. |
| Tag as web-comment | Applies the `web-comment` tag.|
| Twitter::Are you still experiencing? | Use this macro to confirm whether a user is still experiencing the issue they tweeted about. Applies the `support` tag, assigns the ticket to you, and changes ticket status to `pending`. |
| Twitter::BugIssue | Use this macro to provide the user resources/direction to report a possible bug. Applies Tweet template "Sounds like a bug. You should open a bug report about it in https://gitlab.com/gitlab-org/gitlab/issues. We'd like to follow up on it." Applies the `bug` tag, assigns the ticket to you, and changes ticket status to `pending`. |
| Twitter::CurrentIssue | Use this macro when someone reaches out via Twitter about a current Service Incident. Applies Tweet template "Hello! We're sorry for the inconvenience. We're currently investigating this issue here:" Applies the `downtine` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Twitter::Downtime | Applies Tweet template "Sorry for the inconvenience. See the latest @gitlabstatus tweets for more info. Everything should be fine now." Applies `downtime` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Twitter::FeatureProposal| Use to encourage community to open feature proposal issues. Applies Tweet template "Could you open a feature proposal about that over at https://gitlab.com/gitlab-org/gitlab-ce/issues? We'd love to follow up on it." Applies the `feature-proposal` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Twitter::Incident Resolved | Use to follow up after GitLab incidents are resolved. Applies Tweet template "Hello! We're sorry for the inconvenience. The incident should be resolved now, please let us know if you're still experiencing any issues." Applies the `downtime` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Twitter:Retweet | Use to mark community member tweets that are retweeted by GitLab account. Applies the `retweet` tag, assigns the ticket to you, and changes the ticket status to `solved` |
| Twitter::Support | Use to follow up with support questions from paid users. Applies Tweet template "Could you please open a support ticket about that over at https://support.gitlab.com? We'd love to help you out." Applies the `support` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Twitter::SupportTracker| Use to follow up with support questions from free users. Applies Tweet template "Could you open an issue about that at https://gitlab.com/gitlab-com/support-forum/issues with as much info as possible? We'd love to follow-up on it." Applies the `support-forum` tag, assigns the ticket to you, and changes ticket status to `solved`.|
| Twitter::TweetDeckTweet| Tweet sent out from Tweetdeck. Applies the `tweetdeck` tag, assigns the ticket to you, and changes ticket status to `solved` .|
| Upvoted | Use on Reddit tickets when a post is upvocted but doesn't need a reply. Applies the `upvoted` tag, assigns the ticket to you, and changes ticket status to `solved`. |


## Zendesk ticket lifecycle