---
layout: markdown_page
title: "Usecase: Continuous Integration"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}


## Continuous Integration

The Continuous Integration (CI) usecase is a staple of modern software development in the digital age. It's unlikely that you hear the word "DevOps" without a reference to "Continuous Integration and Continuous Delivery" (CI/CD) soon after. In the most basic sense, the CI part of the equation enables development teams to automate building and testing their code.

When practicing CI, teams collaborate on projects by using a shared repository to store, modify and track frequent changes to their codebase. Developers check in, or integrate, their code into the repository multiple times a day and rely on automated tests to run in the background. These automated tests verify the changes by checking for potential bugs and security vulnerabilities, as well as performance and code quality degradations. Running tests as early in the software development lifecycle as possible is advantageous in order to detect problems before they intensify.

CI makes software development easier, faster, and less risky for developers. By automating builds and tests, developers can make smaller changes and commit them with confidence. They get earlier feedback on their code in order to iterate and improve it quickly increasing the overall pace of innovation. Studies done by DevOps Research and Assessment (DORA) have shown that [robust DevOps practices lead to improved business outcomes](https://cloud.google.com/devops/state-of-devops/). Out of the "DORA 4" metrics, 3 of them can be improved by using CI:
- **Deployment frequency:** Automated build and test is a pre-requisite to automated deploy.
- **Time to restore service:** Automated pipelines enable fixes to be deployed to production faster reducing Mean Time to Resolution (MTTR)
- **Change failure rate:** Early automated testing greatly reduced the number of defects that make their way out to production.

[GitLab CI](/product/continuous-integration/) comes built-in to GitLab's complete DevOps platform delivered as a single application. There's no need to cobble together multiple tools and users get a seamless experience out-of-the-box.

<!--
facts about approaching 100mil software developers...
-->

## Personas

### User Persona

The typical **user personas** for this usecase are the Developer, Development team lead, and DevOps engineer.

#### Software Developer [Sacha](/handbook/marketing/product-marketing/roles-personas/#sasha-software-developer)

Software developers have expertise in all sorts of development tools and programming languages, making them an extremely valuable resource in the DevOps space. They take advantage of GitLab SCM and GitLab CI together to work fast and consistently deliver high quality code.

- Developers are problem solvers, critical thinkers, and love to learn. They work best on planned tasks and want to spend a majority of their time writing code that ends up being delivered to customers in the form of lovable features.

#### Development Team Lead [Delaney](/marketing/product-marketing/roles-personas/#delaney-development-team-lead)

Development team leads care about their team's productivity and ability to deliver planned work on time. Leveraging GitLab CI helps maximize their team's productivity and minimize disruptions to planned tasks.

- Team Leads need to understand their team's capacity to assign upcoming tasks, as well as help resolve any blockers by assigning to right resources to assist.

#### DevOps Engineer [Devon](/handbook/marketing/product-marketing/roles-personas/#devon-devops-engineer)

DevOps Engineers have a deep understanding of their organization's SDLC and provide support for infrastructure, environments, and integrations. GitLab CI makes their life easier by providing a single place to run automated tests and verify code changes integrated back into the SCM by development teams.

- DevOps Engineers directly support the development teams and prefer to work proactively instead of reactively. They split their time between coding to implement features and bug fixes, and helping developers build, test, and release code.


### Buyer Personas

CI purchasing typically does not require executive involvement. It is usually acquired and installed via our freemium offering without procurement or IT's approval. This process is commonly known as shadow IT. When the upgrade is required the [VP of IT](/handbook/marketing/product-marketing/roles-personas/#buyer-personas) is the most frequent decision-maker. The influence of the [VP Application Development](/handbook/marketing/product-marketing/roles-personas/#buyer-personas) is notable too.


### [Message House](./message-house/)

The message house for the use case provides a structure to describe and discuss the value and differentiators for the use case.

## Analyst Coverage

- [Forrester Wave for Cloud-Native CI Tools](/analysts/forrester-cloudci19/)
- [Forrester Continuous Integration Tools](/analysts/forrester-ci/)

### [AR Plan](./ar-plan/)

The AR Plan provides key details into how we intend to engage with the analyst community.

## UseCase Capabilities

tbd

## Top 3 Differentiators

| Differentiator | Value | Proof Point  |
|-----------------|-------------|---------------|
| **Leading SCM and CI in one application** | GitLab enables streamlined code reviews and collaboration at proven enterprise scale, making development workflows easier to manage and minimizing context switching required between tools in complex DevOps toolchains. Users can release software faster and outpace the competition with the ability to quickly respond to changes in the market. | - Forrester names GitLab among the leaders in [Continuous Integration Tools in 2017](/analysts/forrester-ci/), Alteryx uses GitLab to have code reviews, source control, CI, and CD [all tied together](/handbook/marketing/product-marketing/usecase-gtm/ci/), [Axway](/customers/axway/) overcomes legacy SCM and complex toolchain |
| **Built in security and compliance** | GitLab comes with security features out-of-the-box and automated security testing with audit controls to facilitate policy compliance. Moving security testing farther left into the SDLC catches potential problems earlier and shortens feedback loops for developers. This means a faster time to market delivering secure, compliant, code and an increase in customer confidence.  | - Gartner recognizes GitLab as a relevant vendor for Application Monitoring and Protection via [2019 Hype Cycle for Application Security](https://www.gartner.com/en/documents/3953770/hype-cycle-for-application-security-2019), [Wag! takes advantage of built-in security and faster releases with GitLab](/blog/2019/01/16/wag-labs-blog-post/), and [Glympse](/customers/glympse/) makes their audit process easier and remediates security issues faster |
| **Rapid innovation** | GitLab embraces an approach to rapid innovation that organizations undergoing digital transformations or adopting CI/CD also work diligently to implement internally with frequent, regular, releases delivered on a monthly basis. This provides end users with the latest and greatest in terms of capabilities/features, consistent security updates, and other incremental value adds over time. By GitLab "walking the talk" in regards to CI/CD, we understand the needs and pains that our users and organizations using GitLab face and share a mutual benefit from fully embracing this model centered around continuous improvement. | - GitLab deploys over 160 times a day and is one of the [30 Highest Velocity Open Source Projects](/blog/2017/07/06/gitlab-top-30-highest-velocity-open-source/) from the CNCF, we're voted as a [G2 Crowd Leader 2018](/is-it-any-good/#gitlab-has-been-voted-as-g2-crowd-leader-in-2018) with more than 170 public reviews and a 4.4 rating noting "Powerful team collaboration for managing software development projects," and have over 2,900 active contributors.  |


## Competitive Comparison
Amongst the many competitors in the DevOps space, [Jenkins](/devops-tools/jenkins-vs-gitlab.html) and [CircleCI](/devops-tools/circle-ci-vs-gitlab.html) are the closest competitors offering continuous integration capabilities.

## Proof Points - customers

### Quotes and reviews

#### Gartner Reviews

*Gartner Peer Insights Customers’ Choice constitute the subjective opinions of individual end-user reviews, ratings, and data applied against a documented methodology; they neither represent the views of, nor constitute an endorsement by, Gartner or its affiliates.*
*Gartner Peer Insights reviews constitute the subjective opinions of individual end users based on their own experiences, and do not represent the views of Gartner or its affiliates. Obvious typos have been amended.*

>"We've migrated all our products from several "retired" VCS's to GitLab in only 6 months. - Including CI/CD process adoption - Without [loss] of code - Without frustrated developers - Without enormous costs"
>
> - **Application Development Manager**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1037269)
>
>"Finally, the most amazing thing about Gitlab is how well integrated the [GitLab] ecosystem is. It covers almost every step of development nicely, from the VCS, to CI, and deployment."
>
> - **Software Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1038051)
>
>"One of the best ways to approach source code management (Git) and release pipeline management [CI/CD]. [Gitlab] gives you a simple yet highly customizable approach to release management which is a complicated topic."
>
> - **System Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1045457)
>
>"The best software tool to manage all our projects and configure [CI/CD]. I will definitely recommend GitLab to everyone that wants to start a new project and doesn't want to use too many tools, GitLab has everything that you need to manage."
>
> - **Web Developer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1063698)
>
>"Over the years, we have successfully taken advantage of [Gitlab's] continuous deployment and integration mechanisms to build [and] maintain a robust and solid codebase."
>
> - **Co-Founder/CEO**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1111080)
>
>"One of the best [tools] for continuous integration and continuous deployment. "
>
> - **Lead - Mobile Apps**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1117401)
>
>"Overall, the experience with Gitlab is very positive, it provides many powerful features especially regarding Continuous Integration and [Continuous Deployment]"
>
> - **Developer Analyst**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1140016)
>
>""[GitLab's] UI is so easy and manageable to understand. Built-in continuous integration is one of its best [features]."
>
> - **Technical Evangelist**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/1092444)
>
>"GitLab isn't just for hosting your code, it's for the entire lifecycle of your code. Since they host code, it makes sense for them to provide services around development and getting code into production. Their integration into other services is really easy. They give you GitLab-CI for any CI/CD needs, driven from a yaml file."
>
> - **Testing Analyst**, [Gartner Peer Review](https://www.gartner.com/reviews/market/application-release-orchestration-solutions/vendor/gitlab/product/gitlab/review/view/886423)
>
>"This is really an amazing source code repository toolset which enables the robust CI practices which are inbuilt features of GitLab. This can be utilized well in any enterprise looking for the smooth CI/CD pipelines."
>
> - **Software Engineer**, [Gartner Peer Review](https://www.gartner.com/reviews/market/enterprise-agile-planning-tools/vendor/gitlab/product/gitlab/review/view/1009762)

### Blogs

#### Jaguar Land Rover

**[How Jaguar Land Rover embraced CI to speed up their software lifecycle](/blog/2018/07/23/chris-hill-devops-enterprise-summit-talk/)**
> Our feedback loops were 4-6 weeks. Could you imagine writing code today and six weeks from now being told whether or not it works or is broken? I don't remember the shirt that I wore yesterday, let alone what I had for breakfast this morning, let alone what I wrote six weeks ago, and chances are I've been working on features for the last six weeks, and for me to try to unpick what I was thinking at that point could be a huge context-switch penalty.

#### Ticketmaster

**[GitLab CI supports Ticketmaster's ramp up to weekly mobile releases](/blog/2017/06/07/continous-integration-ticketmaster/)**
> With the benefit of faster cycle time, and faster releases, we have seen other benefits. Since each release has a smaller change set, our crash-free rates and store ratings have improved. We have less time waiting for build and spend more time improving the quality of our products. Our fans are getting features into their hands more quickly and benefit from a higher-quality and a consistently improving product. The CI analytics available on GitLab are an additional scoreboard for our team to optimize and improve into the future.

### Case Studies

#### Goldman Sachs

**[Goldman Sachs improves from 1 CI feature branch build every two weeks to over a thousand per day](/customers/goldman-sachs/)**
> GitLab has allowed us to dramatically increase the velocity of development in our Engineering Division. We believe GitLab’s dedication to helping enterprises rapidly and effectively bring software to market will help other companies achieve the same sort of efficiencies we have seen inside Goldman Sachs. We now see some teams running and merging 1000+ CI feature branch builds a day!

#### CERN (European Organization for Nuclear Research)

**[CERN, the European-based particle physics laboratory, uses GitLab for more than 12,000 users and 120,000 CI jobs a month](/customers/cern/)**
> The entire infrastructure, with continuous integration and container support, makes it possible to have new scientific results based on code that was developed once before. Having an easily accessible record on how the original code was developed makes that much easier. This is why we are using GitLab CI, pipelines and starting with the Auto DevOps tools.

* [GitLab CI checks off Wish's list](https://about.gitlab.com/customers/wish/)

### References to help you close
[SFDC report of referenceable Verify customers](https://gitlab.my.salesforce.com/a6l4M000000kDwk)

Request reference calls by pressing the "Find Reference Accounts" button at the top of your stage 3 or later opportunity. 

## Resources

### Presentations
* [Why CI/CD?](https://docs.google.com/presentation/d/1OGgk2Tcxbpl7DJaIOzCX4Vqg3dlwfELC3u2jEeCBbDk)

### Continuous Integration Videos
* [CI/CD with GitLab](https://youtu.be/1iXFbchozdY)
* [GitLab for complex CI/CD: Robust, visible pipelines](https://youtu.be/qy8A7Vp_7_8)

### Integrations Demo Videos
* [Migrating from Jenkins to GitLab](https://youtu.be/RlEVGOpYF5Y)
* [Using GitLab CI/CD pipelines with GitHub repositories](https://youtu.be/qgl3F2j-1cI)

### Clickthrough & Live Demos
* [Live Demo: GitLab CI Deep Dive](https://youtu.be/pBe4t1CD8Fc)
