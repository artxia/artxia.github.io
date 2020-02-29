---
layout: markdown_page
title: "Usecase: DevSecOps"
---

<!--

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}
-->

## DevSecOps

The DevSecOps usecase is applicable for customers who are trying to "shift left" to find security vulnerabilities earlier within their DevOps methodology but have not been able to achieve expected results.

Application Security is hard when security is separated from your DevOps flow. Security has traditionally been the final hurdle in the development life cycle. Iterative development workflows can make security a release bottleneck. Customers donn't have enough security people to test all of their code, and hiring more security analysts won't automatically reduce the friction between app sec and engineering teams. Only testing major releases, or limiting tests to certain apps, leaves weak spots hackers can exploit. They need a way to balance risk and business agility. Instead of waiting for security at the end of the development process, they want to include it within their DevOps workflow. Often this is referred to as DevSecOps.

DevSecOps integrates security controls and best practices in the DevOps workflow. DevSecOps automates security and compliance workflows to create an adaptable process for your development and security teams.

### Why is DevSecOps needed?

Balancing business velocity with security is possible. With GitLab, DevSecOps architecture is built into the CI/CD process. Every merge request is scanned through its pipeline for security issues and vulnerabilities in the code and its dependencies using automated tests. This enables some magic to happen.

### Benefits of DevSecOps

Every piece of code is tested upon commit for security threats, without incremental cost.
The developer can remediate now, while they are still working in that code, or create an issue with one click.
The dashboard for the security pro is a roll-up of vulnerabilities remaining that the developer did not resolve on their own.
Vulnerabilities can be efficiently captured as a by-product of software development.
A single tool also reduces cost over the approach to buy, integrate and maintain point solutions throughout the DevOps pipeline.

### Personas

