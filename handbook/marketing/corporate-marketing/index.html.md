---
layout: handbook-page-toc
title: "Corporate Marketing"
---

## Welcome to the Corporate Marketing Handbook
{:.no_toc}

The Corporate Marketing team includes Content Marketing, Corporate Events, PR (Public Relations), All-Remote Marketing, and Design. Corporate Marketing is responsible for the stewardship of the GitLab brand and the company's messaging/positioning. The team is the owner of the Marketing website and oversees the website strategy. Corporate Marketing develops a global, integrated communication strategy, executes globally, and enables field marketing to adapt and apply global strategy regionally by localizing and verticalizing campaigns for in-region execution. Corporate marketing also ensures product marketing, outreach, and marketing & sales development are conducted in a way that amplifies our global brand.
{: .note}

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Brand personality

GitLab's brand has a personality that is reflected in everything we do. It doesn't matter if we are hosting a fancy dinner with fortune 500 CIOs, at a hackathon, or telling our story on about.gitlab.com...across all our communication methods, and all our audiences, GitLab has a personality that shows up in how we communicate.

Our personality is built around four main characteristics.

1. Human: We write like we talk. We avoid buzzwords and jargon, and instead communicate simply, clearly, and sincerely. We treat people with kindness.
1. Competent: We are highly accomplished, and we communicate with conviction. We are efficient at everything we do.
1. Quirky: We embrace diversity of opinion. We embrace new ideas based on their merit, even if they defy commonly held norms.
1. Humble: We care about helping those around us achieve great things more than we care about our personal accomplishments.

These four characteristics work together to form a personality that is authentic to GitLab team-members, community, and relatable to our audience. If we were `quirky` without being `human` we could come across as eccentric. If we were `competent` without being `humble` we could come across as arrogant.

