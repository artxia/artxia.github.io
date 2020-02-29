---
layout: handbook-page-toc
title: Product Communication
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Other Product Handbook pages
{:.no_toc} 

## Communication

- [**Public Issue Tracker**](https://gitlab.com/gitlab-org/gitlab/issues) - please use
confidential issues for topics that should only be visible to team members at GitLab.
- [**Chat channel**](https://gitlab.slack.com/archives/product) - please use the
`#product` chat channels for questions that don't seem appropriate for the
issue tracker or more generic chat channels.

### Internal and external evangelization

Before shipping a new or updated feature, you are responsible for championing
it, both internally and externally. When something is released, the
following teams need to be aware of it as they will all need to do something
about it:

* Marketing: depending on the importance of the feature, we need the help of
marketing to promote this feature on our different communication channels.
* Sales: sales needs to know what's new or changed in the product so they can
have better arguments to convince new or existing customers during their sales
process.
* Support: as they are in constant contact with our users and customers,
support should know exactly how our products work.

You can promote your work in several ways:

* start with documenting what will be released and share this documentation with
the different teams
* schedule meetings, if you think it's important, with the teams listed above.

### Working with Product Marketing (PMM)

Product marketers and managers should be joined at the hip. Just as a feature without documentation
should not be considered shipped, benefits of GitLab that we're not actively talking about might
as well not exist.

Product marketers rely on product managers to be guided to what is important and high impact.
In general, you should:

- always mention the [appropriate PMM](/handbook/product/categories) on epics and high level issues
- regularly meet/talk async with the PMM that is aligned with your product area
- proactively reach out for input when contemplating new features
- involve PMM as early as possible with work on important changes

### Marketing materials

As a PM you're responsible for making sure changes you've shipped are well represented
throughout GitLab's documentation and marketing materials. This means that on
release, [`features.yml`][features] is updated, documentation is merged and deployed, and
any existing content is updated where necessary.

It's not acceptable to do this after the release. GitLab is very complex, and features
and functions are easily missed, even those that provide significant value to customers
(e.g. the many ways you can authenticate with GitLab).

You can recruit the help of the marketing and technical writing team if needed,
but it's highly recommended to do small updates yourself. This takes less time
and overhead than communicating what needs to be done to someone else.

### Major feature rollout

Major features deserve proper attention from Product and Marketing. With a
proper rollout, we'll have ample marketing opportunities and receive more
feedback ahead of, during, and after the release.

Here is the ideal rollout schedule. For each step there is an indication for
who is responsible for it.

1. Feature is drafted in an epic or issue (PM)
1. Feature is planned in an upcoming release (PM)
1. A feature proposal blog post is made (PM or Dev), which includes:
	* What we are planning on doing.
	* How people will be able to get it: CE or any EE Editions.
	* A link to the issue.
	* When it'll be available, if possible.
	* Anything else that is interesting to share in order to fuel the discussion.
1. Feature is implemented, and documentation is written (Dev).
1. Feature should appear on the website (Marketing)
	* For very significant features: Feature page on the website is made and
      pushed, with the mention "Available from X.X"
	* For other features: Feature should be listed on some page (/devops-tools,
      Enterprise page, /features page).
1. Feature is launched with the release (Marketing)
	* "Available from X.X" is removed
	* Documentation and other resources are linked
	* Pricing page is updated if needed
1. Feature is highlighted in a blog post (Marketing)
	* This post is linked from the feature page on the website (if applicable)

### Release posts

As a PM, you are [accountable](/handbook/marketing/blog/release-posts/#general-contributions)
for adding new features (under your umbrella) to the monthly release post, respecting the
guidelines defined in the
[release posts handbook](/handbook/marketing/blog/release-posts/) and its **due dates**.
Be sure to go over all the details.

Every month, a PM will take the
[leadership](/handbook/marketing/blog/release-posts/#authorship)
of the release post, and will be responsible for delivering it in time.

### Writing release blog posts

For every monthly release, there is a blog post announcing features.
The blog post should contain everything _exciting_ or _disruptive_.
All new features should appear in the blog post.
We want to help people understand exciting features (which are often new), and increase adoption.
Disruptive features may significantly improve workflows or occasionally introduce unavoidable inconveniences.
We want to anticipate questions and avoid confusion by communicating these changes through the blog post.
UX improvements that significantly adjust current workflow should be included.
Smaller tweaks and bug fixes don't necessarily need to be mentioned, but if interesting, can be included at the bottom of the post.

### Writing about features

As PMs we need to constantly write about the features and upgrades we ship: in a blog post,
internally to promote something, and in emails sent to customers. There are some
guidelines that one should take into account when writing about features, 
the most important being a clear communication of the problem we're solving for users.

When writing about a feature, make sure to cover [these messaging guidelines](https://about.gitlab.com/handbook/marketing/blog/release-posts/#messaging-review) 
which help produce clear internal and external
messaging.

Let's highlight the messaging guidelines mentioned above with a concrete example, Preventing Secrets in your repositories,
 that [we shipped in 8.12](/blog/2016/09/22/gitlab-8-12-released/#preventing-secrets-in-your-repositories-ee).

* Start with the context. Explain what the current situation is without the
  feature. Describe the pain points and connect back to our [Value Drivers](/handbook/marketing/#go-to-market-value-drivers-and-customer-use-cases) (in this case `Reduce Security and Compliance Risk`).

> It's a bad idea to commit secrets (such as keys and certificates) to your
repositories: they'll be cloned to the machines of anyone that has access to the
repository. If just a single one is insecure, the information will be
compromised. Unfortunately, it can happen quite easily. You write
`git commit -am 'quickfix' && git push` and suddenly you've committed files that
were meant to stay local!

* Explain what we've shipped to fix this problem.

> GitLab now has a new push rule that will prevent commits with secrets from entering the repository.

* Describe how to use the feature in simple terms.

> Just check the checkbox in the repository settings, under push rules and
GitLab will prevent common unsafe files such as .pem and .key from being committed.

* Point to the documentation and any other relevant links (previous posts, etc).

Here are some additional examples of well written release blog posts for inspiration: 

- [Issue Board Work In Progress Limits](https://about.gitlab.com/releases/2020/02/22/gitlab-12-8-released/#issue-board-work-in-progress-limits)
- [Parent-Child Pipelines](https://about.gitlab.com/releases/2020/01/22/gitlab-12-7-released/#parent-child-pipelines)
- [Drag-and-drop Design badges](https://about.gitlab.com/releases/2020/02/22/gitlab-12-8-released/#drag-and-drop-design-badges)
- [Render charts in GitLab issues using a Grafana URL](https://about.gitlab.com/releases/2019/11/22/gitlab-12-5-released/)

### Recording videos to showcase features

In addition to the written medium, video is an important medium that caters to a different learning style.
Depending on the type of video you are recording, there are some guidelines to keep in mind.

**Speed Run:** Informal video meant to focus on a single workflow and the experience for performing that workflow.
It should not require much planning and is typically short in duration (less than 5 min.). This video type is meant
to inform and not necessarily to influence buyers.

See the [Remove docker images via CI/CD speed run](https://youtu.be/jDlFCrH9H7g) video for an example.

**Walk-through:** Informal video meant to focus on cohesiveness across categories and workflows. Requires a bit more
planning than a speed run but doesn't require high production value. These are typically longer in length as they cover
more ground.

See the [Auto DevOps setup and usage walk-through](https://youtu.be/V4NX2j2HQAs) video for an example.

Product Directors are expected to produce a walk-through across their stages at least once per quarter.

**Demo:** Scripted recording meant to influence buyers. Generally has higher production value and typically involves
both a slide-style presentation and/or live screen-sharing. Duration varies depending on the topics being covered.

See the [GitLab for the Enterprise Demo](https://youtu.be/aIYLxMXQiLI) video for an example.

### Including epics

One situation that can happen is that an epic contains many small issues that don't individually
meet the bar for the `direction` label, and therefore inclusion in the release post. More rarely, the last
issue of an MVC that took several releases isn't necessarily a capstone issue on its own. If you find yourself
in a situation where you have closed an epic during a release, you should also ensure that we communicate that
as a combined entity in a feature block, even if there is otherwise no single issue to mention.