[Who uses Secure capabilities](https://about.gitlab.com/handbook/marketing/product-marketing/competitive/application-security/#who-uses-gitlab-secure-capabilities)

[Market topology](https://about.gitlab.com/handbook/marketing/product-marketing/competitive/application-security/)

#### User Persona


#### Buyer Personas

### [Message House](./message-house/)

The message house for the use case provides a structure to describe and discuss the value and differentiators for the use case.

## Analyst Coverage

- [Gartner - AppSec Testing Hype Cycle 2019]()
- [Forrester - SCA Wave]()

### [AR Plan](./ar-plan/)

  The AR Plan provides key details into how we intend to engage with the analyst community.

## UseCase Capabilities

* Scan results presented to the developer in their native workflow, the MR pipeline  
* Static Application Security Testing (SAST): Prevents vulnerabilities early in the development process, allowing to be fixed before deployment
* Dynamic Application Security Testing (DAST): Once code is deployed, prevents exposure to your application from a new set of possible attacks as you are running your web applications
* Dependency Scanning: Automatically finds security vulnerabilities in your dependencies while you are developing and testing your applications, such as when you are using an external (open source) library with known vulnerabilities
* Container Scanning: Analyze your container images for known vulnerabilities
* Auto Remediation: Auto remediation aims to automated vulnerability solution flow, and automatically create a fix. The fix is then tested, and if it passes all the tests already defined for the application, it is deployed to production.
* Secret Detection: There are several types of secrets that need to be protected. Each commit is scanned for secrets within SAST.
* IAST and Fuzzing: Future features GitLab will be adding to its Security capabilities, see the visions for IAST and Fuzzing

## Top 3 Differentiators

| Differentiator | Value | Proof Point  |
|-----------------|-------------|---------------|
| **Scans performed on feature branch before code is merged & scan results in MR pipeline** | GitLab performs security scans like SAST, license compliance, dependency scanning before the code is merged - giving Developers opportunity to identify and fix security vulnerabilities before they context switch to other activities. This improves cycle time and development costs as the time and cost to resolve defects and vulnerabilities exponentially increase the later it is detected in the development cycle | [Gartner - Integrating Security Into the DevSecOps Toolchain](https://www.gartner.com/doc/3975263) explains how Security should be included in the DevSecOps lifecycle in small actionable steps that developers can take action on quickly & integrating into defect tracking workflow to match the pace of security fixes to the pace of development. |
| **Apply security policy & gating within the MR pipeline** | Bring Development and Security Teams closer by allowing security teams to apply organizational security policies before hand and review/approve security exceptions before the code is merged | **-**  |
| **Streamlined Auditing** | GitLab provides a single source of truth for Dev, Sec and Ops through a single data-store. Everything is audited and for every change, there is a single thread that contains the full audit log of every decision and action - making audit compliance a breeze | The auditor for [Glympse](/customers/glympse/) observed that the company had remediated security issues faster than any other company that he had worked with before in his 20-year career. Within one sprint, just 2 weeks, Glympse was able to implement security jobs across all of their repositories using GitLab’s CI templates |

### What Are The GitLab Advantages?

**Contextual**. Unlike traditional application security tools primarily intended for use by security pros, GitLab secure code capabilities are built into the CI/CD workflows where the developers live. We empower developers to identify vulnerabilities and remove them early in the development cycles. While at the same time, providing security professionals a dashboard to view items not already resolved by the developer, across projects. This contextual approach helps each role deal with items that are most important and most relevant to their scope of work within the delivery process.

**Congruent with DevOps processes**. GitLab secure capabilities support the decision-makers, within their natural workflow. Reports are interactive, actionable, and iterative and most important immediate and relevant to changes made. Developers immediately see the cause and affect of their own specific changes so they may iteratively address security flaws alongside code flaws.
Integrated with DevOps tools. When triaging vulnerabilities, users can confirm (creating an issue to solve the problem), or dismiss them (in case they are false positives or there are compensating controls). When using GitLab, no additional integration is needed between app sec and ticketing, CI/CD, etc.

**Efficient and automated**. Eliminates mundane work wherever possible. Auto remediation applies patches to vulnerable dependencies and even re-runs the pipeline to evaluate the viability of the patch.

## Competitive Comparison

See how we [compare against other Security tools](https://about.gitlab.com/devops-tools/)


## Proof Points - customers

### Quotes and reviews
<List of customer quotes/reviews from public sites>

### Customer Case Studies

* [Glympse](/customers/glympse/) consolidated ~20 tools consolidated into GitLab and remediated security issues faster than any other company in their Security Auditor's experience.
>Development can move much faster when engineers can stay on one page and click buttons to release auditable changes to production and have easy rollbacks; everything is much more streamlined. Within one sprint, just 2 weeks, Glympse was able to implement security jobs across all of their repositories using GitLab’s CI templates and their pre-existing Docker-based deployment scripts.
>
>Zaq Wiedmann, Lead Software Engineer, Glympse

* [BI Worldwide](https://about.gitlab.com/customers/bi_worldwide/) simplified their toolchain and migrated from their previous Git tools to GitLab. The migration was painless and they saw an immediate improvement of collaboration and release pace as a result of their move to GitLab.
>“One tool for SCM+CI/CD was a big initial win. Now wrapping security scans into that tool as well has already increased our visibility into security vulnerabilities. The integrated Docker registry has also been very helpful for us. Issue/Product management features let everyone operate in the same space regardless of role.”
>
>Adam Dehnel, product architect, BI Worldwide

* [Alteryx](https://about.gitlab.com/customers/alteryx/) GitLab allowed Alteryx to truly have everything in one place and within one tool.  GitLab was selected because it is one place for CI, CD, source code, source code management, code reviews, and security scanning. 

### References to help you close

[SFDC report of referenceable secure customers](https://gitlab.my.salesforce.com/a6l4M000000kDw2)


## Resources
### Presentations
* [Security customer presentation](https://docs.google.com/presentation/d/1WHTyUDOMuSVK9uK7hhSIQ_JbeUbo7k5AW3D6WwBReOg/edit?usp=sharing)

### White paper
* [A Seismic Shift Left](https://about.gitlab.com/resources/downloads/gitlab-seismic-shift-in-application-security-whitepaper.pdf)

### Integration with third party commercial scanners
* [WhiteSource](https://about.gitlab.com/handbook/marketing/product-marketing/enablement/security-integrations-whitesource/)

### Simplifying DevOps Videos
* [Security Dashboard demo](https://youtu.be/U2_dqwTRUVk)
* [Deep Dive into a Security demo](https://youtu.be/k4vEJnGYy84)


### Integrations Demo Videos
* See how [integration is the key to successful DevSecOps](https://about.gitlab.com/blog/2018/09/11/what-south-africa-taught-me-about-cybersecurity/)

### Clickthrough & Live Demos
* [All Marketing Click Through Demos](/handbook/marketing/product-marketing/demo/#click-throughs)
* [All Marketing Live Demos](/handbook/marketing/product-marketing/demo/#live-instructions)
