---
layout: handbook-page-toc
title: "Application Security Review Process"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# Appsec Engineer Process for Application Security Reviews

This page details the application security review process for appsec engineers. 
The purpose of application security reviews are to proactively discover and 
mitigate vulnerabilities in GitLab developed or deployed applications in order 
to reduce risk and ultimately help make the company's mission successful.

An application security review may include any or all of the following stages:
- Threat modeling
- In-depth code review
- Dynamic testing

The results of each stage will inform the review done in the next stage. 
Ideally, all new features would received some threat modeling, with 
the latter two stages being performed based on the risk profile. Features
already in development or production can received an appsec review as 
well. The testing done is dependent on the circumstances.

## Stable Counterparts

One of the goals of the [stable counterpart][3] is to help identify features that 
need security review in the area to which they are assigned. This process 
is intended for such features, even if the stable counterpart will be 
performing the review.

## Building the Queue

The application security review queue is a priority queue of application 
features for security review. The priority can range from `P1` (Critical) 
to `P4` (Low/Backlog). 

Some guidelines for which features should be added to the queue are: 
- All new major features
- Features that have had repeat vulnerabilities
- Features related to authorization or authentication
- Features that handle [Red or Orange data][1]
- Features that work with cryptography or other data protection solutions

The idea is to capture features determined to be higher risk for 
vulnerabilities. It is quite probable that all features, especially `P4`
issues, will not get a full review, but by capturing those that are at higher 
risk, we can track additional statistics. For example, how many related 
vulnerabilities were reported in the bug bounty program. This data can help us 
to help iterate on priority.

Single Issue/MR pings that can be completed by the engineer on triage rotation
do not need a separate issue. This process is primarily for tracking features
over time. With that in mind, if a ping will need additional review, an issue 
should be created.

### Adding Features to the Queue

Separate issues will be used to track the appsec review process, as this
process could outlive the original issue/merge request.

1. Create an issue in the [Appsec Reviews issue tracker][2] 
    1. Set the title to a unique name for the feature
    1. Include the following in the description
        - A brief description of the feature
        - What security review has been done already
        - What steps you suggest are taken to complete the security review
        - A primary point of contact for the issue
1. Create `Related` links for any issues or merge requests associated with 
the feature. 
1. Add a `appsec priority::P` priority label based on the determined priority. 
See [Assigning Priority](#assigning-priority).
1. If you plan to continue work on the issue, assign yourself to the issue.

### Assigning Priority

Every issue should have a priority assigned to help team members plan
testing. It is up to the application security engineer creating the issue to 
determine priority based on the data available to them. If you are not sure 
of the appropriate priority, be conservative and assign a higher priority. 
It can always be adjusted given feedback from other team members.

Guidelines for Priority (Not comprehensive, please build upon)

| Priority | Criteria |
|----------|----------|
| P1       | Red data, AuthN/AuthZ, Crypto, Single S1, Repeat S2 vulns |
| P2       | Orange data, Single S2 vulns |
| P3       | Yellow data |
| P4       | Only standard secure practices necessary |


[1]: https://docs.google.com/document/d/15eNKGA3zyZazsJMldqTBFbYMnVUSQSpU14lo22JMZQY/edit
[2]: https://gitlab.com/gitlab-com/gl-security/appsec/appsec-reviews/issues
[3]: https://about.gitlab.com/handbook/engineering/security/application-security/#stable-counterparts