GitLab has a [higher purpose](/company/strategy/#mission). We want to inspire a sense of adventure in those around us so that they join us in contributing to making that mission a reality.

## Tone of voice


The following guide outlines the set of standards used for all written company
communications to ensure consistency in voice, style, and personality, across all
of GitLab's public communications.

See [the Blog Editorial Style Guide](/handbook/marketing/corporate-marketing/content/editorial-team/#blog-style-guide) for more.

### About

#### GitLab the community

GitLab is an [open source project](https://gitlab.com/gitlab-org/gitlab-ce/)
with a large community of contributors. Over 2,000 people worldwide have
contributed to GitLab's source code.

#### GitLab the company

GitLab Inc. is a company based on the GitLab open source project. GitLab Inc. is
an active participant in our community (see our [stewardship of GitLab CE](/company/stewardship/)
for more information), as well as offering GitLab, a product (see below).

#### GitLab the product

GitLab is a complete DevOps platform, delivered as a single application. See the
[product elevator pitch](/handbook/marketing/product-marketing/messaging/)
for additional messaging.

### Tone of voice

The tone of voice we use when speaking as GitLab should always be informed by
our [Content Strategy](https://gitlab.com/gitlab-com/marketing/blob/master/content/content-strategy.md#strategy).
Most importantly, we see our audience as co-conspirators, working together to
define and create the next generation of software development practices. The below
table should help to clarify further:


<table class="tg">
  <tr>
    <th class="tg-yw4l">We are:</th>
    <th class="tg-yw4l">We aren't:</th>
  </tr>
  <tr>
    <td class="tg-yw4l">Equals in our community</td>
    <td class="tg-yw4l">Superior</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Knowledgeable</td>
    <td class="tg-yw4l">Know-it-alls</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Empathetic</td>
    <td class="tg-yw4l">Patronizing</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Straightforward</td>
    <td class="tg-yw4l">Verbose</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Irreverent</td>
    <td class="tg-yw4l">Disrespectful</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Playful</td>
    <td class="tg-yw4l">Jokey</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Helpful</td>
    <td class="tg-yw4l">Dictatorial</td>
  </tr>
  <tr>
    <td class="tg-yw4l">Transparent</td>
    <td class="tg-yw4l">Opaque</td>
  </tr>
</table>

We explain things in the simplest way possible, using plain, accessible language.

We keep a sense of humor about things, but don't make light of serious issues or
problems our users or customers face.

We use colloquialisms and slang, but sparingly (don't look like you're trying too hard!).

We use [inclusive, gender-neutral language](https://litreactor.com/columns/5-easy-ways-to-make-your-writing-gender-neutral).

## Updating the press page

### Adding a new press release
1. Create a new merge request and branch in www-gitlab-com.
1. On your branch, navigate to `source` then `press` and click on the [`releases` folder](https://gitlab.com/gitlab-com/www-gitlab-com/tree/master/source/press/releases).
1. Add a new file using the following format `YYYY-MM-DD-title-of-press-release.html.md`.
1. Add the following to the beginning of your document:

```
---
layout: markdown_page
title: "Title of press release"
---
```

5. Add the content of the press release to the file and save. Make sure to include any links. It is important to not have any extra spaces after sentences that end a paragraph or your pipeline will break. You must also not have extra empty lines at the end of your doc. So make sure to check that when copying and pasting a press release from a google doc.

### Updating the `/press/#press-releases` page

When you have added a press release, be sure to update the index page too so that it is linked to from [/press/#press-releases](/press/#press-releases).

1. On the same branch, navigate to `data` then to the [`press.yml` file](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/data/press.yml).
1. Scroll down to `press_releases:`, then scroll to the most recent dated press release.
1. Underneath, add another entry for your new press release using the same format as the others, ensuring that your alignment is correct and that dashes and words begin in the same columns.  
1. The URL for your press release will follow the format of your filename for it: `/press/releases/YYYY-MM-DD-title-of-press-release.html`.

### Updating the recent news section

1. Every Friday the PR agency will send a digest of top articles.
1. Product marketing will update the `Recent News` section with the most recent listed at the top. Display 10 articles at a time. To avoid formatting mistakes, copy and paste a previous entry on the page, and edit with the details of the new coverage. You may need to search online for a thumbnail to upload to `images/press`, if coverage from that publication is not already listed on the page. If you upload a new image, make sure to change the path listed next to `image_tag`.

----

## Design

### Requesting design help

1. Create an issue in the corresponding project repository.
    1. For tasks pertaining to [about.gitlab.com](/) create an issue in the [www-gitlab-com project](https://gitlab.com/gitlab-com/www-gitlab-com/issues).
    1. For all other marketing related tasks create an issue in the [corporate marketing project](https://gitlab.com/gitlab-com/marketing/corporate-marketing/issues).
1. Add all relevant details, goal(s), purpose, resources, and links in the issue description. Also `@` mention team members who will be involved.
1. Set due date (if possible) — please leave at least 2 week lead time in order to generate custom design assets. If you need them sooner, ping @luke in the #marketing-design Slack channel and we will make our best effort to accommodate, but can't promise delivery.
1. Add the `Design` and `Website Redesign` (if applicable) label(s) to your issue.

#### The `Design` label in issue tracker

The `Design` label helps us find and track issues relevant to the Design team. If you create an issue where Design is the primary focus, please use this label.

#### Project prioritization

Per the Design team's discretion, the prioritization of design projects will be based on the direct impact on Marketing.

To get a better sense of [corporate marketing project](https://gitlab.com/gitlab-com/marketing/corporate-marketing/issues) prioritization, you can view the [Design Issue Board](https://gitlab.com/gitlab-com/marketing/corporate-marketing/boards/913023?&label_name[]=Design).

Design projects within the [www-gitlab-com project](https://gitlab.com/gitlab-com/www-gitlab-com/issues) can be tracked using the [Website](https://gitlab.com/gitlab-com/www-gitlab-com/issues?scope=all&utf8=%E2%9C%93&state=opened&label_name[]=Website) label. The prioritization of projects for [about.gitlab.com](/) can be viewed on the [Website Issue Board](https://gitlab.com/gitlab-com/www-gitlab-com/boards/349137?milestone_title=No+Milestone&).

Any design requests that do not fall in line with the goals and objectives of Marketing will be given a lower priority and factored in as time allows.

#### Team logo request guidelines

As the company continues to grow, incoming requests for internal team logos are increasing at a rate that is not scalable for the Brand Design team. We understand the desire for teams within GitLab to have their own identity, so we've created these guidelines to help direct your request:

* Teams can create their own logos that are for internal (non-public) use only.
* If you believe a public-facing team logo would be valuable to our business, please submit a [design request issue](https://gitlab.com/gitlab-com/marketing/corporate-marketing/issues) outlining how it will be used, who will see it, and it's perceived value. Logos will be created and approved on a case-by-case basis to capitalize on brand opportunities and ensure brand integrity.

### Design touchpoints

The Design team has a rather wide reach and plays a big part in almost all marketing efforts. Design touchpoints range from the [GitLab website](/) to print collateral, swag, and business cards. This includes, but certainly not limited to:

#### Web & Digital
{:.no_toc}
- Redesign, updates, and maintenance of the [GitLab website](/)
- Blog post covers & images
- Landing pages (campaigns, webcasts, events, and feature marketing)
- Swag shop (shop design and new swag)
- Presentation decks & assets
- Ad campaigns
- Email template design

#### Field Design & Branding
{:.no_toc}
- Marketing Design System
- Conference booth design
- Banners & signage
- Swag
- Event-specific slide decks
- Event-specific branding (e.g. GitLab World Tour, Team Summits, etc.)
- Business cards
- One-pagers, handouts, and other print collateral
- GitLab [Brand Guidelines](#brand-guidelines)

#### Content Design
{:.no_toc}
- Promotional videos & animations
- Social media campaign assets
- Webcast collateral & assets
- eBooks
- Whitepapers
- Infographics & diagrams

*In the spirit of 'everyone can contribute' (as well as version control and SEO) we prefer webpages over PDFs. We will implement a `print.css` component to these webpages so that print PDFs can still be utilized for events and in-person meetings without the headache of version control*

## Brand Guidelines

To download the GitLab logo (in various formats and file types) check out our [Press page](/press/).

### The GitLab logo

The GitLab logo consists of two components, the icon (the tanuki) and the wordmark:

![GitLab logo](/images/handbook/marketing/corporate-marketing/design/gitlab-lockup.png){: .small.left}

GitLab is most commonly represented by the logo, and in some cases, the icon alone. GitLab is rarely represented by the wordmark alone as we'd like to build brand recognition of the icon alone (e.g. the Nike swoosh), and doing so by pairing it with the GitLab wordmark.

#### Logo safe space

Safe space acts as a buffer between the logo or icon and other visual components, including text. this space is the minimum distance needed and is equal to the x-height of the GitLab wordmark:

![Logo x-height](/images/handbook/marketing/corporate-marketing/design/x-height.png){: .medium.left}

![Logo safe space](/images/handbook/marketing/corporate-marketing/design/logo-safe-space.png){: .small.left}

![Icon safe space](/images/handbook/marketing/corporate-marketing/design/icon-safe-space.png){: .small.left}

The x-height also determines the proper spacing between icon and wordmark, as well as, the correct scale of the icon relative to the wordmark:

![Stacked logo safe space](/images/handbook/marketing/corporate-marketing/design/stacked-logo-safe-space.png){: .small.left}

#### Minimum logo size

Here are the recommended minimum sizes at which the logo may be reproduced. For legibility reasons, we ask that you stick to these dimensions:

##### Logo

![Horizontal logo minimum size](/images/handbook/marketing/corporate-marketing/design/logo-min-size.png){: .small.left}

- Digital: 100px wide
- Print: 1.25in (31.75mm) wide

##### Stacked logo

![Stacked logo minimum size](/images/handbook/marketing/corporate-marketing/design/logo-stacked-min-size.png){: .small.left}

- Digital: 60px wide
- Print: 0.75in (19mm) wide

##### Icon

![Icon minimum size](/images/handbook/marketing/corporate-marketing/design/icon-min-size.png){: .small.left}

- Digital: 30px wide
- Print: 0.50in (13mm) wide


### The Tanuki

The [tanuki](https://en.wikipedia.org/wiki/Japanese_raccoon_dog) is a very smart animal that works together in a group to achieve a common goal. We feel this symbolism embodies GitLab's [mission](/company/strategy/#mission) that everyone can contribute, our [values](/handbook/values/), and our [open source stewardship](/company/stewardship/).

### GitLab trademark & logo guidelines

GitLab is a registered trademark of GitLab, Inc. You are welcome to use the GitLab trademark and logo, subject to the terms of the [Creative Commons Attribution Non-Commercial ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). The most current version of the GitLab logo can be found on our [Press page](/press/).

Under the Creative Commons license, you may use the GitLab trademark and logo so long as you give attribution to GitLab and provide a link to the license. If you make any changes to the logo, you must state so, along with the attribution, and distribute under the same license.

Your use of the GitLab trademark and logo:

- May not be for commercial purposes;
- May not suggest or imply that you or your use of the GitLab trademark or logo is endorsed by GitLab, or create confusion as to whether or not you or your use of the GitLab trademark or logo is endorsed by GitLab; and
- May not suggest or imply or that you are affiliated with GitLab in any way, or create confusion as to whether or not you are affiliated with GitLab in any way.

Examples of improper use of the GitLab trademark and logo:

- The GitLab name may not be used in any root URL, including subdomains such as `gitlab.company.com` or `gitlab.citool.io`.
- The GitLab trademark and/or logo may not be used as the primary or prominent feature on any non-GitLab materials.

### Using other logos

Logos used on the about.gitlab.com site should always be in full color and be used to the specifications provided by the owner of that logo, which can usually be found on the owners website. The trust marks component found throughout the site is the only exception and should use a neutral tone:

<img src="/images/handbook/marketing/corporate-marketing/design/trust-marks.png" class="full-width">

The tanuki logo should also not have facial features (eyes, ears, nose...); it is meant to be kept neutral, but it can be accessorized.

### Colors

While the brand is ever-evolving, the GitLab brand currently consists of six primary colors that are used in a wide array of marketing materials.

##### Hex/RGB

![GitLab Hex/RGB Colors](/images/handbook/marketing/corporate-marketing/design/gitlab-hex-rgb-colors.png)

### Typography

The GitLab brand uses the Source Sans Pro font family. Headers (h1, h2, etc.) always have a weight of 600 (unless used in special situations like large, custom quotes) and the body text always has a weight of 400. Headers should not be given custom classes, they should be used as tags and tags alone (h1, h2, etc.) and their sizes or weights should not be changed, unless rare circumstances occur. Here are typography tags.

`H1: Header Level 1`

`H2: Header Level 2`

`H3: Header Level 3`

`H4: Header Level 4`

`p: Body text`

### Buttons

Buttons are an important facet to any design system. Buttons define a call to action that lead people somewhere else, related to adjacent content. Here are buttons and their classes that should be used throughout the marketing website:

**Note**: Text within buttons should be concise, containing no more than 4 words, and should not contain bold text. This is to keep things simple, straightforward, and limits confusion as to where the button takes you.

#### Primary buttons

Primary buttons are solid and should be the default buttons used. Depending on the color scheme of the content, purple or orange solid buttons can be used depending on the background color of the content. These primary buttons should be used on white or lighter gray backgrounds or any background that has a high contrast with the button color. They should also be a `%a` tag so it can be linked elsewhere and for accessibility. Buttons should also be given the class `margin-top20` if the button lacks space between itself and the content above.

<div class="flex-container flex-column flex-start margin-bottom20">
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn orange margin-top20">Primary Button 1</a>
  <pre class="highlight shell">.btn.cta-btn.orange</pre>
  <p>OR</p>
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn purple">Primary Button 2</a>
  <pre class="highlight shell">.btn.cta-btn.purple</pre>
</div>

#### Secondary Buttons

There will be times when two buttons are needed. This will be in places such as [our jobs page](/jobs/), where we have a button to view opportunities and one to view our culture video. In this example, both buttons are solid, but one is considered the primary button (orange), and the other is the secondary button (white). The CSS class for the solid white button is <br> `.btn.cta-btn.btn-white`.

<img src="/images/handbook/marketing/corporate-marketing/design/jobs-buttons-example.png" class="full-width">

This is the proper use of two buttons, both being solid, but different colors based on hierarchy. If the background is white or a lighter color that doesn't contrast well with a white-backgound button, a ghost button should be used as a secondary button, and should match in color to the primary button beside it as shown below:

<div class="buttons-container flex-start">
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn orange margin-top20">Primary Button</a>
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn ghost-orange margin-top20">Secondary Button</a>
</div>

<div class="buttons-container flex-start margin-bottom20">
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn purple margin-top20">Primary Button</a>
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn ghost-purple margin-top20">Secondary Button</a>
</div>

DO NOT: Do not use these ghost buttons styles as standalone buttons. They have been proven to be less effective than solid buttons [in a number of studies](https://conversionxl.com/blog/ghost-buttons/). They should only be used as a secondary button, next to a solid primary button that already exists. Here are the classes for the secondary buttons:

<div class="flex-container flex-column flex-start margin-bottom20">
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn ghost-orange margin-top20">Secondary Button 1</a>
  <pre class="highlight shell">.btn.cta-btn.ghost-orange</pre>
  <a href="/handbook/marketing/corporate-marketing/#primary-buttons" class="btn cta-btn ghost-purple">Secondary Button 2</a>
  <pre class="highlight shell">.btn.cta-btn.ghost-purple</pre>
</div>

### Iconography

Icons are a valuable visual component to the GitLab brand; contributing to the overall visual language and user experience of a webpage, advertisement, or slide deck. The GitLab iconography currently consists of "label icons" and "content icons", each are explained in further detail below:

#### Label icons

Label icons are intended to support usability and interaction. These are found in interactive elements of the website such as navigation and [toggles](/pricing/).

![Label icons example](/images/handbook/marketing/corporate-marketing/design/label-icons-example.png){: .medium.center}

#### Content icons

Content icons are intended to provide visual context and support to content on a webpage; these icons also have a direct correlation to our illustration style with the use of bold outlines and fill colors.

A few examples include our [event landing pages](/events/aws-reinvent/) and [Resources page](/resources/).

<img src="/images/handbook/marketing/corporate-marketing/design/content-icons-example.png" class="full-width">

### Brand oversight

Occasionally the [old GitLab logo](* https://gitlab.com/gitlab-com/gitlab-artwork/blob/master/_archive/logo/fox.png) is still in use on partner websites, diagrams or images, and within our own documentation. If you come across our old logo in use, please bring it to our attention by creating an issue in the [Marketing](https://gitlab.com/gitlab-com/marketing/general/issues) issue tracker. Please include a link and screenshot (if possible) in the description of the issue and we will follow-up to get it updated. Thanks for contributing to our brand integrity!

### [GitLab Product UX Guide](https://docs.gitlab.com/ee/development/ux_guide/)

The goal of this guide is to provide written standards, principles and in-depth information to design beautiful and effective GitLab features. This is a living document and will be updated and expanded as we iterate.

## GitLab Design System

We've broken out the GitLab interface into a set of atomic pieces to form our design system, [Pajamas](https://design.gitlab.com/). Pajamas includes information such as our principles, components, usage guidelines, research methodologies, and more.

## Brand resources

- [GitLab icons](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/gitlab-brand-files/gitlab-logo) (web RGB & print CMYK)
- [GitLab logos](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/gitlab-brand-files/gitlab-wordmark) (web RGB & print CMYK)
- Print-ready [event one-pagers](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/print/event-one-pagers)
- Color palette and Typography can be found in the [Brand Guidelines](#brand-guidelines)
- [Authorized Reseller GitLab Virtuoso Badge](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/gitlab-brand-files/authorized-resellers/gitlab-virtuoso-badge)

### Asset libraries

#### Icons

- [Line icons](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/presentation-decks/_general-assets/icons/line-icons) (.png)
- [Line icons](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/_resources/icons/svg) (.svg)
- [Icon illustrations](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/presentation-decks/_general-assets/icons/illustrated-icons) (.png)
- [Software Development Lifecycle](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/gitlab-brand-files/software-development-lifecycle/complete-lifecycle-icons/png)

#### Icon patterns

- [GitLab icon pattern](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/gitlab-brand-files/illustrations/icon-pattern)

#### Social media

- [Profile assets](https://gitlab.com/gitlab-com/marketing/general/tree/master/design/social-media/profile-assets/png/assets)

### Templates

#### Issue templates

To work more efficiently as an [asynchronous](/company/culture/all-remote/asynchronous/) team, everything should [begin](/handbook/communication/#everything-starts-with-a-merge-request) in an issue or merge request as opposed to Slack or email.

Creating an issue may seem like an added burden, but the long-term benefit of having [context](/company/culture/all-remote/effective-communication/#understanding-low-context-communication) around a given piece of work prevents [knowledge gaps](https://about.gitlab.com/company/culture/all-remote/asynchronous/#plugging-the-knowledge-leak) from occurring. Issue templates exist to make the process of creating issues easier. If you find yourself starting similar issues over and over, look through existing issue templates. If a suitable one does not exist, consider creating one in the appropriate repository.

For more on how to make beautiful templates, check out GitLab's [Markdown Guide](https://about.gitlab.com/handbook/engineering/ux/technical-writing/markdown-guide/). To add an emoji in an issue, begin by typing `:` and the title of the emoji. A list of emoji markup is [here](https://gist.github.com/rxaviers/7360908).

Remember to always add `Related Issues` and `Epics` after you've created your issue so others have context on what issues connect to this work.

- Visit the [Corporate Marketing Issue Template Repository](https://gitlab.com/gitlab-com/marketing/corporate-marketing/-/tree/master/.gitlab/issue_templates) to view all available issue templates. You'll find templates covering [Corporate Events](https://gitlab.com/gitlab-com/marketing/corporate-marketing/-/blob/master/.gitlab/issue_templates/Corporate-Event-Request.md), [Bulk Swag Requests](https://gitlab.com/gitlab-com/marketing/corporate-marketing/-/blob/master/.gitlab/issue_templates/BulkSwagRequest.md), Social Requests for [Events](https://gitlab.com/gitlab-com/marketing/corporate-marketing/-/blob/master/.gitlab/issue_templates/social-event-request.md) and [General](https://gitlab.com/gitlab-com/marketing/corporate-marketing/-/blob/master/.gitlab/issue_templates/social-general-request.md), Video Requests, [Webpage Updates](https://gitlab.com/gitlab-com/marketing/corporate-marketing/-/blob/master/.gitlab/issue_templates/webpage-update.md), and more.
- If you're for a [general or universal issue template](https://gitlab.com/gitlab-com/marketing/corporate-marketing/-/blob/master/.gitlab/issue_templates/general-project-template.md) to begin tracking discussion and progress on any given piece of work, big or small, search for `general-project-template` in a newly-created [Corporate Marketing Issue](https://gitlab.com/gitlab-com/marketing/corporate-marketing/issues). This template is pre-populated and beautified with emojis and descriptors for common sub-sections such as `Background`, `Details and reach`, `Goals and key messages`, and `Due dates, DRI(s) and next steps/to-dos`.

#### Presentation decks

- [General GitLab deck template](https://docs.google.com/a/gitlab.com/presentation/d/16FZd01-zCj_1jApDQI7TzQMFnW2EGwtQoRuX82dkOVs/edit?usp=sharing)
- [Group Conversation template](https://docs.google.com/a/gitlab.com/presentation/d/1JYHRhLaO9fMy1Sfr1WDnCPGv6DrlohlpOzs48VvmlQw/edit?usp=sharing)
- [GitLab pitch deck template](https://docs.google.com/a/gitlab.com/presentation/d/1LC1lT-gxpl1oUZ2InX4Oni9T4MfR0DFF0RLi4uNxBBQ/edit?usp=sharing)

----

## Speakers

##### For GitLab Team-members Attending Events/ Speaking    

- If you are interested in finding out about speaking opportunities join the #cfp Slack channel. Deadlines for talks can be found in the Slack channel and in the master GitLab [events spreadsheet](https://docs.google.com/spreadsheets/d/16usWToIsD-loDQYpflaMiGTmERMYSieNj_QAuk5HBeY/edit#gid=1939281399).
- If you want help building out a talk, coming up with ideas for a speaking opportunity, or have a customer interested in speaking start an issue in the marketing project using the [CFP submissions template](https://gitlab.com/gitlab-com/marketing/corporate-marketing/issues/new?issuable_template=CFPsubmission) and tag any associated event issues. Complete as much info as possible and we will ping you with next steps. We are happy to help in anyway we can, including public speaking coaching, and building out slides.
- If there is an event you would like to attend, are attending, speaking, or have proposed a talk and you would like support from GitLab to attend this event the process goes as follows:
 1. Contact your manager for approval to attend/ speak.
 1. After getting approval from your manager to attend, [add your event/ talk](https://gitlab.com/gitlab-com/www-gitlab-com/-/blob/master/data/events.yml) to the [events page](/events/) and submit merge request to Emily Kyle.
 1. If your travel and expenses are not covered by the conference, GitLab will cover your expenses (transportation, meals and lodging for days said event takes place). If those expenses will exceed $500, please get approval from your manager. When booking your trip, use our travel portal, book early, and spend as if it is your own money. Note: Your travel and expenses will not be approved until your event / engagement has been added to the events page.
 1. If you are speaking please note your talk in the description when you add it to the Events Page.
 1. If you are not already on the [speakers page](/events/find-a-speaker/), please [add yourself](https://gitlab.com/gitlab-com/www-gitlab-com/-/blob/master/data/speakers.yml).
 1. We suggest bringing swag and/or stickers with you. See notes on #swag on this page for info on ordering event swag.

##### Finding and Suggesting Speakers and Submitting to CFPs   

- Speaker Portal: a catalogue of talks, speaker briefs and speakers can be found on our [Find a Speaker page](/events/find-a-speaker/). Feel free to add yourself to this page and submit a MR if you want to be in our speaker portal and are interested in being considered for any upcoming speaking opportunities.
- If you have a customer interested in speaking start an issue in the marketing project using the CFP submissions template and tag any associated event issues. Complete as much info as possible and we will ping you with next steps. We are happy to help in anyway we can, including public speaking coaching.

##### Best practices for public speaking

Below are some tips on being a better presenter. For an in-depth book that covers the entire speaking process, from submitting an abstract through preparing a structured talk to practicing and delivering read [Demystifying Public Speaking](https://abookapart.com/products/demystifying-public-speaking).

1. Use a problem/solution format to **tell a story**. Many talks, especially tech talks, talk about what they built first and then what the result was. Flip this around and [start with the why](https://www.ted.com/talks/simon_sinek_how_great_leaders_inspire_action). Why did you need to take the action that you did? Talking about what problems you were encountering creates a narrative tension and people will listen intently to the talk because they want to hear the solution.
1. **Drive towards an action**. Ask yourself, "What will people do once they hear this talk?" The answer can't be, "be more aware of this topic." By deciding what action you expect the audience to take you can build your talk to drive towards this action. Talks that motivate the audience to action are more engaging and memorable than talks that simply describe. Some good example answers are
   1. Contribute to an open source project.
   1. Implement the technology or process you've come up with
   1. Follow the best practices you've outlined
1. **Practice how you play**. Practicing your talk is key to being a great presenter. As much as possible, practice exactly how you plan to give the talk. Sand up and pretend you are on stage rather than sitting down. If you'll demo, build the demo first and practice the demo. Even practicing while wearing the outfit you plan to wear can help.
1. **Give concrete examples**. Real life details bring a talk to life. Examples help people to understand and internalize the concepts you present. For each of your points try to have a "for instance." As an example, "We recommend using this script to delete old logs and free up diskspace. For instance, one time our emails lit up as users were complaining about slow performance. Some were reporting tasks hanging for over an hour when they should have completed in less than a minute. It turned out we were out of diskspace because we had verbose logging enabled. Once we ran the script we saw performance return to normal levels."   
1. **Be mindful of your body language** when presenting as it will impact the way the audience perceives your presentation. Move around the stage purposefully (don't pace or fidget). Make natural gestures with your hands, and maintain good posture to convey confidence and openness which will help you to better connect with your audience.

### Customer Speakers

In an effort to grow our engagement and connectivity with our community, we're pleased to offer a SPIFF incentive for our Sales (Sal's, TAM's, SA's, Professional Services), and Support Teams teams to get customers involved in speaking at any GitLab Commit Event.

#### SPIFF criteria- only applicable for Commit our user conference series

##### The SPIFF will payout for each customer speaker submission that has the following criteria met

- Customer industry is financial services, banking, insurance, telecom, federal government agency, software, or embedded software.
- Customer market segment is large, strategic, or a startup in the top 500 ranking on [this list](https://www.startupranking.com/top/)
- The proposed talk is for one of our top Corporate or Field Events (AWS, KubeCon, DOES, Open Source Leadership Summit, please connect with [Technical Evangelism](/handbook/marketing/technical-evangelism/) for others that might apply)
- Customer CFP must be submitted before CFP closes and be reviewed by someone on the [Technical Evangelism](/handbook/marketing/technical-evangelism/) team before being submitted.
- Speaker title must be director or above, and/or be a subject matter expert in their field and on the topic in question.

##### Eligibility

- SAL, AM, AE, TAM, SA, and Support team members are eligible.

##### Payout

- If the above criteria is met the payout will be $500 upon submission of the CFP.
- We will pay out an additional $500 upon acceptance of talk.

For ideas to help customers get their submissions accepted, see [How to Get Your Presentation Accepted (video)](https://www.youtube.com/watch?v=wGDCavOCnA4) or schedule a chat with a [Technical Evangelism](/handbook/marketing/technical-evangelism/) team member.

----

## Corporate Events

### Mission Statement
* The mission of the Corporate Events Team is to:
    * Showcase the value and strengths of GitLab on all fronts
    * Deliver creative solutions to problems
    * Provide exceptional service
    * Build lasting and trusting vendor and internal relationships
    * Treat everyone like they are our most valued customer, including fellow GitLab team-members

### What does the corporate Events team handle?
  * **Sponsored events** (events with 5000+ attendees for NA, 3000+ for other territories and that also have a global audience (50% or more of audience is national or global). There are some exceptions. There are handful smaller events that we handle due to the nature of the audience, and the awareness and thought leadership positions we are trying to build out as a company). The primary goal is always driving brand awareness but that cannot be the only result.
  * **Owned events**
     * [GitLab Commit](/events/commit/), our User Conference
  * **Internal events** (Contribute-sized events)
      * [GitLab Contribute](/events/gitlab-contribute/), our internal company and core community event
      * We also serve as DRI for all internal Sales events- [SKO's](/events/sko21/), Force Management planning, Rewards Travel, SQS, QBR's. Must be above 25 people attending for corp events involvement.
Please review our events decision tree to ensure Corporate Marketing is the appropriate owner for an event. If it is not clear who should own an event based on the [decision tree](https://docs.google.com/spreadsheets/d/1aWsmsksPfOlX1t6TeqPkh5EQXergt7qjHAjGTxU27as/edit?usp=sharing), please email events@gitlab.com.

### Corporate Events Strategy / Goals
  * **Brand**
    *  For Sponsored Events: Get the GitLab brand in front of 15% of the event audience. 40,000 person event we would hope to get 4,000+ leads (10%) and 5% general awareness and visibility with additional branding and activities surrounding participation.
    *  Human touches- Tracked by leads collected, social interactions, number of opportunities created, referrals, current customers met, and quality time spent on each interaction.
    *  Audience Minimum Requirements- volume, relevance (our buyer persona, thought leaders, contributors), reach (thought leaders?), and duration of user/ buyer journey considered.
  * **ROI**
    * Work closely with demand gen campaigns and field marketing to ensure events are driving results and touching the right audience.
    * Exceed minimum threshold of ROI for any events that also have a demand gen or field component- 5 to 1 pipe to spend within a 1-year horizon.
    * Aim to keep the cost per lead for a live event around $100.
    * [ROI Calculator](https://docs.google.com/spreadsheets/d/1SAYGXysUHGXPKrTDFf9yRcQrh9TYNxR9_Ts6H9dq8JY/edit?usp=sharing) we aim to make 5x ROI on pipeline focused events but this can be used to estimate what return we might get on an event.
  * **Thought Leadership and Education**

### GitLab Commit User Conferences
  * [Link to 2019 Epic](https://gitlab.com/groups/gitlab-com/marketing/-/epics/84)
  * [Link to 2019 Enablement](https://gitlab.com/groups/gitlab-com/marketing/-/epics/259)
  * [Link to 2019 Slack Channel](https://gitlab.slack.com/messages/CK8HV2A10)
  * 2020 Updates Coming soon- [planning Epic](https://gitlab.com/groups/gitlab-com/marketing/-/epics/668)
  * Onsite at Commit for GitLabbers:
    * You will be assigend one or multiple onsite tasks. It is crititcal you show up for your set duty and communicate any changes in your plans. Clean your schedule on the day of the event, as it will be a full day commitment.
      * Tasks include:
         * Track Scanning- it is essential you show up and stay for this if you are assigned. Our partners have paid to get leads form thir talks and it is our promise to provide said leads. All talk attendees must be scanned for this purpose.
         * Check in Support
         * Swag table
         * Questions/ help desk
         * Booth Duty (Hiring, UX, Support, Security, Demo) - do not leave the booth unstaffed. We have back up. Ask for helpo on coverage if you need it.
    * Dress code: casual to business casual. Wear what you feel comfortable in. No open toed shoes for safety reasons.
    * Team Travel
      * Team members may come in the day before the event and stay the night of the event. No additional days will be covered unless you have arranged a special circumstance with the Commit planning team.
      * We can only provide Visa support for speakers and extrenal attendees for this event series.
      * If you live within 60 miles of the event you will be asked to commute to the event unless you have a specific arrangement with tehe Commit planning team.

<figure>
  <iframe src="https://calendar.google.com/calendar/b/1/embed?height=600&amp;wkst=1&amp;bgcolor=%23ffffff&amp;ctz=UTC&amp;src=Z2l0bGFiLmNvbV9sbzZ0dm92Nmhtdm50NTYybGlwYWVnbGJ2b0Bncm91cC5jYWxlbmRhci5nb29nbGUuY29t&amp;color=%23009688&amp;showPrint=0" style="border-width:0" width="800" height="600" frameborder="0" scrolling="no"></iframe>
</figure>


### Event Execution
For event execution instructions, please see the [Marketing Events page](/handbook/marketing/events/#event-execution) for detail instruction and the criteria used to determine what type of events are supported.




### Best Practices on site at a GitLab event
  * [Employee Booth Guidelines](/handbook/marketing/events/#employee-booth-guidelines)
  * [Scanning Best Practices](/handbook/marketing/events/#scanning-best-practices)


---
## Swag

### Swag for Events - [see details on Events page](/handbook/marketing/events/#swag)

All swag requests, creation and vendor selection is handled by the Corporate Marketing team.  
- We aim to have our swag delight and/or be useful. We want to create swag that is versatile, easy to store and transport.
- As a remote company with team members in over 50 countries - our swag often has to go on miraculous journeys.
- With this in mind we try to ship things that are durable, light and that will unlikely get stuck in customs.
- We strive to make small batch, limited edition and themed swag for the community to collect.
- Larger corporate events will have custom tanuki stickers in small runs, only available at the specific event.
- Region specific sticker designs are produced quarterly.
- Our goal is to do swag in a way that doesn't take a lot of time to execute -> self-serve => [web shop](https://gitlab.myshopify.com/)


### Community & External Swag Requests
If you would like to get some GitLab swag for your team or event, email your request to `sponsorships@gitlab.com` (managed by the [community advocacy team](/handbook/marketing/community-relations/community-advocacy/#expertises)).     
In your request include:
- expected number of guests
- best shipping address
- phone number
- type of swag you are hoping for  


The swag we have available can be found on our online store. **Note**: It is recommended submit your request for swag at least **4 weeks in advance** from the event date or we may not be able to accommodate your request.

### Internal GitLab Swag Ordering:
* Event Swag (for FM and community): To request GitLab swag for an event you are attending see instructions below.
  * The event must be 3 or more weeks away for all swag and material requests. Rush shipping is not an option.
  * NORAM Field marketing and Community Relations should email our contact at Nadel for event swag shipments. Let them know what you want, when and where you need it. They will send your parcel with a return shipping label to get any remaining items shipped back to their warehouse. We have a list of approved items with Nadel you can order from. Any new items must be approved by brand team for brand consistency - Nadel will email all final designs to brand team for approval.
  * Not in Field Marketing or Community Relations? You can place small event swag orders by emailing `sponsorships@gitlab.com`. Include the date needed, shipping address and items / volume desired. The request will be approved on the back end by the community team. All requests must be made 3 or more weeks out. You can expect a response within 5 business days.
  * Paper/Print Collateral: In order to be [efficient](/handbook/values/#efficiency), we do not make custom print assets for events. We avoiod printed materials because they are instantly out of date and to help support the efforts to reduce waste.
  * We have an event kit with a [banner and table cloth](/images/events/GitLabPopupBoothMarch2019.pdf). Contact `events@gitlab.com` if you would like to borrow this setup. You will be shipped this set along with a return label.
  * For larger swag orders (stickers in a quantity of 100 or greater), do not go through the swag store but rather use our [Stickermule](https://www.stickermule.com/) account or ping `dsumenkovic@gitlab.com`. Include address, date needed and order quantity in request.
  * If you have any issues with your order please email `events@gitlab.com` with your concerns.
* GitLab team-member Swag - if you would like to order something from the GitLab swag shop we have a discount code you can use for 30% off (found in the channel description). Please see the swag Slack channel to get code to be used in the [store](https://shop.gitlab.com/) at checkout.
* We have specific shirts available for customer meetings. If you feel you need one of these shirts please email `events@gitlab.com`.

### Returning Swag to Warehouse
* If you have items that need to be returned to the warehouse please contact `events@gitlab.com` or find the FexEx account number in 1password to create a return label. Returns are only recommended if you have a very large number of items (50+) or a booth setup (banner, tablecloth, backdrop) that need to be returned.

### Swag for customer/ prospects
 * Anyone can request to send swag to customers, prospects, candidates, partners by following the process outlined for external [Swag Requests](/handbook/marketing/community-relations/community-advocacy/workflows/merchandise-handling/#swag-requests).
 * Questions about the order process should be posted in the #swag Slack channel. A Corporate or Community Relations team member will reply within 24-48 business hours.  
 * If you have questions on what is appropriate to send review [sending swag to customers parameters](https://gitlab.com/gitlab-com/sales/issues/144).
 * SA's, TAM's, and AE's should coordinate with their SDR to send swag to customers.
 * Each SDR with an account has a set budget of $50 to spend on sending swag and gift cards monthly. Mid market and SMB reps have $100.
 * All sends are tracked in SFDC, in either the physical or coffee swag campaign.
 * Orders placed for customers via the Printfection link are subject to change based on inventory availability and cost.

* We have GitLab stationary/ note cards- leave note in swag Slack channel of you would like a batch to send notes to use to send to prospects/ customers/ community members.

* *NOTE:* Please keep in mind the [list of countries we do not do business in](/handbook/sales/#export-control-classification-and-countries-we-do-not-do-business-in).

### Swag Providers We Use
* See [issue](https://gitlab.com/gitlab-com/marketing/general/issues/1554) for vendors we use and what we order from them.
* Please direct swag vendor suggestions to the `#swag` Slack channel.

### New and Replenishment Swag Orders
Corporate handles the creating and ordering of all new swag. All swag designs should be run past design (Luke) for approval before going to production.
* If you need swag for an upcoming event complete the swag selection of the event template and corporate will be in touch on issue to complete request. Note: at least 6 weeks to produce anything new and 2-3 weeks to reorder current designs.
* Triggers are setup in Sendoso to remind our account admins when balances and swag inventory is low. No need to ping anyone if you see inventory is low.
* Reordering of inventory for internal swag requests is done by corporate team. See section above on swag providers we use for items not produced by Sendoso.

### Suggesting new items or designs
* You can suggest new designs in the swag Slack channel or more formally in an issue in the [swag project](https://gitlab.com/gitlab-com/swag_suggestions).

---

## Social Marketing and Social Media

Please consult the [Social Marketing Handbook](/handbook/marketing/corporate-marketing/social-marketing/).

## All-Remote Marketing

### Mission Statement

The mission of GitLab’s [All-Remote Marketing](/job-families/marketing/all-remote-marketing/) team is to champion the company’s [all-remote culture](/company/culture/all-remote/) and initiatives. This involves close collaboration with corporate marketing (PR, corporate events), people group ([employment branding](/handbook/people-group/employment-branding/)) and [Diversity & Inclusion](/company/culture/inclusion/).

### Our audience

The audience we aim to reach with our all-remote initiatives is both internal and external to GitLab. It closely aligns with our employment branding audience, and expands to cover key segments in the investor and business communities.

  * Venture capitalists
  * Entrepreneurs
  * Business founders
  * Talent, recruiting, and HR leads
  * Media (business, lifestyle, workplace, finance)
  * Educators and researchers
  * GitLab team members
  * Job candidates and future team members
  * The broader GitLab community
  * People interested in remote work

### Objectives and goals

As detailed in GitLab’s public [CMO OKRs](/company/okrs/), GitLab’s All-Remote Marketing team seeks to elevate the profile of GitLab in the media and investor circles, positioning it as a pioneer of remote work. It will spread the story of GitLab’s global remote employees, remote work processes, transparent culture and the movement to remote work that GitLab has created. It also seeks to position GitLab as an innovator in the eyes of investors, a vital part of GitLab’s [public ambition to become a public company](/company/strategy/).

  * Leverage events to generate business interest and media coverage on GitLab’s all-remote culture
  * Form and foster relationships with other remote companies, creating unity in ramping up mentions and credibility for remote work
  * Position GitLab CEO Sid Sijbrandij as a thought leader in the space, utilizing [interviews, livestreams, podcasts and panels](/company/culture/all-remote/resources/#videos-podcasts-interviews-presentations) to raise visibility
  * Attract new [candidates](/jobs/) that embrace geographic diversity and place a high degree of value on an all-remote culture
  * Maintain and evolve an [all-remote web destination](/company/culture/all-remote/) focused on GitLab’s leadership in remote work culture in the context of the broader movement
  * Work with GitLab team members around the globe, as well as external remote advocates, to highlight remote culture [stories](/company/culture/all-remote/stories/)
  * Employ an ethnographic storytelling approach to document and share authentic, credible stories from the movement offering insights that can be applied to solve problems throughout the organization and also adopted by others outside of GitLab
  * Position GitLab (the product) as a key enabler of remote work
  * Develop strategy for mentoring, advising and consulting within the startup community to foster the creation of more all-remote companies
  * Leverage partners and friendlies in the all-remote space to cross-promote and amplify GitLab’s all-remote messaging across events, web and social media

### Channels for culture curation

#### Web

The team's primary home for publishing informational guides and content is the [all-remote section of GitLab's handbook](/company/culture/all-remote/). This will be the preeminent home to all-remote content, positioned for consumption by media, investors, prospective customers and candidates.  

We are actively working on a GitLab template for GitLab team members to submit stories, photos, videos, etc. for inclusion in the aforementioned web destination. We will spotlight stories unique to GitLab's all-remote culture. Examples include:
  * *How remote work has changed my life*
  * *How security is handled in an all-remote environment*
  * *A year in the life of a digital nomad*
  * *Meetups, hiking, and outings amongst traveling GitLab team members*
  * *Health, budget, and community service impacts of working at GitLab*
  * *Home office arrangements from GitLab team members*

In the interim, GitLab team members wishing to share their remote stories can reach out to [@dmurph](https://gitlab.com/dmurph).

#### Events

All-remote events should elevate GitLab as a thought leader in the remote work space, create new partnerships, generate leads and generate media interest/coverage. We will consider physical events, virtual events and events that combine an in-person presence with a livestream option.

#### Social media

We incorporate all-remote content on GitLab’s [social media](/handbook/marketing/corporate-marketing/social-marketing/) accounts, and are investigating a visual approach to new mediums that are aligned with culture and lifestyle stories.

We are working with employment branding to surface relevant all-remote stories from GitLab team members to recruiting channels and review sites, such as Glassdoor, LinkedIn and Comparably.

There are also a number of videos on GitLab's [YouTube channel](https://www.youtube.com/gitlab) that relate to working here:
- [GitLab Unfiltered Remote Work playlist](https://www.youtube.com/playlist?list=PL05JrBw4t0Kq7QUX-Ux5fOunQotqJbECc)
- [Everyone can contribute](https://youtu.be/V2Z1h_2gLNU)
- [Working remotely at GitLab](https://youtu.be/NoFLJLJ7abE)
- [This is GitLab](https://youtu.be/Mkw1-Uc7V1k)
- [What is GitLab?](https://youtu.be/MqL6BMOySIQ)

## PR (Public Relations)

### Mission Statement
The mission of GitLab’s PR (public relations) team is to amplify GitLab's product, people and partner integrations in the media.

### Our audience
The audience we aim to reach is external press/media. This includes business, lifestyle, workplace, finance, and beyond, using mediums such as print, digital, video, events, podcasts, etc.

### Objectives and goals

As detailed in GitLab’s public [CMO OKRs](/company/okrs/), GitLab’s public relations team seeks to elevate the profile of GitLab in the media and investor circles, positioning it as a pioneer of remote work, increasing share of voice against competitors, and pulling through key messages in feature articles.

  * Leverage events to generate media interest in GitLab's people and products
  * Form and foster relationships with key reporters and publications
  * Position GitLab executives and subject matter experts as thought leaders in their areas of expertise
  * Increase GitLab's presence in media awards and accolades
  * Increase GitLab's contributed content
  * Work with social media team to cross-promote and amplify GitLab's media inclusions

### Contacting GitLab's PR team

For external parties, please visit our [Get In Touch page](/press/#get-in-touch).

For GitLab team members, please use the `#external-comms` Slack channel.

### PR Requests for Announcements:

If you would like to make a formalized announcement around a new product feature and capabilities, partner integration, significant milestone achieved, a new initiative, customer case study, inclusion in an analyst report, etc. through a press release or blog post, you can submit a request via an `announcement` issue template in the [Corporate Marketing project](https://gitlab.com/gitlab-com/marketing/corporate-marketing/issues). In the issue template, you will be able to provide additional information on the proposed announcement. As a general guide, below the team has outlined three levels for announcements based on the type of announcements and suggested communications activities associated with each tier. The PR team will assess your request in the issue and determine how to proceed.
If you are requesting a joint announcement and you are not part of the [Partner Marketing team](/handbook/marketing/product-marketing/partner-marketing/), please ensure you ping them on your issue.

* **Level 1** - A level 1 announcement will be announced via a press release and amplified with social media and an optional blog post. The execution of a blog post will be determined by the blog editorial team on a case by case basis. If the editorial team agrees to have a blog, then the social amplification will be the blog link as it includes assets that are helpful in the link cards across social channels. If there isn't an associated blog post, the social amplification can be for the press release link or relevant news coverage of the announcement. (In this case, the DRI needs to ensure there is an associated image to use with the release link or would make the decision of which news outlet link to select for social amplification.) Example announcements and news include but are not limited to: major GitLab company news around funding, earnings, executive new hires, analyst firm industry awards, acquisitions/mergers, Commit announcements, major joint partner news (ex. a partner such as AWS or Google) and major customer announcement (ex. enterprise or government agencies).

* **Level 2** - A level 2 announcement will be announced via a blog post and amplified with social media. The DRI/SME of the announcement will be responsible for working with the blog editorial team on creating the content and MR for the blog post (please see [the blog handbook](/handbook/marketing/blog/index.html#process-for-time-sensitive-posts) for more on this process). Example announcements and news include but are not limited to: partner integrations, new feature/capability highlights from the monthly release cycles (ex. Windows Shared Runners), customer case study announcement (not household names).

* **Level 3** - A level 3 announcement will be announced and promoted via GitLab’s social media channels. Example announcements and news include but are not limited to: awards from media publications (ex. DEVIES), speaking opps that GitLab employees are participating in (drive attendees/awareness) and ecosystem partner integrations. 

*Note: If you are seeking feedback from customers or our community on a proposed change, our recommendation is to do so using a public issue on GitLab. See [the blog handbook](/handbook/marketing/blog/#posting-to-solicit-feedback) for more information.*

### PR review and media guidelines

Speaking to media or on a podcast as a GitLab team member is a significant responsibility. If you are unsure whether or not you should accept a speaking opportunity or provide comment representing GitLab to a member of the media, please see below for guidance.

#### Speaking opportunities

If you are asked to speak on behalf of GitLab, consider reaching out to the PR and Technical Evangelist teams to ensure that the opportunity aligns with GitLab objectives. Inquiries should be initiated in the `#external-comms` Slack channel.

#### Media mentions and interviews

If you are asked to be quoted or to provide commentary on any matter as a spokesperson of GitLab, please provide detail of the opportunity to the PR team in the `#external-comms` Slack channel.

In the event that a media member, editor, or publisher offers a draft or preview of an article where you are quoted, please allow the PR team to review by posting in the `#external-comms` Slack channel. The PR team will ensure that the appropriate GitLab team member(s) review and approve in a timely manner.

#### Social media

Please consult the [Social Marketing Handbook](/handbook/marketing/corporate-marketing/social-marketing/). If you are contacted on a social media platform and asked to share/retweet or provide commentary as a spokesperson of GitLab, feel welcome to provide detail of the opportunity to the social team in the `#social-media` Slack channel.
