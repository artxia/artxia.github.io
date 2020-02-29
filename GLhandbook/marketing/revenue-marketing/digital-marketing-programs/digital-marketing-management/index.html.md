---
layout: handbook-page-toc
title: "Digital Marketing Management"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Digital Marketing Managers
Digital Marketers are responsible for all inbound marketing.

## DMP labels in GitLab

*Note*: Some of the following labels only exist on the Digital Marketing Programs project level.

* **Digital Marketing Programs**: General label to track all issues related to Digital Marketing Programs
* **SEO**: Used for any issues that require SEO support, including keyword research, reporting, etc.
* **SEM**: Used for issues that require organic and paid search initiatives
* **Paid Ads**: Used for any paid advertising campaign such as Google Ads
* **Paid Social**: Used for paid social campaigns such as LinkedIn InMail and Facebook Ads 
* **Site Optimization**: Used for any issues to optimize the website for conversions
* **Conversion Rate Optimization (CRO)**: Generic label used by Digital Marketing Programs Manager to track all issues related to conversion rate optimization (CRO) (*scoped labels below*)
    *  **CRO::A/B Test**: experiment using two or more variants of the same web page or email (A and B)
    *  **CRO::Analysis/Reporting**: conduct an analysis to determine patterns in data and identify potential experiments or tests to improve conversion rate
    *  **CRO::Copywriting/Editing**: used for copywriting/editing from CRO
    *  **CRO::Multivariate Test**: tests variants of two or more elements simultaneously to see which combination creates the best outcome
    *  **CRO::Redirect Test**: test separate web pages against each other
* **Hotjar**: used for requesting a heatmap for a page on the website from the Digital Marketing Programs team

## DMP Slack channels

*  `#digital-marketing`: General digital marketing conversation and questions
*  `#dmpteam`: Discussion for DMP team members

## Website analytics dashboards

We use Google dataStudio to create an easy to share and repeatable process for sharing analytics data for about.gitlab.com. dataStudio allows us to combine data from Google Analytics, Google Ads, and a variety of other sources to create reports with key data for any GitLab team.

