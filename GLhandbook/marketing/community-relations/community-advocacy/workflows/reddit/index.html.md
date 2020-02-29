---
layout: markdown_page
title: "Reddit response workflow"
---

## Overview

The purpose of this is to monitor all mentions of GitLab within Reddit.

<i class="fas fa-hand-point-right" aria-hidden="true" style="color: rgb(138, 109, 59)
;"></i> There is currently no way to filter whether the mention of GitLab is only from a URL ([example here](https://www.reddit.com/r/ProxyScrape/comments/a7p3je/help_us_translate/)), so there may potentially be a high volume of noise.
{: .alert .alert-warning}

<i class="fas fa-info-circle" aria-hidden="true" style="color: rgb(49, 112, 143)
;"></i> To request [user flair for the /r/gitlab subreddit](/images/handbook/marketing/community-relations/reddit-flair-example.png), ping `@advocates` in the `#reddit` Slack channel, and include your Reddit username. Your flair will read `GitLab Staff`.
{: .alert .alert-info}

## Workflow

1. Go through each ticket in Zendesk in the `Reddit` view

2. See if the comment or post has received a response

3. Respond if necessary using your **personal** Reddit account
   * Post the comment on the original website ([https://www.reddit.com/](https://www.reddit.com/), not Zendesk) using the link provided in the ticket
   * If needed, [ask an expert for help](/handbook/marketing/community-relations/community-advocacy/workflows/involving-experts)
   * Mark ticket as `On Hold` if you're waiting for an expert to reply
   * If your response asks a question or sparks conversation, mark the ticket as `Pending`
   * NOTE: Typically, the only posts that will need responses are those that are questions, support issues, feedback, or are spreading misinformation. Comments such as "I use GitLab and I love it!" should not be replied to as they would on other social media platforms.
   * Most new posts on the /r/gitlab subreddit should have responses.
4. If comment/post does not need a response but is still good or valuable, upvote it and apply the `Upvoted` macro
   * If it is particularly insightful or useful, it may be a good idea to share it on an appropriate Slack channel for visibility
   * If you see a comment you want all community advocates to upvote as well, start a thread on the particular comment in Slack and ping `@advocates`
5. Solve the ticket with the `Replied` macro (Replied macro will use the public response field in order to track the first reply time)

## Best practices

* Always be kind and understanding, no matter how the other person acts
* If you are new to Reddit, it may be useful to review this [beginner's guide](https://lifehacker.com/a-beginners-guide-to-reddit-1798643829)
* Use a **personal** reddit account, not a company one (although you may [request user flair here](https://gitlab.slack.com/archives/CELBBKQTZ/p1545233365007200)). It makes comments seem much more authentic
* If you use Reddit a lot, it may be useful to create a separate, more professional (but still personal) account
* Upvote good posts/comments
* Only downvote if a post is abusive or spreads false information. Don't just downvote because someone doesn't like the product or mentions a competitor
* [Brush up on your "reddiquette"](https://www.reddit.com/wiki/reddiquette)
* [Make sure your comments are formatted well](https://www.reddit.com/wiki/commenting)

## Automation

All mentions of GitLab, whether comments or new posts, are handled by Zapier. It first creates a ticket in Zendesk under the `Reddit` view, and then posts to the `#reddit` Slack channel.

<i class="fas fa-info-circle" aria-hidden="true" style="color: rgb(49, 112, 143)
;"></i> In Slack, new comments are posted by a bot with a blue icon by a bot called `Reddit Comment`, and new posts with an orange icon called `Reddit Post`.
{: .alert .alert-info}

There are often bot posts that include GitLab URLs that generate a lot of unwanted noise. There is a step in the Zapier automation that blacklists bots that do this. If you notice a large number of posts coming from a bot, please add it to the blacklist by following these steps in Zapier:
1. In Zapier, go to `Zaps` > `Community Advocacy` > `New Reddit Mention`
2. Go to the `Filter Noise` step
3. Select `Filter Setup & Testing`
4. Click `+ AND`
5. For the first dropdown, select `Username`
6. For the second, select `(Text) Does not exactly match`
7. In the third box, paste the name of the bot to exclude
8. Run a test and continue
9. Zapier automatically turns off processes that have been modified, so make sure you turn it back on
