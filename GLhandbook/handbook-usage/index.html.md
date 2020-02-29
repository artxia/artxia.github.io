---
layout: handbook-page-toc
title: "GitLab Handbook Usage"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Flow structure

1. A (process) problem comes up, frequently in an issue or chat.
1. A proposal is made in a merge request to the handbook.
1. Once merged, the change is announced by linking to the diff in the MR or commit. Major ones are put in the agenda of the company call. Medium ones are posted in the #handbook channel for visibility, with a one line summary of the change. If there was an issue, close it out with a link to the diff.

Sometimes you want to have real time editing of a proposal during a meeting and you need to use a Google Doc for that. When doing so the first item should be the URL of the handbook page this content will be moved to when the meeting is over.

## Why handbook first

Documenting in the handbook before taking an action may require more time initially because you have to think about where to make the change, integrate it with the existing content, and then possibly add to or refactor the handbook to have a proper foundation. But, it saves time in the long run, and this communication is essential to our ability to continue scaling and adapting our organization.

This process is not unlike writing tests for your software. Only communicate a (proposed) change via a change to the handbook; don't use a presentation, email, chat message, or another medium to communicate the components of the change. These other forms of communication might be more convenient for the presenter, but they make it harder for the audience to understand the context and the implications for other potentially affected processes.

Having a **"handbook first"** mentality ensures there is no duplication; the handbook is always up to date, and others are better able to contribute. 

<!-- blank line -->
<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/EuGsen3FxXc?start=991" frameborder="0" allowfullscreen="true"> </iframe>
</figure>
<!-- blank line -->

