---
layout: handbook-page-toc
title: "Security Automation"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Our process

Opportunities for security automation originate from the day-to-day operations of other teams, active security abuse, and from internal requirements. If you have an automation idea for anything security-related at GitLab, please add the **security-automation** label to your issue and we will prioritize requests during our bi-weekly meeting.

## Slack bots

### [Security Pager](https://gitlab.com/gitlab-com/security-tools/security-pager)

The security pager creates the /security command to create urgent security issues as [designed](https://gitlab.com/gitlab-com/security-tools/security-pager/issues/1) to support the security on-call process.

### [h1-gitlab](https://gitlab.com/gitlab-com/security-tools/h1-gitlab)

The h1-gitlab project is a suite of tools for integrating HackerOne with GitLab. It creates the /h1import command in our many Slack channels.

### Security Release Emails

Coming soon.

### Tenable.io Scanner

Coming soon.

## Third-party service audit ingestion

GitLab uses many third-party services with audit trails that must be centralized for thread analysis and detection.

### Audit log storage in ELK

All service logs are stored in a special security-only [ELK cluster](https://a869810ddfaf4581a33acbb86edb2c35.us-east-1.aws.found.io:9243/app/kibana#/discover).

### Services in-scope

| Service | Feature | Status | Method | Project |
| --- | --- | --- | --- | --- |
| 1Password | Activity Log CLI | Investigating | Poll | |
| Google Suite | Reports API (Watch) | Complete | Webhook | [gsuite-ingestor](https://gitlab.com/gitlab-it-opsbot/gsuite-ingestor) |
| Okta | ? | In Progress | Poll | |
| Slack | Audit Log API | [Blocked](https://gitlab.com/gitlab-com/gl-security/secops/operations/issues/224) | Poll | |

## Threat analydid & detection

### CI Runner Abuse Detection
