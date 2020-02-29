---
layout: handbook-page-toc
title: "Release UX Team"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

The [Release stage](/stages-devops-lifecycle/release/) includes all features that help you guarantee software delivery by automating the release and delivery of applications, shortening the delivery lifecycle, streamlining manual processes, and accelerating team velocity. 

The Release UX team's goal is to enable these complex flows by providing the best experience in software delivery. Our design mission is bring to the forefront simple, clean ways to make GitLab the tool of choice for deploying where, when, and how users want to.

Our biggest partners are the stages under the CI/CD section ([Verify](/direction/cicd/#verify) & [Package](/direction/cicd/#package)), Ops ([Configure](/direction/cicd/#package)), and Infrastructure ([Delivery](https://about.gitlab.com/handbook/engineering/infrastructure/team/delivery/)).

### Release UX DRIs

- Progressive Delivery UX [DRI](/handbook/people-group/directly-responsible-individuals/): [Mike Nichols](https://gitlab.com/mnichols1)
- Release Management UX [DRI](/handbook/people-group/directly-responsible-individuals/): [Rayana Verissimo](https://gitlab.com/rayana)

### Shared UX

We divided the Release stage into dedicated experience groups to align with a similar [split](/handbook/product/categories/#release-stage) undertaken by our engineering and PM counterparts. In order to continously deliver a seamless user experience, we share responsibility in the overal vision, goals, and research initiatives related to overlapping features. The Progressive Delivery & Release Management UX teams work closely together and have shared coverage in the following areas:

- gitlab-ci.yml
- Environments
- Merge requests
- Issues
- Project settings
- User settings
- Kubernetes
- Runner
- Audit log

## Our users

We have different user types we consider in our experience design effort. Even when a user has the same title, their responsibilities may vary by organization size, department, org structure, and role. Here are some of the people we are serving:

- [Release Manager](/handbook/marketing/product-marketing/roles-personas/#rachel-release-manager)
- [Software Developer](/handbook/marketing/product-marketing/roles-personas/#sasha-software-developer)
- [Development Tech Lead](/handbook/marketing/product-marketing/roles-personas/#delaney-development-team-lead) 
- [DevOps Engineer](/handbook/marketing/product-marketing/roles-personas/#devon-devops-engineer)
- [Product Manager](/handbook/marketing/product-marketing/roles-personas/#parker-product-manager)
- QA

## Our customer

### Customer: Release Management

The product vision for Release Management has become more focused on providing advanced administration capabilities for release coordination and deployment tracking in GitLab. This is to build on the data asset we have at GitLab that starts from users purchasing GitLab to build product fast in a continuously integrated way. We will expand this journey by helping them coordinate and deploy at scale.

Today, mono-repository projects deploying with Kubernetes are most able to take advantage of our offering. We are targeting customers needing to coordinate across many teams and groups to successfully deploy. Regulated industries are top benefactors of our offering.

### Customer: Progressive Delivery

Coming soon.

## Our UX strategy

We will commit to stay aligned on shared UX with the engineering groups as much as possible, being the conversation drivers with product managers and other counterparts.

The Release UX team is working together to uncover customers' core needs, what our users’ workflows look like, and defining how we can make tasks easier. Our strategy involves the following actions:

| Strategy | Cadence |
| ------ | ------ | 
| Jobs to be done framework | Quarterly |
| [UX Scorecards and recommendations](/handbook/engineering/ux/ux-scorecards/) | Quarterly |
| [Opportunity canvas](https://about.gitlab.com/handbook/product-development-flow/#opportunity-canvas) | Ad hoc | 
| Stakeholder interviews | Ad hoc | 
| User and customer interviews | Ad hoc |

Visit [CI/CD UX](/handbook/engineering/ux/ci-cd/) to read about the department strategy. 

### Other innitiatives we value

- **Think Big sessions**: Every two weeks we brainstorm as a technical, product, and design team about our vision, roadmap, and all other components involved in creating a great experience for our GitLab customers. We aim to align on medium and long term goals.
- **UX Vision**: Clarify and establish a shared understanding of our user experience foundations together with Product Managers.
- **Perform heuristic evaluation on competitors.**
- **Improve the product overall user experience**: Partner up with other teams/individuals responsible for improving our product's UI, and bringing back knowledge to Pajamas and gitlab-ui.
- **Share and learn**: Stay up to date with other design teams to learn from their experience.

### Our UX Scorecards 

#### Primary Jobs to be done ([JTBD](https://gitlab.com/groups/gitlab-org/-/epics/1326))

| JTBD | Description | Walkthrough | Recent recommendation | Rescoring |
| ------ | ------ | ------ | ------ | ------ |
| **Create a Release and update it** | When tracking important deliverables in my project, I want to easily create and manage release entries in GitLab, so I can provide packaged software, notes, and files for people to use. | [View issue](https://gitlab.com/gitlab-org/gitlab-design/issues/431) | [View issue](https://gitlab.com/gitlab-org/gitlab-design/issues/505) | [View issue](https://gitlab.com/gitlab-org/gitlab-design/issues/516) |
| **Deploy to GitLab Pages** | When using a static site generator, I want automatic deployments every time I commit a change, so that I can keep my site up to date without manual builds. | [View issue](https://gitlab.com/gitlab-org/gitlab-design/issues/412) | [View issue](https://gitlab.com/gitlab-org/gitlab-design/issues/513) | [View issue](https://gitlab.com/gitlab-org/gitlab/issues/197956) |

## Release UX Team

The following people are members of the Release Team:

- [Rayana Verissimo](https://gitlab.com/rverissimo) - Senior Product Designer
- [Mike Nichols](https://gitlab.com/mnichols1) - Senior Product Designer

### Stable counterparts

The following members of other functional teams are our stable counterparts:

- [Nadia Udalova](https://gitlab.com/nudalova) - UX Manager 
- [Lorie Whitaker](https://gitlab.com/loriewhitaker) - Senior UX Researcher
- [Marcia Ramos](https://gitlab.com/marcia) - [Senior Technical Writer](https://about.gitlab.com/job-families/engineering/technical-writer/), Create, Release

### Our team meetings

- **Release PM/UX**: Twice a week.
- **Release Managers**: Once a week. Meeting to collaborate as a cross-functional team on top Release topics that require speed or might be better served as a working session.
- **CI/CD UX**: Every two weeks. Meeting to discuss our stages UX shared efforts, review designs, and iterate on our strategy.

### Follow our work

Our [Release (CD) UX YouTube channel](https://www.youtube.com/playlist?list=PL05JrBw4t0KoyqCjN4f79w0dYZusHLx15) includes UX Scorecard walkthroughs, UX reviews, group feedback sessions, team meetings, and more.
