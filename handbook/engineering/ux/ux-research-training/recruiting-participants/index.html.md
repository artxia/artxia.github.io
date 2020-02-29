---
layout: handbook-page-toc
title: "Recruiting participants"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}


### How to recruit participants

There are four phases of recruiting: identifying your target participants, crafting your survey or screening survey (screener), opening a recruitment request issue, and opening an incentives request issue. A UX Researcher or Research Coordinator may collaborate with you throughout the process, and we’re always available to answer questions. 

#### Identify target participants

- What research methodology have you chosen?
- How many participants do you need?
- Who do you want to hear from/speak with?
- What’s your ideal research timeline?

The answers to these questions should flow directly from the [goals and objectives](/handbook/engineering/ux/ux-research-training/defining-goals-objectives-and-hypotheses/) that you’ve previously identified for your study. It’s important that everyone involved in the research study agrees on these and that they’re finalized before we start recruiting. It’s better to start with clear objectives than to try to shoehorn participants into a study which they simply aren't a match for. 

Be aware that some of your criteria can also be hypotheses — for example, sometimes we think of job title as a proxy for tasks and responsibilities that we think a role comprises. But, there may be people who have a different job title but perform all the tasks and responsibilities you’re interested in. One should be open to different ways of identifying your target participants.

#### Craft your survey

