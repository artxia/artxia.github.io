---
layout: handbook-page-toc
title: "Brand and Digital Design Handbook"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# About Marketing Brand and Digital

We build deliverables and experiences in both digital and physical realms such as the about.gitlab.com website, brand collateral, and more.

We assist with conversion design, growth marketing, user experience (UX), search-engine optimization (SEO), and performance metrics to build the logged out experience. We're involved with related marketing campaigns, events, lead-generation, and more. We guide the brand design and experience to assist with creating a cohesive identity.

# Contact us

* Slack: [#marketing-brand-and-digital](https://gitlab.slack.com/app_redirect?channel=marketing-brand-and-digital)
* Slack: [#marketing-design](https://gitlab.slack.com/app_redirect?channel=marketing-design)
* Slack: [#marketing-website-team](https://gitlab.slack.com/app_redirect?channel=marketing-website-team)
* Email: [brand-and-digital@gitlab.com](mailto:brand-and-digital@gitlab.com)

# How we work

## Working with issues, groups, and labels

In general issues, labels, boards, and milestones can all be created in either a project or a group. Epics can only exist in a group. Because the website exists as a project at the top level, labels and boards for our team should usually be created in the root gitlab.com group. For more information on this works, please see [How it all fits together](https://about.gitlab.com/handbook/marketing/#how-it-all-fits-together). 

### Issue labels

**At a minimum, website related issues should have the label `mktg-website` applied in order to populate appropriate boards.**

They should also have a label for your team and/or subject matter (ex: `blog`, `Digital Marketing`, `SEO`). These labels need to exist in either the root `GitLab.com` group or the `www-gitlab-com` repository.

Issues should follow the [standard marketing status labels](/handbook/marketing/#boards-and-labels) flow labels, with a few additions.

* `mktg-status::triage` this work is in the pre-planning stage. We're still discussing what to do.
* `mktg-status::plan` this work is in the planning stage. We know what we want to do but don't know how we want to do it yet.
* `mktg-status::design` this issue needs some prototyping or other UX designs before we know where we're going.
* `mktg-status::groomed` this issue has been planned and detailed. We know what needs to be done. We can start building it.
* `mktg-status::wip` this issue is actively being worked on.
* `mktg-status::blocked` something is blocking progress on this issue.
* `mktg-status::review` enough work has been completed that this is ready for review and approval.
* `mktg-status::scheduled` this issue cannot be merged until a scheduled date but the work is complete and approved.

**Issues with an immovable due-date because of contractual and/or meatspace obligations should apply the `hard-deadline` label.**

Examples of optional labels include:

* `OKR`
* `outsource`

### Issue boards

#### General

##### [Design Handbook](https://gitlab.com/groups/gitlab-com/-/boards/1498563)

This board shows the status of all mktg-website issues labeled design-handbook. These are issues relating to team documentation and NOT general issues with the handbook.

#### Brand Design

##### [Design - Priority](https://gitlab.com/groups/gitlab-com/-/boards/1511332)

This board shows the status of all Brand Design issues labeled with a design priority label.

##### [Design - Outsource](https://gitlab.com/groups/gitlab-com/-/boards/1511334)

This board shows the status of all outsourcable issues labeled with design.

#### Digital Design

##### [Blocked](https://gitlab.com/groups/gitlab-com/-/boards/1485169)

This board shows all mktg-website website issues with the mktg-status::blocked label.

##### [Bugs](https://gitlab.com/groups/gitlab-com/-/boards/1483331)

This board shows the status of all mktg-website issues filed using the website bug template.

##### [CMO](https://gitlab.com/groups/gitlab-com/-/boards/1486533)

This board shows the status of all mktg-website issues labeled mktg-website which have the CMO Attention label.

##### [Debt](https://gitlab.com/groups/gitlab-com/-/boards/1485186)

This board shows the status of all mktg-website issues labeled technical-debt.

##### [OKR](https://gitlab.com/groups/gitlab-com/-/boards/1483333)

This board shows the status of all mktg-website issues labeled OKR.

##### [Overall](https://gitlab.com/groups/gitlab-com/-/boards/1472883)

This board shows the status of all appropriately labeled mktg-website issues.

##### [Mktg Web - Priority](https://gitlab.com/groups/gitlab-com/-/boards/1483370)

This board shows the status of all mktg-website issues labeled with a design priority label.

##### [Marketing Web - Outsource](https://gitlab.com/groups/gitlab-com/-/boards/1502288)

This board shows the status of all outsourcable issues labeled mktg-website.

##### [Team Dev](https://gitlab.com/groups/gitlab-com/-/boards/1485124)

This board shows all issues assigned to a member of the marketing website design & delivery teams. It is recommended to filter this by a particular mktg-status:: label such as ::wip or ::groomed.

##### [Hard Deadlines](https://gitlab.com/groups/gitlab-com/-/boards/1485208)

This board shows the status of all mktg-website issues labeled hard-deadline (please refer to the definition on the label).

### Team-subject boards

* [All Remote](https://gitlab.com/groups/gitlab-com/-/boards/1485066)
* [Analyst Relations](https://gitlab.com/groups/gitlab-com/-/boards/1485071)
* [Blog](https://gitlab.com/groups/gitlab-com/-/boards/1483337)
* [Content Marketing](https://gitlab.com/groups/gitlab-com/-/boards/1483354)
* [Corporate Events](https://gitlab.com/groups/gitlab-com/-/boards/1485090)
* [Corporate Marketing](https://gitlab.com/groups/gitlab-com/-/boards/1485085)
* [Digital Marketing](https://gitlab.com/groups/gitlab-com/-/boards/1485086)
* [Field Marketing](https://gitlab.com/groups/gitlab-com/-/boards/1533790)
* [Marketing Ops](https://gitlab.com/groups/gitlab-com/-/boards/1485111)
* [Product Marketing](https://gitlab.com/groups/gitlab-com/-/boards/1485129)
* [Recruiting](https://gitlab.com/groups/gitlab-com/-/boards/1485175)
* [Strategic Marketing](https://gitlab.com/groups/gitlab-com/-/boards/1489415)
* [Social](https://gitlab.com/groups/gitlab-com/-/boards/1485179)
* [Technical Evangelism](https://gitlab.com/groups/gitlab-com/-/boards/1485182)

## Prioritization

We use the following criteria to assess issue priority:

Common

* Frequency of use - How often is the single application diagram used? Web traffic to this page?
* Number of people impacted - How many GitLabbers would benefit from this asset? How many unique users would benefit from this page?

Critical

* High customer risk - If we don't do this, what are the risks to customers? How severe are those risks?
* High business risk - If we don't do this, how might it create risk for our business? Could it create a large volume of support calls? Make us non-GDPR compliant?
* Business criticality - Part of high ROI opportunity or other business critical initiative?
* Impact to important stakeholders - CEO or CMO request? Impacts bottom of funnel (BOFU) prospects very close to buying? Impacts key partners or customers?

Differentiator

* Brand and or product differentiator - Creates value by positioning our brand and or product against competition.

Reusable

* Can we reuse - If we build this, can we reuse it elsewhere to get more ROI. Perhaps it's low value score for this project, but high "lifetime" value via reuse.

Time & Cost

* Time and cost required to complete the work.

Deadlines

* Are there any hard deadlines due to contract or event obligations?

## Issue grooming template

This template can be used while [grooming](https://www.agilealliance.org/glossary/backlog-grooming/) an issue to prepare it for production.

```
# Goals

* Increase X
* Decrease Y
* etc

## Proposed methodology

Based on A  do B to C (url)

* Reason(s) why
* Given constraints

Should change:

* D
* E
* etc

Won't change:

* F
* G
* etc

#### Stakeholders

* Internal or name(s) of stakeholder(s). Recommended to show @ username first then review during (name of meeting. Example: weekly brand+digital team meeting).

#### Deliverables phase 1

- [ ] Obtain before screenshots
- [ ] Measure preexisting page-speed of (subject pagename)
- [ ] Begin (information gathering. Ex: heatmap or analytics dashboard) test for baseline comparison known as the "before"

#### Deliverables phase 2

- [ ] Evaluate heatmap results from the baseline in order to inform data-driven design decisions

#### Deliverables phase 3

Prototype and/or wireframe containing:

- [ ] 1 updated (source pagename) section linking to
- [ ] 1 desktop view of (subject pagename) before event (example: form submit)
- [ ] 1 desktop view of (subject pagename) after event (example: form submit)
- [ ] 1 mobile view
- [ ] Obtain review approval from prototype

#### Deliverables phase 4

- [ ] Build updated pages
- [ ] Measure page-speed improvements of (subject pagename)
- [ ] Obtain review approval from review-app
- [ ] End previous heatmap
- [ ] Release updated pages
- [ ] Review on the production server to validate requirements including regression testing
- [ ] Create new (information gathering. Ex: heatmap or analytics dashboard) known as the "after"

#### Proposed deliverables phase 5

- [ ] Monitor statistics
- [ ] Report results

## Regression Risks

- [ ] Do any gated content forms still work?
- [ ] Does Cookiebot still work in CCR & GDPR?
- [ ] Do Marketo forms still present GDPR & Ukraine required fields?
- [ ] Any other regression risks
- [ ] etc
```

## Tools

[ TODO : list tools, descriptions, uses, reasons ]

* Adobe Creative Cloud / Suite
* Sketch
* Mural
* Google Analytics
* Periscope
* Hotjar
* Launch Darkly
* Google Optimize

## Experiments

This section is related to A/B and multivariate testing on the marketing website, about.gitlab.com. It is a work in progress while we assess new testing tools for integration into our toolkit.

Until the toolkit assessment is finalized, please reference digital marketing's [testing documentation](https://about.gitlab.com/handbook/marketing/revenue-marketing/digital-marketing-programs/digital-marketing-management/#create-a-culture-of-testing-and-optimization).

Going forward, we hope newly created issues align with the [growth team's testing template](https://gitlab.com/gitlab-org/growth/product/-/blob/master/.gitlab/issue_templates/Growth%20experiment.md).

### Before you experiment

Always gather relevant heatmaps, analytics, metrics, KPI (key performance indicators), etc.

### Testing Tools

We are in the process of establishing a new toolset for running experiments. Our hybrid suite of tools will include:

#### Testing via feature flags

This is where we plan to do the bulk of our testing. We can run several of these at the same time. For full-page, partial-page, component, and small changes.

#### Feature flag best practices

Feature flags should be implemented in code similarly to the includes system. Example:

* Login to our third party service and create a feature flag and related configuration variables.
* Assign ownership of that flag from within the interface.
* Edit a page.
* Put the existing contents of the page into an include file named `/source/experiments/1234-control.html.haml`, where experiments is the folder name instead of includes and 1234 is the id number of the associated issue. "Control" refers to the baseline measurement you are testing against.
* Duplicate that include file with the name `/source/experiments/1234-test.html.haml`
* Make your changes and validate the feature toggle works locally and/or on a review app before deployment.
* Ensure you'll be able to collect all the data you need. Setup appropriate tools like heatmaps and analytics.
* Note that one advantage of feature flags is that they can be released to production without being turned on.
* When ready, enable the test. Start gathering data.

### Testing via CDN

This is an advanced tool meant to test large-scale changes at a systemic level. For now we plan to run only one of these at a time.

### Testing via WYSIWYG

This is a rudimentary tool for small-scale changes with few safeguards and important caveats. We can use this for small items like colors and copy but not layout. This is mainly meant as a tool for non-developers.

# Resources

[ TODO : Document  ]

## Best practices

[ TODO : Document  ]

## Design systems

* The about.gitlab.com website currently uses a forked bootstrap based design system with a 1200px max width and a 12-column grid.

## Recommended reading

[ TODO : Document  ]