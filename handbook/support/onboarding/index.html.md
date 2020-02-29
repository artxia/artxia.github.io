---
layout: handbook-page-toc
title: Support Onboarding
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Expectations of the Support Team
{: #expectations}

As members of the support team we are the first to interact with someone when they have a problem or question.
As such it is up to us to represent the company and make sure we present ourselves properly. Therefore we are
expected to:

- Always be friendly and respectful.
- Be open to new ideas and points of view.
- Be OK if you don't know something. You can always ask someone else.
- Be comfortable saying no to a customer. (But try to suggest a workaround and escalate to a Senior if necessary)

## Support Bootcamps
{: #se-bootcamp}

When you first join the team everything will be new to you. In order to get you
started with GitLab quickly a [Support Engineering Bootcamp Checklist](https://gitlab.com/gitlab-com/support/support-training/blob/master/.gitlab/issue_templates/Onboarding%20-%20GitLab.com%20Support%20Engineer.md) or [GitLab.com Support Agent Bootcamp Checklist](https://gitlab.com/gitlab-com/support/support-training/blob/master/.gitlab/issue_templates/Onboarding%20-%20GitLab.com%20Support%20Agent.md)
will be created for you to help guide you through your training.

## Tools

We use Zendesk to handle tickets, and we will sometimes schedule calls. That is most often done through Zoom, but can also be done through WebEx if the customer's system does not allow them to install the Zoom plugin.

### 1Password

Before your first day at GitLab, you'll ideally have created an account with 1Password, the password management tool that all GitLab team-members use. Any service that you'll need to log in to while performing your duties will have credentials stored in 1Password - it's all you need!

### Zendesk

We have several [workflows relating to Zendesk](/handbook/support/workflows/#Zendesk).

Tasks during onboarding include

- Setting up [unbabel](/handbook/support/workflows/unbabel_translation_in_zendesk.html)
- Add [a profile picture](https://support.zendesk.com/hc/en-us/articles/203690996-Updating-your-user-profile-and-password#topic_rgk_2z2_kh) to your Zendesk account
- Checking that, under your profile in Zendesk, it reads `Support Staff` and not `Light agent`

### Zoom

Zoom is a powerful and light-weight videoconferencing tool that works for 90% of customer calls (see the bit about WebEx for the other 10%). As part of your support boot camp, you should have received a Pro account there so that you can schedule your own calls. To start a call, log on to [gitlab.zoom.us](https://gitlab.zoom.us/) using your personal credentials and click on "My Meetings" for a link to your personal meeting room. Share this with the customer.

Zoom allows you to see the customer's desktop and
to control it on request; and it also offers the option of recording the call (we do not typically do this, be certain to ask for the customer's permission of you have a good reason for recording). It also gives the customer the possibility to join via phone and
us the possibility to use our computer audio connection.

### WebEx

For some customers, only Cisco systems are allowed and for those cases, WebEx will be the best tool for calls. To start a call / session use the `GitLab Support` WebEx account. Go to our
[WebEx Portal](https://gitlabmeetings.webex.com), click on the login button on the top right and use the
credentials found in the Support Vault on 1Password.

![WebEx Login](/images/support/web-ex-login.png)

Once logged in, click the `Enter Room` button to start the WebEx meeting and send the following link to
the customer and ask them to join the call.

```
https://gitlabmeetings.webex.com/meet/gitlabsupport
```

![WebEx Room](/images/support/web-ex-room.png)

>Note: Make sure you lock the meeting so that you (as the presenter) have to allow people in. Otherwise others may attempt to use the room.

WebEx allows you to see the customer's desktop and
to control it on request. It also gives the customer the possibility to join via phone and
us the possibility to use our computer audio connection.

## Handling tickets
{: #handling-tickets}

### Point to documentation, or make it
{: #document-it}

As a general rule, you should always include a link to the applicable documentation as
part of your response to a ticket. If the documentation does not exist yet, then
_make_ the documentation and send the link to the WIP MR in the response. For those situations
where making documentation is a more time consuming exercise, we have set up a process to automatically create an issue in our [Docs Project](https://gitlab.com/gitlab-com/support/docs) to track documentation tasks that need to be completed:

- Click the "Document this" checkbox (found on the left-hand side of the ticket)
- Enter an ["internal note"](https://support.zendesk.com/hc/en-us/articles/213519318-Adding-comments-to-tickets#topic_bpn_sbd_bv) describing the documentation requirements. Always start your private note with the word `Docs:`, include the title of your issue after the colon (:) and the description of your issue in a new line after four slashes (that are used to delimit the title from the description). Example: 

>`Docs: This is the title`
>
>`////`
>
>`This is the description of your issue`

- Submit the private note

When working on creating the new docs, please follow the [documentation styleguide](https://docs.gitlab.com/ee/development/doc_styleguide.html#location-and-naming-of-documents).

This workflow is implemented using a GCP functions as an intermediary between Zendesk and GitLab.

#### The GCP Documentation Function

In case you need to troubleshoot the function that creates new issues, you can find its logs in the GCP project `gitlab-internal` 
under `zendesk-support-doc-integration`.

The function uses the NodeJS runtime, and creates issues from the latest comment (sent from Zendesk). It assigns the issue to you based on your GitLab ID (also 
from Zendesk), and links back to the ticket using metadata provided, again, by Zendesk.

The title and body are separated by using the native `String.split()` method, with the four slashes acting as as delimiter. The array that is returned sends its 
first element (index `0`) as the issue title, and its second element (index `1`) as the issue description.

Due to constraints imposed by the GitLab application, if you do not include these slashes and your text is more than 255 characters, 
your issue may not be created properly because the entire text will be sent as a title. If this happens, check the logs in GCP and look 
for the following message:

`"{"message":{"title":["is too long (maximum is 255 characters)"]}}"`

This indicates that the delimiter was not applied properly - if this happens, check the formatting in your Zendesk comment and resubmit it.

### Create issues

During your interaction with the customers you will most likely need to create or update an
issue, either for a feature request, for a bug, or for further documentation.
Since we do everything in the open, it is good practice to send the link of the
issue to the requesting customer, so that they can also keep an eye on the discussion
there, and weigh in if necessary.


Workflow for creating an issue:

- Visit the issues page of the project, [example here](https://gitlab.com/gitlab-org/gitlab/issues)
- Search to make sure the issue doesn't already exist
- Click **New Issue**
- Choose a template from the **Choose a template** dropdown and take a look at the
**Typical kinds of issues created** below.
- Fill in all the relevant sections
- @mention someone in the issue to attract attention to it. Choose an expert [here](/company/team/) or feel free to ask
in the `#support-team-chat` channel on Slack who it should be reviewed by. Do not worry that you are poking
someone to review a job when you don't even know them and they might be much more senior than you,
if it's not appropriate for them, they will know the right person to pass it along to and do that.

Typical kinds of issues created:

- **Bug**
   - Make sure it looks like a bug - otherwise ping one of the developers to confirm.
   - Reproduce the bug
   - Report back to customer with a link to the issue
- **Proposed feature request**
   - Provide maximum information and use case from customer in the issue,
mention any alternatives, how badly the customer wants it.
   - Ask a developer for opinion (do we want this feature in GitLab: yes/no, the
developer might ask more questions before answer)
   - Report back to customer with a link to the issue

Typical workflow for updating an existing issue:

1. Comment on the issue that another customer is having a problem, adding relevant details
and a link to the Zendesk ticket. Also if it is an EE customer, add the `~customer`
label to the ticket.
1. Send the customer a link to the issue and invite them to comment.
1. If the customer replies with satisfaction that their concern is
being addressed after seeing the issue, ask them if it would be okay to mark
the ticket as resolved and to instead continue the conversation on the issue.

Sometimes it is helpful to create an issue on the [support issue tracker](https://gitlab.com/gitlab-com/support/support-team-meta/issues)
when dealing with a **tough ticket**. Creating an issue allows more people within
GitLab easy access to the questions and suggestions since not everyone is familiar
with Zendesk. When in doubt, create an issue. Also see the section on [getting help and escalating tickets](#getting-help-and-escalating).

### Ticket fields

The only custom ticket field we use is the `GitLab issues` field. In here you will fill in every
related GitLab issue that is related to this ticket as a way to cross-link between them.

Every issue you mention here must also contain a link to the ticket in question, either in the
description or in a comment.

Use this field as a reminder of when and where to follow up.

### Recording information about the organization
{: #fix-organization}

We use Zendesk Organization Profiles that are automatically generated by SFDC account information to store
relevant information about the customer, like Market Segment, Support Level, number of licenses and TAM (if applicable). If you need
this information, it is readily available from within Zendesk. To see this information, click on the
link to the left of the requester's name (in our example it's the link that says 'GitLab' right next to Haydn's name).

![Zendesk Organizations](/images/support/zendesk-org.png)


### After the first response
{: #first-response}

When you're expecting the customer to reply, the ticket should be
marked as `Pending`. If this ticket doesn't receive a reply within 4 days, the system will automatically
request an update from them. If we do not receive a reply within 7 days, Zendesk will automatically mark
the ticket solved. A customer can always re-open an issue, so this is just to keep our process tidy.

If a feature request or bug fix has been scheduled for a future release (signified by a Milestone), you should let the
customer know about the version for which this has been scheduled and when that version is going to be
released, e.g. June 22nd for 11.9.

Sometimes a customer will send an email to ask for a response to an issue that was
already created on a public issue tracker. In such
cases, include the link to the given issue in the "GitLab Issue" box, go ahead and
reply from the issue tracker, but also follow-up through Zendesk by providing a link
to your comment in the issue tracker. Providing the response to the customer is
what sets the "first response time" metric, and allows the tickets to be closed
when appropriate.

### Getting help and escalating tickets
{: #getting-help-and-escalating}

If you're stuck, don't hesitate to ask for help with a ticket. You can ask any of your colleagues for assistance by [@mentioning](https://get.slack.help/hc/en-us/articles/205240127-Using-mentions) (avoid using [@here](/handbook/communication/#chat)) them in any of the support Slack channels and providing a link to the ticket with an overview of the issue. You can also seek assistance from your fellow GitLab team-members outside of support in the `#questions` channel.

If a ticket must be escalated, please see the [Issue Escalations](/handbook/support/workflows/issue_escalations.html) workflow for in-depth details on how to do so.

### When to mark a ticket as solved
{: #when-solved}

A ticket can be marked as solved when you are certain that you were able to resolve the requester's
problem, or, as mentioned above, automatically when we haven't received a reply from the requester.

### Clearing out Suspended Tickets
{: #clear-suspended}

In Zendesk, various filters send a ticket straight to "suspended" status. This is mostly useful
to remove spam and it works quite well. However, it is possible that actual tickets
are accidentally routed to Suspended Tickets, so it is important to check the new Suspended Ticket queue
at least once a day. Doing this on a regular basis also keeps that queue manageable.

### Avoiding ticket collision
{: #avoiding-collision}

Since we work using a ["hot queue"](/handbook/support/workflows/working-with-tickets.html#hot-queue-how-gitlab-manages-ticket-assignments) system, it's important to be mindful of whether or not another team member is already working on a ticket that you're interested in taking on. Be sure to check out [this section](/handbook/support/workflows/working-with-tickets.html#what-if-someone-is-working-on-a-ticket-that-id-like-to-work-on) for information on recognizing when another team member may already be working on a ticket that you'd like to work on.

### Update agent signature
{: #agent-signature}

Your personal Zendesk signature is shown at the end of every ticket response.
You can update this to include a personalized valediction like "Thanks" or "Best Regards" by following these steps.

* In Zendesk, click your user icon in the upper-right corner and select View Profile.
* Under Signature in the left sidebar, enter the signature text.

An example agent signature:

```
{{agent.name}}
{{agent.role}}
GitLab, Inc.
```
You can add e.g. `Thanks` or `Best` to your signature, but it's better to always end your message with an applicable and friendly text. 

### How to handle emails forwarded from others at GitLab

Every now and then, a GitLab team-member will forward a support request from a customer, prospective customer, user, etc. These requests then appear as tickets from the team member, instead of from the original requestor. Always reply directly to the original requester, keeping the person who forwarded it in the cc. You will need to manually alter the "Requester" field of the ticket, by clicking on the "(change)" link next to the email address of the apparent requester in the ticket title.

## Receiving feedback
{: #feedback}

After 24 hours of marking the ticket as solved a survey is sent to our customers, where they can rate
the level of support they received. If a customer rates a ticket to which you were assigned as bad, an
email will be sent to you and the Zendesk manager to notify you of the fact. When this happens, you should
let a Senior know about the problem and follow up with the customer to see if something you did can
be improved.

You will also receive a message if the feedback is positive, and it is encouraged to
celebrate those "wins" with the rest of the team through the #support-team-chat or #thanks
chat channel. Read the positive feedback carefully, often it contains a question
or suggestion for improvement which should be followed up on.

If a customer has useful feedback, please follow the [Feedbacks and Complaints Workflow](/handbook/support/workflows/feedbacks_and_complaints.html).


## Customer Calls Best Practices

### Before a Call

After sending the call link, go to the ticket and ask for confirmation. Having the customer confirmation will also help to detect errors on the scheduling process such as an incorrect timezone, date, etc.

Add the call with description and duration to the Support Team Calendar.

### During a Call

Once you have started the call and the client connects, identify yourself. Example:

> Hi {customer name}, this is {agent name} from GitLab Support.

If you started the call and the client doesn't join, wait for a couple minutes. After 10 minutes of waiting
go to the ticket and send a reply to check if the customer is having either issues with the scheduled time
or connecting.

If after another 5 minutes you don't get answer, go ahead and re-schedule.

If a call takes too long (> 1 hour), and/or if you're not making progress, discuss with the customer the need to schedule a follow-up session.

+ If you were having problems helping the customer, make sure to contact a teammate to join you on the follow-up call (Call Escalation)
+ If the customer had problems either with their setup, environment, or connectivity, remind them to solve them before the new
call when re-scheduling or before the follow-up session.

### After a Call

Update the ticket with a brief description of what was accomplished or not during the call, making sure to point out the missing
information to solve the ticket.

## Keeping up to date with new GitLab versions

Since we ship a new release each month on the 22nd, and since we manage to fit _a lot_ of great new features and fixes into each release, it is sometimes difficult for the Support Team to keep up to date with key changes.

In general, it is the responsibility of each Support Team member individually to read the release blog post, dig deeper where you need to or want to, and keep yourself up to date. However, to facilitate this further, we have a Retrospective every month (it is listed on the GitLab Team Meetings calendar).

## Taking Time Off

You're encouraged to take advantage of GitLab's time off policy. Before taking time off, it's important that you ensure that any tickets awaiting your attention on the days that you'll be out will be handled by another team member.

Details on how to take time off and more can be found in the [time off section](/handbook/support/#time-off).

### Illness and Unforeseen events

You should always take care of yourself and make sure you are healthy. If you need to take a sick day or have something urgent to take care of, let your team members know via `#support-team-chat` Slack channel. If you have a call scheduled, ask one of your colleagues to take the call on your behalf or they can reschedule the call for you.
