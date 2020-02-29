---
layout: markdown_page
title: Growth
---

## On this page
{:.no_toc}

- TOC
{:toc}

## Overview

The [Growth stage](https://about.gitlab.com/handbook/product/categories/#growth-stage) is responsible for 
scaling GitLab's business value. To accomplish this, Growth analyzes the entire customer journey from acquisition of 
a customer to the flow across multiple GitLab features - and even reactivation of lost users. Several groups 
help with this mission:
* [Acquisition](https://about.gitlab.com/direction/acquisition/), [Conversion](https://about.gitlab.com/direction/conversion/), [Expansion](https://about.gitlab.com/direction/expansion/) and [Retention](https://about.gitlab.com/direction/retention/) connect users to the existing value that GitLab already delivers by
rapid experimentation.
* [Fulfillment](https://about.gitlab.com/direction/fulfillment/) ensures a terrific experience throughout the 
buyer journey for customers doing business with GitLab.
* [Telemetry](https://about.gitlab.com/direction/telemetry/) builds the backbone of data that other groups need to be successful, enabling a data-informed product 
culture at GitLab.

Growth is commonly asking and finding solutions for these types of questions:

* Why are so many users signing up for GitLab but never logging in?
* How do we successfully attract new customers to GitLab?
* How do we successfully win back customers that once used and/or paid for GitLab but have canceled their subscription?
* What is the first action taken after logging in and is it the right one for maximum connection to value?
* How can we grow the amount of customers that use all stages of GitLab?

### Why Invest in a Growth Section in 2019?

We believe we have found product-market fit by providing a single application
for the entire DevOps lifecycle, highlighting the value created when teams don’t
have to spend time integrating disparate tools. Now that product-market fit has
been achieved, we must do a better job of connecting our value to our customers.
Therefore, a Growth focus is required. Additionally, we are beginning to put
more strategic focus on the growth of GitLab.com, which is a different user
signup and activation process than self-managed instances, which typically
involves direct sales.

## Acquisition, Conversion, Expansion, and Retention groups

While the Growth function is becoming more common in late stage, well funded
software companies, it is still a relatively nascent discipline. At GitLab, we
seek to derive best practices from the industry and adapting them to work with
our culture. Here are a few articles we’ve found helpful as we are formulating a
Growth strategy and vision:

* [What Are Growth Teams For, and What Do They Work On?](https://news.greylock.com/what-are-growth-teams-for-and-what-do-they-work-on-a339d0c0dee3)
* [Sustainable Product Growth](https://www.sequoiacap.com/article/sustainable-product-growth)

The Acquisition, Conversion, Expansion and Retention groups are GitLab's approach to a dedicated, 
experiment-driven Growth team. These groups are expected to always start with a hypothesis. 
The hypothesis should be fully defined prior to execution in order to safeguard from "bad 
science," namely data that may correlate but not have any causal relationship. After a hypothesis has been
defined, Growth relies on two primary constructs to make decisions: analysis of data, or
what people do in the application, and qualitative research, in essence the
“why” behind the data.

Growth should focus on metrics that are important at the company level, while also considering
company strategy. Each group will own a north star KPI which are linked [here](https://about.gitlab.com/handbook/product/metrics/). At the same time, we strive to be *informed by data* and *driven by empathy* towards our users. This guideline will help us make informed decisions that align with our strategy *and* bring value to our users, avoiding the usage of dark patterns to move a KPI in the right direction.

Acquisition, Conversion, Expansion and Retention will consist of a product manager, engineering manager, UX manager, 
some full-stack engineers, a (shared) data analyst, and four Product Designers.
Each group member will have a functional reporting structure, in order to report
to a leader that understands their job function. More information about the [Growth UX Team](https://about.gitlab.com/handbook/engineering/ux/stage-group-ux-strategy/growth/).

### Weekly Growth meeting
The Growth Product Management Director should run a weekly growth meeting to review, prioritize, and plan experiments.  The meeting should take place on Tuesdays for 50 min and should cover the following agenda.
15 min: metrics review
10 min: last week’s testing activity review (update on live experiments) 
15 min: lessons learned 
15 min: select this week’s tests
5 min: check on idea backlog

To prepare for the meeting, the Growth PM's and the Growth Director should check in on experiments to identify which can be concluded, and to collect data for review.

### Growth ideation and prioritization
Anyone is welcome to submit ideas offline to idea backlog as issues (name, description, hypothesis, metrics to measure, and ICE score).

To prioritize, the growth groups will use the [ICE framework](https://blog.growthhackers.com/the-practical-advantage-of-the-ice-score-as-a-test-prioritization-framework-cdd5f0808d64), which consists of the following elements, scored on a scale of 1-10:
* Impact - high score for high impact
* Confidence - high score for high confidence
* Ease - high score for ease

### Feature Ownership
The Fulfillment Group is responsible for the maintenance and technical strategy of the customer portal application, the license application, and the billing and licensing experience for both internal and external customers. Fulfillment is also concerned with e-commerce compliance, add-on products, and internal tools for GitLabbers to work more efficiently when helping customers.  

Key areas of focus for the Fulfillment Group are:

* Payment gateway integration (Stripe, Zuora and other providers where necessary), management, and support.
* Implementing new Pricing, Plans, and account requirements as directed by the Principal Pricing Manager.
* Abstracting the customers application away from users to provide a seamless experience for account management of self hosted and GitLab.com accounts.
* Ensuring the technical backend and frontend of the customers and license applications have strong test coverage, deployment, and monitoring processes and meet performance and scalability requirements.
* Prioritization and action on the removal of technical debt by staying inline with GitLab.com best practices for technology stack, architecture, design systems, and coding. Collaborating with other Growth groups for common concerns. 
* Reviewing and merging internal and external contributions to the customers and licensing applications.
* Allowing customers to manage billing/customer information (company details, billing address, customer address, credit card / banking information)

The Acquisition, Conversion, Expansion, Retention, and Fulfillment Product Teams will collaborate on longer-term strategic initiatives that involve the customers and license applications to ensure that the underlying technical architecture implemented by the Fulfillment engineering team supports the longer-term roadmap of each of the below areas.

*Acquisition* is measured by the New Signup ARR KPI and this team is responsible for optimizing the UX workflow for new user sign-ups, both self-hosted and on GitLab.com. This team will also be involved in sign up messaging (in conjunction with the marketing team), first-run experiences, initial purchase, and multi-channel engagement for users that have not progressed into active product use.

*Conversion* is measured by the Free to Paid Trial ARR growth KPI and owns the experience of new customers choosing to trial GitLab (both self hosted and on GitLab.com). This team will manage processes related to trial lengths, restrictions and internal touch points, and optimize both in product and external messaging for customers trialing GitLab.

*Expansion* is measured by the Net Retention KPI and owns the experience of customers upgrading to higher tiers, and adopting more users. Upgrades can be influenced by messaging, navigation changes, empty state UX, and other forms throughout other sections of the product.

*Retention* is measured by the Gross Retention KPI and works holistically to prevent customer churn by improving the customer journey and internal processes of renewing accounts (including true-ups), soliciting and acting on feedback from customers who have chosen not to renew, and owning multi-channel messaging such as email and in-app messaging to drive renewals.

Ownership of an experience or workflow includes the priorisation and delivery of related bugs, security fixes and other [technical priorities](https://about.gitlab.com/handbook/engineering/#prioritizing-technical-decisions) by that team.

### Growth Deliverables

A growth deliverable should be a released feature or a launched effort that is expected to directly impact KPIs, improve external & internal customer experiences

We will use the label  `~growth deliverable` to differentiate this from a typical product deliverable.  A "growth deliverable" should be:

*  Able to stand on its own (can be potentially released/launched on its own)
*  Expected to directly impact KPI or improve internal/external user experience on its own
*  Typically should be a product change, but can include emails etc. if it meet 1) AND 2)
*  Growth deliverable can also be a piece of UX research, analysis, if these are large scope and require significant amount of work from PM, OR they provide valuable insight for growth experiments

### Working across stages

The hypotheses explored by Growth will span across groups and stages. How do other groups interact with Growth?

Growth does not own areas of the product, but finds ways to help users discover and unlock value throughout the GitLab
application. They will do a combination of shipping low-hanging fruit themselves, but will partner with other stages
on larger initiatives that need specialized knowledge or ongoing focus.

It is the responsibility of other stages to maintain and expand core value in their respective product areas; it's
Growth's mission to streamline delivery of that value to users. For example:

* [Manage](https://about.gitlab.com/handbook/product/categories/#manage-stage) is responsible for user registration and
management. This stage maintains a long-term vision on how users are created and maintained in GitLab, with a roadmap that
includes other categories and priorities.
* Growth may identify user registration as an opportunity to further the group's [priorities](#growth-priorities). Growth's
engineering team may ship smaller improvements independently of Manage's direct involvement during implementation (such as [soft email confirmation](https://gitlab.com/gitlab-org/growth/product/issues/7)), but may need to partner with Manage on larger efforts like a completely [new onboarding](https://gitlab.com/gitlab-org/gitlab-ce/issues/57832) experience.
* The group ultimately owning the change - in this case, Manage - would review Growth's contributions into their area of the product 
and - like a contribution coming from the wider community - ultimately own the final result.

### Growth RADCIE and DRIs

In alignment with with Gitlab's [RADCIE](https://about.gitlab.com/handbook/people-group/directly-responsible-individuals/#radcie) approach, the DRIs for the following tasks would be:

| Task | DRI |
| ------ | ------ |
| Hypothesis Generation | Growth Product/Engineering |
| Experiment Design | Growth Product/Engineering | 
| Experiment Implementation | Growth Product/Engineering | 
| Contribution Review | Stage Product/Engineering |
| Experiment Ramp | Growth Product/Engineering |
| Post-Experiment Analysis| Data Team |
| Post-Experiment Decision | Growth Product/Engineering |
| Maintenance | Stage Product/Engineering |

## Fulfillment group

Responsible for licensing & billing workflows, which have a huge impact on renewal rates, upgrade rates, and customer satisfaction, and represent important levers for the Growth team.

Please see the [Fulfillment direction page](https://about.gitlab.com/direction/fulfillment/) for more information about Fulfillment's mission, vision, and priorities. 

## Telemetry group

Responsible for product usage data, including proper instrumentation, working with BizOps and Engineering to ensure product usage data is stored correctly, and working across the Product team to ensure product usage data is analyzed and visualized in a way that can drive product and growth decisions.

Please see the [Telemetry direction page](https://about.gitlab.com/direction/telemetry/) for more 
information about Telemetry's mission, vision, and priorities.

