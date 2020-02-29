---
layout: handbook-page-toc
title: "Sales Enablement Sessions"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# Sales Enablement Sessions

## Upcoming Training
To see what training is coming soon, view the [Sales Enablement Session issue list](https://gitlab.com/groups/gitlab-com/sales-team/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=sales%20enablement%20sessions).

### Get an invite to the weekly session

To get a calendar invite to the weekly Sales Enablement session, make sure you are added to the one of the following email groups. 

- Sales Team `sales-all@`
- SDR Team `sdr@`
- Marketing team `marketing@`

You can [fill out an access request](/handbook/business-ops/it-ops-team/#access-requests) to request access to the email group. These groups are invited to the meeting so that each individual person does not need an invite.

### Training Playlist

There are a few places to see previous Sales Enablement sessions:

- The latest, most relevant sessions are highlighted within the [GitLab Sales Learning Framework](/handbook/sales/training/#gitlab-sales-learning-framework) 
- [Sales enablement Youtube playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0KrirMKe3CyWl4ZBCKna5rJX) on GitLab Unfiltered YouTube
- [Sales enablement Youtube playlist](https://www.YouTube.com/watch?v=ZyyBq3_rzJo&list=PLFGfElNsQthYe-_LZdge1SVc1XEM1bQfG) on GitLab YouTube
- Historical sessions that were recorded in Google drive can be accessed via this [deprecated spreadsheet](https://docs.google.com/spreadsheets/d/1ETY7FfCzb2q9h2EkYttlW_Qpl7IHUF-F2rOJG2W03Yk/edit#gid=0)

#### Recording 

#### Public vs Private

- Some enablement sessions, typically those that focus on industry or technical product knowledge, are [made public](/handbook/values/#public-by-default), including the Q&A
- Other sessions that focus on topics like competitive analysis or openly discussing customers are [kept private](/handbook/communication/#not-public)
- At the start of every session, and before moving into Q&A, the facilitator will announce to the audience if the call is public or private
- Here is a [how-to video](https://www.youtube.com/watch?v=LKZ23pRfpBg&list=PL05JrBw4t0KrirMKe3CyWl4ZBCKna5rJX&index=33&t=0s) on accessing private videos

### Enablement pages
- [GitLab CI/CD for GitHub FAQ](/handbook/marketing/product-marketing/enablement/github-ci-cd-faq/)
- [Cloud Native Ecosystem](/handbook/marketing/product-marketing/enablement/cloud-native-ecosystem/)
- [Enterprise IT Roles](/handbook/marketing/product-marketing/enterprise-it-roles/)
- [How to set up Chorus.ai call recording](/handbook/business-ops/tech-stack/#chorus)
- [GitLab Serverless FAQ](/handbook/marketing/product-marketing/enablement/serverless-faq/)
- [GitLab.com Subscriptions](/handbook/marketing/product-marketing/enablement/dotcom-subscriptions/)
- [Services to Accelerate Customer Adoption](/handbook/customer-success/professional-services-engineering/sales-enablement)

### To request new sales enablement sessions
- Create an issue in the [GitLab Sales Team issue tracker](https://gitlab.com/groups/gitlab-com/sales-team/-/issues)
- Label the issue with `sales enablement sessions`.
- @mention `@dcsomers` in the issue description and he will coordinate with key stakeholders in sales and marketing to prioritize and schedule the training.
- If you need a training prioritized @ mention `@dcsomers` in the `#sales` slack channel.

### Scheduling trainings

**4-6 weeks before the start of a new quarter**
*   Solicit input from sales leaders, product marketing, and others (e.g. Sales Ops) on sales enablement topics for the next quarter

**2-4 weeks before the start of a new quarter**
*   Alignment call to finalize topics & tentative schedule with
    *   Manager, Product Marketing (John Jeremiah)
    *   Sales Training Facilitator (John Blevins)
    *   Director, Sales & Customer Enablement (David Somers)
*   After alignment call, John Blevins to open issues for each enablement session with
    *   Documentation of preliminary learning objectives, title, expected outcomes, etc.
    *   Tentative dates listed as “TENTATIVE - ZZZ”
    *   Intended SME/speaker(s) assigned to the issue
    *   Ping the SME in the issue to ask if they can commit to it, get their commitment before you schedule. 
*   John Jeremiah to open issues in Product Marketing aligned to each of the above

**1-2 weeks before the start of a new quarter**
*   John Blevins to schedule meeting with all SMEs/speakers 
    *   Goal: Ensure SMEs/speakers are aware of the upcoming sessions and can own the sessions
        *   Review schedule, outcomes, objectives
        *   Answer questions
        *   Adjust as needed
    *   Manage ongoing collaboration via issue, Google Docs, and public Slack channels (e.g. #product-marketing or #sales-and-customer-enablement)

    - The Sales and Customer Enablement team discusses upcoming trainings in regular meetings with sales leadership and the GitLab Product Marketing Management (PMM) team.
- Sessions picked to execute on should be chosen from the backlog, or a new issue created, and moved to the `status:plan` column.
- Assign the issue to the speaker and add `Moderator: <name>` to the issue description.
  - The speaker will then research and generate the conent for the training.
- Once the speaker is ready, a moderator and date should be chosen for the training.
  - Assign the moderator (in addition to the speaker) to the issue and add `Moderator: <name>` to the issue description.
  - Add a due date to the issue.
  - Add the date in ISO format to the issue title.
  - Move the issue to the `status:scheduled` column.
  - Manually drag the issue to order issues in the column by date.

### Enablement calendar
Sales enablement sessions are scheduled on the [Sales Enablement calendar](https://calendar.google.com/calendar/embed?src=gitlab.com_5n3g60l58thum9aovp8iisav34%40group.calendar.google.com&ctz=America%2FLos_Angeles) so that everyone on the Sales and Customer Enablement and PMM team has the ability to edit the calendar event.

## How to conduct a sales enablement training

- Each training session has a [speaker](#speaker) and a [moderator](#moderator)
- Sessions are 30 minutes long
- The presentation portion should be 15 minutes leaving 15 minutes for Q&A

### Speaker

- Create your content as a handbook page (don't use a slide deck)
  - Create a new directory under `https://about.gitlab.com/handbook/sales/training/sales-enablement-sessions/enablement/` with the title of your talk
    - For example: `/handbook/sales/training/sales-enablement-sessions/enablement/cloud-native-ecosystem/`.
  - Add an `index.html.md` file to that directory.
    - Use this template:

    ```
    ---
    layout: markdown_page
    title: "Title goes here"
    ---

    ## On this page
    {:.no_toc}

    - TOC
    {:toc}

    ## Title goes here
    ```

  - Add your content to this page.
  - Add links to any other pages you need to reference on this page so you can present from training page.
  - Add a link to the training page from this page in the [#enablement-pages](#enablement-pages) section.

### Moderator

The moderator should serve as the host of the call and overall wingperson for the presenter. The moderator monitors chat to raise questions to the presenter and searches for links that are mentioned on the call to make sure they get linked in the handbook page for the training.  

- Log in to zoom 5 minutes ahead of time
- The video should not be recording, but pause if this is the case
- At 12pm ET / 9am PT welcome everyone to the call and remind them that the presentation will be public/private. Specifically mention how to talk about sensitive info on every intro.

> Hello and welcome to today's sales enablement session. As a reminder we'll be posting this session to YouTube. Please remember to not share any private info such as the names of non-referenceable customers.

- Record the call to your local computer.

> For today's GitLab sales enablement training we are pleased to have `<speaker name>` talk to us about `<topic>`. With that, I'd like to pass it over to `<speaker name>`

- Monitor the time. If the presentation goes longer than 15 minutes, interrupt to remind the speaker that we are at 15 minutes and we want to leave time for Q&A.
- Stop the recording.
- After the sales enablement session, upload the video to  the [YouTube Unfiltered channel](https://www.youtube.com/channel/UCMtZ0sc1HHNtGGWZFDRTh5A). Here's a video tutorial on how to upload a video to the GitLab Unfiltered channel: 

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/xGwX9zjNr2E" frameborder="0" allowfullscreen="true"> </iframe>
</figure>

- Make sure a link to the handbook page is included in the description of the YouTube video
- Post a link to the YouTube video in the #sales slack channel
