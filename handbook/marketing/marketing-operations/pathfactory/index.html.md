---
layout: handbook-page-toc
title: "PathFactory"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Uses

PathFactory (PF) is leveraged as our [content library & content distribution system](/handbook/marketing/corporate-marketing/content/#content-library). The [Digital Marketing Programs team](/handbook/marketing/revenue-marketing/digital-marketing-programs/) is primarily responsible for all the of the content within the PathFactory tool. Marketing program managers work with other teams in marketing to organize and curate assets into tracks that are then disseminated for use in Marketo, `about.gitlab.com`, and other campaign-related channels.

## Access   

The Marketing Operations team is responsible for managing access requests & provisioning the appropriate level of access for each role/function. Providing access is generally hanlded via baseline entitlement; however, if you need access and it is *not* part of your roles baseline entitlement please open a [`Single Person Access Request` issue](/handbook/business-ops/it-ops-team/access-requests/#single-person-access-request) and provide business reason why access is needed.   

### User Roles   
There are three levels of access - Admin, Author, Reporter - which are granted based on the persons' role and team function within GitLab. **All access levels** have the ability to view the analtyics page within the tool. 

#### Admin  
Admin access is granted to Marketing Operations only.  

#### Author 
`Author` access allows user to build, edit and publish content tracks applying existing tags to the assets. This level of access is granted to the Marketing Program Managers and select Content team members.  

#### Reporter 
`Reporter` access provides general visibility to content within PathFactory but does not allow end user to create or modify any of the content, tracks or tags. This level of access is granted for the general GitLab team member both within Marketing and elsewhere who have a business need to have access.  

## Training

*  [Knowledge base](https://lookbookhq.force.com/nook/s/kb)
*  [Getting started video series](http://successwith.pathfactory.com/c/lookbookhq-tutorial-?x=Blrk3E)
*  [Digital marketing brown bag session overview](https://drive.google.com/open?id=1Hzb6ard48k-11r5a8oBDD_NLjeZnkMK2) - [Slides](https://drive.google.com/open?id=1XxOIE2O-VW0I9z09kpLs5ops52oF6iDSP1a1MF8NkGY)

## Changelog

Periodically, significant changes are made or added to PathFactory and processes that affect overall data and reporting. As such we have a [changelog](https://docs.google.com/document/d/1qd9X-V0WNBTklCKNYVRmjJtiOcPu6dZYkfJ2uuQt_Co/edit?usp=sharing). **Everyone with `Author` access that is making additions or changes to assets, content tracks, or otherwise should add their changes to the changelog with a linked issue.** Scenarios for adding to the changelog:

1.  Creation or launch of a new content track and where it will be used
1.  Creation or launch of a new website promoter
1.  Additions or changes to a form strategy within a live content track
1.  Additions or changes to assets within a live content track
1.  Expiration of an asset from the content library
1.  Change of a custom URL slug for an asset or content track and why
1.  Change of promote settings within a live content track and why

### Instructions

1.  Open the [PathFactory changelog doc](https://docs.google.com/document/d/1qd9X-V0WNBTklCKNYVRmjJtiOcPu6dZYkfJ2uuQt_Co/edit?usp=sharing).
1.  Add the date you made the change if it doesn't already exist.
1.  Add a bullet with your GitLab username and document the changes you made, making sure to include links to issues or relevant PathFactory links.

## Content library

**Before uploading content:** 

1. Follow the [blog style guide](/handbook/marketing/corporate-marketing/content/editorial-team/).
1. Use the search to determine if it’s already been added. If you try to add an asset that's already in the library, the system will tell you it already exists.
1. Ensure you have the most valuable version of the asset (blog post vs. case study or PDF).
1. Ensure you have the most recent version of the asset.

### How to upload content

1. Click `Add Content` in the top right of the content library.
1. Choose how you will upload the asset (Website URL, file upload, or CSV).
   * For a Website URL, copy/paste the URL. For multiple URLs, paste one per line.
   * For a file upload, select this option and either drag and drop the file onto the file upload window or select it from your computer. Files can be up to 100MB.
   * If you want to [bulk upload multiple assets using the CSV option](#bulk-uploading-new-assets-to-the-content-library), create an issue in the Marketing Operations project and assign `@sdaily`.
1. Enter the title of the asset under `Public Configurations`. Ensure that the title is free of SEO meta information such as `| GitLab`.
1. Provide a clear and concise description of the content if one does not exist.
1. Select the content type from the dropdown.
1. Leave the engagement score at a default of 20 seconds with a score of 1.
1. Copy and paste the public title into the internal title field.
1. Funnel stage and estimated cost is set automatically based on the content type you chose earlier. Please leave these auto-generated tags as is and do not force change. If you require a change to how content type is tied to funnel stage and estimated cost, please open an issue and assign `@sdaily`.
1. Set the language of the asset.
1. Select the Business Unit of the asset based on use and sales region.
1. Set the expiry date of the asset if one exists.
1. Leave External ID blank.
1. Select the content topics on the right-hand side that categorize the asset. Follow the [content tag map below](#tracking-content) when tagging content with topics.

**After adding the asset to the library:**

1. Select the asset you just added to the library. A preview of the content will appear on the right-hand side of the content library. Scroll down the window pane under `source URL` and locate `Custom URL slug`.
1. Update the custom URL slug to be descriptive of the content with no stop words (and, the, etc.).
    1.  **Please Note:** DO NOT change a custom URL slug that is part of a `[LIVE]` content track. You can see whether an asset is part of a live content track by clicking on it in the content library and scrolling to the bottom of the preview pane. This action can affect any links to this item that have been previously shared and break the asset consumption tracking via [listening campaign](#listening-campaigns). 
    1. If a URL slug needs to be modified, please open an issue, assign to `@sdaily`.  
1. We force `https://` to content tracks by default. As a result, all assets must use `https://` in the link to work in the content track properly. If you upload content that is *not secure*, it *will not* show a lock icon next to the URL and it will not work in a secure content track. Please manually add `https://` if it is not already there.

### Bulk upload

You can bulk upload multiple assets to the content library via a CSV file.

1.  Make a copy of this [CSV template](https://drive.google.com/a/gitlab.com/file/d/1Ad4iSwHt2bdRKp5GGUZtrtzY5YShZlyI/view?usp=sharing) for your upload.
2.  Provide all the information in the template for your new assets and save as a CSV.
3.  Create an issue and tag `@sdaily` to review the template and upload to PathFactory.

### Analyst reports

Expiry dates will not automatically deactive content after expiration. You must manually deactivate the content if it’s past the expiry date. To expire an analyst report from PathFactory, [open an issue](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/issues/new?issuable_template=Gated-Content-Expiration-Analysts-MPM) in the digital marketing programs project using the `Gated-Content-Expiration-Analysts-MPM` issue template.

## Content tracks

Before creating a new content track, decide what type of content track (target vs. recommend) you want to create. Use the criteria below to decide the best option:

### Best practices

**Target track**

* Curated content
* Known audience
* Personalized journey (email, website, targeted display)
* 5-7 pieces of content
* Use target in webinar reg and follow-up
* Use target to GUIDE

**Recommended track**

* Dynamic content sequence (it will automatically move content to the top of the track that is performing well)
* Anonymous audience
* Personalized journey (web, general display, social)
* Tracks the most popular journey (which pieces are being viewed, can be exported into a target track)
* Use recommend to DISCOVER

### Create a content track

1. When you're ready, navigate to the content track type you want to create (target or recommend), and click the "Create track" button in the top right.
1. Name your content track. Be descriptive about the topic or campaign that your track will be used for. If you're unsure, review the names of other content tracks to get an idea. The content track name is for internal use only and will not be shown to visitors. Each content track has to have a unique name. You cannot use duplicate names for content tracks.
1. Choose to clone an existing content track, which will copy all assets from that content track into yours, or simply start from scratch.
1. Choose the folder where your content track will live. Follow the current folder hierarchy for organization. If none of the folders accurately represent your content track, ping `@sdaily` to create a new folder in the structure.
1. Tag your content track with labels that will tell everyone accessing the content track which channels it will be used on (internal use only). If you will be launching on a channel that doesn't exist from the picklist, ping `@sdaily` to add a track label for your channel.
1. Click "Create Track".
1. Add assets to your track by clicking the "Add content" button at the top right. A window will pop up with the content library. Use the sorting options at the top to quickly add content by topic, type, funnel stage, etc. PathFactory content tracks are meant to encourage content binging (visitors reading more than 1 asset to accelerate them in the pipeline by helping them self educate faster in one visit). So as best practice, have more than 1 asset in a track.

#### Configuring content track settings

##### Track settings

1. Set the `custom URL slug` for the content track. [Follow the instructions](#after-adding-the-asset-to-the-library) for creating a custom URL slug for an asset. **Important:** All content tracks should be set up with custom URL slugs to prevent any future changes to the track from breaking the link and thus the user experience. If you change the custom URL slug after a PathFactory link has been implemeneted, those links have to be updated wherever they were used (ads, emails, website, etc.).
1. Ensure that the Search Engine Directive is set to `No Index, No Follow`.
1. Set the appearance for the track. If you require a new appearance, create an issue in the Marketing Operations project and assign `@sdaily`.
1. Set the language for the track.
1. Leave `Links & Sharing` set to default.
1. Leave `External ID` set to default.
1. Turn on the `Cookie Consent` before providing the approved content track link for live use.

##### Promoters

This is where you will choose how your content track displays to the visitor. Note the different functionality of each below. Before going live, you can test each promoter to find the one that works best for the goals of your PathFactory experience.

* You can only use the `Header` feature with the `Sign Posts` and `Bottom Bar` promoters.
* The `Header` is used to add additional branding to your content track.
* The `Flow`, `Sign Posts`, and `Bottom Bar` cannot be used together. Choose 1 of the 3.
    * **Flow:** Scrollable content menu allows visitors to jump ahead in their Content Track, or simply use the Next buttons to move forward.
    * **Sign Posts:** Customizable Next and Previous buttons allow visitors to navigate through content. Used for more of a linear journey through the content.
    * **Bottom Bar:** Collapsible content menu along page bottom.
* The `End Promoter`, `Exit`, and `Inactivity` promoters can be used in conjunction with either the `Flow`, `Sign Posts`, or `Bottom Bar` promoters.
    * **End Promoter:** Opens final asset in a new tab. 
        * Available overrides:
            * Link
            * CTA Label
            * Delay (seconds)
    * **Exit:** Suggested content window appears when visitor tries to navigate away from the Content Track. 
        * Available overrides:
            * Headline
            * Message
            * Items to show (choose from assets within the current track)
            * Delay (seconds)
    * **Inactivity:** Message flashes on tab when left inactive.
        * Available overrides:
            * Inactive tab title
            * Delay (seconds)

##### Form strategy

Form strategy is used on content tracks to collect data from unknown visitors and should only be used when a track entry point is **not** from a webform or landing page (i.e. direct link from digital ad or web promoter). Not all content tracks will or should have form strategy turned on. The forms used in PathFactory are directly tied to currently existing Marketo forms. If the form strategy is implemented, please ensure `Show to Known Visitors` is left **unchecked**. For help with PathFactory forms and workflows, please create an issue in the Marketing Operations repository, apply `MKtgOps` & `PathFactory` labels, and assign `@sdaily`.  

**Please Note:** We have [listening campaigns](#listening-campaigns) in Marketo set up to capture consumption of content that would have been gated had PathFactory not been implemented. The listeners also incorporate PathFactory activity into the [MQL scoring model](/handbook/business-ops/resources/#mql-scoring-model). This means that you do not need to add form strategy to a content track if entry point is from a landing page and there are listening campaigns set up for assets in your track that would normally be gated. [Please create an issue](https://gitlab.com/gitlab-com/marketing/marketing-operations/issues) in the Marketing Operations repo and assign `@sdaily` to set up a lisetning campaign for an asset.

###### Adding form strategy to a content track

1.  In the content track settings sidebar (left), toggle "Forms Strategy" to `On`.
1.  Click `View Form Strategy` located below the `Add Content` button.
1.  Determine whether the form strategy will be applied to individual assets or the entire track. For individual assets, you'll choose `Content Rules`; for form strategy on the entire content track, you'll choose `Track Rule`. 

**Form strategy for individual assets:**

1.  Click `Add Rule` in the `Content Rules` row. 
1.  Select the `General Form (2074) LIVE` form. This is the only form that is set up with capture tags to appropriately track data from PathFactory to Marketo. Do not use any other forms.
1.  Under `Display Behavior`, click the dropdown and choose the assets where you want the form to show. (**Please Note:** only assets that you have added to the content track will show in the dropdown. If you want the form to show on an asset that *is not* in the track, you will need to add it first.)
1.  Select the amount of seconds you want to delay before the form shows on the asset. Ten seconds is the default selection.
1.  Select additional options for the form behavior. If you will be using the content track or individual asset links in an email, you are working with a known audience and therefore should only select `Show to unknown users`. This prevents forms being shown to users who are already known in Marketo. However, if you are using the form on the web or other channels, you'll want to select `Show to unknown users` only.
1.  Leave `If submitted, allow form to show again` turned off.
1.  You can `allow visitors to dismiss the forms` if it is not crucial to its use to have them submit their info. This decision ultimately lies with the directly responsible MPM.
1.  The option `Keep promoters active when form is shown` is also up to the directly responsible MPM. For example, if the `Flow` promoter is used on a content track, they will still be able to see the sidebar of avialable content while the form is shown to them. If this option is turned off, the visitor *will not* be able to click on any content in the sidebar until they fill out the form.

**Form strategy for content tracks:**

1.  Click `Add Rule` in the `Track Rule` row. 
2.  Select the `General Form (2074) LIVE` form.
3.  Under `Display Behavior` you can choose to serve the form based on the number of content assets viewed or the total time spent on the track. This decision lies with the directly responsible MPM.
4.  All other options for content track rules are the same for individual assets (see above).

#### Testing a track link:

1. Click through the experience to ensure assets, CTAs, and forms load properly and that promoters are working as intended.
1. Remove any extraneous `?` (there should only be one immediately after the end of the URL).
1. Watch for extra `&` when appending UTMs.
1. Ping `@sdaily` to test and ensure the experience is working as intended.

**When a track is LIVE (in use):**

1. Change the target track title in use to `[LIVE] Name of track`.

#### Adjustments to live content tracks

* You can add assets and adjust the position of assets to a `[LIVE]` content track. 
* Before you remove an asset from a content track, please create an issue in the Marketo Operations repo and assign `@sdaily`. Removing an asset or changing the custom URL slug of an asset in a `[LIVE]` track can disrupt the user experience for the visitor and activate the `#all` track or fallback URL (`about.gitlab.com`) instead of the intended content track.

## Using PathFactory links

*  Only content track links are meant to be used and shared. Do not share individual asset links from the content library.
*  You can use a content track link for multiple use cases as long as you apply UTMs appropriately. Applying UTMs helps us differentiate how the track performed across different channels.
*  To ensure proper tracking of an asset in PathFactory, it should be included within a content track and not shared with an individual link from the content library.
*  If the link breaks or an asset is deleted, the user will be redirected from your content track to the `#all` track, which includes all assets uploaded to PathFactory. In a case where the user is not redirected to the `#all` track, they will be redirected to the `Fallback URL` which is set to `about.gitlab.com`.

### Target track links

1.  Use the `Get Share URL` feature next to the title of the track. `Share links` are to be used in locations such as the website whereas `Email tracking links` are only for use in email. **Note:** If it’s in email, it’s a known audience so don’t gate any assets in the track. Only use `share links` on the web and those tracks *can have* gated assets within PathFactory.
1.  If you want a particular asset to show first, that asset should be located in the first position of the target track. 

### Recommended track links

1.  To use a recommended track link, click on any of the assets in the track and copy the link from the asset window on the right. The asset you choose to share the link will be shown to the user first.

### Appending UTMs to PathFactory links

1. First check and see if there is a question mark `?` already existing in the PF link. Typically there is one. The only time it won't have a `?` is when you set a custom URL.
1. If there is a question mark `?`, first add an ampersand `&` at the end of the PF link, followed by the UTMs. 
    * For example:
        * PF Link: `https://learn.gitlab.com/c/10-strategies-to-red?x=53kuPb`
        * PF Link with UTMs: `https://learn.gitlab.com/c/10-strategies-to-red?x=53kuPb&utm_source=email&utm_campaign=test`
1. If there is no question mark `?`, first add a question mark `?` at the end of the PF link, followed by the UTMs.
    * PF Link: `https://learn.gitlab.com/c/10-strategies-to-red`
    * PF Link with UTMs: `https://learn.gitlab.com/c/10-strategies-to-red?utm_source=email&utm_campaign=test`

**Marketo links**

1. For a PF Marketo link, it will typically already include a question mark "?". To add UTMs, first add an ampersand `&` at the end of the PF link, followed by the UTMs.
    * Example: `https://learn.gitlab.com/c/devops-explained-git?x=GVFK3F&lb_email={{lead.Email Address}}&utm_source=email&utm_campaign=test`

### Adding a PathFactory URL to Marketo:

1. Remove any extraneous `?` (there should only be one immediately after the end of the URL).
1. Watch for extra `&`.
1. Ping `@sdaily` to review the link before implementation for quality assurance purposes.

## Tracking content

Unsure what content topics align with your asset? Use the table below as a guideline to tag content you upload to PathFactory accordingly.

| Topic | Use | Example |
| ------ | ------ | ------ | 
| Agile delivery | Content that relates to the agile delivery process decision framework which emphasizes incremental and iterative planning. | [What is an Agile mindset?](/blog/2019/06/13/agile-mindset/) |
| Agile software development | Content that relates to the agile software development methodology which emphasizes cross-functional collaboration, continual improvement, and early delivery | [How to use GitLab for Agile software development](/blog/2018/03/05/gitlab-for-agile-software-development/) |
| Application modernization | Content that relates to the process of converting, refactoring, re-writing, or porting legacy systems to more modern programming and infrastructure. Content on this topic may cover cost/benefit of updating legacy systems, process, system, and culture changes, and toolstack comparisons. | [3 Strategies for implementing a microservices architecture](/blog/2019/06/17/strategies-microservices-architecture/) |
| Application security | Content that covers the production and delivery of secure software, security techniques and capabilities, and trends in the application security field. | [5 Security testing principles every developer should know](https://about.gitlab.com/blog/2019/09/16/security-testing-principles-developer/) |
| Automation | Content that relates to using technology to automate tasks. Likely use cases are how automation impacts productivity and workflows, feature highlights & tutorials, and case studies. | [How IT automation impacts developer productivity](/blog/2019/05/30/it-automation-developer-productivity/) |
| AWS | Content that relates Amazon Web Services. Likely use cases are case studies where the customer uses GitLab + AWS and integration information & tutorials. | [How to set up multi-account AWS SAM deployments with GitLab CI/CD](/blog/2019/02/04/multi-account-aws-sam-deployments-with-gitlab-ci/) |
| Azure | Content that talks specifically about Microsoft Azure. Likely uses cases are tutorials on using GitLab + Azure cloud or competitive content. | [Competitive analysis page for Azure DevOps](/devops-tools/azure-devops-vs-gitlab.html)
| CI/CD | Content that covers continuous integration, continuous delivery, and continuous deployment. This content is likely to be more technical, explaining tools, methods for implementation, tutorials, and technical use cases. | [A quick guide to CI/CD pipelines](/blog/2019/07/12/guide-to-ci-cd-pipelines/) |
| Cloud computing | Content that relates to the practice of using a network of remote servers hosted on the Internet to store, manage, and process data. Likely uses cases are content discussing various cloud models (public, private, hybrid, and multicloud), integrations, and tutorials. Some customer case studies may be tagged with this label if the case study is *primarily* about GitLab enabling their cloud computing model. | [Top 5 cloud trends of 2018: What has happened and what’s next](/blog/2018/08/02/top-five-cloud-trends/) |
| Cloud native | Content that relates container-based environments. Specifically, technologies are used to develop applications built with services packaged in containers, deployed as microservices and managed on elastic infrastructure through agile DevOps processes and continuous delivery workflows. | [A Cloud Native Transformation](/webcast/cloud-native-transformation/) |
| Containers | Content that relates to using, running, maintaining, and building for containers. | [Running Containerized Applications on Modern Serverless Platforms](https://www.youtube.com/watch?v=S8R7sSePAXQ)
| Continuous delivery | Content that covers methods and tools for delivering or updating software in smaller increments, resulting in a better end-user experience. Both technical and strategic content may be found. | [Securing the journey to Continuous Delivery](https://about.gitlab.com/blog/2019/10/30/secure-journey-continuous-delivery/) |
| DevOps | Content that relates to DevOps methods, process, culture, and tooling. [Keys to DevOps success with Gene Kim](https://www.youtube.com/watch?v=dbkj0qXQ22A)
| DevSecOps| Content that relates specifically to integrating and automating security into the software development lifecycle. Content that relates to cybersecurity should be tagged `security` and not `devsecops`.| [A seismic shift in application security](/resources/downloads/gitlab-seismic-shift-in-application-security-whitepaper.pdf) |
| Digital transformation | Content that covers the process, methods, and strategy of integrating technology into all aspects of business. This content also includes strategies, tools, and tactics for furthering innovation, building new efficiencies, and delivering higher value faster. | [The cloud adoption roadmap](https://about.gitlab.com/blog/2019/12/05/cloud-adoption-roadmap/) |
| Git | Content that relates to implementing and using the distributed version contronl system, Git. | [Moving to Git](/resources/downloads/gitlab-moving-to-git-whitepaper.pdf) |
| GKE | Content that is specifically about Google Kubernetes engine and Google Cloud Platform. Likely use cases are integrations, tutorials, and case studies | [Demo: Deploy to GKE from GitLab](https://www.youtube.com/watch?v=u3jFf3tTtMk)
| Information technology management | Content that relates to the monitoring and administration of IT systems, including hardware, software, and networks. (Definition adapted from [IBM](https://www.ibm.com/topics/it-management)) Content may be either technical or strategic. | [Shifting from on-prem to cloud](https://about.gitlab.com/blog/2020/01/09/shifting-from-on-prem-to-cloud/) |
| Jenkins | Content that is specifically about Jenkins. Likely uses cases are integrations, competitive, comparisons, and case studies. | [3 Teams left Jenkins: Here's why](/blog/2019/07/23/three-teams-left-jenkins-heres-why/) |
| Kubernetes| Content that relates to implementing and using kubernetes. Likely use cases are cost/benefits, tutorials, and use cases. | [Kubernetes and the future of cloud native: We chat with Kelsey Hightower](/blog/2019/05/13/kubernetes-chat-with-kelsey-hightower/) |
| Microservices | Content that covers the practice of breaking out application components individually as services for the purpose of running applications at scale with greater flexibility. | [3 Strategies for implementing a microservices architecture](https://about.gitlab.com/blog/2019/06/17/strategies-microservices-architecture/) |
| Multicloud | Content that relates to how enterprises use multiple cloud providers to meet different technical or business requirements. | [What does Kubernetes have to do with it?](https://about.gitlab.com/blog/2020/02/05/kubernetes-and-multicloud/)
| Open source | Content that covers open source projects, partnershipship initiatives, and community contributions. | [What to consider with an open source business model](https://about.gitlab.com/blog/2019/07/05/thoughts-on-open-source/)
| Remote work | Content that covers remote work, including best practices, stories, and advice. | [The case for all-remote companies](https://about.gitlab.com/blog/2018/10/18/the-case-for-all-remote-companies/)
| SCM | Content that relates to source code management, Git, GitLab Flow, and version control. | [GitLab Workflow: An Overview](https://about.gitlab.com/blog/2016/10/25/gitlab-workflow-an-overview/)
| Security | Content that relates to cybersecurity and application security practices. | [When technology outpaces security compliance](/blog/2019/06/10/when-technology-outpaces-security-compliance/)
| Severless computing | Content that relates to the ability to deploy functions on any infrastructure managed through a single UI. | [Announcing GitLab Serverless](https://about.gitlab.com/blog/2018/12/11/introducing-gitlab-serverless/)
| Single application | Content that covers the methods and benefits of using a single application throughout the software development lifecycle, including increased efficiency and transparency. | [Customer story: Driving better developer and customer experiences with a single application](https://about.gitlab.com/blog/2018/09/26/customer-interview-charter-communications/) |
| Software development | Content that covers software development methodologies, cycle time, and development techniques. | [How to use GitLab for Agile software development](https://about.gitlab.com/blog/2018/03/05/gitlab-for-agile-software-development/)
| Toolchain | Content that relates to toolchain and stack management. | [How to manage your toolchain before it manages you](/resources/downloads/201906-gitlab-forrester-toolchain.pdf)
| VSM | Content that relates to the topic of value stream mapping and management. Topics that fall under this tag may include cycle time, cycle analytics, and software delivery strategies and metrics. | [The Forrester Value Stream Management Report](/analysts/forrester-vsm/index.html) |
| Workflow | Content that relates to understanding and implementing workflows throughout the software development lifecycle. Likely uses are content that explains a particular workflow or how to set up a workflow in GitLab. For example: how a workflow might change when a level of automation is introduced. | [Planning for success](/resources/downloads/gitlab-planning-for-success-whitepaper.pdf) |

## PathFactory analytics

All roles and permissions have access to reporting functionality in PathFactory. Feel free to peruse `Path Analytics` or view insights in the content library and content tracks. If you would like a scheduled report or have a different PathFactory data request, create an issue in the Marketing Operations repo and assign `@sdaily`.

## Listening Campaigns 

In Marketo, we have programs built to "listen" for PathFactory (PF) activity & content consumption allowing us to track behaviour without having to physically gate all the assets which disrupts the user experience.   

The PF<>Marketo listening programs are built to triggered based on the `slug` associated to each of asset. **Very Important: Do NOT to change the `slug` in PF without notifying Ops *prior* to making the change**. Each listening campaign has a Salesforce (SFDC) campaign associated to it tracking consumption and applying Bizible touchpoints.  

The naming convention for each of the listeners is specific to the asset type & is used as a trigger to the appropriate scoring campaign *within Marketo* at this time these listening campaigns have **no impact** on PathFactory engagement scores. The same naming convention is used for **both** Marketo & Salesforce campaigns.   

| **Asset Type** | **Naming Convention** |
| :--------- | :---------------- |
| Whitepaper | PF - Whitepaper - | 
| eBook      | PF - eBook -      | 
| Analyst Report | PF - Analyst Report - | 
| Research Report | PF - Research Report - | 
| Demo  | PF - Demo - | 
| Datasheet | PF - Datasheet - |  
| Webcast | PF - Webcast - |

### Salesforce Campaign Type  

For the PathFactory listening campaigns there is a corresponding Salesforce `Campaign Type` to be used. The `Campaign Member Status` simply tracks if the content was consumed. This Salesforce `Campaign Type` should be used for **nothing** else. For greater details, see the [Business Ops Resources - Campaign details](/handbook/business-ops/resources/#campaign-type--progression-status).

### PathFactory SFDC Panel   

In Salesforce (SFDC) there is a `PathFactory` section on both the LEAD and CONTACT layout that provides information about Pathfactory content consumption. 

1. These fields are all **session** based - this is by design from PathFactory and the field values overwrite with new data for every session. 
1. A piece of content is considered "consumed", by default, when it has been viewed for 20 seconds minimum. 
     - This can be modified per asset. 
     - At this time all assets have been set up the same. If that changes, this page will be updated with details.
1. A PF "session" is a single content consumption period. 
1. A "session" closes after 30 minutes of inactivity or at 11:59pm (instance set timezone - SFDC is set to Pacific time).
1. If a person consumes more than one content track in a **single session** all of the assets/tracks viewed will be displayed in the fields cumulatively. 

### PF Panel Fields

![](/images/handbook/marketing/marketing-operations/pf_sfdcpanel.png)

| **Field Name** | **Purpose** | 
|:---------- | :------ | 
| PathFactory Experience Name | The PathFactory track name - [more details](#content-tracks) | 
| PathFactory Assets Viewed | Cumulative number of assets viewed. **This is not associated to time consumed! See Content Count for difference** |
| PathFactory Asset Type | A tag to help categorize types of content (whitepaper, video, eBook, etc) |
| PathFactory Funnel State | Each asset is tagged with stage of funnel most applicable to asset - Top of Funnel, Middle of Funnel or Bottom of Funnel | 
| PathFactory External ID | A non-unique ID that can be added to tracks &/or assets, which can be leveraged to organize content and configure it in Marketing Automation Platform (i.e Marketo) | 
| PathFactory Engagement Score | Each asset in content library can be assigned an engagement score; this score is passed from PF to SFDC and used to determine meaningful engagement with content. | 
| PathFactory Engagement Time | Cumulative time a person spends consuming assets in session. | 
| PathFactory Content Count | Cumulative count of assets consumed. Example: if person consumes 2 whitepapers, 1 video and blog post for *minimum of 20 seconds each* in a **single session** this field would show 4. | 
| PathFactory Content List | Cumulative list of each assets content id/slug for each asset consumed. | 
| PathFactory Topic List | Assets are tagged by **topic**. This is manually set & aligns with the [tracking content](#tracking-content) list. | 