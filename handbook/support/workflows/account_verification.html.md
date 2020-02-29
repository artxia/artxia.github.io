---
layout: handbook-page-toc
title: Account Ownership Verification
category: GitLab.com
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

While this workflow focuses on disabling [Two-factor Authentication](http://docs.gitlab.com/ee/profile/two_factor_authentication.html) on a GitLab.com account, this same workflow should be used any time ownership of an account needs to be verified, such as for [account changes](/handbook/support/workflows/account_changes.html).

2FA removal and other account actions can only be taken if the [workflow](#workflow) below is successful.

## Access by User Action

In many cases, users can regain access to their account using the following methods:

### User has recovery codes

Users can try and login using their saved [two-factor recovery codes](https://docs.gitlab.com/ee/user/profile/account/two_factor_authentication.html#recovery-codes).

### User has a valid SSH key:

If a user didn't save their recovery codes, new ones can be generated with the command below via SSH if they've previously added an SSH key to their account. The new recovery codes can then be used at sign in. This option is presented to users in the Zendesk macro. If they cannot use this method then move on to the manual methods below.

```
ssh git@gitlab.com 2fa_recovery_codes
```

If a user has added an SSH key to their account but receives a `Permission denied (publickey)` error when using the command above, they may need to manually register their private SSH key using `ssh-agent` if they're using a non-default SSH key pair file path. Direct the user to [this](https://docs.gitlab.com/ee/ssh/README.html#working-with-non-default-ssh-key-pair-paths) documentation on how to resolve this.

## Access with Support Intervention

If the user is unable to remove 2FA or otherwise regain access to their account using the above methods and responds with the need for further verification, then the user can provide evidence of account ownership.

If a user has lost their account recovery codes and has no SSH key registered, proving they own the account can be difficult. In these cases, please use the workflow below.

### Workflow

As part of access recovery, if 2FA removal is not involved, then skip the following steps and move on to the next section.

1. Apply the **"Account::2FA Removal SSH Info & Challenges"** Macro
1. The macro marks the ticket as "Pending"

#### If the user responds with the need for further verification (by answering the challenges)

1. Using the [Risk Factor Worksheet](https://docs.google.com/spreadsheets/d/1NBH1xaZQSwdQdJSbqvwm1DInHeVD8_b2L08-V1QG1Qk/edit#gid=0) (internal only), determine the appropriate data classification level and the risk factor you have determined from customer's answers to the challenges.
   - For almost all cases, the originating email should be the same as the one listed on the account.

1. Use the macro **"Account::2FA::2FA Internal Note"** It leaves an internal note on the ticket. Edit with the relevant admin link, your proposed data classification level,challenges and the risk factor.

1. Request that your decision be peer-reviewed by another member of the team via Slack.
 
1. For disabling 2FA: If you agree with the decision; log into your admin account and locate the username in the users table or by going to `https://gitlab.com/admin/users/usernamegoeshere`
      1. Under the account tab, click `Edit`, add an [Admin Note](/handbook/support/workflows/admin_note.html), and save.
      1. On the account tab, click on `Disable 2FA`.
      1. Use the **"Account::2FA::2FA Removal Verification - Successful"** macro.

1. In case you disagree, leave an internal note on the ticket stating your thoughts on what the risk factor should be and reply to the slack conversation for further discussion. Once agreed, apply above step.

**Note**: This only applies if you think the challenges were passed, in case the user sends back very minimal information and it's clear it's not sufficient, reply asking for more information immediately after their response.

##### User responds with repository verification

1. Verify the file uploaded
    - File contains the provided text string.
    - File has been uploaded to a "Personal Repository"
1. Apply an "Internal Comment" with a link to the commit (if not already included)

#### User Successfully Proves Account Ownership
   
   1. For other situations other than 2FA, please see [Account Changes workflow](account_changes.html).

#### User Fails to Prove Account Ownership

1. If the user is unable to pass the selected challenges:
   1. Inform them that without verification we will not be able take any action on the account. For 2FA, use the **Account::2FA::2FA Removal Verification - GitLab.com - Failed** macro.
   1. Mark the ticket as "Solved"

### GitLab Team Members

If the user is a GitLab employee, follow the below process:

1. Perform steps for SSH key and recovery codes, if possible.
1. Confirm authenticity of the request by contacting the employee via phone or video call.
1. Add an [Admin Note](/handbook/support/workflows/admin_note.html) with relevant information.
