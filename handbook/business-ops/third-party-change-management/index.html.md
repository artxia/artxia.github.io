---
layout: markdown_page
title: "Third-Party Change Management"
---

## On this page
{:.no_toc}

- TOC
{:toc}

## Third-Party Change Request Workflow

Making a user- or group-level change doesn't require a third-party change request. For example, if your team decides to make a change to one of your team's group settings on GitLab.com, a third-party change request isn't required. However, if you decide to make a change to a configuration or setting for GitLab.com globally, that requires a change request. Another example is Google Drive. If you decide to make a change to one of your team's Google Drive folders, no third-party change request is required. But if you change the the default sharing setting of all of Google Doc for GitLab, a third-party change request is required.

Third-party change requests are important because they help us track and manage the risk of making wide-reaching configuration and setting changes. To make a global configuration or settings change to a [third-party application or service](/handbook/business-ops/tech-stack-applications/):

* [Create an issue in the Change Management project](https://gitlab.com/gitlab-com/business-ops/change-management)
* Select either the Change Management template (internal changes) or the Third Party Change Management template.
* A Review Board, consisting of Security, IT, and Legal (as needed) will review the change request.
  * Security and IT will review the change request and engage Legal as needed.
* After Security, IT, and Legal (if applicable) has reviewed and approved the change request, IT will engage our Approval Board (consisting of our Director level team members) for review and approval. 
  * To move forward with the change, we will need at least a 75% approval rate from our Approval Board. 
* In the event a change request is not approved, IT will work with the individual submitting the change request to address any blockers/concerns. 

## Communication Changes

If during the third-party change request process it's decided team members should be notified of a change (for example, changing the default Google Doc sharing settings), IT will communicate the change and its impact by posting in `#company-announcements` and during the company call as well.

**If the change is approved and requires communication to team members, communicate the change and its impact.**

Once the change request has been approved, IT will make company announcements providing the change implementation timeline (call and slack channel) for 4 days prior to completing the change request. Regardless of when the change request has been approved, communication will always begin on a Monday and communicated daily through to Thursday. This will fall inline with our Company Calls. Please note the change will always be implemented on a Monday following the communication schedule. This will allow the ability and coverage should the change need to be backed out and re-reviewed. 

**If no communication is required or the change has been communicated already, make the change.**
