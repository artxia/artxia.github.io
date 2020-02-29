---
layout: handbook-page-toc
title: Customers Portal Admin Panel Documentation
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Introduction

The target audience is the internal GitLab team, and covers the [admin panel](https://customers.gitlab.com/admin/) of the [Customers Portal](https://customers.gitlab.com). Customers or subscription managers should refer to the [Customers](https://docs.gitlab.com/ee/subscriptions/index.html) section of GitLab's user documentation for help in using the portal, or the [licensing FAQ](https://about.gitlab.com/pricing/licensing-faq/) for questions on subscriptions such as how users are counted.

## Searching

When using the admin panel search, be aware that results will be based on searching only one field at a time. For example, entering a person's full name will likely provide no results because the system will not search first and last name at the same time, only one or the other.

We recommend searching by email address, partial email address (e.g. company domain), or company name. When searching by name, enter only first *or* last name.

## Adding another account to manage subscription

NOTE: **Note:**
Due to [issue 654](https://gitlab.com/gitlab-org/customers-gitlab-com/issues/654), this is currently discouraged as it will break the upgrade process.

1. Find existing customer and click on `Edit`.
1. Copy the Zuora and SFDC IDs.
1. Paste the IDs into the same fields for the requesting customer.

## Check or change trial expiry date

NOTE: **Note:**
Until [issue 420](https://gitlab.com/gitlab-org/customers-gitlab-com/issues/420) is implemented, the trial status and expiry date will only show on the account that initiated it. Other accounts that are group owners will show trial as `false`.

1. Find customer who initiated the trial.
1. Click on the `GitLab Groups`.
1. Change the trial date as necessary. **Warning:** Do not change the date to a date prior to today's date in UTC timezone.
