---
layout: markdown_page
title: "Usecase: Source Code Management"
---

<!--

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}
-->

## Source Code Management

As organizations accelerate delivery, through DevOps, controlling and managing different versions of the application artifacts from code to configuration and from design to deployment is incredibly important.
Velocity without robust version control and traceability is like driving a car with out a seatbelt.

Source code management is more than simply tracking changes, versions, and branches of code. Effectively, it includes practices such as:

- Enabling development teams to work in distributed and asynchronously
- Managing changes and versions of code and artifacts
- Enabling *Review* and *Collaboration* of code and other artifacts
- Tracking approvals of proposed changes
- Resolving merge conflicts and related anomalies

At GitLab, *source code management* is a  gateway use case to GitLab, where many customers adopt GitLab specifically for SCM.  In GitLab, this use case refers to the specific categories [Source Code Management](https://about.gitlab.com/product/source-code-management/) and [Code Review](https://about.gitlab.com/product/code-review/) both under the [Source Code Group](https://about.gitlab.com/handbook/product/categories/#source-code-group) in the [Create stage](https://about.gitlab.com/handbook/product/categories/#create-stage). Increasingly, this use case is making use of the [WebIDE](https://docs.gitlab.com/ee/user/project/web_ide/index.html) and the [Code Snippets](https://docs.gitlab.com/ee/user/snippets.html) categories of the [Editor Group](https://about.gitlab.com/handbook/product/categories/#editor-group) and the [Wiki](https://docs.gitlab.com/ee/user/project/wiki/) and the [Design Management](https://docs.gitlab.com/ee/user/project/wiki/) categories of the [Knowledge Group](https://about.gitlab.com/handbook/product/categories/#knowledge-group) both under the Create Stage too.

Most of our clients are acquired through the capabilities included in these groups. Given the relevance of this entry point, this page will elaborate on how Source Code Management is used, how our clients solve their problems with these parts of the product and how they leverage these set of features to benefit then from the broader stages of GitLab. Source Code Management is required because software is constantly changing. Regardless of the stage of development, there will be change to deal with. Constantly.

> No matter where we are in the system life cycle, the system will change, and the desire to change it will persist throughout the life cycle.

> E.H. Bersoff, 1980.

Changes are of different nature:

| Change | Outcome |
| --- | --- |
| Requirements or features may change in scope | Business changes |
| New team members may join | Stakeholder changes |
| Docs are updated all the time | Technical changes |
| Dependencies may have changed | Technical changes |
| The actual code will change!| Technical changes |

## Personas

### User Persona
Being the entry point to GitLab means that many user personas find utility and a solution to their problem in Source Code Management. Let's go through the list of power user personas and describe briefly their key motivations to use Source Code Management in GitLab:
[Parker the Product Manager](https://about.gitlab.com/handbook/marketing/product-marketing/getting-started/102/#step-three-get-docker-and-configure-middleman)
- PMs coordinate feature development and project success among other things. The ability to monitor progress through commits, review app and validate those changes and provide feedback is key to they success of their role
- These changes, in time will generate valuable statistical insight for the PM to assess accurately development efforts of planned new features

[Delaney the Development Team Lead](https://gitlab.com/gitlab-com/www-gitlab-com/-/merge_requests/38512/commits?commit_id=b0887cc5146ba8c31c0422c06094efb7b2975f60)
- Just like the PM, Team Leads need also to understand their team's capacity to assign upcoming tasks to meet goals on time accordingly
- Approval workflows in Code Review allows them to become faster real team work enablers

[Sasha the Software Developer](https://gitlab.com/gitlab-com/www-gitlab-com/-/merge_requests/38512/commits?commit_id=b0887cc5146ba8c31c0422c06094efb7b2975f60)
- Sasha takes advantage of both Command Line Tools and GitLab's GUI to have complete control of every commit he does to complete his tasks
- Even when scope changes, a frequent hurdle and a source of frustration, branching, merging and conflict resolution will be performed in Source Code Management and will trigger CI for fast resolution

[Devon the DevOps Engineer](https://about.gitlab.com/handbook/marketing/product-marketing/roles-personas/#devon-devops-engineer)
- All information relevant to the role's goals is congregated in Source Code Management to take action on it. Time to resolution and, in general, any other key metric in DevOps is measured and its performance tracked in Source Code Management
- Any improvement applied to the development process will reflect in Source Code Management's interfaces, whether its the Merge Requests or Issues.

### Buyer Personas
Source Code Management purchasing typically do not require executive involvement. It is usually acquired and installed via our freemium offering without procurement or IT's approval. This process is commonly known as shadow IT. When the upgrade is required the [VP of IT](https://docs.google.com/presentation/d/17Ucpgxzt1jSCs83ER4-LdDyEuermpDuriugPNYrz8Rg/) is the most frequent decision maker. The influence of the [VP Application Development](https://docs.google.com/presentation/d/1pYyAu8ezJZBVLb5k8-E_4Hhtf8w5l11AWhaAxU4GK50/edit#slide=id.g5050420c27_0_0) is notable too.

## [Message House](./message-house/)

The message house for the use case provides a structure to describe and discuss the value and differentiators for the use case.

## Analyst Coverage

Unfortunately, analysts do not cover the Source Code Management market, for several reasons.

### [AR Plan](./ar-plan/)

  The AR Plan provides key details into how we intend to engage with the analyst community.


## Critical Capabilities

TBD

## Top 3 Differentiators

| Differentiator | Value | Proof Point  |
|-----------------|-------------|---------------|
| TBD | TBD | TBD |
| TBD | TBD | TBD |
| TBD | TBD | TBD |

---


## Competitive Comparison
TBD

## Proof Points - customers

### Quotes and reviews

#### Gartner Reviews

*Gartner Peer Insights Customers’ Choice constitute the subjective opinions of individual end-user reviews, ratings, and data applied against a documented methodology; they neither represent the views of, nor constitute an endorsement by, Gartner or its affiliates.*
*Gartner Peer Insights reviews constitute the subjective opinions of individual end users based on their own experiences, and do not represent the views of Gartner or its affiliates. Obvious typos have been amended.*

>"The software is intuitive and quite easy to use. Since many software development projects require more than one person, this makes it easy to create teams and collaborate."
>
> - **Quality Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1037713)
>
>"Improves productivity of engineers by providing easy and fast ways to keep feature branches and merge them quickly and efficiently."
>
> - **Engineering Manager**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1060524)
>
>"Keeps your software projects under control. Rogue developers are kept at bay via enforced review processes and pipelines."
>
> - **Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1063180)
>
>"For managing git repositories it is the best product available right now in the market." 
>
> - **Sr. Software Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1074452)
>
>"This has really aided in our ability to automate software delivery and return wasted overhead back to the pool of resources! This is a very simple to use and fast delivery tool to assist your code pipeline."
>
> - **Project Manager**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1078302)
>
>"We use this platform in our company to version our source [code] ensure they are up to date and as a backup option. It enables us build scalable and high quality products. Ease of use and compatible with most development environments."
>
> - **Sr. Software Developer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1135664)
>
>"I appreciate its ability to run limitless. It has various features like issue tracker, protected branches and merge requests, which gives very nice experience."
>
> - **Sr. Software Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1142879)
>
>"Gitlab is a very useful SCM. In our [organization] we have used it as a source code repository. We have extensively used branching and tags creation feature. As we work in a sprints, we have several sprint and feature branches."
>
> - **Lead Developer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1144638)
>
>"GitLab is a superb source code management [provider]." 
>
> - **Systems Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1194415)
>
>"Before GitLab, we used to make local copies of code or backup the code and then pass on the code through the server. But if our organization knew about GitLab from start, we would have immediately integrated with our development practises for ease of deployment." 
>
> - **Software Developer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/enterprise-agile-planning-tools/vendor/gitlab/product/gitlab/review/view/1016152)

