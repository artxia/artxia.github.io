---
layout: markdown_page
title: "101 - No Tissues with Issues"
---
## Objective:
 A quick overview of how to plan and manage regular work using GitLab.   The focus of this page is to help you learn how to work with Groups, Projects, Issues and Boards to plan and manage the your work and your team's work.


### Orient on the big picture

(what is it, why do we have it, what does it do, how is it related to everything else)

### GitLab Groups
:5

| In order to manage multiple projects (portfolios of projects), the GitLab Group is the entity that enables strategic planning and tracking of business initiatives through delivery.  At the Group Level, you can manage sub-groups, projects, epics, milestones, roadmaps and group level boards. [Groups](https://docs.gitlab.com/ee/user/group/)  With GitLab Groups you can assemble related projects together and grant members access to several projects at once. Groups can also be nested in subgroups.  | ![GitLab Group](/images/solutions/scaled-agile/gitlab-groups.png){: .margin-right20 .margin-left20 .margin-top20 .margin-bottom20 .image-width80pct } ‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾ |

### GitLab "Project"
:10

| The project in GitLab is the core building block, where work is organized, managed, tracked and delivered.  A project in GitLab enables the team to collaborate and plan their work in the form of Issues (use cases/requirements), Issue boards (Kanban), and Milestones (Sprints). With [Projects](https://docs.gitlab.com/ee/user/project/) in GitLab, you can create projects for hosting your codebase, use it as an issue tracker, collaborate on code, and continuously build, test, and deploy your app with built-in GitLab CI/CD.  Your projects can be available publicly, internally, or privately, at your choice. GitLab does not limit the number of private projects you create. | ![GitLab Project](/images/solutions/scaled-agile/gitlab-project.png){: .margin-right20 .margin-left20 .margin-top20 .margin-bottom20 .image-width80pct } ‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾ |
|  The GitLab Project is much, much, much more than simply project management.  The GitLab project unlocks the power of an industry leading source code management repository and a CI/CD pipeline.  The Merge Request is the linkage between the issue and the actual code changes.  The merge request captures the design, implementation details (code changes), discussions (code reviews), approvals, testing (CI Pipeline), and security scans.  | ![GitLab Repository](/images/solutions/scaled-agile/gitlab-repository.png){: .margin-right20 .margin-left20 .margin-top20 .margin-bottom20 .image-width80pct } |

### Group vs Project

:15

#### Group  

- Groups are like 'folders'

![GitLab Group](/images/solutions/scaled-agile/group_overview.png)

#### Project

- Projects have many 'things' like issues, repositories, merge requests, etc.

![GitLab Project](/images/solutions/scaled-agile/project_overview.png)  

#### Hands on: Explore Groups and Projects
- [Link to the GitLab Marketing Group](https://gitlab.com/gitlab-com/marketing?sort=name_asc)  
- [Link to www-gitlab-com Project](https://gitlab.com/gitlab-com/www-gitlab-com)
- [GitLab 101 Exercise Group and Projects](https://gitlab.com/gitlab_101)  This group (subgroups and projects is for GitLab 101 exercises)

### Labels

:20

The label in GitLab is a flexible and powerful mechanism to tag and track work.   Labels are used to define columns in the issue boards and make it easy to search and find issues or merge requests related to a common theme. **Labels can be defined at EITHER Group or Project level**

[Labels](https://docs.gitlab.com/ee/user/project/labels.html) allow you to categorize issues or merge requests using descriptive titles like bug, feature request, or docs. Each label also has a customizable color. Labels allow you to quickly and dynamically filter and manage issues or merge requests you care about, and are visible throughout GitLab in most places where issues and merge requests are located.

#### Hands on: Explore Group and Project Labels
Explore these two examples of Labels:

- [Link to Group Label List in the GitLab 101 Group](https://gitlab.com/groups/gitlab_101/-/labels)
- [Link to GitLab 101 ABM Sample Project Label List](https://gitlab.com/gitlab_101/marketing/account-based-marketing/labels)
- Create a Label in this project [GitLab 101 ABM Sample Project](https://gitlab.com/gitlab_101/marketing/account-based-marketing/labels)  

### Issue

:30

The issue in Gitlab is the fundamental planning object.  It is where the team documents the use case in the description, discusses the approach, estimates the size/effort (issue weight), tracks actual time/effort, assigns work, and tracks progress.  Labels enable the team to tag issues, track status, and associate issues with different initiatives.  **Issues are part of a Project**

[Issues](https://docs.gitlab.com/ee/user/project/issues/)  Issues can have endless applications. For example, Issues can be used to; Discuss the implementation of a new idea, Submit feature proposals, Ask questions, Report bugs and so on.

 ![Issues](https://docs.gitlab.com/ee/user/project/issues/img/issues_main_view.png)  

#### Hands on: Create an Issue

- Examine these issues:
  - [A discussion](https://gitlab.com/gitlab-com/marketing/field-marketing/issues/76)
  - [Planning an event (using an issue template):](https://gitlab.com/gitlab-com/marketing/field-marketing/issues/175)

- Create an Issue in this project:
[GitLab101: Account Based Marketing sample project](https://gitlab.com/gitlab_101/marketing/account-based-marketing/issues)


#### Boards

:35

Boards provide a flexible and dynamic approach to visually manage a project.  Boards make it easy for a team to create lists and move issues from one list to another.  List on the board can be defined by a **label**, **assignment**, or **milestone**.  Here, teams can manage their backlog of work, prioritize the items, and then move the issues to the team or specific stage in the project.  Each list in the board calculates the total size (weights) of the associated issues, enabling the team to understand how much work is assigned at any given time. **Boards are available for EITHER Group or Project**

[Project Issue Boards](https://docs.gitlab.com/ee/user/project/issue_board.html) The GitLab Issue Board is a software project management tool used to plan, organize, and visualize a workflow for a feature or product release. It can be used as a Kanban or a Scrum board. It provides perfect pairing between issue tracking and project management, keeping everything in the same place, so that you don’t need to jump between different platforms to organize your workflow. With GitLab Issue Boards, you organize your issues in lists that correspond to their assigned labels, visualizing issues designed as cards throughout that lists.  
![Boards](https://docs.gitlab.com/ee/user/project/img/issue_boards_core.png)

The **group level issue board** makes it possible for oversight and governance of the projects and sub groups.  This view, makes it easy to see how specific issues are flowing through the lifecycle and to understand the overall capacity of the teams.
 ![GitLab Kanban Board](/images/gitlab-kanban-board.png)


##### Hands on: Play with boards


   - Todd's CMO board is a group level board, where labels define the lists: https://gitlab.com/groups/gitlab-com/marketing/-/boards/906226
   - The Strategic Marketing Sales Enablement board: https://gitlab.com/gitlab-com/marketing/product-marketing/boards/918030
   - The Plan/ Milestone board, where the lists are defined by Milestones: https://gitlab.com/groups/gitlab-org/-/boards/706864
   - The Plan Backend assignment board, where the lists are defined by **who** will be doing the work on a specific release: https://gitlab.com/groups/gitlab-org/-/boards/631316


  - **Create an BOARD in this Project** : [Account Based Marketing](https://gitlab.com/gitlab_101/marketing/account-based-marketing/issues)

#### Milestones

:40

Milestones establish a target date for a sprint or specific bundle of issues and code changes to be delivered.  The milestone enables the team to either set a specific Start and Stop for the work, as in a Sprint, or the milestone could be a fixed point in time.  **Milestones are EITHER Group or Project**

| [Milestones](https://docs.gitlab.com/ee/user/project/milestones/)  Milestones in GitLab are a way to track issues and merge requests created to achieve a broader goal in a certain period of time. Milestones allow you to organize issues and merge requests into a cohesive group, with an optional start date and an optional due date. |  ![Milestone burndown chart](https://docs.gitlab.com/ee/user/project/milestones/img/burndown_chart.png) ‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾  |


### Group Level Planning

:50

#### Epics

In order to track groups of related issues, the GitLab epic gives product owners and leaders the ability to link and manage work over an extended time frame.  Planning work use Epics allows you to create parent and child epics. An epic can span multiple milestones and makes it easier to manage the overall flow and priority of work. **Epics are GROUP ONLY**

| [Epics](https://docs.gitlab.com/ee/user/group/epics/)  let you manage your portfolio of projects more efficiently and with less effort by tracking groups of issues that share a theme, across projects and milestones | ![Epics](https://docs.gitlab.com/ee/user/group/epics/img/epics_list_view_v12.5.png)  |

#### Roadmaps

| The roadmap is a visual representation of the various epics for the group.   The roadmap view can be filtered by label and organized by start / stop date of the epics in order to visualize the sequence of work.   At this point, Gitlab doesn't create dependencies between issues or epics. | ![GitLab Roadmap](/images/solutions/scaled-agile/gitlab_roadmap.png)‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾ |


**Consider Deprecating this table**

| Object  |   Description  |
| [Merge Requests (MR)](https://docs.gitlab.com/ee/user/project/merge_requests/) allow you to exchange changes you made to source code and collaborate with other people on the same project.  | ![Merge Requests](https://docs.gitlab.com/ee/user/project/merge_requests/img/project_merge_requests_list_view.png)  |
| [Repository](https://docs.gitlab.com/ee/user/project/repository/)  is what you use to store your codebase in GitLab and change it with version control. A repository is part of a project, which has a lot of other features. | ![Repository](https://docs.gitlab.com/ee/user/project/repository/img/jupyter_notebook.png)  |
| [Pipelines](https://docs.gitlab.com/ee/ci/pipelines.html)  is a group of jobs that get executed in stages. All of the jobs in a stage are executed in parallel (if there are enough concurrent Runners), and if they all succeed, the pipeline moves on to the next stage. If one of the jobs fails, the next stage is not (usually) executed. You can access the pipelines page in your project’s Pipelines tab. | ![Pipelines](https://docs.gitlab.com/ee/ci/img/pipelines.png) |
