---
layout: handbook-page-toc
title: Defend Planning
---

# On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# How we do planning

To better ensure we are ready to start work on issues in the next iteration, the planning process works as part of a monthly cadence. Since [GitLab releases ship](/upcoming-releases/) on the 22nd of each month, this schedule for the **current+1** release begins on the first week of the month when the **current** release is being executed.


## Week 0 / ONGOING: Planning Breakdown

*if release X.0 ships on March 22, then planning for release X.1 starts by the week of Jan 27-31*

Issues at the top of our *backlog* (&/or upcoming release milestones) will go through **Planning Breakdown** with Project Managers & the respective Engineering teams at least ONE week prior to Week 1. Weekly group level syncronous meetings will facilitate this discussion. 

As we improve, this planning breakdown activity should become an ongoing discussion around new issues as they are created. 

Weekly syncronous group meetings will: 
* Review list of issues for that group which are in the `workflow::planning breakdown` stage.
* Questions to be answered
     * [ ]  Are requirements clear enough to understand intent of request?
     * [ ]  Do we know the boundaries of work to be accomplished?
     * [ ] Is research, solution validation complete?
* If the issue is acceptable, the EM will move it to the workflow::scheduling step to indicate EMs & PMs should include it in capacity planning & release scope discussions. 
* If the answer is, “No”, to any of the above questions, enumerate questions and assign back to PM. 


## Week 1: Release Scope DRAFT Complete

*if release X.0 ships on March 22, then week 1 for planning breakdown for release X.1 begins on or before the week of Feb 3-7*

Engineering Managers and Product Managers complete a first pass of **current+1** release. Initial questions, calling out known availability/vacation, rough scope identified.

* PM Output: All issues for current+1 release put in `workflow::scheduling` state.
* EM Output: Candidate engineers identified for issues in `workflow::scheduling` state and are assigned for grooming.

## Weeks 2: Grooming

*if release X.0 ships on March 22, then week 2 for planning release X.1 is Feb 10-14*