### Case Studies
* All the new strategic pieces of [Goldman Sachs](/customers/goldman-sachs/)’ software development platforms are tied into GitLab. GitLab is used as a complete ecosystem for development, source code control and reviews, builds, testing, QA, and production deployments.
> We’re bringing into the firm a platform that our engineers actually want to use – which helps drive adoption across multiple teams and increase productivity without having to ‘force’ anyone to adopt it. This is really helping to create an ecosystem where our end users are actively helping us drive towards our strategic goals - more releases, better controls, better software..
>
> George Grant, VP technology fellow, Goldman Sachs

* At [ESA (European Space Agency)](/customers/euorpean-space-agency/) GitLab is used as a central version control system to allow opportunities for collaboration, synergies and multiple exploitations of efforts in visible way.
>GitLab was validated and adopted for the European Space Agency as a code repository platform in 2016. Usage was initially limited to a hand-picked group of first-wave users, but demand quickly escalated. In just two years, more than 140 groups adopted GitLab as their software versioning tool. Across ESA, more than 1500 software projects have been created. These range from mission control systems, onboard software for spacecraft, image processing and monitoring tools for Labs. The ESA IT Department also uses GitLab to host their code tools and configurations infrastructure..

* [Worldline](/customers/worldline/) benefits from Git availability through GitLab. With their precious installation of Subversion, Worldline faced bottlenecks and lack of ownership. It took 1-2 weeks to get a source code repo, now it takes a few seconds.
> We started using GitLab because we wanted to get an easy Git repository management system and because we wanted people to be able to use merge requests. We wanted the ability to have more code reviews and to ease discussions between developers.
>
> Antoine Neveux, Software Engineer, Kazan Team, Worldline.

The adoption of GitLab was quite successful and, within six months, over 1,000 users were active users. Developers explained that the adoption rate was high because GitLab is so easy to use. People actually felt encouraged to contribute code reviews with GitLab Merge Requests. Previous code review tools had 10-20 developers using them, while Worldline currently has 3,000 active users of GitLab - an adoption rate increase of 12,000 percent.

### References to help you close
<Link to SFDC list/report of use case specific references>


## Resources
### Presentations
* WIP

### Source Control Videos
* [Source Code Walk Through, January 2020](https://www.youtube.com/watch?v=wTQ3aXJswtM) by James Ramsey, Group Product Manager for the Create Stage.
* [Merge Request and Source Control as part of the Software Development Life Cycle](https://youtu.be/UuX-GnYWNwo?t=274) by William Chia and Jen Parker, PMMs.
* [User pain points and improved code reviews](https://www.youtube.com/watch?v=utfq9-ExXGE) by Pedro Moreira da Silva, UX Manager for the Source Code Group.

### Integrations Demo Videos
* [Jira & Jenkins Integration Video](https://www.youtube.com/embed/Jn-_fyra7xQ)
* [How to setup the Jira Integration](https://www.youtube.com/watch?v=p56zrZtrhQE)
* [GitHub Integration Video](https://www.youtube.com/embed/qgl3F2j-1cI)

### Clickthrough & Live Demos
* [All Marketing Click Through Demos](/handbook/marketing/product-marketing/demo/#click-throughs)
* [All Marketing Live Demos](/handbook/marketing/product-marketing/demo/#live-instructions)
