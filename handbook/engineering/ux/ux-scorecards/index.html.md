---
layout: handbook-page-toc
title: "UX Scorecards"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## UX Scorecards

As UX practitioners, we must think strategically about fixing usability challenges within the GitLab product. 

Creating an UX Scorecards with associated Recommendations enables us to *identify, scope, and track* the effort of addressing usability concerns within a specific workflow. When it's complete, we have the information required to collaborate with Product Managers on grouping fixes into meaningful iterations and prioritizing UX-related issues. 

**All of the UX Scorecards can be found in this [epic](https://gitlab.com/groups/gitlab-org/-/epics/1714).**

Below is a recommended step by step process for completing a UX Scorecard. Note that every scorecard is not the same. Product Designers are welcome to adapt the steps to their needs as long as they are as objective as possible and the spirit and outcome remains the same.

### Setup

1. Create a stage group epic with the following title: `UX Scorecard - {{Stage Group}} FY{{YY}}-Q{{Quarter Number}}` 
    > Example: “UX Scorecard - Create:Source Code FY21-Q1”
1. Work with your Product Manager to identify the top tasks (in frequency or importance) for users of your stage group. Ideally, you will base this task list on user research (analytics or qualitative findings).
1. Select one of the top tasks to complete a UX Scorecard.
1. [Create an experience scoring issue](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Scorecard%20Part%201), using the template “UX Scorecard Part 1”, and add it to the stage group epic. 

    This issue should have the **UX Scorecard** label. If it's related to an OKR, also apply the **OKR** label for easier tracking.
1. [Create a recommendations issue](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Scorecard%20Part%202), using the template “UX Scorecard Part 2”, to be done after the experience scoring.
1. Follow the instructions in the templates to complete the scorecard, and use the [Grading Rubric](#grading-rubric) below.
1. Once you have completed the walkthrough evaluation and provided your recommendations, remove the "WIP:" prefix from the issue title.

If you'd like to view or edit the templates, you can find them here: 

* [Part 1 - UX Scorecard  ](https://gitlab.com/gitlab-org/gitlab-design/blob/master/.gitlab/issue_templates/UX%20Scorecard%20Part%201.md) 
* [Part 2 - Recommendations](https://gitlab.com/gitlab-org/gitlab-design/blob/master/.gitlab/issue_templates/UX%20Scorecard%20Part%202.md)

### Grading Rubric

**A (High Quality/Exceeds):** Workflow is smooth and painless. Clear path to reach goal. Creates “Wow” moments due to the process being so easy. User would not hesitate to go through the process again.
- Frustration: *Minimal to none*
- Task Completion: *Successful*
- Steps to Accomplish Task: *Minimal*

**B (Meets Expectations)** Workflow meets expectations but does not exceed user needs. User is able to reach the goal and complete the task. Less likely to abandon.
- Frustration: *Low*
- Task Completion: *Successful*
- Steps to Complete Task: *Minimal*

**C (Average)** Workflow needs improvement, but user can still finish completing the task. It usually takes longer to complete the task than it should. User may abandon the process or try again later. <br>
- Frustration: *Medium*
- Task Completion: *Successful but with unnecessary steps*
- Steps to Complete Task: *Average complexity*

**D (Presentable)** Workflow has clear issues and should have not gone into production without more thought and testing. User may or may not be able to complete the task. High risk of abandonment.
- Frustration: *High*
- Task Completion: *Unlikely, but there may be a chance that there is completion*
- Steps to Complete Task: *Excessive*

**F (Poor)** Workflow leaves user confused and with no direction of where to go next. Can sometimes cause the user to go around in circles or reach a dead end. Very high risk of abandonment, and user will most likely seek other methods to complete the task. <br>
- Frustration: *Very High*
- Task Completion: *Very Unlikely*
- Steps to Complete Task: *Lacking*