Identify volunteers to provide a high-level implementation plan and weight. Assign if necessary.
Kick back to PM if the issue covers more than one work boundary.
* Engineers [groom](#grooming) issues assigned in the **current+1** release. 
* They are encouraged to ask questions and autorized to push back on PM if issues aren’t ready.
* Upon completion, Engineers unassign & move issues which pass grooming to `workflow::ready for development` state.

### *Why are we assigning issues for grooming?*

Issues are assigned to engineers to ensure we have focus on the highest-priority items, as determined by Product Management. This is **not** an assignment to work on the issue, though there will be an effort made to make sure the engineer(s) who groom an issue will be the one(s) working upon it.


## Week 3: Release Scope FINAL & Kickoff!

*If release X.0 ships on March 22, then week 3 for planning release X.1 is Feb 17-21. **Execution of release X.1 begins on Feb 18**!*

Scope of the next release is finalized by Engineering Managers and Product Managers.

* EM output: `Deliverable` or `Stretch` labels applied to issues for which we have capacity to achieve.
* PM output: Remove all issues lacking above labels from the next release.
* EM output: assignment of issues to individuals to work in the next release.



# Grooming

Backlog grooming is the most important step to ensure an issue is ready to move into development and that the issue will match everyone's expectations when the work is delivered. 

The goal of the grooming process is to 
*  Identify and resolve outstanding questions or discussions.
*  Raise any questions, concerns or alternative approaches.
*  Outline an implementation plan.
*  Ensure issue is ready to be worked on.
*  Assign a weight to the issue.


## Grooming steps for Engineers:

1.  Assign yourself the issue.
2.  Backend/Frontend labels:
    * If a backend engineer is required for the issue, ensure a `backend` label. Otherwise, remove any backend label, assign any relevant labels and you are done. 
    * If a frontend engineer is required for the issue, ensure a `frontend` label. Otherwise, remove any frontend label, assign any relevant labels and you are done. 
3.  Check the issue for completeness.
    *  Does it have the necessary designs?
    *  Is the functionality clearly articulated and is there a consensus or decision on how it should function?
    *  Are the technical details outlined? 
    *  Has a consensus been reached or decision been made in areas of discussion?
    *  Are there dependencies? Call those out. 
4. If the issue is not complete:
    *  Tag the relevant people that can help complete the issue and outline what is needed. Tag the appropriate EM and PM, so they know that the item can not be fully groomed.
    * If you are unable to resolve blockers to your grooming within a reasonable amount of time (2-3 days dependign on size of initative) see [Failing Grooming](#failing-grooming).
5. Ensure the issue is fully understood.
    *  Update the issue description with the final description of what will be implemented.
    *  Update the issue description with an [implementation plan](#implementation-plan). 
    *  Ensure the issue title is accurate for the work being done.
    *  Open up new issues for 'follow-up' work, or work that was forced out of scope. 
6. Assign a [weight](#weights) and set the label `workflow::ready for development`.

When you are done grooming, anyone should be able to read the issue description and should know what the issue is solving, how it is solving the problem, 
and the technical plan for implementing the issue. 

In order for someone to understand the issue and its implementation, they should **not** have to read through all the comments. The important bits should be captured in the description as the **single source of truth.** 

## Failing Grooming:

An issue should fail grooming if it can not be worked on without additional information or decisions to be made. To fail an issue:
1.  Leave a comment on the issue that it can not be worked on, and highlights what still needs to be done.
2.  Unassign yourself if you can not contribute further to issue at the current time. 
3.  Assign the `workflow::blocked` label.

## Weights

Weights are used as a *rough* order of magnitude to help signal to the rest of the team how much work is involved. 
Weights should be considered an artifact of the grooming process, not the purpose of the grooming process. 

It is perfectly acceptable if items take longer than the initial weight. We do not want to inflate weights, 
as [velocity is more important than predictability](/handbook/engineering/#velocity-over-predictability) and weight inflation over-emphasizes predictability. 

### Possible Values

We are using the Fibonacci sequence for issue weights.

- 1: trivial task - can be completed in less than a day.
- 2: small task - can be completed in 1 day.
- 3: medium task - can be completed in 2-3 days.
- 5: large task - can be completed in 1 week.
- 8: extra-large task - can be completed in 2-2.5 weeks.
- 13: extra-extra-large task - will take someone the entire iteration to complete.
- Bigger: the task may be an epic in disguise and needs to be split up. The issue has failed grooming if it falls in this range.

The weighting system roughly aligns with other teams within GitLab. We deviate from the scales used by other teams to provide enough granularity in our planning process.

* [Plan:Project Management BE Team Capacity Planning](/handbook/engineering/development/dev/plan-project-management-be/#capacity-planning)
* [Create: Source Code BE Team Weights](/handbook/engineering/development/dev/create-source-code-be/#weights)
* [Geo Team Weights](/handbook/engineering/development/enablement/geo/#weights)
* [Enablement:Memory](/handbook/engineering/development/enablement/memory/)

## Implementation Plan

A list of the steps and the parts of the code that will need to get updated to implement this feature. The implementation plan should also 
call out any responsibilities for other team members or teams. An example: https://gitlab.com/gitlab-org/gitlab/issues/5656#execution

The goal of the implementation plan is to spur critical analysis of the issue and have the groomer think through what parts of the application will get touched.
The implementation plan will also permit other engineers to review the issue and call out any areas of the application that might have dependencies or 
been overlooked.

## FAQs

**Q:** Should discovery issues be groomed?

**A:** Yes. Discovery issues should be groomed but some of the steps above may not be relevant. Use good judgement to apply the process above. The purpose of 
grooming a discovery issue is to make sure the scope of the discovery is clear, what the output will be and that the prerequisites for the discovery are known 
and completed. Discovery issues can have a habit of dragging out or not creating actionable steps, the grooming process should lock down what needs to be answered
in the discovery process. 

**Q:** If an issue has both frontend and backend work how should I weight it?

**A:** Issues that require both frontend and backend work can be broken into [sub-issues as outlined in this document](https://gitlab.com/gitlab-com/www-gitlab-com/issues/4588). 
