---
layout: markdown_page
title: "Customer Use-Cases"
---
**Customer Use Cases:**
A customer use case is:
* A customer problem or initiative that needs a solution and attracts budget
* Defined In customer terms
* Often aligned to industry analyst market coverage (i.e. Gartner, Forrester, etc. write reports on the topic)
* Relatively stable over time.

* These are discrete problems that we believe GitLab solves and are reasons customers choose GitLab (hence which we should seek out in prospects)

### **Specific Use Cases**

1. **Create, manage and protect my intellectual property (i.e. source code, design, images, etc)** - in simple terms Source Code Management(**SCM**), but more inclusively, *product configuration management* or *product asset management*.
I need a better way to manage changes to documents, software, images, large web sites, and other collections of code, configuration, and metadata among disparate teams. (Examples in GitLab include Git, branches, merge requests, code review, InnerSourcing, WebIDE, and files.)

    **Analyst Coverage**: IDC, to some extent, forecasts this market. No spot on, recent reports, though Gartner may be considering a future report.

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* Share and reuse code, prevent rework, and make reviews more efficient.
      1. *Deliver Better Products Faster:* Streamline reviews and collaboration around code changes.
      1. *Reduce Security and Compliance Risk:* Easier compliance through approvals of code changes.

1. **Increase the quality of my code while decreasing time to delivery** - Continuous Integration (**CI**)
I need to automate the build and testing processes to consistently integrate code and continuously test. I want to run the unit and integration tests, measure performance and automate manual QA processes. I may use GitLab SCM or another. (Examples in GitLab include Pipeline, CI Runner, Jobs, Scheduled Jobs, Testing, Security Scanning (SAST), and Code Quality).

    **Analyst Coverage**: Forrester CI and Forrester Cloud CI

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* Single source of truth between SCM and CI; consistent and efficient dev experience.
      1. *Deliver Better Products Faster:* Automation to speed the process.
      1. *Reduce Security and Compliance Risk:* test my code automatically and early to reduce risks