If you have chosen to run a survey, you should enter your survey questions into Qualtrics. You should have fully tested the survey before asking the relevant Research Coordinator to [distribute the survey](#open-a-recruitment-request).

#### Craft your screener (user interviews and usability testing)

The screener has a specific function - it’s meant to identify the people who are your target demographic, so that you can ask them the things you really want to know in the study. Team members often draft these and collaborate in Google Docs. Once finalized, you should enter the screener into Qualtrics. 

There should be a 1:1 match of your questions to each criterion you have, so that a Research Coordinator can look at your desired criteria and know which answers you want to see on the screener. The more abstract or open-ended you get in the screener, the harder it is for Research Coordinators to parse which answer it is you’re looking for. 

Common questions we include are:
- Consent to record the session
- Consent to store the recording in GitLab
- Job title
- Industry
- Team and company size
- Common tasks
- Tools 

There are copies of these questions with standard phrasing available in the UX Research library in Qualtrics.

It’s important to remember that a screener is not the same as a survey. There can be a temptation to pile on extra questions that you want to know the answer to, but aren’t strictly necessary for determining whether that participant should get through the door. You may benefit from including these questions in your discussion guide or script instead. 

#### Open a recruitment request

Open a `Recruiting request` issue in the [UX research project](https://gitlab.com/gitlab-org/ux-research/issues) and be sure to @ mention the relevant Research Coordinator. They will work with you to clarify any of your criteria.

Once your survey or screener is finalized and in Qualtrics, the Research Coordinator can take action. Depending on your desired participants and timeline, they might send an invitation to our research panel, GitLab First Look, open a campaign via a third-party recruiting service, request social promotion from the marketing team, suggest a blog post and newsletter placement, ask other team members for introductions to users, or try other tactics. 

Recruitment may only take a few days if your target users are plentiful -- Engineers, DevOps professionals, etc. Recruitment can take longer for low-incidence users, like security professionals or users of a newly released feature. Generally, two weeks is enough time to recruit even difficult-to-reach users. In rare cases when your target users cannot be found, the Research Coordinator will suggest other options such as relaxing your criteria. In all cases, the Research Coordinator will keep you updated on the progress of the recruitment effort by commenting in the recruiting issue. 

#### Scheduling participants (user interviews and usability testing)

The Research Coordinator will share the screener results and suggest which users best fit your criteria. They will work with you to configure your Calendly, and will invite users to schedule with you. 

#### Reimbursing participants for their time

Open a `Incentives request` issue in the [UX research project](https://gitlab.com/gitlab-org/ux-research/issues) and be sure to @ mention the relevant Research Coordinator. The Research Coordinator will send thank you gifts to participants who have completed research sessions or that have been randomly selected to win a prize through completing a survey. Once all participants have been sent gifts, the request can be closed. 

### Recruitment case study

To understand how the above process works in action, the following research study is a great example:

[Accessibility solution validation research issue](https://gitlab.com/gitlab-org/ux-research/issues/576)

#### Identifying target respondents

The stated goals of the study were:

> As part of our continued effort to improve the automated testing capabilities of GitLab, we want to ship a new feature for accessibility testing. We want to validate some solutions for this feature. Questions we have are:
> - How exactly users want to see Accessibility issues introduced during their development shown to them.
> - Which of the proposed designs suffice their use case for Automated Accessibility Testing as part of the CI process.

**How many participants did they need?** 

It was a usability test, so around five users is generally the sweet spot.

**What was the timeline?** 

The Product Designer stated that they were ready to begin any time, and notified the Research Coordinator of their vacation time. 

**Who did they want to speak with?** 

The following criteria was submitted:

> Frontend engineers who are working to ensure their code is accessibility compliant.

There was some ambiguity in the phrasing here that we need to clear up before sending out the screener. 

Does this mean we want people whose job is to test for accessibility compliance? Unfortunately, these people are rare and historically difficult to find for studies. Often, accessibility is a subject that people are passionate about, and champion unofficially rather than as a stated responsibility of their role. This is a case where a job title or job responsibilities would not be good criteria to strictly adhere to. 

In the recruiting issue, the Research Coordinator worked with the Product Designer to clarify the criteria. Both agreed that we could also invite people to interview who did not say that they were responsible for accessibility compliance in their role, but who strongly agreed that accessibility compliance is important.

#### Crafting the screener

In this example, the key questions that recruiting hinged on were really clear - the Research Coordinator expected to see a question about job title, common tasks participants' performed or job responsibilities they had, and something about how they perceived the importance of accessibility compliance. The Research Coordinator also expected to see things that we almost always include - like company size and industry, which we try to get a mixture of when they’re not the object of the study. 

This study is unusual in that we're not asking about what tools people use. Often, we explicitly want to see what someone with or without GitLab experience thinks. It wasn't relevant for this study, so we're not collecting that information. 

Keeping things short and sweet increases the completion rate of screeners. 

**Check out the [finished screener](https://gitlab.eu.qualtrics.com/jfe/preview/SV_cT80heuzGIlAdZH?Q_SurveyVersionID=current&Q_CHL=preview)** 

#### Opening a recruitment request

A lot of the conversation above occurred in the recruitment request.

The Research Coordinator took great care in creating a segment from our research panel (GitLab First Look). Because the study was about accessibility, a topic about which many people are passionate, this study was a good one to use custom subject lines and email copy. The Research Coordinator sent out an email with subject line `New study - let's talk accessibility`. After two emails, we received over 20 responses. 

The Research Coordinator highlighted in green the people who said they do accessibility testing in their jobs, and strongly agreed that accessibility compliance is important (4 total). They highlighted in orange people who only fit the latter criterion (9). Altogether, this is a surplus of participants, however, we now have some participants that we can reach out to directly when the next accessibility study is available.

**See how the [recruitment process, scheduling, and thank you gifts were coordinated](https://gitlab.com/gitlab-org/ux-research/issues/577)**

### Obtaining consent (user interviews and usability testing)

Note: The below are available as templated questions within the UX Research library within Qualtrics.

#### Written consent to record

* Collect the participant's response in a screener (Qualtrics).
* Use single select checkboxes.
* A participant must select 'I agree...' in order for you to be able to record the conversation.
* Verbally double check permission to record at the start of your user interview.

```
What you say and do during a research study is really important to GitLab. We create issues to resolve the problems we witness during a study. To make sure our issues correctly represent what you say and do, we would like to record:

(1) the conversation you have with our [researcher/designer/product manager/team]

(2) anything you choose to share on your screen with us during the study 

Please indicate below whether you give your permission to be recorded.

* I agree, I give my permission for my voice and screen to be recorded.

* I disagree, I do not want my voice or screen to be recorded.
```

#### Written consent to share

* Collect the participant's response in a screener (Qualtrics).
* Use single select checkboxes.
* A participant must select 'I agree...' in order for you to share the recording publicly on GitLab. 
* Verbally double check permission to share at the start of your user interview.
* Recordings should be stored on Google Drive and permissions set as appropriate.
* If the participant agrees to be recorded, but doesn't agree for the recording to be shared, ensure the permission on the video is `On - Anyone at GitLab with the link`.
* Please use common sense. If a participant agrees for the recording to be shared publicly (`On - public on the web`) but the recording includes either sensitive information or could be defamatory to an individual or organization, please refrain from sharing the video (use the permission of: `On - Anyone at GitLab with the link`).

```
At GitLab, we value transparency. By making information public, we can reduce the threshold to contribution and make collaboration easier. We would love to share the recording of the research study on GitLab. This is completely voluntary and up to you. 

Please indicate below whether you give your permission for the recording to be shared on GitLab.

* I agree, I give my permission for the recording to be shared on GitLab.

* I disagree, I do not want the recording to be shared on GitLab.
```
