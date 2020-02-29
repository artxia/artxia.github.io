---
layout: handbook-page-toc
title: "Documenting research findings"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Documenting research findings
The [UX Research Insights repository](https://gitlab.com/gitlab-org/uxr_insights) is a record of all the user insights discovered through GitLab’s UX research program. User insights can be gathered through methods such as user interviews, usability testing, surveys, card sorts, tree tests and more. 

#### Why did we create this repository?
The UX Research team has [always faced challenges](https://about.gitlab.com/blog/2019/07/10/building-a-ux-research-insights-repository/) in finding the best way to create research reports that are easy to digest and access. When using methods such as PDFs, Google docs, and even GitLab CE issues themselves, it was difficult to track and share study findings. Additionally, since we are often asked to readily recall information we've learned in prior studies, it can be tedious to read through old reports, look through pages of interview notes, or rewatch video recordings to find the information we need. This problem compounds, since we are continuously producing research reports and the wealth of information grows infinitely.

The goal of this repository is to make research findings searchable, concise, and easy to reference. It also gives us the opportunity to [dogfood](https://about.gitlab.com/handbook/values/#dogfooding) GitLab as a way to understand what users may experience, if they use GitLab for similar purposes. 

#### What is an insight? 
When we conduct research studies, we have a set of [goals and objectives](/handbook/engineering/ux/ux-research-training/defining-goals-objectives-and-hypotheses/) that guide us as we investigate the research question. Whether we're evaluating the usability of a feature, conducting exploratory interviews, or gathering quantitative data, the research study will likely result in a list of observations, patterns, and behaviors related to a user's experience. The raw data from the study are the research findings. 

A list of findings, alone, is often not enough to fully communicate how users conceptualize a topic or why they experienced a certain struggle. Through [analysis and synthesis](/handbook/engineering/ux/ux-research-training/analyzing-research-data/) of the data gathered in a research study, we are able to distill *insights* that connect the dots between related concerns and provide an additional layer of understanding. 

These synthesized research findings evolve into a cohesive collection of insights that enables stakeholders to make informed decisions. We support each insight with evidence that can be referenced during discussions, typically in the form of video clips, interview quotes, or statistical data.

#### So, how does it work?
At the end of each research study, the study's moderator is responsible for documenting the research in the Insights Repository. We use GitLab issues to report on key findings from research studies. Every issue within the UXR_Insights repository contains a single insight on a particular topic. We connect a study's insights together by marking them as related, through GitLab's related issue functionality. Each issue is tagged with labels related to the feature area, type of research, and other relevant information that may help people find the issue.

Epics are used to organize issues from the same research study. The epic description should describe the research methodology used and any background information we have about the research participants. We tag all epics with the `~uxr_insights` label so they are easily found within the GitLab.org group.

A helpful approach to the documentation process is to start by creating an epic to house all of the insight issues. After creating the epic, it will be possible to use [quick actions](https://docs.gitlab.com/ee/user/project/quick_actions.html) to assign issues to the epic as you fill out the issue description.

When creating a new issue, guidelines for reporting insights can be found in the templates dropdown. These templates are there to help you see examples of how we document findings from studies that involve different research methods.  After you are finished adding context to an insights issue, it's best to close the issue so that it is clear that the work is complete.

One of the best ways to simplify the reporting process is to closely tie your note-taking approach to the research questions. You may find it useful to utilize this [notes template for user interviews](https://docs.google.com/spreadsheets/d/1hnIqg-fnCYW2XKHR8RBsO3cYLSMEZy2xUKmbiUluAY0/edit#gid=0) or the [Rainbow Analysis Chart for usability testing studies](https://docs.google.com/spreadsheets/d/1j5mIFNWvHhxSUz0E1pXr1wGI385EDFc7uRtRHB_6ACc/edit#gid=3).

#### Creating useful insights
It's important to remember that insights often need context, since people may read them in isolation and misinterpret them. As you work on reporting on your study, it's important to keep the audience in mind and think about what you'd like them to learn from the study.
 
For example, you may find it useful to document all insights (big or small) from studies conducted on the GitLab interface, in order to provide explanation for why the interface has changed over time. This creates a record of why previous design decisions were not ideal, which can be helpful for discussions with newer team members. On the other hand, for design evaluations or tests with prototypes, it may be more relevant to focus on documenting the insights that answer the overarching research questions, since these studies often result in additional design iterations before implementation. 

In either case, adding a brief "context" section at the top of the issue description and providing a link to the relevant design artifact can help the reader better understand the background of the study.

Here are some examples of useful insights created for common types of research studies:

- [Usability testing insight](https://gitlab.com/gitlab-org/uxr_insights/issues/571) from [SAST Setup research](https://gitlab.com/groups/gitlab-org/-/epics/1784)
- [User interview insight](https://gitlab.com/gitlab-org/uxr_insights/issues/842) from [Project & Portfolio Management research](https://gitlab.com/groups/gitlab-org/-/epics/2259)
- [Survey insight](https://gitlab.com/gitlab-org/uxr_insights/issues/706) from [Marketplace Nomenclature research](https://gitlab.com/groups/gitlab-org/-/epics/2138)
- [Icon testing insight](https://gitlab.com/gitlab-org/uxr_insights/issues/161) from ["Closed" Issue research](https://gitlab.com/groups/gitlab-org/-/epics/1286) 

#### Leveraging the Insights Repository
Searching through the Insights Repository is a great way to get acquainted with GitLab users and learn about studies that have already been conducted. Since we use labels to tag insights, you can search and filter through issues to find the insights that are relevant to any stage, feature, and type of research.

Another approach is to look through the directory of completed research that is listed on the [UXR project README](https://gitlab.com/gitlab-org/uxr_insights#directory-of-completed-research), if you'd like a higher-level overview. These epics are typically labeled with `~uxr_insights`, to make it easier to access them.

Whether you're looking to better understand a user persona, learn about use cases for features, gather context for solving a problem, or plan a future research study - the Insights Repository has something for you.