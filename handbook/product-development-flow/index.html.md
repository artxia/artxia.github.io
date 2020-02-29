---
layout: handbook-page-toc
title: Product Development Flow
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview & philosophy

GitLab's [product mission](/handbook/product/#product-team-mission) is to consistently create products and experiences that users love and value. To deliver on this mission, it's important to have a clearly defined and repeatable flow for turning an idea into something that offers customer value. Note that it's also important to allow open source contributions at any point in the process from the wider GitLab community - these will not necessarily follow this process. 

This page is an evolving description of how we expect our cross-functional development teams to work, but at the same time reflects the current process being used. All issues are expected to follow this workflow, though are not required to have passed every step on the way.

The goal is to have this page be the single source of truth, but it will take time to eliminate duplication elsewhere in the handbook; in the meantime, where there are conflicts this page takes precedence. 

Because this page needs to be concise and consistent, please ensure to follow the prescribed [change process](#change).

## Workflow Summary

| Stage (Label) | Track | Responsible | Completion Criteria | Who Transitions Out |
| ----- | --------- | ------------------- | --------------- | ------------------ |
| `workflow::start` | N/A | Product | Item has enough information to enter problem validation. | Product | 
| `workflow::problem validation` | [Validation](#validation-track) | Product | Item is validated and defined enough to propose a solution | Product | 
| `workflow::design`  | [Validation](#validation-track) | UX | Design work is complete enough for issue to be implemented | UX | 
| `workflow::solution validation`  | [Validation](#validation-track) | Product, UX, Engineering | Product Manager works with UX and Engineering to confirm proposed solution is valuable, usable, viable and feasible | Product |
| `workflow::needs issue review` | [Review](#review-track)(Optional) | Product (Original PM) | Issue needs review by a Peer PM to help issue become more iterative, clearer, and better aligned with GitLab strategy | Product (Reviewer PM)
| `workflow::issue reviewed` | [Review](#review-track)(Optional) | Product (Reviewer PM) | Issue has been reviewed and is ready to move to Build | Product (Original PM) |
| `workflow::planning breakdown`  | [Build](#build-track) | Product, UX, Engineering | Issue has backend and/or frontend labels and estimated weight attached | Engineering | 
| `workflow::scheduling`  | [Build](#build-track) | Engineering | Issue has a numerical milestone label | Product/Engineering |
| `workflow::ready for development` | [Build](#build-track) | Engineering | An engineer has started to work on the issue | Engineering | 
| `workflow::In dev` | [Build](#build-track) | Engineering | Initial engineering work is complete and review process has started | Engineering | 
| `workflow::In review` | [Build](#build-track) | Engineering | MR(s) are merged | Engineering | 
| `workflow::verification` | [Build](#build-track) | Engineering | Work is demonstrable on production | Engineering | 
| `workflow::blocked` | N/A | Product/Engineering | Work is no longer blocked | Engineering |

## Validation track  

For new ideas where the customer problem and solution is not well understood, PMs and UXers should work together to validate new opportunities before moving to the Build track. The **Validation** track is an independent track from the always moving **Build** track. 

PMs and UXers should work together to get 1-2 months ahead, so that the Build track always has well-validated product opportunities ready to start. Milestone work should be prioritized with the understanding that some milestones may include more validation efforts than others. We should heavily prioritize validation when our confidence about the proposed problem or solution is lower than 80%. 

Validation cycles may not be necessary for things like bug fixes, well understood iterative improvements, minor design fixes, etc.

### Opportunity Canvas

One of the primary artifacts of the validation track is the Opportunity Canvas. The Opportunity Canvas introduces a lean product management philosophy to the validation track by focusing on level of confidence, hypotheses, and lessons learned as the document evolves. At completion, it serves as a concise artifact for understanding user pain, business value, and the constraints to a particular problem statement.

Please note that an opportunity canvas is not required for product functionality or problems that already have well-defined jobs to be done (JTBD). For situations where we already have a strong understanding of the problem and its solution, it is appropriate to skip the opportunity canvas and proceed directly to solution validation. It might be worth creating an opportunity canvas for existing features in the product to test assumptions and current thinking, although not required. 

**References**:
* [Opportunity Canvas Template](https://docs.google.com/document/d/1pTEMcwH10xWilQEnVc65oC6PdC3VMjn2XoARfNTaHkc/edit#)
* [Recorded Video of an Opportunity Canvas Review](https://www.youtube.com/watch?v=8-5i-zKFgMk)
* [Example Opportunity Canvas - Fine Grained Access Control (GoogleDoc)](https://docs.google.com/document/d/1c_FPLZ8W7Gjl0tvZSybEKWvcCzJ3AgxlQNFvwm92IHo/edit#heading=h.4mt5fmtn0ax4)
* [Example Opportunity Canvas - Error Tracking (Mural)](https://app.mural.co/t/gitlab2474/m/gitlab2474/1568925801645/71e7e6352180a1492a19a3d3ed6f96d48fefd597)

### Validation phase 1: Validation backlog

Label: `workflow::validation backlog`

Every PM should maintain a backlog of potential validation opportunities. Validation opportunities may come from customers, internal stakeholders, product usage insights, support tickets, win/loss data, or other [sensing mechanisms](/handbook/product/product-management/process/#sensing-mechanisms). Validation opportunities should be captured as an issue and described in customer problem language, and should avoid jumping ahead to feature/solution language. 

Sometimes it can be tricky to identify a good issue for problem validation. The following situations often are good criteria:

- Initiating work on a new [product category](/handbook/product/categories/)
- Defining the next [maturity state](/direction/maturity/) for a product category (for example, when researching how to go from `Complete` to `Lovable`)
- The envisioned feature is large or introduces a major change to the user experience (for example, reorganizing the sidebar navigation)
- Understanding if a job to be done [(JTBD)](https://hbr.org/2016/09/know-your-customers-jobs-to-be-done) is the purpose for which customers buy or use the product 
- Targeting a new user or buyer persona

Some items will skip the problem validation phase. In these cases the problem is well understood and has been validated in other ways. When skipping problem validation, ensure the issue description is clear with the rationale and sensing mechanisms used to skip the problem validation phase.

To queue an item in your validation backlog:

1. Create a new issue describing the problem using the "Problem Validation" issue template in the [GitLab project](https://gitlab.com/gitlab-org/gitlab/issues), applying relevant stage and group labels. If you are doing research related to an open issue/epic, consider notifying participants there of the research issue so they can participate.
1. Once each section of the issue template has been filled out (or validated, in the case of pre-existing issues), apply the [RICE formula](https://www.productplan.com/glossary/rice-scoring-model/) as a prioritization mechanic and record this in the description.
1. Apply the `workflow::validation backlog` label

### Validation phase 2: Problem validation

Label: `workflow::problem validation`

Good product development starts with a well understood and clearly articulated customer problem. Once we have this, then generating solutions, developing the product experience, and launching to the market is much more effective. The danger in not starting with the problem is that you might miss out on solutions that come from deeply understanding the customer problem. A poorly defined problem statement can also cause the design and development phases to be inefficient.

You should pull items from your validation backlog in the problem validation process on a regular cadence to ensure you always have validated problems for your groups to start working on.

To run the problem validation process:

1. PM creates an issue using the [Problem Validation template](https://gitlab.com/gitlab-org/gitlab/-/blob/master/.gitlab/issue_templates/Problem_Validation.md).
1. PM applies the `~"workflow::problem validation"` label to the associated issue; this automatically removes the `~"workflow::validation backlog"` label.
1. PM fills out an [opportunity canvas](#opportunity-canvas) to the best of their ability. Ensure the problem and persona is well articulated and add the opportunity canvas to the issue's [Designs](https://docs.gitlab.com/ee/user/project/issues/design_management.html#the-design-management-page). Note that you should include content for the solution and go-to-market sections, possibly with low confidence; this section may be likely to change, but thinking it through will help clarify your thoughts.
1. PM fills out a customer interview guide with a draft list of interview questions. You can find a good guide [here](https://www.nngroup.com/articles/user-interviews/).
1. PM reviews customer interview guide and opportunity canvas with UX peers. UX Research can help craft interview questions and recruit candidates for interviews: request their help by following the [UX research request process](/handbook/engineering/ux/ux-research/#how-ux-research-product-and-product-design-work-together-on-research).
1. PM and UX together conduct at least 5 interviews with target customers. Interview notes should be logged as an issue in the [user interview project](https://gitlab.com/gitlab-com/user-interviews) and labeled with relevant stages. (training video coming soon)
1. PM and UX synthesize customer feedback using affinity mapping or other techniques.
1. PM finalizes the opportunity canvas with the synthesized feedback.
1. PM schedules a review of the opportunity canvas with Scott Williamson, Christie Lenneville, and the Product Director for your section. Weekly time blocks will be held. You can contact Stefanie Haynes to get your review added to one of the weekly time blocks.
1. Once approved:
   1. If the result of the canvas is to move forward and solve the problem, move to design and solution validation phase below to begin solutioning the validated problem.
   1. If the result of the canvas is to _NOT_ move forward solving the problem, write that in the canvas and the original issue and close it. Making an active decision to not do something is just as valuable, and sometimes moreso, than deciding to move forward on the wrong thing.

### Validation phase 3: Solution Validation

Labels: `workflow::design` followed by `workflow::solution validation`

Once the customer problem is well understood, it's time to ideate and validate solutions to the problem. As always, you should be consistently moving issues forward from the backlog, to problem validation, and solution validation to ensure that there's validated problems to deliver.

Solution Validation is also relevant for APIs and other technical features that don't require a UI. Communicate these solutions using artifacts such as API docs, workflow diagrams, etc. Involve your Engineering Managers in creating and reviewing these artifacts to gain a shared understanding of the solution and receive input on feasibility.

To run the solution validation process:

1. PM applies the `~"workflow::design"` label to the associated issue, automatically removing the `~"workflow::problem validation"` label.
1. PM and UX co-create the user stories required to solve the customer problem. The UX Research handbook has resources to [learn more about story mapping](/handbook/engineering/ux/ux-research-training/user-story-mapping).
1. UX ideates to create one or more concepts based on feedback from assigned stakeholders (PM, engineering, technical writers, and other peers). This ideation results in a prototype (low- or high-fidelity wireframes or an interactive UI prototype) that addresses the user stories for at least the first (and potentially subsequent) releases. UX shares the prototype with stakeholders and requests feedback.
1. When the design is complete and the team is ready to test the solution, UX applies the `~"workflow::solution validation"` label.
UX and PM validate the prototype with at least 5 target users through usability testing interviews. 
1. PM updates the associated user stories and/or story map and opportunity canvas with any final changes.
1. PM must articulate success metrics for each opportunity and ensure a plan for product instrumentation and dashboarding are in place.
1. UX presents the design as part of the [Product design process](/handbook/engineering/ux/ux-designer/#product-design-process) which serves as an approval to move to the build track.

At this point we have validated the problem and solution, and the issue is ready to enter the build track. _Alternately_, if you have concerns that the issue(s) you created isn't small enough of an iteration, consider running it through the Review track.

## Review track (optional*)

The (iteration) Review track is an **optional step** in the flow that brings peer PMs in to help you hone your skills at _iteration_, _clarity_, and _strategy_. Keeping issues small an iterative is core to how GitLab maintains [velocity](), writing a "small" issue is often (counterintuitively) more difficult than writing a bigger one, and understanding the _entire strategy_ of how GitLab operates is a herculean task. Having a helping hand with these tasks is important to professional development, and it ensures that our entire Product organization continues to improve.

You should consider requesting a review when:

1. If you're having specific challenges defining the problem, identifying the affected personas, or breaking down the solution to small chunks of work.
1. If there are potential design or technical dependencies across Sections, Stages, or Groups.
1. This issue takes the product in a novel direction or adds functionality unlike anything else in the product

_*Note: **If you are a new GitLab team member**, you should request reviews of the first 2-3 issues you create. It will help familiarize you with what we're looking for in an iteration, get more comfortable with our process, and meet your fellow team members. Once you've gone through a few reviews, this track can be considered optional._

If you would like a peer to reivew one of your issues (or epics):

1. Add the `workflow::needs issue review` label to your issue
1. Post a link to the issue in the [**#issue-reviews**](https://gitlab.slack.com/archives/CSX3RHE4C) channel in Slack
   1. _Note: if there is a time crunch and you need a review quickly, be sure to mention when it needs to be done by._
1. The issue gets picked up by a Reviewer PM, who adds a ✅ reaction on the Slack message.
1. Reviewer PM reads through the issue and leaves feedback on these criteria:
   1. **Iteration:** Has the solution been broken down as much as possible? Is it small enough to be completed in one milestone rather than spanning multiple milestones? Have implementation risks been considered and minimized?
   1. **Clarity:** Is the problem well versed and the personas identified? Could someone outside the group or category understand the issue? Is the  value being delivered to the users articulated?
   1. **Strategy:** How will it work in Gitlab as whole? Does it tie back to category strategy or stage direction?
1. Things for the reviewer to **not** do:
   1. Don't just _enforce the template_. Instead, give contextual feedback with the appropriate template as a reference point.
   1. Don't treat this as another task to check off, but instead, take this opportunity to engage in conversation and improve our organizations ability to iterate.
   1. Don't assume that the other PM will do exactly what you say. You're providing recommendations, not edicts.
1. When complete, the Reviewer PM adds the `workflow::issue reviewed` label and lets the original PM know that the review is complete.

You can view all the work in happening in this track [on this board](https://gitlab.com/groups/gitlab-org/-/boards/1569699).

## Build track  

The build track is where we develop, launch, and improve validated solutions over time.

### Build phase 1: Plan

Label: `workflow::planning breakdown`

The build track starts with PM, UX, SET, and Engineering Managers breaking down the opportunities into well-defined issues: 

1. PM applies the `workflow::planning breakdown` label.
1. PM, UX, and EM do a final review of the designs to ensure everyone understands the solution. Then, PM, UX, and EM start breaking down the implementation into smaller issues. Story mapping is a recommended technique to do this in a rapid and collaborative fashion. The resulting issues should be written by PMs in user-story-style language whenever possible: "As a (who), I want (what), so I can (why/value)." Issues should not only be about feature details, but should also establish functional, performance, documentation, and security acceptance criteria. In some cases, you need to update existing issues - if you were doing problem validation on an issue that already had a problem to solve/proposal in the issue (i.e., an older or customer-created issue), and you've come up with a new problem statement that isn't very close to the original, you should strongly consider opening a new issue for the new problem. Changing the problem statement in an issue almost always causes the discussion to become confused and may lose track of the original (potentially still valid for some users) problem statement.
1. Using the output of story mapping, PM creates separate epics and issues for implementation. Use the [feature proposal template](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/.gitlab/issue_templates/Feature%20proposal.md) as a guide for writing both epics and features. For issues requiring documentation changes/additions, add the `documentation` label and complete other relevant [PM documentation responsibilities](https://docs.gitlab.com/ee/development/documentation/workflow.html#product-managers). For issues requiring new or updated UI text, add the `UI text` label.
1. At this point, the original validation issue can be closed as further work labeling and activity will happen on the implementation issues.
1. PM should break the issue down into the smallest possible iteration definition that adds customer value. 
1. If sizing for it is large, or won't fit into a milestone, then PM + EM should collaborate to break it down further.
1. If PM + EM can't figure out an iteration definition that will fit within the sprint/milestone, then it is ok to push it to the next milestone to give the team more time to find an iteration definition that will fit.
1. SET owns the completion of the `Availability and Testing` section in the Feature Proposal to complete the definition of done. As we grow to reach our [desired ratio](/handbook/quality/#staffing-planning), we will only have the quad approach in groups where we have an assigned SET in place. 
   1. PM assigns the issue to the counterpart SET.
   1. SET is the DRI for the `Availability and Testing` section, ensuring that the strategy accounts for all test levels and facilitating discussions and feedback with the group.
   1. SET determines if the feature change needs to run `package-and-qa` regression job, this is made clear in the above section.
   1. SET applies the ~"quad-planning" label and unassign themselves from the issue.
1. EM works with assignees to create a `Build Plan` that outlines the number of MRs and responsibilities for assigned team members. EM and PM provide a focus on [iteration](/handbook/product/#iteration) when reviewing these plans.
1. EM applies `workflow::scheduling` to allow for a buffered priority queue.
1. PM assigns them to a specific milestone/release. Follow the product development timeline when scheduling implementation issues into milestones. Note that engineering will apply the workflow::ready for development and deliverable labels during the next phase, in alignment with the PM.

### Build phase 2: Develop & Test

Labels: `workflow::ready for development`, `workflow::In dev` (along with `workflow::ready for review` as queue state while waiting for maintainer), `workflow::In review`, `workflow::blocked`, `workflow::verification` (sub-states for verification are `workflow::canary` and `workflow::staging`)

The develop and test phase is where we build the features and test them before launch:

1. Engineering teams move items into workflow::ready for development and apply the deliverable as they commit to them, in alignment with the PM.
1. When the milestone arrives, engineering teams execute on the scheduled work. Acceptance criteria as set forth in the issues must be met before a feature is deemed complete.
1. In parallel with development, the PM creates release post content, collaborating with PMM on messaging and positioning
1. Work deemed out of scope or incomplete by engineering is taken back into the plan phase for grooming and rescheduling for completion. The label `workflow::planning breakdown` should be reapplied.
1. During the launch phase, the delivery team updates the validation labels as it flows through the validation process in staging and canary.
1. Engineering/quality performs testing to ensure the feature is working as it flows through the environments
1. PM should also conduct feature-level acceptance testing to ensure that the intended user value was, in fact, delivered.
1. Documentation should be complete and available before proceeding to the launch phase.

### Build phase 3: Launch

Labels: `workflow::production`

1. Once the feature is deployed to production, the delivery team sets the workflow label to `workflow::production`. At this point the feature is launched.
1. Engineering/quality/PM should validate again that the feature works for all users.
1. The release post item needs to be merged following the instructions in the [template](https://gitlab.com/gitlab-com/www-gitlab-com/-/blob/master/.gitlab/merge_request_templates/Release-Post.md), which will then cause it to appear on the [gitlab.com releases page](/releases/gitlab-com/).

If the feature is part of the [Dogfooding process](/handbook/product/product-management/process/#dogfooding-process):

1. At this point, you should label the issue as `Dogfooding::Promote Feature`
1. You should present it in the weekly Product Call to get everyone on board
1. You could consider announcing it on the Company Call or in #company-announcements
1. Your Section Lead should also be actively promoting the feature to other sections

### Build phase 4: Improve

Label: TBD

After launch, the PM should pay close attention to product usage data and customer feedback to guide follow-on iterative improvements, until success metrics are achieved or a decision is made that the product experience is sufficient.

## Change
All substantive merge requests to this page require the following approvals before merging:
1. VP of Product
1. Director of User Experience

The following people need to be on the merge request to stay informed:
1. Senior Director of Development
1. Director of Quality 