1. **Want to speed up my build and release process and empower my developers to automatically deploy code** - (CI/**CD**)
I want to automate the build, test and packaging, configuration and deployment of applications to a target environment. (Examples in GitLab include: Pipeline, CI Runner, Jobs, Scheduled Jobs, Testing, Security Scanning (SAST), and Code Quality.CI Runner, Container Repository, Deploy Boards, Canary Deploys, Partial Deploys, Manual Deploys, Environments.)  

    **Analyst Coverage**: Gartner ARO, Forrester CDRA

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* Scalable, self-service, reusable deployment template. Deploy anywhere.
      1. *Deliver Better Products Faster:* Automatically deploy and test application with early feedback.
      1. *Reduce Security and Compliance Risk:* Enforce common controls and scan for vulnerabilities at the point of code change.

1. **Test for application security vulnerabilities early in my app dev lifecycle** - (Shift-left security or **DevSecOps**)
I need to identify vulnerabilities during development with actionable information to empower dev to remediate vulnerabilities earlier in the life cycle. (In GitLab, SAST, DAST, Dependency Scanning, and Container Scanning.)

    **Analyst Coverage**: Forrester SCA Wave, Gartner Application Security MQ

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* Fix vulnerabilities at point of code change to reduce rework
      1. *Deliver Better Products Faster:* Ability to start testing early in dev process to eliminate vulnerabilities at the source
      1. *Reduce Security and Compliance Risk:* Fix vulnerabilities with actionable feedback to the developer at point of code change. Auto remediate when possible.

1. **Need a better way to manage projects using Agile methodology** - (**Agile** Project Management)
I need a better way of initiating, planning, executing, controlling, and closing the work of a team to achieve specific goals and meet specific success criteria at the specified time. (Examples in Gitlab include Issues, Issue Boards, Issue Weights, Labels, Milestones, and burndown charts.)  

    **Analyst Coverage**: Gartner EAPT, Forrester PPM

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* Scalable, self-service, templated CI/CD, Consistent and efficient dev experience
      1. *Deliver Better Products Faster:* Ability to work in parallel and collaborate. Single source of truth between dev, sec and the business.
      1. *Reduce Security and Compliance Risk:* Single source of truth between dev and sec

1. **Want to achieve expected results of DevOps given siloed teams, lack of visibility and collaboration which inhibits my speed of delivery** - (Simplify **DevOps**)
I want to manage my entire DevOps lifecycle more efficiently with better outcomes. The number of tools and maintenance of integrations is overwhelming and costly and security is challenging to integrate. My processes may include planning to production or may be a segment of the SDLC. (GitLab examples: Epics, Issue Boards, Source Code Management, CI, CD, Security Scans and Monitoring from GitLab. Value Stream Management: (VSM) helps you visualize and manage the flow of new innovation from ideas to customers. In GitLab, cycle analytics is a key element of managing the value stream.)

    **Analyst Coverage**: TBD

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* consistent and efficient dev experience with single source of truth and simplify tool chain
      1. *Deliver Better Products Faster:* More collaboration, working in parallel
      1. *Reduce Security and Compliance Risk:* Testing early, and enforcing common controls like single sign on, and shared view for collaboration, reporting and visibility.

1. **Want to use more modern, cloud-native approaches to application development** (**cloud native**)
I want to use things like containers, K8s, and/or serverless for new development or containerize legacy applications. Help me lift and shift to cloud. Minimize my learning curve to set up, maintain and use clusters.

    **Analyst Coverage**: TBD

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* consistent dev experience, streamline cloud native deployment, simplified tool chain
      1. *Deliver Better Products Faster:* developer self-service, application scalability, resiliency
      1. *Reduce Security and Compliance Risk:* Reduce technical and operational risk of migrating to the cloud. Enforce common controls.

1. **Want to automatically provision, administer and maintain infrastructure as code** - (CI/CD Infrastructure-as-code or **GitOps**)
I manually stage and test environments for infrastructure making it hard to track and error-prone. I want to stage all components and test them to be sure it works to automate my release pipelines, provide consistency, reduce cost, and  eliminate errors. I may frequently leverage integration with Terraform, Kubernetes, Ansible, OpenStack and others.

    **Analyst Coverage**: TBD

    **Value Drivers:**
      1. *Increase Operational Efficiencies:* consistent dev experience, reusable scripts for operations.
      1. *Deliver Better Products Faster:* developer self-service, reusable CI/CD templates.
      1. *Reduce Security and Compliance Risk:* Enforces common controls

### **Other Usecases to consider**

* **Repository Management:** I want a package repository so that I can manage my organization's dependencies and control how they are built, published and shared throughout my organization. I need a local repository to store, version and access dependencies, that allows me to cache, proxy and audit all of my external dependencies in one place. I want all of the above to work securely and seamlessly with my pipelines so that I never have to worry about external dependencies causing problems during the software development lifecycle.

* **Application Monitoring:** (APM) Monitoring application performance and feedback is a most critical step in the DevOps lifecycle. Product teams need to understand how their changes impact the business value of their applications. Examples in GitLab include Application Performance monitoring, server monitoring, Kubernetes Cluster Monitoring, and Kubernetes pod log review.

* **Portfolio Management:** The goal of portfolio management is to determine the optimal resource mix for delivery and to schedule activities to best achieve an organization’s operational and financial goals, while honoring constraints imposed by customers, strategic objectives, or external real-world factors. Examples in GitLab include epics, roadmaps, and milestones. Analyst Coverage: Gartner EAPT, Forrester. GitLab does Agile project mgmt, not Portfolio Mgmt at this time.

* **Incident Management:** I need a platform that consumes alerts from from my monitoring stack and provides me with tools to take action on the critical ones by creating incidents. This tooling would allow us to triage, troubleshoot, remediate, and optimize to reduce risk of future incidents.


### **Non-Use Cases:**

* **Integration - Planning:** Integrations with Project Planning tools like: VersionOne, Rally, Jira, Trello, Monday, Workfront, and Basecamp.  Or integrations with Portfolio Planning tools like Clarity, MicroFocus PPM, or others.
* **Integration - SCM(GitHub):** The most common SCM integration is with GitHub
* **Integration - CI:**  Integrations with Jenkins, CircleCI, Bamboo or other CI servers.
* **Integration - CD:** Integrations with common CD tools such as Puppet, Chef, Ansible, Jenkins and others.



**Specific GitLab Usage Examples**

1. Using JIRA with GitLab
    * A company in the healthcare space had been using GitLab for about a year now,
    and the number one reason they decided they could make the move to GitLab
    was because it works well with JIRA. They had been using JIRA for years, so
    any interruption to this workflow would not be easy for them. Because GitLab
    works well with JIRA, they were able to move over quickly and found features
    like referencing JIRA issues in GitLab merge requests, issues, and commits,
    as well as the ability to close JIRA issues with GitLab commits to be easy
    for them.
    * Placeholder to add another story
1. Using Jenkins with GitLab, then trying GitLab Integrated CI
    * Like the case above, another company had been using Jenkins as their CI
    tool for a long time. As they were evaluating GitLab and found we had a
    Jenkins CI integration, this allowed them to make the move to GitLab
    without disrupting what their team was already use to. Being able to
    display merge request status for builds on Jenkins CI within GitLab was the
    number one reason they decided to make the move to GitLab. They also became
    aware of GitLab's recently implemented Integrated CI, which their users have
    started to test and are finding it may be a solution that ends up working
    better for them.
    * Placeholder to add another story
1. Moving from Core to EE
    * A long time CE user decided to move their company to EE as they grew from
    10 users to 120 in 2 years. Their needs changed, so features like LDAP
    Group Sync that allowed the Admin. to manage group's and their permission
    levels easier, were essential. Another key feature in EE that they now
    needed was Git Hooks. They wanted to prevent git tag removal from their
    users, so implementing a Git Hook allowed them to now do this. On top of
    these features, they were happy to discover how easy it was to upgrade to EE
    from CE simply by using the Omnibus package.
    * Placeholder to add another story
1. Using High Availability with GitLab
    * A current Standard Subscriber decided they wanted to move from having a
    single instance on GitLab EE, to having an HA setup. GitLab offered them
    multiple HA solutions, and after speaking with our Support Engineer's, they
    decided that using two machines with one being a single slave server was
    their best option. What was important to them was each machine had all of
    their GitLab repositories, configuration, and the database. With the slave
    server being a copy of the master, they used DRBD to ensure their data from
    the master is being replicated to the slave server in a timely manner. This
    of course made everyone feel better :)
    * Placeholder to add another story
1. Access to your server and security
    * A customer in the banking industry had security as their number one
    concern. An on-premises solution like GitLab is exactly what they needed
    as it allowed them to have access to their own server, view log files, and
    they could also install additional software like intrusion detection. Since
    GitLab also comes with Audit Events, they could have a history and view
    changes made within the GitLab server which was of extreme importance to
    them.
    * Placeholder to add another story
1. Importing repos and files from GitHub
    * A startup was using GitHub for their source control needs. They wanted to
      leverage GitLab to streamline their DevOps processes. As a startup, it was
      important that they not lose any time or metadata to the transition
      process. Using the GitHub importer tool, they were able to transfer all of
      their data to GitLab without any impact to timeline or productivity.
    * Placeholder to add another story
1. Migrating from SVN to Git
    * Placeholder to add story
    * Placeholder to add another story
1. Protected Branches
    * The customer had been using Bitbucket and was not able to limit developer
      permissions to specific branches and repositories.  They had an ongoing
      problem with developers accidentally pushing branches to the wrong project
      or without proper code review. They decided to switch to GitLab because
      we offer protected branches with more of a fine grained level of
      permissions at the Master level.
    * Placeholder to add another story
