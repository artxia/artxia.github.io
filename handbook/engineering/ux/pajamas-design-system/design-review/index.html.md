---
layout: handbook-page-toc
title: "Design Review Process"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

Design reviews are mandatory for every [`design.gitlab.com`](https://gitlab.com/gitlab-org/gitlab-services/design.gitlab.com), [`gitlab-ui`](https://gitlab.com/gitlab-org/gitlab-ui), and [`gitlab-svgs`](https://gitlab.com/gitlab-org/gitlab-svgs) merge request, as well as for [`gitlab-ce`](https://gitlab.com/gitlab-org/gitlab-ce) and [`gitlab-ee`](https://gitlab.com/gitlab-org/gitlab-ee) merge requests that have the [UX label](/handbook/engineering/ux/ux-department-workflow/#how-we-use-labels) added to it.

All designers are maintainers of the [`gitlab-design`](https://gitlab.com/gitlab-org/gitlab-design) project. If you are interested in becoming a Maintainer of UI (`.scss`) for `gitlab-ce`, `gitlab-ee`, and `gitlab-ui` projects, please follow the [Engineering Review Workflow](/handbook/engineering/workflow/code-review/).

To perform a review, you should familiarize yourself with and follow our [Code Review Guidelines](https://docs.gitlab.com/ee/development/code_review.html), [Design Contribution Guidelines](https://gitlab.com/gitlab-org/gitlab-design/blob/master/CONTRIBUTING.md), and the contribution guidelines for every aforementioned project.

You can find all design reviewers and maintainers by looking on the [team page](/company/team/) and filtering by `UX Department` or on the list of [GitLab Engineering Projects](/handbook/engineering/projects/), both of which are fed by `data/team.yml` file.

These guidelines describe who would need to review, approve, and merge your (or a community member's) merge request.

## Reviewer

All GitLab designers can (and are encouraged to) perform design and code reviews on merge requests that impact product design. This includes contributions from GitLabbers and the wider GitLab community. If you want to review merge requests, you can wait until someone assigns you one, but you are also more than welcome to browse the list of open merge requests and leave any feedback or questions you may have.

Note that while all designers can review all merge requests, the ability to accept merge requests is restricted to maintainers.

## Maintainer

Maintainers are GitLab designers who: 

* Are experts at design and [code review](https://docs.gitlab.com/ee/development/code_review.html)
* Know the GitLab product, design guidelines, and code base very well
* Are empowered to accept merge requests in one or several [GitLab Engineering Projects](/handbook/engineering/projects/)

Every project has at least one maintainer, but most have multiple, and some projects (like gitlab-ui and design.gitlab.com) have separate maintainers for design and frontend.

As with regular reviewers, design maintainers can be found on the [team page](/company/team/) or on the list of [GitLab Engineering Projects](/handbook/engineering/projects/).

Read more about what makes great maintainers in the [Engineering Review Workflow](/handbook/engineering/workflow/code-review/#maintainer).

### How to become a maintainer

We follow the same maintainer guidelines as our Engineering counterparts. Read more about guidelines and how to become a maintainer in the [Engineering Review Workflow](/handbook/engineering/workflow/code-review/#how-to-become-a-maintainer).

#### Trainee maintainer

We follow the same trainee maintainer program as our Engineering counterparts. Anyone may nominate themselves as a trainee by opening a tracking issue using the [Trainee design maintainer template].

During the traineeship, one of the existing design maintainers is assigned as Support Maintainers to each trainee. The Support Maintainer will direct merge requests for review, give feedback on proposals, and discuss process or progress during 1:1 sessions. Trainees can always reach out to other maintainers for feedback and guidance separate from the dedicated Support Maintainer.

#### Current trainee maintainers

| Trainee | Support Maintainer |
| ------ | ------ |
| [Rayana Verissimo](https://gitlab.com/rayana) | [Taurie Davis](https://gitlab.com/tauriedavis) |
| [Jeremy Elder](https://gitlab.com/jeldergl) | [Taurie Davis](https://gitlab.com/tauriedavis) | 
| [Juan J. Ramirez](https://gitlab.com/jj-ramirez) | [Pedro Moreira da Silva](https://gitlab.com/pedroms) |
| [Amelia Bauerly](https://gitlab.com/ameliabauerly) | [Pedro Moreira da Silva](https://gitlab.com/pedroms) |

[Trainee design maintainer template]: https://gitlab.com/gitlab-com/www-gitlab-com/issues/new?issuable_template=Trainee%20design%20maintainer
