---
layout: handbook-page-toc
title: "UX Department"
---

#### On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Hello,

we're the GitLab User Experience (UX) Department. We hope you find what you are looking for here. If you don't, please open an [issue](https://gitlab.com/gitlab-org/gitlab-design/issues/new) and give us feedback.

## Mission
Our mission is to support designing and building software that solves important problems, is easy to use, enables everyone to contribute, and is built for a diverse, global community. We want GitLab to become the easiest and most delightful product in its class.

We partner closely with product management and engineering. 

We work with the wider GitLab community to understand our customers and users. 

We support the business of GitLab by becoming experts in our stage group, educating ourselves about the entire product, and staying engaged with business goals shared with us through the executive team and business partners in sales, marketing, and support.

## FY21 Direction
Our direction for fiscal year 2021 is to offer a best-in-class user experience for all of the DevOps categories in which we compete. 

It's important to note that, even though we're internally organized into teams that compete with specific industry segments, we can't design in silos. Because we're a single application for the DevOps lifecycle, we must strive to create experiences that flow seamlessly across the entire product. Instead of thinking about individual features, we must always consider the end-to-end job that a user wants to get done.

We measure the quality of our user experience in a variety of ways. A few examples are our quarterly [System Usability Scale survey](/handbook/engineering/ux/ux-resources/#system-usability-score), [UX Scorecards](/handbook/engineering/ux/ux-scorecards/), and Category Maturity Scorecards. We're actively working to improve our SUS score (which was [flat during FY20](/handbook/engineering/ux/performance-indicators/#perception-of-system-usability)) by emphasizing solution validation and resolving UX debt. We're continuing to evaluate current experiences within the product with UX Scorecards, and we're also validating Category Maturity Scorecards to ensure that the wider GitLab community has input to our [category maturity](../direction/maturity/) ratings.

Our UX and Product Management departments both understand that creating a great user experience is only possible when we actively solicit feedback from users. That's why we have a robust UX Research program that is guided by our [research team](https://about.gitlab.com/handbook/engineering/ux/ux-research/). They help our product managers and designers conduct extensive research, including (but not limited to) problem and solution validation. 

Based on experience, we know that having a robust Design System that offers single-source-of-truth components is a great way to increase productivity, drive UI consistency, and improve our visual design. Accordingly, we're working hard to make [Pajamas](https://design.gitlab.com/) a robust system that's customized to our unique needs. During FY21, we're adding a dedicated UX Foundation team to guide this work, making sure our UI components are beautiful, scalable, and accessible. While we'll have a small dedicated team, it's still imperative for every product designer to contribute to Pajamas.

In FY21, we're adding additional leadership to our rapidly growing department to maintain appropriate manager/direct report ratios that ensure everyone has the support they need. Research and Technical Writing will both have a Senior Manager and multiple team managers, and Product Design will also add two senior leaders to help guide the strategy led by the UX Managers of our product sections.

When we hire UXers, we look for practioners who have existing experience in the subject matter areas they will support. Because GitLab is a complex product, our goal is to set new UXers up for success, and existing domain knowledge makes that process easier.

Additionally, we hire UX generalists who are experienced in multiple areas. For example, our Product Designers are strong UI and visual designers, they can conduct their own research, they're experienced in defining and communicating UX strategy, and they sometimes have front-end development expertise. Similarly, our Technical Writers create great documentation, but they also know how to write compelling UI text and manage docs as code.

## Team Structure
UXers are assigned to stage groups as stable counterparts. We have three different roles on our team.

**Product Design** teams are organized by stage group. Product Designers learn everything they can about their product stage and they are great at designing easy-to-use, beautiful workflows and experiences. They also contribute to our design system, Pajamas.

Information about and strategic direction for these teams can be found here:
* Development (@gitlab-com/gitlab-ux/dev-ux)
    * Manage: Coming soon! {::comment}[Manage](/handbook/engineering/ux/stage-group-ux-strategy/manage/){:/comment}
    * Plan: Coming soon! {::comment}[Plan](/handbook/engineering/ux/stage-group-ux-strategy/plan/){:/comment}
    * Create: [Create](/handbook/engineering/ux/stage-group-ux-strategy/create/)
* [CI/CD](/handbook/engineering/ux/ci-cd/) (@gitlab-com/gitlab-ux/ci-cd-ux)
    * [Verify UX](/handbook/engineering/ux/stage-group-ux-strategy/verify/)
    * [Release UX](/handbook/engineering/ux/stage-group-ux-strategy/release/)
    * [Package UX](/handbook/engineering/ux/stage-group-ux-strategy/package/)
* Ops (@gitlab-com/gitlab-ux/ops-ux)
    * Configure: Coming soon! {::comment}[Configure](/handbook/engineering/ux/stage-group-ux-strategy/configure/){:/comment}
    * Monitor: Coming soon! {::comment}[Monitor](/handbook/engineering/ux/stage-group-ux-strategy/monitor/){:/comment}
* [Secure and Defend](/handbook/engineering/ux/stage-group-ux-strategy/secure-and-defend/) (@gitlab-com/gitlab-ux/secure-defend-ux)
    * [Secure UX](/handbook/engineering/ux/stage-group-ux-strategy/secure/)
    * [Defend UX](/handbook/engineering/ux/stage-group-ux-strategy/defend/)
* [Growth](/handbook/engineering/ux/stage-group-ux-strategy/growth/) (@gitlab-com/gitlab-ux/growth-ux)
* [Enablement](/handbook/engineering/ux/stage-group-ux-strategy/enablement/) (@gitlab-com/gitlab-ux/enablement-ux)

The **[UX Research](https://about.gitlab.com/handbook/engineering/ux/ux-research/)** team is great at finding answers to questions we have about our customers and how they use and think about our product. They generate valuable customer and user insights via quantitative and qualitative research methods, and then they share those insights with the rest of the company. UX Researchers are assigned to multiple stage groups, and they spend much of their time helping Product Managers and Product Designers conduct their own research.

The **[Technical Writing](https://about.gitlab.com/handbook/engineering/ux/technical-writing/)** team is great at taking complex, technical concepts and flows and presenting them to GitLab users in a simple way, so they can get the most out of GitLab. This team owns our world-class user documentation site and can also write clear and concise UI copy. Technical Writers are assigned to multiple stage groups.

You can reach us in issues and MRs by mentioning the different UX teams and roles shown on our [UX Group page](https://gitlab.com/gitlab-com/gitlab-ux).


## Our Strategy
### We support all users from beginners to experts
We believe that GitLab software should be unintimidating and accessible for a beginner, without oversimplifying important features for advanced users. We stay with users every step of the way to help them learn fast as a beginner and then become an expert over time. 

### We're building one product, together
We're highly focused on ensuring that no matter how big our product gets, the entire experience stays cohesive, consistent, and interconnected.

### We're humble facilitators of user experience design
Everyone is a designer; everyone can contribute. We are not egotistical, moody experts who alone hold the keys to user delight. We encourage Product Managers, Engineers, and the wider GitLab community to contribute to creating an exceptional user experience. 


### We look for small changes and big impacts
Sometimes the simplest, most boring solution is what is needed to make users successful. We want our UI to stay out of the user’s way. We work iteratively to make modest but valuable changes that make users more productive, faster, and better at accomplishing their tasks.

### We're informed by empathy
We’re human, and we design for humans, so we strive for understanding, self-awareness, and connection. We are quirky, and we introduce our quirks into designs when appropriate.


## Areas of Responsibility 

* **Pajamas Design System:** To ensure that everyone can contribute to GitLab with confidence we provide everyone with the right resources and know-how. The [Pajamas](https://design.gitlab.com/) design system is the single source of truth for everything anyone needs to know about contributing to GitLab. The UX Department owns the visual and interaction design, as well as implementation of Pajamas.
* **Navigation of GitLab UI:** Navigation is an extremely important part of the user experience. Our goal is keeping the navigation architecture intelligible, comprehensible and making sure it serves every user need.
* **UX Scorecards:** As we grow our platform, we want to keep evaluating user experience of various user tasks and flows to make sure we are tracking progress and improvements over time. [UX Scorecards](https://about.gitlab.com/handbook/engineering/ux/ux-scorecards/) is our framework for achieving this goal. 
* **Technical Documentation:** Our users need reliable documentation, as it helps keep track of all aspects of a platform and it improves on the quality of a software product. We manage [docs.gitlab.com](https://docs.gitlab.com/) as well as related processes and tooling.
* **First Look:** Inviting users into everything we do is very important to us in order to be able to collect feedback. [First Look](https://about.gitlab.com/community/gitlab-first-look/) is our user engagement and recruiting program, which enables us to connect with our users and get their thoughts on our product.
* **UX Showcase:** Collaboration is one of our values. Our [UX Showcase](https://www.youtube.com/playlist?list=PL05JrBw4t0Kq89nFXtkVviaIfYQPptwJz) is a bi-monthly presentation of notable User Experience projects, where Product Designers from every stage group take turns sharing their accomplishments to collect feedback. 

## Heuristics for Success 
The more we can check off each item in this list the more successful we will be:


- **General**
    - Use the simplest, most boring solution for a problem.
    - You are automatically granted permission to experiment and learn from your mistakes.
    - If you identify a problem, just go ahead and fix it. We only ask that you validate that it's a real problem first.
    - Assist the community in making an impact on our product.
    - Quirkiness is part of our DNA. We should embrace it in the right moments and contexts. 🤪
- **Empathy**
    - See the world through other people's eyes, and try to understand their experiences deeply and meaningfully.
    - Understand the user journey and goals.
    - Provide sufficient feedback and direction to achieve user goals.
    - Steer the user in the right direction if they end up in a “bad” place (without blaming them), and recognize their efforts and accomplishments!
- **Structure**
    - Maintain a strong information architecture.
    - Design holistic experiences and workflows.
    - Create hierarchy and a sense of direction to guide users through the flow.
- **Focus**
    - Respect the importance of users' work and avoid gimicky details.
    - Minimize distractions and clutter so users can focus.
    - Remove things that don't contribute to the user flow.
- **Iteration**
    - Never stop improving our products, Pajamas, and documentation.
    - Continuously iterate on our processes.
    - Think big, but break it down into small steps.
    - Aggressively break down issues into the smallest effort that gets results.
    - When applying the [MVC](https://labs.sogeti.com/the-minimum-lovable-product/) approach, make things smaller by reducing the scope of the job-to-be-done rather than sacrificing the end UX.
    - Whenever possible, start in low-fidelity (wireframes, greyscale, etc.) to make sure we get it right before we go any further.


## More Reading About UX

* [How we work](/handbook/engineering/ux/how-we-work/): Learn how we work within our department and with cross-functional partners.
* [Pajamas](/handbook/engineering/ux/pajamas-design-system/): See our Design System, also known as "Pajamas".
* [UX resources](/handbook/engineering/ux/ux-resources/): Helpful information and links.
* [UX Research](/handbook/engineering/ux/ux-research/): Learn about our UX research team and how they work.



## Design Culture
The culture of the design department is characterized by the following:
* We're independent, autonomous, and not hierarchical.
* We have a high level of commitment and reliability to our team.
* We have ownership over our work and are motivated to step up, take risks, and go beyond our roles.
* We don't ask for permission, and we believe that everyone can be a part of the design process.
* We're passionate, kind, honest, direct, transparent, inclusive, and unafraid to ask for help.
* We work asynchronously, we value iteration, and our designs are never complete.
* We're open to ideas and actively collaborate with other teams.
* We're willing to use whatever tools or mediums best communicate our design solutions.

## Personas

Existing personas are documented within the [handbook](/handbook/marketing/product-marketing/roles-personas/).

New personas or updates to existing personas can be added at any time.

Personas should be:

* Informed by research.
* Driven by job title or feature.
* Gender neutral.
* Use bullet points and avoid long narrative.
* Use the [Jobs To Be Done framework](https://hbr.org/2016/09/know-your-customers-jobs-to-be-done)

## Meet Some of Our Team Members

This section is inspired by the recent trend of Engineering Manager READMEs. _e.g.,_ [Hackernoon: 12 Manager READMEs (from some of the best cultures in tech)](https://hackernoon.com/12-manager-readmes-from-silicon-valleys-top-tech-companies-26588a660afe). Get to know more about the people on our team!

* [Christie Lenneville](/handbook/engineering/ux/one-pagers/christie-readme/) - UX Director
* [Valerie Karnes](https://gitlab.com/vkarnes/readme) - UX Manager
* [Sarah Jones](/handbook/engineering/ux/one-pagers/sarahod-readme/) - UX Research Manager
* [Jacki Bauer](https://gitlab.com/jackib/jacki-bauer/blob/master/README.md) - UX Manager
* [Nadia Udalova](https://gitlab.com/nudalova/readme) - UX Manager
* [Justin Mandell](https://gitlab.com/jmandell/readme) - UX Manager
* [Rayana Verissimo](https://gitlab.com/rverissimo/readme) - Sr. Product Designer
* [Matej Latin](https://gitlab.com/matejlatin/focus) - Sr. Product Designer
* [Kyle Mann](https://gitlab.com/kmann/introspection) - Sr. Product Designer
* [Mike Lewis](https://gitlab.com/mikelewis/about) - Technical Writing Manager
* [Iain Camacho](https://gitlab.com/icamacho/koda/blob/master/README.md) - Sr. Product Designer
* [Jeremy Elder](https://gitlab.com/jeldergl/view/blob/master/README.md) - Sr. Product Designer, Visual Design
* [Dimitrie Hoekstra](https://www.notion.so/Readme-0dbd5e5daf3c466787b3e8d52d4263e7) - Product designer
* [Nadia Sotnikova](https://gitlab.com/nadia_sotnikova/tasks/blob/master/README.md) - Product Designer, Monitor
* [Taurie Davis](https://gitlab.com/tauriedavis/readme/blob/master/README.md) - Staff Product Designer

[ux-guide]: https://docs.gitlab.com/ee/development/ux_guide/
[ux-label]: https://gitlab.com/groups/gitlab-org/issues?scope=all&state=opened&utf8=%E2%9C%93&label_name%5B%5D=UX
[ux-ready-label]: https://gitlab.com/groups/gitlab-org/issues?scope=all&state=opened&utf8=%E2%9C%93&label_name%5B%5D=UX+ready
[gitlab-design-project-readme]: https://gitlab.com/gitlab-org/gitlab-design/blob/master/README.md
[twitter-sheet]: https://docs.google.com/spreadsheets/d/1GDAUNujD1-eRYxAj4FIYbCyy8ltCwwIWqVTd9-gf4wA/edit
[everyone-designer]: https://library.gv.com/everyone-is-a-designer-get-over-it-501cc9a2f434
[pajamas]: https://design.gitlab.com

## Join our UX Team

Are you interested in joining our team, hearing about new roles that open up within our department, or unable to find the right vacancy on our [jobs page](https://about.gitlab.com/jobs/apply/)? Fill in [this short form](https://gitlab.fra1.qualtrics.com/jfe/form/SV_djtSRYi6ecLWvxX) and we'll email you whenever we open up a new UX Research, Product Design, Technical Writing, or UX Management position. 
