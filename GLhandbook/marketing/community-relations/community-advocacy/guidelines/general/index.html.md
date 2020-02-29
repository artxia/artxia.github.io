---
layout: handbook-page-toc
title: "General guidelines"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Handling mentions

### Urgent and important mentions

It's important to be able to recognize events that are both _important_ **and** _urgent_. Some might be important but not urgent, others urgent but not important while some are neither important nor urgent. However, mentions that are both urgent and important should be handled as top priority. [HackerNews](#hacker-news) is a channel that commonly sees this type of mentions.

* **Important mentions** are mentions whose content bears a lot of weight and is important to the company - it's often content about our policies, product and/or marketing pieces (blog posts, articles, etc.)
* **Urgent mentions** are mentions whose content is time-sensitive by nature - often when the spotlight and discussion enthusiasm are perishable - such as HackerNews threads

These mentions might be intimidating and/or hard to answer by yourself. Please [involve several topic experts](/handbook/marketing/community-relations/community-advocacy/workflows/involving-experts) to respond instead.

When this type of mention comes up during a weekend, please ping more people than you would usually do. It's not considered rude (anyone and everyone can always snooze Slack notifications during weekends), you're just increasing the chance someone sees it in time.

#### Examples

|Mention|Important|Urgent|Explanation|
|-|-|-|-|
|<https://news.ycombinator.com/item?id=17032274>|✖|✖|The OP mentions GitLab out of context.|
|<https://news.ycombinator.com/item?id=17101902>|✖|✓|This required an urgent response because the thread momentum was very perishable.|
|<https://news.ycombinator.com/item?id=16914775>|✓|✖|The OP expressed dissapointment with his support experience - This is important to address, but not time sensitive (a one or two hour response time woudln't have any difference in impact compared to a 6h response time).|
|<https://news.ycombinator.com/item?id=13537052>|✓|✓|Content is volatile and affects a lot of users and the company image. This needed to be addressed as soon as possible and with care.|

## Community interaction archetypes

### Stability complaints

- Apologize for the inconvenience
- Search for an active issue that could be the cause of instability (deployment downtime, load spikes, ...)
    - [Sentry](https://sentry.gitlab.net/gitlab/)
    - [Infrastructure Issue Repository](https://gitlab.com/gitlab-com/infrastructure/issues/)
    - [`production`](https://gitlab.slack.com/messages/production) Slack channel
- Determine if the user is still affected
- Link to the relevant issue

### Feature requests

- Analyze the request
- Open an issue for it
- Thank the user for the contribution (See [our Social Media Guidelines](/handbook/marketing/social-media-guidelines/))
- Link back to the community member to provide further feedback on the issue

### General questions and issues with gitlab.com

- Gauge the complexity of the question
- Search related issues / documentation
    - [GitLab CE Issues Tracker](https://gitlab.com/gitlab-org/gitlab-ce/issues/)
    - [GitLab Documentation](http://docs.gitlab.com/)
- Forward to [GitLab Support Forum](https://gitlab.com/gitlab-com/support-forum/issues/)

### Bug reports

- Reproduce the bug
- Open an issue
    - [GitLab CE Issues Tracker](https://gitlab.com/gitlab-org/gitlab-ce/issues/)
    - [GitLab EE Issues Tracker](https://gitlab.com/gitlab-org/gitlab-ee/issues/)
    - Label the issue
- Link back to the community member
- (Optional) Link in the appropriate chat channel

### General positivity

Tweets expressing positivity about GitLab.

- Like the message
- Respond positively

Sample responses:

- "Thanks for using GitLab."
- "Thanks for writing about GitLab."

### Others

- If somebody is mentioning GitLab as part of a group message -> Use the `Mention` ZenDesk macro
- For posts about remote jobs and other kind of announcements that aren't strictly related to GitLab -> Use the `Mention` ZenDesk macro

- EE Customer issues / GitHost customers / anyone who cannot access GitLab.com (including 2FA reset queries) -> Forward to [Support](https://support.gitlab.com)
- For issues related to our marketing site -> Forward to [www-gitlab-com Issue Tracker](https://gitlab.com/gitlab-com/www-gitlab-com/issues)
- For issues related to self-managed instances -> Forward to [Community Forum](https://forum.gitlab.com)

- Non-English Tweets -> Use the `Non-English` ZenDesk macro

### Special types

- Event Sponsorship Requests -> Forward to [emily@gitlab.com](mailto:emily@gitlab.com)
- Spam -> Mark as spam
- GitLab package reported as compromised -> [immediately stop packagecloud via Slack](https://gitlab.com/gitlab-com/runbooks/blob/master/howto/stop-or-start-packagecloud.md)
- Any kind of political questions / remark (even if they're just asking if we're politically neutral or not) -> Do not respond (They tend not to be productive.)

## External resources

When responding to community messages, you may face a situation where our documentation doesn't have an official solution. In these circumstances, you can consider replying with a link to an external resource.

Before that, consider documenting the missing piece. It is time-consuming, but it saves time for both you and your colleagues when this comes up again. Respond after updating the documentation. This approach encourages immediate documentation improvements/edits, and it allows avoiding all external resources. If you have any questions about writing the documentation, ask the relevant Technical Writer or Product Manager. When your content is ready, assign it to one of them for review.

If you determine that this question is too specific for our documentation and decide to use an external resource, please make sure that:
* The author has a solid reputation - we don't want to share suspicious posts
* The post isn't related to [countries we don't do business in](/handbook/sales-process/images_sales_process/#export-control-classification-and-countries-we-do-not-do-business-in-)

## Notes / remarks

- When asking something in Slack that's relevant for a ticket, leave a link to the chat message as an internal comment in the ticket
- Always be sure to check if an issue (bug or feature proposal) exists before opening one / asking a user to open it
