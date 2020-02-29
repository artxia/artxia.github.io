---
layout: handbook-page-toc
title: "Forum response workflow"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

New posts to the GitLab forum are brought in to Zendesk and #gitlab-forum on Slack

## Best practices

- Always be courteous, especially if they are a new poster.
- Add a welcome message when replying to new posters. It could be as simple as "Hi, and welcome to the forum! :smile:" at the start of your post.
- Use the like button as much as you can, to thank users for their input and to inspire other users to do the same.

## Administration

Most administration tasks will be done from the [Discourse Admin Dashboard](https://forum.gitlab.com/admin)

### How to grant admin permissions

If you need to add an admin:

1. Go to the [list of forum users](https://forum.gitlab.com/admin/users/list/active)
2. Use the search box to find the user you want to grant admin permissions to
3. Click on the user to modify their profile
4. Scroll down to the `Permissions` section
5. Click on the `Grant Admin` button
6. An e-mail confirmation will be sent to the Admin that granted the permission (i.e. you). Go to your inbox and click on the link to confirm granting Admin permission to the user
7. If all went well, the `Permissions` > `Admin?` section on the user's profile admin should read `Yes`

## Workflow

How to respond to the GitLab forum tickets: 

1. Go through the tickets in Zendesk `GitLab Forum` view
2. See if all comments have received responses
3. Write the response if necessary, involve an expert for assistance if you don't know the answer
4. Post the comment on the original website ([https://forum.gitlab.com](https://forum.gitlab.com), not Zendesk) using the link provided in the ticket
5. Solve the ticket with the `Replied` macro (Replied macro will use the public response field in order to track the first reply time)

Follow the relevant workflow depending on the question:


```mermaid
graph TD
A((Non-support)) --> B
B(Account) --> |Sales/Renewal| E[ping #sales]
B --> |Other|F(Have they opened a support ticket?)
F --> |Yes, using GitLab.com| G[ping #support_gitlab-com]
F --> |Yes, self-managed| H[ping #support_self-managed]
F --> |No| I[Direct them to support.gitlab.com]
A --> J(GitLab vs Competitor)
J --> |Question|K[Find answer via devops tools page/blog and link]
J --> |Discussion|L[Link on #competition]
A --> M(Feature Proposal)
M --> |Already exists|N[Link to the open issue]
M --> |Doesn't exist|O[Ask them to open an issue]
```

```mermaid
graph TD
A((Support)) --> B(What level of GitLab are they on?)
B --> |Not free|C(Have they opened a support ticket?)
C -->|No| E[Link them to the support portal]
C -->|Yes| F(Have they provided the ticket number?)
F --> |No|R(Ask them for the ticket number)
R --> F
F --> |Yes|G(Self-hosted or .com?)
G --> |Self-hosted|H[ping #support_self-managed]
G --> |.com|I[ping #support_gitlab-com]
G --> |not provided|J(Ask what they're using)
J --> G
B-->|Free| D(Is there an issue open already?)
D --> |Yes|K[Link the issue]
D --> |ask the following questions|L(Self-hosted or .com?)
L --> M(What version are they on?)
M --> N(Has this happened on a previous version?)
N --> O(How long have they been experiencing it?)
O --> P(What integrations do they have, if relevant?)
P --> |Questions answered|Q[ping relevant product channel]
```


## Automation

New mentions are brought into Slack and Zendesk via Zapier.
