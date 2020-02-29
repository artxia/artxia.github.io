---
layout: handbook-page-toc
title: "Twitter response workflow"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

### Handles

| HANDLE | RESPOND FROM | GUIDELINES |
| - | - | - |
| [@GitLabStatus](https://twitter.com/GitLabStatus) | Zendesk | Post service updates |
| [@GitLab](https://twitter.com/GitLabs) | Zendesk | Respond to mentions and questions |
| [@MovingToGitLab](https://twitter.com/MovingToGitLab) | Tweetdeck | Respond to mentions and questions |

- The [@GitLabStatus](https://twitter.com/GitLabStatus) account should only be used to give updates on the availability of [GitLab.com](https://gitlab.com) and to follow up on users reporting that [GitLab.com](https://gitlab.com) is unavailable or responding to a previous availability update on [@GitLabStatus](https://twitter.com/GitLabStatus).
- Only the infrastructure team should be posting updates on [@GitLabStatus](https://twitter.com/GitLabStatus). There is a [defined process](/handbook/engineering/infrastructure/team/reliability/incident-management/) for this describing who should do this, how and what channels should be alerted.
- When a tweet mentions more than one handle described above, always reply from the main [@GitLab handle](https://twitter.com/GitLab), unless it's about GitLab availability status
- If a wrong handle is used in a response, take note and respond from the correct one in the follow-up (if there is one)

## Workflow

<i class="fas fa-hand-point-right" aria-hidden="true" style="color: rgb(138, 109, 59)
;"></i> All initial Twitter responses should be sent from Zendesk. If a follow up tweet from a user warrants a response, follow the Tweetdeck workflow below.
{: .alert .alert-warning}

- Reply to almost all tweets, following the [social media guidelines](/handbook/marketing/social-media-guidelines/), regardless of whether the tweet is of a technical nature or not.
- Follow up with the support team if the issue is too complex to handle.

When resolving Twitter tickets in Zendesk you should:

1. Use [Play mode](https://support.zendesk.com/hc/en-us/articles/203690856-Working-with-tickets#topic_avj_hfg_vt) in the Twitter view. The default Twitter view will sort tickets by created date (ascending).
1. Not skip any tickets
1. Assign the ticket to yourself or ask in the appropriate chat channel if you don't know how to answer it
1. Not cross assign tickets

## Best practices

## General

- Tweets use short links which require you to visit that link to make sure you understand the context.
- Clarify if the request refers to GitLab.com or an externally hosted GitLab instance as we can only handle requests for [GitLab.com](https://gitlab.com).

### Reports of Spam

Users might take to Twitter to report instances of spam on the [GitLab.org Issue Board](https://gitlab.com/gitlab-org/gitlab/issues). To report this, post in the [#abuse slack channel](https://gitlab.slack.com/messages/abuse) with a link to the issue board and the timing of the spam report. Respond to the user and thank them for getting our attention on the issue.

The same workflow can be applied for spam reports that come through on other social channels, however, Twitter is the most common place for these reports.

### Usage of Likes

Use "Likes" on Twitter for promoting positive feedback about our product, since we direct users there when we want to show that people really love the product. Avoid using it for anything else.

### Retweeting

Advocates shouldn't retweet anything from the official GitLab Twitter accounts. If you see something that should be retweeted, paste the tweet in [`#social_media` Slack Channel](https://gitlab.slack.com/archives/C4UGNMF9A) for the social team to review.

### Direct Messages

We have direct messages disabled in our Twitter accounts, but they can be used if we first send a direct message to a user. This should only be used when the user needs to communicate with us privately (e.g. to give a mailing address).

## Automation

Tweets that mention [@GitLab](https://twitter.com/GitLab), or [@GitLabStatus](https://twitter.com/GitLabStatus) will create a ticket in Zendesk, and show up in the "Twitter" view.

If a tweet is responded to from TweetDeck, this risks duplicate responses. Responding from Zendesk also enables us to track our response times vs. [our internal SLA](/handbook/support/#sla).

## Tweetdeck

The Twitter/Zendesk integration does not correctly thread Twitter conversations. Follow-up tweets sent via Zendesk will appear as a response to the user's first tweet rather than any subsequent tweets. To work around this, advocates use Tweetdeck to respond directly from the @Gitlab account.

If a user's response to your initial tweet sent from Zendesk warrants a response, open the tweet in Tweetdeck. Respond directly to the tweet via Tweetdeck. Add a link to your response in an internal note on the Zendesk ticket.

Tweetdeck can also be used to delete tweets if something is sent accidentally from Zendesk.