When we connect data from Google Sheets everyone on the DMP team needs to able to access and edit data as needed. To accomplish this we add all Google Sheets used in dataStudio to the Shared Drive in the [dataStudio sub-folder](https://drive.google.com/drive/folders/1pO0fVLM-K0KrLNu8MWvzI-i96QXFdgeR). Be sure you only share your Google Sheets in the shared drive because dataStudio does not currently support sharing data sources from shared drives.

## Self-serve Website analytics dashboards
* Google Analytics traffic: If you would like to check the traffic, referrals, or clicks off of a page hosted on the marketing site (about, docs, etc) just enter your page URL or URLs into the `Page` field in this dataStudio report [Page-level Google Analytics data](https://datastudio.google.com/u/0/reporting/11pNZyzJ1JEudO4jRWaX989etLLcR6wUn/page/KNqS).
* Google Search results keywords: If you would like to check the keywords from a specific about.gitlab.com page in Google search, just enter your page URL into the `Landing Page` field in this dataStudio report [Google Search Console keyword lookup](https://datastudio.google.com/open/1No1sSsCH2EHkqPyLl-AEEQ1be3_p_kpj).
* Google Search results pages: If you would like a list of URLs surfacing for a specific keyword surfacing for about.gitlab.com in Google search (about, docs, etc) just enter your keyword into the `Query` field in this dataStudio report [Google Search Console landing page lookup](https://datastudio.google.com/open/10Qa9AgGt11xJWaycUDfvFq1Nn714sJQq).

### Active dataStudio dashboards

- [Marketing metrics dashboard](https://datastudio.google.com/reporting/1mvDffnzlIWsr-2S_cvkpRx0X25hiM_TI/page/1M) — Used to generate data for our monthly marketing metrics deck. A few elements update manually, ping the Digital Marketing team in #digitalmarketing if you need updated numbers.
- [Content marketing dashboard](https://datastudio.google.com/reporting/1NIxCW309H19eLqc4rz0S8WqcmqPMK4Qb/page/FCsh) — Blog content reports, primarily used by the content team to track OKR progress.
- [Just Commit dashboard](https://datastudio.google.com/reporting/1dbt-3WI6KzySYrnolIUfCufvvtba20f9/page/kWdQ) — Tracks progress of Just Commit integrated campaign.
- [Job pages dashboard](https://datastudio.google.com/reporting/1w6TwUeGjkQpPZz4jvp9Hye8vdGP6MYel/page/JcPY) — Provides context around job page interactions.
- [Security releases dashboard](https://datastudio.google.com/reporting/1bP748BOhYmgWRcfeoRiSCOHz7q4NUMkV/page/l7vj) — Website analytics data for security release blog posts.
- [about.gitlab.com CrUX dashboard](https://datastudio.google.com/reporting/1f-akzELoGzJRdBFPgMTzgHPrSOshUgki/page/cJUR) — *Public* See [Chrome User Experience Report](https://developers.google.com/web/tools/chrome-user-experience-report/) for definition of report dimensions. This dashboard shows CrUX data for about.gitlab.com, assembled with PageSpeed Insights and Public Google BigQuery.  

## Requesting Digital Marketing Promotions

If you would like to request a paid digital marketing promotion in paid search, paid social, paid sponsorships or other paid marketing to support your event, content marketing, or webcast, asset, etc. create an issue in the [Digital Marketing Programs Repo](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/issues) and use the [`mktg-promotion-template`](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/blob/master/.gitlab/issue_templates/mktg-promotion-template.md)

If you request a digital marketing promotion you probably also need a marketing campaign and should consult with the [Marketing Program Managers](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/).

## Requesting LinkedIn Inmail as part of campaign

LinkedIn Inmail campaigns are a good way to reach people at specific companies, industries, and more. They work best for inviting people to events and webinars if you do not have specific people in mind (unlike a Marketo campaign). If you would like to request an Inmail campaign as part of your marketing campaign, create an issue in the [Digital Marketing Programs Repo](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/issues) and use the [`linked-inmail`](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/blob/master/.gitlab/issue_templates/linkedin-inmail.md) template.

## Create a Culture of Testing and Optimization

### Conversion Rate Optimization (CRO)

A process of collecting and analyzing data, formulating hypotheses, and conducting experiments to increase the percentage of website visitors that convert into leads or potential customers. Testing and experiments generally occur on website pages that include desired actions such as watching a product demo, signing up for a newsletter, or signing up for a free product trial. This also extends to email recipients in email marketing wherein the recipient responds to the main call-to-action (CTA) of an email, driving additional traffic to the website, and converting into a new customer or upsell a current customer.

**Goals**

1. Understand what’s working and what’s not
1. Gain business insight
1. Improve customer experience

### Statistical significance

In order to draw accurate conclusions from a test, a large data set (sample size, time) is required. Customer behavior is not always consistent and responses fluctuate between times, offerings, and segments (e.g. device type, location, new vs. returning visitors). Other considerations include seasonality, competitor landscape, and industry evolution.

When analyzing results, it’s important to take different segments into account. Testing one element may reveal statistical significance in one area and affect another poorly. For example, an increase in conversions on the website via desktop could cause a decrease in conversions for mobile and vice versa. 

### Always be testing
In order to iteratively improve the site, we should test all major site changes before implementing. Testing requires a control and a variant within the same time period, while holding all other variables constant. Using a/b testing tools will allow us to create tests that follow testing best practices and gather data about what works or does not work to encourage people to spend time on our site or have a [conversion event](/handbook/business-ops/resources/#mql-scoring-model). With testing, we can make informed decisions about what works for our audience and helps them reach their goals, and what works for us to help use meet our business goals.

### Types of experiments

#### Website tests

* **A/B Test:** tests two variants of a page
* **A/B/n Test:** tests two or more variants of a page
* **Multivariate Test:** tests variants with two or more different sections
* **Redirect Test:** tests separate web pages identified by different URLs or paths
* **Personalization:** personalize your page for targeted visitors

#### Email A/B tests

**Body**
* Copy
* Images
* Layout

**Send Time**
* Time of day
* Day of week
* Personalized for each user

**Subject Line**
* Long
* Short
* Happy
* Serious
* Emojis

**Call-to-Action (CTA)**
* Button styling
* Copy

### CRO Process and Framework

Rather than simply testing ideas that we feel are relevant, we focus on building a solid hypothesis using data and information to ensure we are testing a hypothesis with the best chances of conversion. Theoretically, there are two approaches to building a hypothesis:

1. **Inductive approach:** Brainstorm a set of ideas and then look at the data to validate those ideas and form a hypothesis.
1. **Deductive approach:** Look at patterns in observations first, and then deducing a hypothesis for testing.

### Requesting a Website or Email Test

1. Build a test: If you would like to request an a/b or multivariate test, create an issue for [Digital Marketing Programs using this template](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/issues/new?issuable_template=ab-test).
1. CRO process and MVCs: Not all changes to pages need to be tested, only pages that we want to optimize for [conversion activities](/handbook/business-ops/resources/#mql-scoring-model). These pages/elements are often being tested:
    * [Homepage](/)
    * Top navigation
    * [Pricing page](/pricing/)
    * [Free trial](/free-trial/)
    * [Contact sales](/sales/)
1. Please check the [A/B and CRO issue board](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/boards/1086590?&label_name[]=Conversion%20Optimization&label_name[]=a%2Fb%20test) to see if a page you plan to update is being tested and also to see if a page you want to test is being tested or in plan to test. The URL will be the first word or `HP` for the homepage. If you have an MVC update to any of the pages in the `Doing` column, let us know in the `#digitalmarketing` Slack channel and we can scheduled tests around MVC updates or determine if updates can wait for tests to finish. Tests take 1 day to 4 weeks depending on traffic and conversion volume.

### Setting up a CRO test

We use [Google Optimize](https://optimize.google.com/optimize/home/#/accounts/4049624381/containers/9871021) to move and replace on-page elements for testing. If you need access to Optimize, please reach out to the Digital Marketing Programs team.

Google Optimize recommends using an anti-flicker snippet. Without this script installed, visitors may experience the page flickering and briefly see the original page before the test loads. This can skew the results of the test and confuse visitors. Tests can and will run without the anti-flicker snippet installed, but there is a chance it running without can impact visitor experience.

To install the anti-flicker script, add `google_optimize: true` to pages with active tests.

There's an `Active tests` section in CODEOWNERS for about.gitlab.com to notifiy the DMP team when changes are made to pages with active tests.

### Active Experiments

### Requesting a Hotjar heatmap test or report

[Use this link](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/issues/new?issuable_template=hotjar-heatmap-request) to request a heatmap test or results for a page on `about.gitlab.com`.

New heatmaps will record data until the page has reached 2,000 pageviews. A digital marketing program manager will ping you when the results are complete (Duration depends on average traffic to the page. Some tests can take up to a month or more.)

**Note:** Every page viewed by a visitor is counted as a single pageview.

## Links on about.gitlab.com

We should link to resources that will help our readers. Be sure to include links to blog posts, guides, and other reference material. You can also include links to company or product websites if they are relevant to your topic. These links do not need to be "nofollowed" if they are informational.

However, we should use [Google's guidelines on nofollowing links](https://webmasters.googleblog.com/2016/03/best-practices-for-bloggers-reviewing.html) when we exchange a link for a product or service. It's also a best practice to ask for a nofollow link when we sponsor and disclose our links to sponsored content.

## UTMs for URL tagging and tracking
All URLs that are promoted on external sites and through email must use UTM URL tagging to increase the data cleanliness in Google Analytics and ensure marketing campaigns are correctly attributed. 

We don't use UTMs for internal links. UTM data sets attribution for visitors, so if we use UTMs on internal links it resets everything when the clicked URL loads. This breaks reporting for paid advertising and organic visitors.

You can access our internal [URL tagging tool in Google Sheets](https://docs.google.com/spreadsheets/d/12jm8q13e3-JNDbJ5-DBJbSAGprLamrilWIBka875gDI/edit#gid=0). You will also find details in this spreadsheet on what "Campaign Medium" to use for each URL. If you need a new campaign medium, please check with the Digital Marketing Programs team as new mediums will not automatically be attributed correctly.

If you are not sure if a link needs a UTM, please speak with the marketer who is managing your campaign to ensure you are not interrupting the reporting structure they have in place.

UTM construction best practices:
- lowercase only, not camelcase
- alphanumeric characters only
- no spaces
- **Campaign Medium** covers general buckets like `paidsearch`, `social`, or `sponsorship` 
- **Campaign Source** names where the link lives. Examples include `ebook`, `twitter`, or `qrcode`
- **Campaign Name** describes a specific campaign. Try to add additional context like `reinvent`, `forrester`, and `bugbounty`
- **Campaign Content** differentiates ad types.
- **Campaign Term** identifies keywords used in a campaign

## Website Health Check

Regular website health checks should be performed. These checks are meant to ensure that there are no issues with the website that could cause issues with traffic to the site. These are the following things to check to ensure the health of the site:

- [Google Search Console](https://www.google.com/webmasters/tools/)
- [Google Analytics](https://analytics.google.com/analytics/web/)

Issues to look for in each of these tools:

- **Google Search Console**: Check the dashboard and messages for any important notifications regarding the website. Also check under `Search Traffic` > `Manual Actions` for any URLs that have been identified as spam or harmful content. Forward security warnings to the Abuse team and follow the [DMCA complaint process](/handbook/support/workflows/dmca.html) with the support team.
- **Google Analytics**: Compare organic site traffic from the most previous week compared to the previous week and look for any large fluctuations.

## Using robots metadata to manage search index

There are times we need to keep pages out of search indexes. For example, we might duplicate most of a page to improve conversion for an ad campaign. It's relatively rare to use this, but it's an important tool that helps us increase organic reach and paid advertising efficiency.

All pages are set to `meta name="robots" content="index, follow"` by default. To exclude a page from the index add `noindex: true` to the frontmatter, and this will set the robots metadata to `meta name="robots" content="noindex, follow"`.

## about.gitlab.com redirects

Occasionally we need to change URL structures of the website, and we want to make sure that people can find pages they need. We use 301 redirects to send people to the right URL when it's appropriate. 

### about.gitlab.com redirect policy

We will redirect URLs included in Google's search index. A simple test to see if a page is indexed is to search for the URL with a site modifier, `site:url`, using Google.

It's a best practice to reduce the number of internal redirects as much possible, which means we need to try and update links across about.gitlab.com when we change URLs. When you request a redirect you can indicate whether or not you were able to search across about.gitlab.com and update the links for a page that moved.

### Request an about.gitlab.com redirect

The Digital Marketing Programs team can set up and manage all redirects for about.gitlab.com.

To redirect an outdated page, open an issue with the [set up a new redirect template in the Digital Marketing Programs project](https://gitlab.com/gitlab-com/marketing/digital-marketing-programs/issues/new?issuable_template=set-up-a-new-redirect). You'll need to provide the following:

- Old URL that needs to be redirected
- New URL where users should now be sent
- Were you able to update existing links to the old URL across about.gitlab.com?

If you have any questions or concerns regarding your redirect request, ask for help in the `#digital-marketing` channel on Slack.

### Redirect process documentation

The Digital Marketing Programs team uses these [technical details for the redirect process](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/doc/redirects_on_about_gitlab_com.md) on about.gitlab.com.

## GitLab Google Tag Manager system

We use Google Tag Manager(GTM) to simplify activity tracking on about.gitlab.com with Google Analytics. This documents the system the Digital Marketing Programs team uses with our Google Tag Manager container.

### Naming convention

We use semantic names for tags, triggers, and variables to make it simpler to determine what these components are supposed to do. Use an em dash (shift+option-_) to divide the components of each GTM component name.

Tags start with the platform, followed by the tag’s purpose, and are finally contextualized to about.gitlab.com. Any tags related to timed events need the timeframe indicated in a note attached to the tag in GTM to make it clear when to remove a tag.

#### Tag naming examples

- Google Analytics Event — Free Trial CTA click  
- Google Ads —  conversion tracker  
- Facebook — base pixel
- Drift — snippet v 0.3.1

Triggers start with a description of the action triggering a tag, followed by contextualization for about.gitlab.com.

#### Trigger naming examples

- Link click — Learn more 100M carousel  
- CTA click — cta-btn  
- Custom event — mktoformSubmit free trial  

Variables start with the tag or trigger they reference, followed by contextual data about their purpose.

#### Variable naming examples

- Google Analytics — GitLab Universal Analytics ID  
- dataLayer — postType custom dimension  

If you are making changes to the GTM container and have questions about what to name one of these components the Digital Marketing Programs team can help.

### dataLayer values

Today we’re using the dataLayer sparingly on about.gitlab.com, with our primary use focused on [differentiating blog content with `postType`](/handbook/marketing/blog/#definitions). We’ll expand how we use the dataLayer to create content groupings for improved customer journey insights and document those updates here.

### Event tags

We need consistent tags across Google Analytics events and have introduced the following structure to our event tags. Our goal is to cover important visitor events with the smallest number of tags in Google Tag Manager. Reducing the number of tags and the overall complexity of our Google Tag Manager container helps us spot and fix coverage issues faster.

![GitLab Google Tag Manager event structure](/images/handbook/marketing/GTM-event-structure.png)

These three components help us organize and identify specific event data. **Event Categories** help us group specific customer journey steps, **Event Actions** describe visitor interactions with about.gitlab.com, and **Event Labels** provide contextual details for reporting our performance.

**Example Event Label**  
{{Page URL}} | {{Referrer}} | {{Click text}} | {{Click URL}} | {{Click Class}}

Google Analytics limits event label fields to around 2000 characters, and we'll update the handbook if we start to see truncated event labels.

## Google Tag Manager inventory

We're using Simo Ahava's Googl Sheets Add-On to sync notes for our tags and create a [GitLab Google Tag Manager inventory](https://docs.google.com/spreadsheets/d/1oT5AQQ0nH4-7iS-QY-UJP4vbFxv2GCGy9XiKpj8ebuU/edit#gid=1443259273) This simplifies scanning and searching over the Google Tag Manager web app.

## Changes of note
Whenever we make major changes to tags through Google Tag Manager we document them in [changes of note](/handbook/marketing/revenue-marketing/digital-marketing-programs/digital-marketing-management/changes-of-note/). Examples of changes we document are adding or removing tags, changing tag sequencing, or changing when a tag is fired.

## Using marketing trend data

Search term volume is hard to estimate. Different tools use different methodolgies and models for reporting this data. AdWords provides data from Google, but the ranges are broad and terms can be combined into a single phrase. Google Trend data normalizes search trends from 1 to 100 based on the terms you're exploring, which doesn't give us any idea of how many people are using a particular phrase.

For our keyword research we rely on Moz Keyword Explorer data because it provides a narrower volume with full phrase integrity. When we report keyword volume, this is the tool we use for this data.

## Google Analytics Crash Course

### Dimensions vs Metrics

Dimensions are the different attributes of your data. For example, the landing page is a dimension that is the first page a person views when they come to the site.

Metrics are the numbers that are being measured, such as number of page views or number of sessions.

Each dimension and metric has a scope, so it’s important to understand the three different scopes:

1. User-level
1. Session-level
1. Page-level

Due to the scoping, not every dimension can be combined with every metric. In most cases, the dimensions and the metrics should match the scope.

### Understanding Reporting

#### Setting a date range

You can use the calendar in the top right to set the active date range. You can also select the `compare to` box to compare metrics from different time periods. This will allow you to see month over month or year over year growth for the desired metrics.

#### Annotations

Annotations are used to mark a point in time in Google Analytics. They can be used to mark an important event such as a change to the setup of Google Analytics, or an event that heavily impacted traffic positively or negatively.

To create an annotation, double-click on a date. The double-click will bring up the annotation field where you can enter details, and select `private` or `public`. Public annotations can be seen by anyone that has access to that view within Google Analytics, and private annotations can only be seen by you.

#### Data Tables

Most reports have a data table below the graph. The data tables contain a dimension and associated metrics.

The `Primary Dimension` of the data tables can be changed by selecting a different primary dimension from above the table.

A secondary dimension can also be added by clicking on the `Secondary Dimension` button above the table and selecting the secondary dimension you’d like to add to the table.

### Audience Reports

The audience reports are used to understand characteristics of your users such as location, and browser used, and user behavior over multiple visits such as average session time.

### Acquisition Reports

The acquisition reports help you know how people find the website. These reports will help you to analyze the benefits of the different digital marketing efforts that you are involved in.

#### Channels Report

The `All Traffic > Channels` report breaks down all the different channels that are sending traffic to the site. You can click on any of the channels to drill down  and get more granular data about that specific channel. For example, if you click on the `Referral` channel, you will see which sites are referring traffic to your site.

### Behaviors Reports

The behaviors section is about how users use the website. This includes what pages of the site people are looking at as well as how they flow through the site.

#### All Pages Report

The `All Pages` report shows the number of times a given page was viewed within the selected period of time. You can change the primary dimension to `Page Title` if it is easier to tell what the page is by looking at the title rather than the URL.

`Avg. Time on Page` and `Bounce Rate` can be used to find underperforming content or content that is very engaging to users and can be used in future marketing efforts.

#### Landing Pages and Exit Pages

The `Landing Pages` and `Exit Pages` reports are scoped at the session and tell us how many people are beginning a session at a certain page (landing page) and how many people are ending a session at a certain page (exit page).

These reports can be valuable to see what content is bringing people to the site and what content is causing people to leave the site.

#### Events

Events can be set up to track actions that people take on the website, such as clicking links or selecting drop downs. These events can be set up in Google Tag Manager and for the most part won’t require any additional code to be placed on the website.