When asked during an [INSEAD](http://insead.edu/) case study interview (shown above) about challenges related to being all-remote, GitLab co-founder and CEO Sid Sijbrandij provided the following reply.

> The biggest problem is GitLab not working handbook first. We have an amazing handbook that allows us to collaborate, onboard new people, and think collectively.
>
> However, it is counterintuitive to communicate changes to the handbook. The default of people, when they wish to communicate a change, is to send a Slack message, send an email, give a presentation, or tell people in a meeting — *anything* but make a change in the handbook.
>
> It's slower for them. It's quicker to use any other form. If they make a change in the handbook, they first have to find the relevant part of the handbook, they sometimes have to adjust the handbook to make sure their change will fit in, they have to go through a technical process and a review or two, and they have to wait a bit before it's deployed. 
>
> It's slower than any other option. However, it allows people that commit a change after that to build upon a change. When they take that extra time, it's building a foundation for the next thing.
>
> I think of it as brick laying. Every piece of information is a brick. At GitLab, there is a well-structured house, and everyone adds to that one house. Because we're pretty particular on how we build it, it has a strong foundation and we can build it very high.
>
> In every other company, they send the brick into the hands of people. Everyone is receiving bricks daily that they have to add to the house they're building internally. They forget things and things are unclear. A lot of context has to be created because there is no context around where to place the bricks.
>
> So, you can end up with a thousand houses that look quite different, that are all hanging a bit, and each time you add a brick to the top one pops out at the bottom. — *GitLab co-founder and CEO Sid Sijbrandij*

## Handbook guidelines

Please follow these guidelines and remind others of them.

### How we use the guide every day
1. Most guidelines in this handbook are meant to help, and unless otherwise stated, are meant to help more than being absolute rules. Don't be afraid to do something because you don't know the entire handbook, nobody does. Be gentle when reminding people about these guidelines. For example say, "It is not a problem, but next time please consider the following guideline from the handbook."
1. If you ask a question and someone answers with a link to the handbook, they do this because they want to help by providing more information. They may also be proud that we have the answer documented. It doesn't mean that you should have read the entire handbook, nobody knows the entire handbook.
1. If you need to ask a team member for help, please realize that there is a good chance the majority of the community also doesn't know the answer. Be sure to **document** the answer to radiate this information to the whole community. After the question is answered, discuss where it should be documented and who will do it. You can remind other people of this request by asking "Who will document this?"
1. When you discuss something in chat always try to **link** to a URL where relevant. For example, the documentation you have a question about or the page that answered your question. You can remind other people of this by asking "Can you please link?"
1. Remember, the handbook is not what we hope to do, what we should formally do, or what we did months ago. **It is what we do right now.** Make sure you change the handbook in order to truly change a process. To propose a change to a process, make a merge request to change the handbook. Don't use another channel to propose a handbook change (email, Google Doc, etc.).
1. The handbook is the process. Any sections with names like 'process', 'policies', 'best practices', or 'standard operating procedures' are an indication of a deeper problem. This may indicate a duplication between a prose description of a process and a numbered list description of the same process that should be combined in one description of the process.
1. When communicating something always include a link to the relevant (and up-to-date) part of the **handbook** instead of including the text in the email/chat/etc. You can remind other people of this by asking "Can you please link to the relevant part of the handbook?"
1. Everyone should subscribe to the #handbook channel to stay up-to-date with changes to the handbook


### How to change or define a process
1. To change a guideline or process, **suggest an edit** in the form of a merge request.
After it is merged you can talk about it during the company call if applicable. You can remind other people of this by asking "Can you please send a merge request for the handbook?"
1. When substantially changing handbook layout, please leave a link to the specific page of the review app **that is directly affected by this MR**. Along with the link, include as much info as possible in the MR description. This will allow everyone to understand what is the purpose of the MR without looking at diffs.
1. Keeping up with changes to the Handbook can be difficult, please follow the [commit subject guidelines](https://docs.gitlab.com/ee/development/contributing/merge_request_workflow.html#commit-messages-guidelines) with a particular focus on your merge request's title, to ensure someone reading the [Handbook Changelog](/handbook/CHANGELOG.html) can quickly understand the MR's content. 
1. Communicate process changes by linking to the **merged diff** (a commit that shows the changes before and after). If you are communicating a change for the purpose of discussion and feedback, it is ok to link to an **unmerged diff**. Do not change the process first, and then view the documentation as a lower priority task. Planning to do the documentation later inevitably leads to duplicate work communicating the change and it leads to outdated documentation. You can remind other people of this by asking "Can you please update the handbook first?"
1. Like everything else, our processes are always in flux. Everything is always in draft, and the initial version should be in the handbook, too. If you are proposing a change to the handbook, whenever possible, **skip the issue and submit a merge request**. (Proposing a change via a merge request is preferred over an issue description). Mention the people that affected by the change in the merge request. In many cases, merge requests are easier to collaborate on since you can see the proposed changes.
1. **If something is a limited test** to a group of users, add it to the handbook and note as such. Then remove the note once the test is over and every case should use the new process.
1. If someone inside or outside GitLab makes a good suggestion invite them to add it to the handbook. Send the person the URL of the relevant page and section and offer to do it for them if they can't. Having them make and send the suggestion will make the change and will reflect their knowledge.
1. When you submit a merge request, make sure that it gets merged quickly. Making single, small changes quickly will ensure your branch doesn't fall far behind master, creating merge conflicts. Aim to make and merge your update on the same day. Mention people in the merge request or reach them via Slack. If you get a suggestion for a large improvement on top of the existing one consider doing that separately. Create an issue, get the existing MR merged, then create a new merge request.
1. If you have to move content have a merge request that moves it and does nothing else. If you want to clean it up, summarize it, or expand on it do that after the moving MR is merged. This is much easier to review.
1. Try to **add the why of a handbook process**, what is the business goal, what is the inspiration for this section. Adding the why makes processes easier to change in the future since you can evaluate if the why changed.


### Style guide and information architecture
1. **Single Source of Truth** Think about the information architecture to eliminate repetition and have a Single Source of Truth (SSoT). Instead of repeating content cross-link it (each text has a hyperlink to the other piece). If you copy content please remove it at the origin place and replace it with a link to the new content. Duplicate content leads to having to update it in multiple changes, which is a lot of work and very easy to forget. If you forget one of the pieces of content is out of date.
1. Make sure to always cross-link items if there are related items (elsewhere in the handbook, in docs, or in issues).
1. The handbook is **organized by function and result** to ensure every item in it has a location and owner to keep it up to date.
 * It's essential that we adhere to this hierarchy and that we not maintain separate structures for company training materials (e.g. onboarding materials, how-tos, etc.), videos, or other documentation.
 * Adhering to this hierarchy is sometimes counter-intuitive.
   We've learned over the years that keeping content in context helps to ensure consistency when making future updates.
 * At times, a change of perspective may be desired.
   In those cases, link to relevant sections of the handbook but don't include the content itself.
   See the [onboarding template](https://gitlab.com/gitlab-com/people-ops/employment/blob/master/.gitlab/issue_templates/onboarding.md) as an example.
   Or for example a list of [Key Performance Indicators](/handbook/business-ops/data-team/metrics/) that links to performance indicators but doesn't duplicate definitions.
 * **Avoid unstructured content based on formats like FAQs, lists of links, resource pages, glossaries, courses, videos, tests, processes, standard operating procedure, or how-to's.**
   These are very hard to keep up-to-date and are not compatible with organization per function and result.
 * Instead, put the answer, link, definition, course, video, or test in the most relevant place. Use descriptive headings so that people can easily search for content.
 * That said, please mix *formats* where and when appropriate in the handbook, even within a single page. Utilizing multiple formats can be valuable, and different people may prefer certain formats over others.
 * Worry only about the organization **per function and result**, not about how the page will look if you embed varying types and formats of content.
1. **Use headings liberally**. If a page includes more than two headings (especially if it's larger than a single "screen"), add an automatically generated Table of Contents (ToC) by copying [line 6 to 10 in this MR](https://gitlab.com/gitlab-com/www-gitlab-com/merge_requests/7141/diffs#f054d0f855ebef2a11559c362a356a2f9e010b99_6_6)).
 * Headings should have normal capitalization: don't use [ALL CAPS](https://en.wikipedia.org/wiki/All_caps) or [TitleCase](http://www.grammar-monster.com/glossary/title_case.htm)).
* After a heading, leave one blank line; this is [not required in the standard](http://spec.commonmark.org/0.27/#example-46), but it is our convention.
1. Strongly consider learning how to edit the [handbook using git](/handbook/git-page-update) and/or via [the web IDE](/handbook/git-page-update/#webide-using-the-browser), and please read through the [Writing Style Guidelines](/handbook/communication/#writing-style-guidelines) before contributing.

#### Fine points
* Keep your handbook pages short and succinct. Eliminate fluff and get right to the point with the shortest possible wording. Keep in mind that the biggest challenge cited by new employees is the vast amount of information to take in during on-boarding.
* We don't need [.gitkeep files](https://stackoverflow.com/questions/7229885/what-are-the-differences-between-gitignore-and-gitkeep) in our handbook, they make it harder to quickly open a file in editors. Don't add them, and delete them when you see them.
* When mentioning currency amounts that team members may need to convert to their local currency (e.g. benefits, expenses, or bonuses), link those amounts to our [Exchange Rates](/handbook/people-group/global-compensation/#exchange-rates) section (e.g. [500 USD](/handbook/people-group/global-compensation/#exchange-rates)).


### Scope of this handbook
* All documentation that also applies to code contributions from the wider community should be in the GitLab CE project (for example in [CONTRIBUTING](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/CONTRIBUTING.md) or the [code review guidelines](https://docs.gitlab.com/ee/development/code_review.html)), not the Handbook, which is only for team members. Read more in the [Documentation](../documentation/) section of the Handbook.
* The handbook is for things concerning current and future GitLab team-members only. If something concerns users of GitLab, it should be documented in the [GitLab documentation](https://docs.gitlab.com/), the [GitLab Development Kit (GDK)](https://gitlab.com/gitlab-org/gitlab-development-kit), the [CONTRIBUTING file](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/CONTRIBUTING.md) or the [PROCESS file](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/PROCESS.md).

## Moving Pages and Adding Redirects to the Handbook
The handbook is a living document and we'll occasionally need to change URLs or move pages. This is [the process the Digital Marketing uses to set up and manage redirects](/handbook/marketing/revenue-marketing/digital-marketing-programs/digital-marketing-management/#aboutgitlabcom-redirects) for about.gitlab.com.

## Management

It is each department and team member's responsibility to ensure the handbook stays current. People Operations Specialists will partner with a representative from each department (engineering, marketing, etc) through weekly reviews to verify the content in the handbook is accurate and follows the same format as outlined in the [Guidelines](/handbook/handbook-usage/#handbook-guidelines). For questions on who to submit a merge request to, or assistance with the handbook, please reach out on the '#handbook' Slack channel.

If you need permissions to directly merge changes to the handbook, please submit a [New Access Request](https://gitlab.com/gitlab-com/access-requests) issue and follow the process for access approval. Request a 'Maintainer' role under www-gitlab-com. See [here](https://docs.gitlab.com/ee/user/permissions.html) for a full description of roles and permissions.

Any changes to the handbook as part of this review will be shared in the `#handbook` channel in Slack. People Operations Specialists will also ensure that questions asked in `#questions` are documented and all announcements on the company call have a relevant link.

## Screenshare the handbook instead of creating a presentation

Presentations are great for ephemeral content like [group conversations](/handbook/people-group/group-conversations/) and board presentations. [Evergreen content](https://www.thebalance.com/what-is-evergreen-content-definition-dos-and-don-ts-2316028) like a [leadership training](/handbook/leadership/#training) should be based on the handbook. Please screenshare the handbook instead of creating a presentation for evergreen content because:

1. It saves you the effort of creating a presentation.
1. People can easily find the handbook section later on.
1. The handbook is checked and improved as part of the preparation.
1. The content is open to contributions.
1. The content is integrated with the rest of our processes.
1. Also see some of the [advantages of using our handbook](/handbook/handbook-usage/).

If you do require a presentation, default to using screenshots and links to the handbook rather than copy and pasting content:

1. This is faster since you won't have to reformat it
1. It gets people used to the format of the handbook
1. It confirms that it is already in the handbook

## Make it worthwhile

Another company asked how we managed to work with the handbook because at their company it wasn't working: "There are many occasions where something is documented in the knowledge base, but people don't know about it because they never bothered to read or search. Some people have a strong aversion against what they perceive as a 'wall of text'."

To ensure that people's time is well spent looking at the handbook we should follow the 'handbook guidelines' above, and also:

1. Follow the [writing style guide](/handbook/communication/#writing-style-guidelines)
1. Have a great search function (we use Algolia), plus make it public so you can Google search
1. Test people on their knowledge during onboarding
1. Give real examples
1. Avoid corporate speak, describe things like you're talking to a friend

## Wiki handbooks don't scale

Company handbooks frequently start as wikis.
This format is more comfortable for people to work in than a static website with GitLab Merge Requests and GitLab Pages.
However wikis tend to go stale over time, where they are badly organized and get out of date.

In wikis it is impossible to make proposals that touch multiple parts of a page and/or multiple pages. Therefore it is hard to reorganize the handbook. Because GitLab Merge Requests and GitLab Pages are based on distributed version control you can split the role of submitter and approver. This allows for a division of work that keeps the handbook up to date:

- Anyone who can read the handbook can make a proposal
- Leaders (who tend to be short on time) only have to approve such a proposal

Wikis also do not encourage collaboration on changes, because there is not way to discuss a proposed change like there is with merge requests.


## External use of the Handbook

Remember that, like virtually everything we do, our handbook is [open source](/solutions/open-source/), and we expect that other companies may use it as inspiration for their own documentation and practices. That said, the handbook should always be specific on **what we do**, not **who we want to be**, and every company will need to fill out their own handbooks over time.

### Inspired by GitLab

If your company has been inspired by GitLab's handbook, we would love to know what inspired you. Please see our [Inspired by GitLab page](/handbook/inspired-by-gitlab/).

## Searching the Handbook

Every GitLab Handbook page offers a search field near the top of the page. Some web browsers and productivity tools allow you to integrate custom search engines, including the GitLab Handbook search engine.

### Google Chrome

If you use Google Chrome, you can add GitLab Handbook search to your address bar in about a minute.

#### Setup

1.  Open Chrome’s search engine settings. You can navigate through Chrome > Preferences… > Search engine > Manage search engines or just load [chrome://settings/searchEngines](chrome://settings/searchEngines) directly.
1.  Click the “Add” button next to “Other search engines”.
1.  Type something like “GitLab Handbook” in the “Search engine” field.
1.  Type something like “handbook” or “hb” in the “Keyword” field.
1.  Copy `https://about.gitlab.com/handbook/#stq=%s&stp=1` and paste it into the “URL with %s in place of query” field.
1.  Click the “Add” button.

#### Usage

1.  Select Chrome’s address bar by clicking, tapping, or pressing `⌘-L` on macOS or `Ctrl+L` on Linux.
1.  Type whatever you entered as your keyword (e.g., “handbook” or “hb”) and Chrome should suggest that you “Press Tab to search GitLab Handbook” over on the right side of the address bar (or something similar if you used a name other than “GitLab Handbook”).
1.  Press tab and your address bar should change to indicate that it will search the GitLab Handbook.
1.  Search as you normally would. Note that this will search with the Handbook’s search engine directly, _not_ Google.
  
### Even More  
Even more tips on finding things at GitLab can be found at [Searching the GitLab Website Like a Pro](/handbook/tools-and-tips/searching/).
