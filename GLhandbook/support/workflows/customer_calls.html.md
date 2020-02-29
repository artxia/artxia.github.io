---
layout: handbook-page-toc
title: Customer calls
category: Handling tickets
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Customer calls

### Scheduled calls
#### Internally scheduled calls

All scheduled calls involving Customer Success, Sales, Development, and/or Support should be organized via the support project [issue tracker](https://gitlab.com/gitlab-com/support/support-team-meta/issues) using the [customer call template](https://gitlab.com/gitlab-com/support/support-team-meta/blob/master/.gitlab/issue_templates/Customer%20call.md).

The template can be used when coordinating a call with other engineering/sales team members or when scheduling another Support Engineer in a more preferable timezone. These calls may involve customers as well.

#### Customer scheduled calls

##### Providing the call link

When you know a ticket is ready for a call, use the `General::Invite customer call` macro in Zendesk. (Please modify the `PERSONAL_CALENDLY_LINK` to your own personal Calendly link)

A few point to consider when sending a customer the invite to call link.

* Always use [single-use Calendly link](/handbook/support/workflows/calendly.html#generating-a-single-use-calendly-link) to invite customers to a call so that we can avoid ghost-calls.
* If you know your availability is limited, or you need additional backup, check with another engineer to see if they might also be available to take the call.
* If you're not comfortable enough to take the call, **you should shadow any call that does take place** to upskill.


#### Pre-call email

Please consider sending a pre-call email. This helps set expectations to the call regarding goals, duration, and
the people required to be on the call for effective troubleshooting. You can use the `General::Pre customer call` macro in Zendesk
for that, please modify it as you see fit.

##### Tips to keep calls within the scheduled time:

* Set expectations (again) at the start of the call

1. Call duration will be 1 hour
1. At 45 minutes - call wrap up will happen (below)
1. Will need access to applicable systems
* When 15 mins left: start to wind down the call
* Stop the call and determine where we are (solved, not solved more info needed)
1. Solvable in the next few minutes
1. Need to research/schedule additional call
* Review
1. Summary of what was learned
1. Next steps for GitLab agent
1. Next steps for user
1. Next call recommendations (timing/goals/expectations)

##### Notes on intake, upgrade and installation support calls

For Premium Support customers, and customers who have purchased Implementation Support, we offer intake and installation support. Premium Support customers also receive live upgrade assistance. The different levels of service that are offered are described on the [support page](/support), and Implementation Support is described in more detail in the [support handbook](/handbook/support/#implementation-support).

Call/screen sharing sessions involve guiding a customer through the GitLab upgrade process or taking control of the customer's server to perform the upgrade.
You should make sure that the customer has finished creating a backup **before** you start the call, as they can take a lot of time to complete and you don't want to do them while in the call.

**Important information to collect**

1. Type of installation: Source/Omnibus
1. Current GitLab version
1. Version you're upgrading to (it isn't always the latest)
1. Use of GitLab CI (need to upgrade to 8.0 first, then 8.+)

We collect this information in Zendesk and link it to the organization, see the
[responding to tickets section in onboarding](/handbook/support/onboarding).

##### Call summary

Following your scheduled or unscheduled call you should complete a summary of the call in Zendesk using the
macro `General::Post Customer Call`.  This will provide a record of events for the next support agent in the hot queue
as well as the customer.  It will also provide valuable information for support agents in the future who search Zendesk
looking for similar issues and their resolutions.

### Unscheduled calls

While engaging with customers you should always be prepared to jump on a call with them. It is easier to get
all the information you might need on a 20 minute call than on 10 2-minute emails. If a conversation goes through
several back and forth emails and the problem still isn't close to being resolved, suggest a call via Zoom.

If you feel too inexperienced to handle a call, ask someone more experienced to handle the call and
listen in if at all possible. After someone else had the call with the customer it is still your responsibility
to handle the ticket as long as the ticket is still assigned to you.

If the problem is urgent you can simply send the customer a Zoom link and jump on immediately. For less urgent
calls, you may send the customer a Calendly link so that they can schedule a convenient time in their time zone.
The link you send may be a link to your personal calendar or to the Team Calendly event, depending on the circumstances,
but in every case you should send a
[single-use Calendly link](/handbook/support/workflows/calendly.html#generating-a-single-use-calendly-link),
to ensure proper processes are followed for scheduling calls.
