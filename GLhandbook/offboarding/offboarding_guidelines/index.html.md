---
layout: handbook-page-toc
title: "GitLab Offboarding Guidelines"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Offboarding Issue

Before starting an offboarding issue, make sure that the team member's resignation or termination has been discussed and cleared with _at least_ the member of the executive team to whom the team member (in)directly reports.

1. In Slack, go to your profile as if you were going to send a Slack message to yourself. Type the command `/pops run offboarding BambooHR_ID_number` (not Employee ID #). This number is found in the team member's BambooHR profile URL, after `id=`. It is a 5-digit number. An example of the command would be `/pops run offboarding 00000`. If BambooHR's API is down, this ChatOps command will fail and will need to be created manually.
1. You will be pinged in Slack once the offboarding issue is created, which usually takes 30 seconds or so. The ping will include a link to the new offboarding issue.
1. You will need to add the Gitlab handle and email address in the placeholders in the issue.

Note: If the team member is transitioning to a [temporarily positioned contractor](/handbook/general-onboarding/consultants/), please proceed with the full offboarding and create a separate onboarding issue to grant only specific temporary access for what they would need to fulfill their contractual obligations.

## Tools Offboarding

## G Suite

People Operations specialist will follow the below steps to set up an auto-response that notifies the sender that the team member they are trying to reach is no longer with GitLab and who to contact.
1. Add the team member to the `former_employees@gitlab.com`'s email account by selecting the dropdown icon `ˇ` in the `User information` section and adding the team member's GitLab email address.

_Note: Be sure to scroll down and `Save` this change or it will not be reflected._
1. Set up a routing rejection rule for the team member by;
   1. Navigate to Google admin portal then Apps > G Suite > Gmail > Advanced settings > Routing > Routing. 
   2. Hover over the routing option and click on `Add another`. Please enter a name below the tittle "Routing" with `lastname firstname rejection rule`
   3. Check the option `Inbound` and `Internal-receiving` under `Messages to affect`.
   4. Check `Only affect specific envelope recipients` under the `Envelope filter` tittle.
   5. Enter the team members's email  address right below the tittle `Email address`.
   6. Under the tittle `For the above types of messages, do the following`, please change from `Modify message` to `Reject message`.
   7. Add the [appropriate template](https://gitlab.com/gitlab-com/people-group/employment/blob/master/Offboarding%20Rejection%20Email%20Templates) per team member's department under the `Customize rejection notice`
   8. Scroll down and click on `Add setting` and then on `Save` at the bottom (once the window closes).

After 30 days, once you receive a notification that the former team member's offboarding issue is due, delete their gsuite account now refered to as `former_username@gitlab.com`. You will receive a prompt to transfer their docs, please transfer to the manager's email.

## Slack

People Operations Specialist check if the team member has created any bots before disabling the account. Go to [Slack](https://gitlab.slack.com/apps/manage) or on your admin Slack profile click Menu >> Configure Apps >> Custom Integrations >> Bots and search through the bots' list for the team member.
If a bot exists, please DM the manager to confirm if the bot should be removed.

## Team Page

Navigate to the [team.yml file](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/data/team.yml). Using Web IDE or your editor of choice, search the team member name and delete their team page entry. Don't forget to delete the image by navigating to Source/images/team while still here and search for their image. Ideally saved as firstnamelastname.png. The images are in alphabetical order.
To remove pet entry and any mentions from the handbook and documention, you will need to download the [www-gitlab-com project](https://gitlab.com/gitlab-com/www-gitlab-com) to your computer and use a prefered text editor.

To download;
1. Navigate to the [Gitlab.com project](https://gitlab.com/gitlab-com/www-gitlab-com)
2. On the far right corner, click `Clone` and copy the clone with SSH URL, git@gitlab.com:gitlab-com/www-gitlab-com.git
3. On your command line, run `git clone git@gitlab.com:gitlab-com/www-gitlab-com.git `
This downloads the project to your computer mostly on the document folder. Consider going through the [Clone a repository](https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html#clone-a-repository) and the [Command Line](https://docs.gitlab.com/ee/gitlab-basics/command-line-commands.html) documents to understand further.

To `Find All` using Atom;
1. Download Atom at atom.io
2. After installing, click `Open Project` on the Welcome Guide Page.
3. Choose www-gitlab-com project from your Documents folder
4. On the Find tab drop down menu, click `Find in Project`
5. Search all variations of the departing team members name; firstname, lastname and gitlab username.
6. Follow the File path given in the results on the Web IDE and delete all the mentions, make sure to replace any mentions you deem appropriate with who is standing in for the position.
DO NOT delete any blog mentions.

## Code Ownership

Code ownership by departing team members should be transferred to their successors, supervisors, or other appropriate colleagues by editing their entries in the relevant CODEOWNERS files.

* [CODEOWNERS for the GitLab platform](https://gitlab.com/gitlab-org/gitlab/blob/master/.gitlab/CODEOWNERS)
* [CODEOWNERS for the marketing site](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/.gitlab/CODEOWNERS)
