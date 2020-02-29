---
layout: handbook-page-toc
title: Documentation
---

GitLab’s documentation is crafted to help users, admins, and decision-makers learn about GitLab features and to optimally implement and use GitLab to meet their [DevOps needs](/stages-devops-lifecycle/).

The documentation is an essential part of the product. Its source is developed and stored with the product in its respective paths within the GitLab [CE](https://gitlab.com/gitlab-org/gitlab-ce/tree/master/doc), [EE](https://gitlab.com/gitlab-org/gitlab-ee/tree/master/doc), [Runner](https://gitlab.com/gitlab-org/gitlab-runner/tree/master/docs), and [Omnibus](https://gitlab.com/gitlab-org/gitlab-ee/tree/master/doc) repositories. It is published at [docs.gitlab.com](https://docs.gitlab.com) (offering multiple versions of all products’ documentation) and at the `/help/` path on each GitLab instance’s domain, with content for that instance’s version and edition.

It is GitLab’s goal to create documentation that is complete, accurate, and easy to use. It should be easy to browse or search for the information you need, and easy to contribute to the documentation itself.

All standards and practices for contributing documentation are found within the docs in the [GitLab Documentation guidelines](https://docs.gitlab.com/ee/development/documentation/) section.

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Documentation is the single source of truth (SSOT)

Please see the [SSOT section in the Documentation Style Guide](https://docs.gitlab.com/ee/development/documentation/styleguide.html#documentation-is-the-single-source-of-truth-ssot)
and especially read the [docs-first methodology](https://docs.gitlab.com/ee/development/documentation/styleguide.html#docs-first-methodology).

## Who contributes to the documentation

Everyone can contribute. For documentation needs resulting from the development
and release of new or enhanced features, the developer responsible for the code
writes or updates the docs.

Technical writers monitor the planning and merging of documentation, reviewing all changes after they are merged, unless they are brought in to the process earlier for specific questions, reviews, or projects.

For more information on these processes, see the [Documentation section of our Development docs](https://docs.gitlab.com/ee/development/documentation/).

## Who merges the documentation and when

Anyone with master access at GitLab is welcome to merge documentation changes to GitLab's master branches,
provided they believe the content is:

- clear and sufficiently easy to understand for the intended audience
- technically accurate (per their own knowledge or trust in the author or SME reviewers)
- in line with GitLab's [Documentation Guidelines](https://docs.gitlab.com/ee/development/documentation/) and [Style Guide](https://docs.gitlab.com/ee/development/documentation/styleguide.html)

GitLab's technical writers review all merged content to confirm it is clear and meets the structure/style guidelines, often making further improvements.

Note that documentation does not need to be perfect in structure and style to merge.
It is better to publish an improved doc (simply better than what's
currently there) and later refine it than to hold the doc in a review process
where users do not know it exists or are using an inferior version of the doc.

However, if you know or suspect that a doc has been merged while in need of further
enhancement, please create another MR or issue for this work.

For more information, see the [Documentation section of our Development docs](https://docs.gitlab.com/ee/development/documentation/).

## Resources about GitLab documentation

- The [Documentation Guidelines](https://docs.gitlab.com/ee/development/documentation/), including pages on:
   - [Documentation workflow](https://docs.gitlab.com/ee/development/documentation/workflow.html)
   - [Documentation page structure and template](https://docs.gitlab.com/ee/development/documentation/structure.html)
   - [Documentation Style Guide](https://docs.gitlab.com/ee/development/documentation/styleguide.html)
   - [Documentation site architecture](https://docs.gitlab.com/ee/development/documentation/site_architecture/index.html)
- The [Documentation Markdown Guide](/handbook/engineering/ux/technical-writing/markdown-guide/)
- The [GitLab Docs project](https://gitlab.com/gitlab-org/gitlab-docs/) which contains the code that pulls the documentation content from multiple repositories and builds docs.gitlab.com

## The Technical Writing team

For more information on the team and how it works to continually improve GitLab docs, see
[Technical Writing](../product/technical-writing/) in the Product section of the handbook.
