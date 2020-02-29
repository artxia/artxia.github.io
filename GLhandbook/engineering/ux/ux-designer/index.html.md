---
layout: handbook-page-toc
title: "Product Designer Workflow"
---

## On this page

{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## GitLab wide workflows

Like other departments at GitLab, we follow the [GitLab Workflow](/handbook/communication/#everything-starts-with-a-merge-request), the [Engineering Workflow](/handbook/engineering/workflow/), and the [Product Development Workflow](/handbook/product-development-flow/). Reviewing those resources is a good starting point for context on the Product Designer workflows below.

## UX Department workflows

### Product Designer onboarding

If you are just starting out here at GitLab, welcome! Make sure to review all the pages here in the UX section of the handbook, they will help you get oriented. There is also a specific page dedicated to [Product Designer onboarding](/handbook/engineering/ux/uxdesigner-onboarding/).

### Planning and managing capacity

Product designers are responsible for stage- and UX-team-assigned work. Product designers are responsible for working with their stage peers and managers, as needed, to manage their capacity and complete their work on target and on time.  Here are some guidelines to help Product Designers manage their work:

Product Designers:
* Make sure discipline peers are aware of UX team assignments, such as UX OKRs, and what you'll need from them to succeed.
* Account for time off (both yours and others) as best you can during milestone planning.
* Let your manager know right away, if you believe you're not trending to complete your work. The sooner your manager knows, the higher the likelihood they can resolve the issue and manage expectations.

Managers:
* If requested by Product Designers, help them set a baseline capacity for stage- and UX-team-assigned work each milestone. Designers can use this information to balance work and manage expectations.
* Quantify strategy work with clear time-to-complete (TTC) expectations, measurable goals, and deadlines.
* Resolve team questions, concerns, and blockers quickly.
* Make sure cross-functional partners are aware of UX OKRs and their associated dependencies.

### Going out of office (OOO)

When going out of office (OOO), be sure to commit your working Sketch files to your [progress folder in the GitLab Design repository](https://gitlab.com/gitlab-org/gitlab-design/blob/master/CONTRIBUTING.md#for-gitlabbers-), so designers covering for you are able to access working drafts of designs that may get shipped during milestones you are OOO.

Read more in the [Paid time off](/handbook/paid-time-off/#pto-ninja) and [How we work](/handbook/engineering/ux/how-we-work/#time-off) pages.

### Working on issues

This section provides an overview of how we work with issues. But it's very important for you to communicate with your PM and EMs early and often about how you should work together. Many teams have different flavors of this process as they have adapted to the needs of that product and that team.

#### Scheduling issues in a milestone

All issues in a milestone labeled [`Deliverable`](https://gitlab.com/groups/gitlab-org/issues?state=opened&label_name%5B%5D=Deliverable) that need UX will be assigned to a Product Designer by the kickoff. Issues labeled [`Stretch`](https://gitlab.com/groups/gitlab-org/-/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=Stretch) may or may not be assigned to a Product Designer by the kickoff. Learn more about how we use Workflow labels in the [GitLab Docs](https://docs.gitlab.com/ee/development/contributing/issue_workflow.html).

#### Priority for UX issues

UX works on issues in the following order:
* Has the current release milestone and is labeled `Deliverable`, `workflow::problem validation`, `workflow::design`, or `workflow::solution validation`.
* [UX OKRs](/company/okrs/) 
* Has the current release milestone and is also labeled `Stretch`
* Has the `Pajamas` label
* Has the next release milestone
* [Has the `Accepting merge requests` label](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&label_name[]=Accepting+merge+requests&label_name[]=UX)
* [Has milestone **Next 2-3 months**](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&milestone_title=Next+2-3+months&label_name[]=UX)
* [Has milestone **Next 3-6 months**](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&milestone_title=Next+3-6+months&label_name[]=UX)
* [Has milestone **Backlog**](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&milestone_title=Backlog&label_name[]=UX)
* [Popular or with high community involvement (number of comments or upvotes)](https://gitlab.com/groups/gitlab-org/issues?label_name[]=UX&sort=upvotes_desc&state=opened)
* [Everything else](https://gitlab.com/groups/gitlab-org/-/issues?state=opened&label_name[]=UX)

### Product design process

#### Define the opportunity:
* Work with your PM to [validate][product-dev-flow] *who* you're designing for, *what* you're designing, and *why* you're designing it.
* Help your PM express the who/what/why as a user story. For example, "As a (who), I want (what), so I can (why/value)." If you’re asked to implement a non-evidence-based how, then ask the PM to refocus on the who/what/why, so everyone can work together to find the best how.
* Help your PM to define [MVC](/handbook/values/#minimum-viable-change-mvc) success criteria, prioritizing MVC “must-haves” and non-MVC “should-haves” and “could-haves.” (Note that this success criteria is subject to change based on new learning from the iterative design process and customer feedback.)

Before you design:
* Investigate whether there is [existing UX Research](/handbook/engineering/ux/ux-research#ux-research-archive) or data that could help inform your decisions and measure results. If there isn't, contact your UX Researcher to conduct (or guide you in conducting) research for the problem.
* Consider conducting competitive analysis to inform your work. Look for terminology, functionality, and UX conventions that can help refine success criteria. Only stray from industry conventions with strategic intent, such as capitalizing on [disruptive innovation](https://www.economist.com/the-economist-explains/2015/01/25/what-disruptive-innovation-means) opportunities. We want users to migrate from other tools to ours, and they’re more likely to be successful and satisfied when our products use conventions that are familiar based on other tools they've used.
* Consider creating user flows or journey maps to help ensure you've considered the entire workflow and also to help communicate that workflow to your team.

#### Ideate and iterate:
* Share design ideas in the lowest fidelity that still communicates your idea. To keep the cost of change low, only increase fidelity as design confidence grows and implementation requires.
* Ask for feedback from your PM throughout the design process to help refine your understanding of the problem and solution criteria.
* Ask for feedback from other UXers to help improve your work. At minimum, you'll get objective feedback and new ideas that lead to better solutions. You might also get context you didn’t know you were missing, such as GitLab-specific or industry-standard design conventions.
* Collaborate with your group's technical writer when the work involves substantial UI text, such as user-assistance or links back to documentation. For details on how to collaborate, see the [UI text Planning and authoring](/handbook/engineering/ux/technical-writing/workflow/index.html.md) section of the Technical Writing handbook. Additionally, involve your technical writer in the [review process](#technical-writer-ui-text-reviews) for smaller copy changes, such as UI elements labels.
* For a significant UX change, like a new workflow or feature, include your UX Manager in feedback sessions, as they might have input into the overall direction of the design or knowledge about initiatives on other teams that might impact your own work.
* Engage engineering peers early and often. Their insight into technical costs and feasibility is essential to determining viable designs and MVCs. Also, invite design feedback, especially if you’re solving for a development workflow they’re familiar with.
* [Validate][product-dev-flow] your proposed solution with customers/users.

#### Design reviews:
Gathering feedback is an essential part of the design process. Design reviews, similar to engineering code reviews, allow Product Designers to solicit feedback on proposed solutions. Because GitLab is an all-remote company, design reviews are also important for building shared understanding with the broader UX team.
* Each Section UX Manager will regularly coordinate with their stage group Product Designers to incorporate peer reviews and provide feedback on research process/findings, designs, and prototypes.
* We record Design Reviews to share with Product Managers and UX peers asynchronously.
* Optionally, each stage group can post their Design Reviews to GitLab Unfiltered.

#### Refine MVC:
* UX issues have a tendency to expand in scope. Work with your PM and developers to revisit which aspects of the design are “must haves” versus those that can be pushed until later. Document non-MVC concepts and research in new issues, marking the new issues as related to the original issue. If you’re ever unsure how to split apart large issues, work with your UX Manager. 
* If developers need to begin before you have validated your designs, and a planning pivot to another validated UX issue or perhaps dev debt issues is not an option, then look for high confidence and low risk changes devs can start work on while you validate the remainder of the solution. To mitigate these scenarios, PMs and UXers should work together to [get 1-2 months ahead](/handbook/product-development-flow/#validation-track), so that the Build track always has well-validated product opportunities ready to start.
* Developers should be able to build a working feature within one release. If a feature is too large to build within one release, work with your PM and Engineering team to determine the best way to split the feature into smaller segments.

#### Present an MVC solution:
* After you've validated your solution with users, propose just one solution. Proposing multiple alternative solutions for others to pick undermines your position as a UX expert and leads to design by committee. If you have a good reason to propose multiple alternative solutions, make sure to explain why.
* When sharing asynchronously in an issue, make sure your audience has the context necessary to understand your proposal and how they can help. Is it clear who will use the solution and what it will enable them to accomplish? Do you need feedback or assistance from stakeholders? If so, on what specifically?  Or, are you looking for approval? To make reviewing easier, have you highlighted things that changed since the last review?
* @mention your UX Manager on the issue for feedback. UX Managers have a broader view of work that's happening across the product, enabling them to provide feedback that is helpful for maintaining strategic alignment, a consistent level of quality, and functional consistency.
* Frame design discussions around the customer and the problem being solved, not the UI or functionality itself. When presenting, start with the current state and how it fails to meet user needs, and then walk through the proposed solution from the user’s point of view. As the discussion unfolds, continually tie everything back to the user’s experience and needs.
* Anticipate questions that others might have, and try to answer them in your proposal comments. You don’t have to explain everything, but try to communicate a bit of your rationale every time you propose something. This is particularly important when proposing changes or challenging the status quo, because it reduces the feedback loop and time spent on unnecessary discussions. It also builds the UX Department’s credibility, because we deal with a lot of seemingly subjective issues.
* Keep the SSOT updated with what’s already agreed upon so that everyone can know where to look. This includes images or links to your design work.
* If you’re working with design files, follow the instructions in the [GitLab Design project contribution guidelines][gitlab-design-project-contribution-guidelines] and regularly commit them.
* If you are proposing a solution that will introduce a new UX paradigm, or change an existing one, please consider the following:
    1. Will this pattern be inconsistent with other areas of the application?
    1. Will other areas of the application need to be updated to match?
    1. Does this new pattern significantly improve the user experience?
    1. If you decide that it is worth changing/updating the pattern, there are additional steps that must be followed. See the [Maintain](/handbook/engineering/ux/ux-designer#maintain) section below for those steps.

#### Deliver
* Once your work is complete and all feedback is addressed, make sure that the issue description, the SSOT, is updated with a section called "Solution". This is where you should direct people when they have questions about what should be done and how.
* As applicable, commit all design assets and files according to the instructions in the [GitLab Design project contribution guidelines][gitlab-design-project-contribution-guidelines].
* Whenever possible, provide spec-previews using the Sketch Measure plugin. Details on how to use this are located in the [design repository on the contribution page](https://gitlab.com/gitlab-org/gitlab-design/blob/master/CONTRIBUTING.md#superpowers-).
* If the solution needs to be broken out into smaller issues for implementation, apply the `workflow::planning breakdown` label and stay involved by walking PM and Engineering through the proposed solution and participating in the conversation to break down the issue.
* If the solution needs to be scheduled by PM and/or EM, apply the `workflow::scheduling` label and mention the [responsible product manager](/handbook/product/categories/#devops-stages) to [schedule it](/handbook/engineering/workflow/#scheduling-issues). It is also the Product Designer's responsibility to communicate with the assigned engineer to ensure they understand the solution.
* If the issue is meant for implementation in the current milestone, review the solution with the assigned engineer(s) and/or engineering manager. If they are comfortable with the solution, you can apply the `workflow::ready for development` label.
* There are times that a Product Manager might request that an issue is moved to the Build phase before the Product Designer feels that the experience meets UX Department standards. In that case, the Product Designer should create follow-on issues and/or apply the `UX debt` label to indicate that the product doesn't meet UX requirements and will require immediate iteration. 

#### Follow through
* Encourage Engineers to scope down features into multiple merge requests for an easier, more efficient review process.
* When breaking down features into multiple merge requests, consider how the UX of the application will be affected. If merging only a portion of the total changes will negatively impact the overall experience, consider using a feature branch or feature flag to ensure that the full UX scope ships together.
* When breaking solutions into smaller parts, make sure to share the end design goal, so that the entire team has context. Giving everyone the full picture helps developers write code aimed at achieving that goal in the future.
* Keep the issue description updated with the agreed-on scope, even if doesn’t impact your work. This is everyone’s responsibility. The issue description must be the Single Source Of Truth (SSOT), not the discussion or individual comments.
* Not all issues are scheduled immediately, which means changes are likely needed when the issue is prioritized. The Product Designer responsible for a particular stage group should be aware of open issues within their product area and work to prioritize them accordingly with their respective product managers, even if they are not the original designer who worked on the issue.
    * To stay up to date with issues in your product area, subscribe to the label that matches your stage group.
    * Review issues within your stage group label regularly.
    * Actively contribute to planning meetings to ensure all open issues are being discussed and prioritized.
* When working on an issue, keep the SSOT in the description updated until the issue is closed. This applies to both text and mockups. Previous content (by a PM, for example) should be removed or archived into a separate section in the description. If the developer working on the issue ever has any questions on what they should implement, they can ask the designer to update the issue description with the design.
* For obvious changes, make the SSOT description update directly. [You don't need to wait for consensus](/handbook/values/). Use your judgement.
* When the issue is actively being worked on, make sure you are assigned and subscribed to the issue. Continue to follow both the issue and related merge request(s), addressing any additional UX issues that come up.

#### UX visual reviews
* UX is part of the MR review process.
* UX Review requests are high priority. Tackle them as quickly as you are able.
* Test locally, and do not rely on screenshots.
* Be thorough. There should be as little back and forth as possible.
* If you are asked to review an MR for an issue you were not assigned to, remind the author who the assigned designer is and assign to original designer for review.
* When reviewing an MR, please use the following order of importance:
    * Functionality first: Does it work?
    * Edge cases: Are there any unexpected edge cases?
    * Visual consistency: Does it conform to our Design System and workflows in other product areas?
* Remember to stick to the issue, create issues for further updates to avoid scope creep.

Sometimes you will find a UX problem but a decision will be made to merge the code anyway. When this happens, create a new issue to fix the problem and label it with `UX Debt` per this section on [UX labels](handbook/engineering/ux/ux-department-workflow/#how-we-use-labels).


#### Follow-up after design is complete

For changes that affect Pajamas, such as introducing a new UI component, refining an existing component, or adding significant clarity to the usage of a component, you should take the following additional steps:

* For changes that affect the user interface: [Create a **UX Pattern** issue](https://gitlab.com/gitlab-org/gitlab-design/issues/new?issuable_template=UX%20Pattern) in GitLab Design and follow its checklist to record the new standard.
* For other changes: Create an issue and/or MR in the [Design System](https://gitlab.com/gitlab-org/gitlab-services/design.gitlab.com) to update the documentation.
* As applicable, create issue(s) to update areas of the application that are affected by this pattern.
* Add an agenda item to the next UX weekly call to inform everyone of those changes.
* If the change/addition is a significant one, consider adding it to the Company Call to inform the company of the changes.

### Working on UI text with technical writers
Any additions or changes to UI text require review by the group's technical writer, though you may have already discussed plans and ideas during the Product Design phase.
This includes button or menu labels, error messages, user-assistance microcopy, and any other text that may be surfaced in the UI.

* Ensure the issue and MR have the `UI text` label.
* Message the [technical writer for the group] in the MR to request a review, including any specific files or lines they should review, and how to preview or understand the location/context of the text from the user's perspective.

### UX Showcase

The UX Showcase is a recurring meeting that allows each stage group to walk through various research findings and design solutions with key stakeholders from Product, UX, Engineering, and Leadership. These sessions are recorded and available on GitLab Unfiltered.

Showcase objectives:
* Increase awareness of the value delivered through UX by highlighting business and customer value.
* Increase visibility into UX research, design opportunities, and solutions.
* Increase exposure of stage group UX activities to the broader organization.

Process:
* Prepare and share an agenda prior to meeting.
* Provide context for the problem: the scope of the problem, why it's an important problem to solve, what we learned during research, and any constraints (business and technical) that impacted the solution.
* State the desired goals of the showcase.
* Walk attendees through the solution(s).
* Tip: Be yourself and tell the story of the work you did. Try to use existing assets from the project, like mockups and flows, rather than creating something new. It shouldn't take a lot of time to prepare for the meeting. You might prepare a few slides, but this is optional.

Artifacts:

Presenter(s) should come prepared with sufficient artifacts to tell the story of the user's journey. Use your best judgement to determine what will most effectively convey your story: a presentation, process diagram, journey map, series of mockups, prototype, etc.

Audience:
* Stage Group Product Designer/Researcher (Presenter)
* Product
* Engineering
* Relevant Leadership (Director of UX, VP of Eng, CEO, VP of Product)

Frequency:

Showcases will happen on a biweekly (every other week) basis. Meetings will be an hour long, allowing 4 stage groups to present. Each stage group Product Designer is expected to fill out the agenda (attached to the meeting invite) for that week prior to presenting. The current schedule can be found [here](https://docs.google.com/spreadsheets/d/1gw0DlbLy8WJclSQsYIbay8gPbNJH_S8k8pesejCVSew/edit?usp=sharing).



### Approach to communication

As design can be subjective, discussion can heat up. Sometimes team members won't agree on the best approach. Always try to be [direct](/handbook/values/#directness) but [kind](/handbook/values/#kindness). Try to give your best reasoning for your choices, and evaluate everyone's ideas and suggestions. Come up with a solution instead of discussing endlessly. If you think additional perspective is needed, mention a fellow Product Designer in the issue, or take it a step further and suggest that we perform some [solution validation](https://about.gitlab.com/handbook/engineering/ux/ux-research/#solution-validation) to let the data guide our design direction. Finally, remember that at GitLab we can [disagree, commit, and disagree](https://about.gitlab.com/handbook/values/#disagree-commit-and-disagree).

### Creating a design evaluation (guidance for Product Designers)

1. Create a new issue using the `Design evaluation` template in the [UX research project](https://gitlab.com/gitlab-org/ux-research) and `@` mention the relevant UX Researcher, UX Manager, and Product Manager for the product stage.

1. Update the `Design evaluation` with the following:
    * Add as much information as you can to the issue.
    * Label the issue with the area of GitLab you’re testing (for example, `navigation`), the status of the issue (`in progress`), and the Product stage (for example, `devops::manage`).
    * Mark the issue as `confidential` until the research is completed so it doesn’t influence user behavior.
    * Assign the issue to yourself.

1. The UX Researcher will quickly review the issue and advise whether it is feasible to send the study during the time frame you have requested (Occasionally, we may need to stagger when the study is sent since we do not want to bombard users with research studies). The UX Researcher will add a milestone to the issue.

1. Create your test in [UsabilityHub](https://usabilityhub.com/). Product Designers share a login for UsabilityHub. The credentials are stored in 1Password. Some tips for creating a test:
    * Use a descriptive test name. Make sure it includes the issue number of the research proposal.
    * We don't incentivize users to participate in design evaluations. In order to encourage participation, keep the test length under 10 minutes (UsabilityHub will provide you with an estimated completion time as you build your test).
    * Try to avoid [priming users](https://www.nngroup.com/articles/priming/). For example, when writing tasks for a first click or navigation test, where possible, avoid using terms that appear in the interface or which give the answer away.
    * Always question whether you are using the right research methodology. For example, if you are asking lots of straight-up questions, would it be best to ditch the design evaluation and write a survey instead? Check out the [UsabilityHub guides](https://usabilityhub.com/guides) for common use cases for each methodology.
    * Remember what users say and what they do can be very different. Just because users prefer a design, doesn't mean they can use it. Find out more about [when you should use preference tests](https://www.nngroup.com/articles/first-rule-of-usability-dont-listen-to-users/).
    * Read more about how to [test visual design](https://www.nngroup.com/articles/testing-visual-design/).
    * If you're ever in doubt when creating your test, reach out to a UX Researcher!

1. When your test is ready, update the `Design evaluation` issue with any outstanding information and ping the relevant UX Researcher for a final review.

1. Once you and the UX Researcher are happy with the test, the UX Researcher will distribute the test to subscribers of GitLab First Look.

1. When you and the UX Researcher feel that sufficient data has been collected, the test can be closed in UsabilityHub.

1. You are responsible for analyzing any tests you have created. You are always welcome to reach out to a UX Researcher for assistance.

1. Document the study within a Google document. The report should include:
    * Research hypotheses
    * Research methodology
    * Findings
    * Next steps/recommendations.

1. Update the `Design evaluation` issue with the following:
    * Link to the report.
    * Unmark the issue as `confidential`.
    * Update the status of the issue to `done`.
    * Close the issue. You should stay assigned to closed issues so it's obvious who completed the research.

[ux-guide]: https://docs.gitlab.com/ee/development/ux_guide/
[gitlab-design-project-contribution-guidelines]: https://gitlab.com/gitlab-org/gitlab-design/blob/master/CONTRIBUTING.md
[twitter-sheet]: https://docs.google.com/spreadsheets/d/1GDAUNujD1-eRYxAj4FIYbCyy8ltCwwIWqVTd9-gf4wA/edit
[product-dev-flow]: /handbook/product-development-flow/
