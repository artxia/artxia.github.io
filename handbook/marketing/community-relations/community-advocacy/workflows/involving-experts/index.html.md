---
layout: handbook-page-toc
title: "Involving experts workflow"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

When responding to community messages, you should always strive to involve a resident GitLab expert on the subject if possible.

This gives:

* a higher quality of answers
* shows that our whole company is committed to helping people
* the expert receives more feedback from users
* opportunity to build relationships between community and GitLab team members

## Workflow

Refer to the [Product stages, groups, and categories page](https://about.gitlab.com/handbook/product/categories/#devops-stages) to locate the appropriate expert/team.

Please mention the expert by name in the relevant Slack channel (e.g. in `#frontend` if it's a frontend question) with the following template. If you are unsure of the correct channel, you can ping the experts in the [`#questions`](https://gitlab.slack.com/messages/questions) channel.

For expert responses on blog posts, first check if the blog author is a GitLab team member, and reach out to them directly. If the blog author is not a GitLab team member, the content team may be able to help connect you over email. 

<i class="fas fa-info-circle" aria-hidden="true" style="color: rgb(49, 112, 143)
;"></i> If you are working on a mention that requires an expert from a particular [devops stage](/handbook/product/categories/#devops-stages), you can find them in the Slack channels named `#s_<devopstage>` (e.g. `#s_plan`, `#s_verify`, etc.).
{: .alert .alert-info}

### Expert Involvement Template

```plain
@expert_username [LINK TO COMMUNITY COMMENT]
Hello! I need support from an expert to respond to this. Can you please answer on [name of social platform] using your personal account? Even if you are in a rush, remember - your direct response is a better experience for you and the requestor! If you don't know the answer, could you share your thoughts and ping a specific expert who might? We're trying to make sure every comment gets a response. Thank you! https://about.gitlab.com/handbook/marketing/community-relations/community-advocacy/#can-you-please-respond-to-this
```

* After reaching out to experts via slack, add the Slack outreach link as an internal note and submit Zendesk ticket as 'Open'.
* Consider responding yourself via the @gitlab handle through Zendesk with as much information as you currently have while you're waiting for the expert. This will enable us to engage with the user faster and assure them that our team will get back to them with more details soon. 
* Apply the 'Expert Responded' macro to the Zendesk Ticket to automatically solve the ticket.


If there is no Zendesk ticket related to the mention (e.g. a HackerNews mention) track it in the [`#community-relations`](https://gitlab.slack.com/messages/community-relations) Slack channel.

## Metrics

### Slack
* The template above has the keyword phrase 'support from an expert' for ease of searching in Slack.
* Search slack using keyword phrase 'support from an expert' to track total number of times advocates reached out to experts

### Zendesk
* Tickets are solved with the `expert-responded` macro and tag.
* In Zendesk, navigate to the Reporting -> Insights section. Scroll down to the sections titled 'Tags with rising usage' and 'Tags with falling usage'.
* Here, you can see usage of the `expert-responded` tag in the past 30 days. You can also filter the data by view to study usage of the tag in individual Zendesk views.
* Advocates can use this number compared with the total tickets created per month to find the percentage of GitLab mentions that are responded to by an expert.
* To see total all-time usage of the `expert-responded` tag in Zendesk, navigate to the Admin section and choose Tags. Click on the `expert-responded` tag to view all tickets solved with this macro.


## Best practices

When trying to figure out who has expertise on what segment of the product, refer to the ["DevOps Stages"](/handbook/product/categories/#devops-stages) section of the [Product stages, groups, and categories](/handbook/product/categories/) page in the handbook. The [team page](/company/team/) can also be useful.

## Automation

TBD: Zendesk
