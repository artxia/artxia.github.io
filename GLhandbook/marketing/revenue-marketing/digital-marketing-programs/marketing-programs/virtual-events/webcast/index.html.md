---
layout: markdown_page
title: "Webcast"
---

## Hosted demand gen webcast

This section focuses on best practices, timelines and logistical set up on GitLab hosted demand gen webcast.

### Project Planning

Once the speakers and webcast dates are secured, the webcast project is officially in motion. The marketing programs team will immediately:

1. Create the necessary epic and MPM support issues as [outlined here](/handbook/marketing/revenue-marketing/digital-marketing-programs/marketing-programs/virtual-events/#below-is-a-step-by-step-guide-on-how-to-request-marketing-programs-support-for-a-virtual-event). 
2. Send over a Gcal invite for the webcast and dry run to the webcast execution team.
3. Clone and fill out [this GANTT/Webcast planning doc](https://docs.google.com/spreadsheets/d/1VTrWNX9qfY99b2TnrX93P39aXiRoNnChB6tduTvmysA/edit#gid=1899924336). *Note: If the webcast falls within the scope of an integrated campaign then you will want to fill out the webcast GANTT tab within the larger integrated campaign GANTT doc. Otherwise, if the webcast falls outside the scope of an intergated campaign then create a new GANTT/Webcast planning doc by cloning the template.*

Due dates for each action item and DRIs are outlined on the GANTT/Webcast planning template.

**Webcast project planning overview**
<iframe width="560" height="315" src="https://www.youtube.com/embed/0brFyfvRvLo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Best Practices

1. Give yourself at least 30 business days of promotion.
2. Send invitation emails 2 weeks out, 1 week out, and if needed 2 hours before event. Sample emails can be found here.
3. Only send promotional emails Tuesday, Wednesday, or Thursday for optimal results.
4. Send reminder emails to registrants the day before, and one hour before the event.
5. Host webcasts on a Wednesday or Thursday, see note below about scheduling.
6. Post links to additional, related resources during the event.
7. Include "contact us" information and a clear CTA at the end of the presentation.
8. Video recording of webcast uploaded to YouTube within 24 hours as event occurred.
9. Send the recording to all registrants, whether they attended or not within 48 hours post webcast.

### Speaker Approval

Marketing Programs sometimes depend on GitLab's subject matter experts to deliver webcast presentations. However, we must ensure that when we ask a speaker to participate on a webcast that the work is approved. Please use the following guideline when asking a subject matter expert to participate on a webcast.
1. Have a high-level abstract of the content prepared before asking for a presenter.
2. Send the abstract to both the proposed speaker and their manager to review. A speaker is not considered booked unless they have approval from their manager.
3. Address and resolve any concerns regarding the abstract.
4. Once the manager approves and the speaker accepts, you can move forward with the webcast.

#### Tips for Speakers

Here are some basic tips to help ensure that you have a good experience preparing for and presenting on a webcast.

##### Before Committing
{:.no_toc}
Ask us any questions you have about the time commitment etc. and what exactly our expectations are. Talk about it with your manager if you're on the fence about your availability, bandwidth, or interest. Make sure you're both on the same page. We want this to be a meaningful professional development exercise for you, not a favor to us that you're lukewarm about — if you feel that way, none of will be able to do our best job. We'll be honest with you, so please do the same for us.

##### Before the Dry Run
{:.no_toc}
Select and set up your presentation space. Pick a spot with good wifi, and we recommend setting up an external mic for better audio quality, although this is optional. If you will be presenting from your home, alert your spouse/roommates of the time/date & ask them to be out of the house if necessary. Depending on your preferences and comfort level with public speaking, run through the script several times.

##### Before the Presentation
{:.no_toc}
Try to get a good sleep the night before, and, if the presentation is in the morning, wake up early enough to run through your notes at least once. Review our [Positioning FAQ](/handbook/positioning-faq/), or keep the page handy in case you are asked in the Q&A about how GitLab compares to our competitors.

### Logistical Set up 

#### LIVE webcast registration and tracking

##### Step 1: Create the landing page

1.  Navigate to:  [www-gitlab-com/data/webcast.yml](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/data/webcasts.yml)
2.  Click edit, copy the following code, and paste to the top of the page

```
- url: firstwordinwebcasttitle-secondwordinwebcasttitle (e.g:debunking-serverless)
  title: `Add title from copy doc`
  subtitle: `Add subtitle from copy doc`
  date: `Add webcast Month DD, H:MM am/pm PT/ H:MM am/pm UTC`
  form: 1592
  success_message: "Thank you for registering. You will receive an email with additional webcast details."
  image: `Add header image url in the following format [/images/icons/imagename.svg]`
  description: "Add a sentence to describe what the webcast is about at a high-level."
  content: |

    `Add P1 from copy doc while making sure you keep the indentation the same`
    
   `Add P1 from copy doc while making sure you keep the indentation the same`


    ### In this webcast, we'll cover:
    * `Add bullet 1`
    * `Add bullet 2`
    * `Add bullet 3`

```
3. Add commit message to name your Merge request using syntax Add [webcast name] landing page (i.e. Add Debunking Serverless security myths webcast landing page).
4. Create a name for the target branch - NEVER leave it as the master (i.e. 20191030-Debunking-WC-LP).
5. On the next screen (New Merge Request), add WIP: to the beginning of the title and add a quick description (Add LP for [webcast name] will suffice).
6. Assign to Jackie Gragnola and scroll down, check the box for `Delete source branch when merge request is accepted`.
7. Click Submit Merge Request.
8. You’ve now created the merge request.

**Creating a new landing page in the webcast yml.**
<iframe width="560" height="315" src="https://www.youtube.com/embed/UxaNIHfAY18" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


##### Step 2: Add the webcast to the /events page
*  To add the webcast to the /events page follow this [step by step guide](/handbook/marketing/events/#how-to-add-events-to-aboutgitlabcomevents).

##### Step 3: Configure Zoom

*Note: The webcasts@ zoom license can only be used for a single session at a time. This license is used for all internally hosted webcasts. Therefore, when a webcast is requested please confirm there is not going to be a conflict between the pre-scheduled sessions using that license by checking this virtual events gcal. Schedule no less than 30min between sessions (before & after) so there is less chance of a conflict and allows for a buffer.*

1. Log in to Zoom,  go to the Webinars tab then click “Schedule a webinar”.
2. Fill out the topic as follows “Webcast title - Month DD, YYYY - HH:MM am/pm PT/HH:MM am/pm UTC” (for example: Debunking Serverless security myths - October 21, 2019 - 8:30 am PT/3:30 pm UTC).
3. Fill out the description with a sentence to describe what the webcast is about at a high-level.
4. Make sure to select “TEMPLATE” in the use a template section.
5. For  WHEN fill out the webcast date and time.
6. For Duration, fill out how long the webcast will be.
7. Make sure you select the correct TIMEZONE.
8. Do not change all the other settings that are prepopulated by the template.
9. Add marketing programs DRI, internal speaker(s), and Q&A resource as alternative hosts.
10. Add external Gitlab speakers as panelists by following the video instructions below. 

**Adding alt-host and panelist to a webcast**
<iframe width="560" height="315" src="https://www.youtube.com/embed/4YvV8AoyqXc?rel=0&amp;controls=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

11. If applicable, edit the confirmation and reminder emails under the email setting tab.
    * Make sure the registration confirmation email and the reminder emails are set to send from Zoom. As Zoom implements their more robust Marketo integration, we will send from Marketo, but for now we need to send from Zoom to ensure that the correct unique link is sent to registrants.
    * There is limited editing capabilities within Zoom. In the confirmation email you can add a snippet of text after the templatized body text and the footer of the email can be edited. In the reminder email, only the footer can be edited.
12. Click on branding and update the header (optional).
13. If applicable, add polling questions to the webcast  by following the instructions in the video below.

**Adding poll questions to a webcast**
<iframe width="560" height="315" src="https://www.youtube.com/embed/QIrRcUIYEwo?rel=0&amp;controls=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

14. Makes sure the Marketo smart campaigns outlined in the documentation below are set up before proceeding to the next step.
15. Set up Marketo integration within Zoom by clicking on the Integration tab.
   *  Click Edit next to Generate Leads in Marketo section.
   *  Check  Send registration information to a Smart Campaign and select the Registered From Zoom smart campaign that you set up in marketo for this webcast.
   *  Check  Send attendee information to a Smart Campaign and select the Zoom Attended smart campaign hat you set up in marketo for this webcast.
   *  In the `Gather other information to Marketo (optional)` section, select the ZoomWebinarOtherInfo custom object, check the following boxes, and select the corresponding Marketo Custom Object Fields:
      * Webinar ID
      * Webinar Topic
      * Q&A
      * Poll

##### Step 4: Set up the webcast program in Marketo and SFDC

1. Create the webcast program in Marketo by cloning the YYYYMMDD_WebcastTopic_Region (Single time slot) template.
    * Select clone to `A campaign folder`.
    * Title the webcast in the following format: YYYYMMDD_{Webcast Title}_[Region - only if applicable]. For example, 20170418_MovingToGit.
    * Save to the `GitLab Hosted` folder.
    * Click salesforce campaign sync and select create new to create campaign in SFDC. Make sure to put the landing page url and also the link to the epic in the description.

2. Update `My Tokens` at the webcast program level.
   * DO NOT UPDATE THE `apiKey` or `apiSecret`. These should be the same for every webcast.
   * Update the `{{my.email header alt}}` token with the webcast title.
   * Update the `{{my.email header image url}}` with the  image url in marketo design studio.
   * Update the `{{my.landingPageUrl}}` token with the webcast landing page url.
   * Update the `{{my.utm}}` token by appending the program name to the utm campaign token.
   * Skip updating the `{{my.ondemandUrl}}` token for now (until the LIVE webcast has been completed).
   * Update the `{{my.webcastTitle}}` token with the webcast title.
   * Update the `{{my.zoomWebinarId}}` token with the webinar ID from the Zoom webcast created in step 1.

3. Turn on smart campaigns in Marketo.
  * Activate the `Attended` campaign.
  * Within the `Registration from Landing Page` smart campaign, on the `Fills out Form` trigger, add the webcast landing page url without the https (e.g: about.gitlab.com/webcast/securing-serverless/), then activate the campaign.
  * Activate the `Registered From Zoom` campaign.

4. Go to the campaign in salesforce.
  * Change the campaign owner to your name.
  * Change the status to `in progress`.
  * Edit the Bizible touchpoint field to `Include only "Responded" Campaign Members`.

5. Submit a test lead using your gitlab email on the LIVE landing page to make sure the registartion is tracked appropriately in the Marketo program and you get a confirmation email from zoom.

#### Webcast invitation

1. Update emails `invitation 1 - 2 weeks prior`,  `invitation 2 - 1 week prior` , and if needed `invitation 3 - 1 week prior` with relevant copies related to the webcast. *Note: We normally use the same copy for all 3 emails and simply tweaked the templated subject lines to sound more like “Reminders”.*
2. If you previously updated the `{{my.email header alt}}`, `{{my.email header image url}}`, `{{my.landingPageUrl}}`, and `{{my.webcastTitle}}` tokens on the program level as outlined in the event set up documentation, the email header,  CTA, and Subject line should auto-populate with the correct landing page URL and the webcast title.
3. Approve copy and send samples to Sarah Daily from digital marketing programs, the requestor, and the presenter (if different from requestor).
4. Go to the List folder and edit the `Similar past programs list` smart list and input the names of past similar programs and applicable program statuses to the `Member of program` filter. This will make sure people that have attended programs with similar topics in the past are included in the invite.
5. Go to the  `One time - Marketing invited status` smart campaign and click run once.
6. Once you get approval on the sample email copy, and step 5 has finished running, schedule the email programs outlined in step 1.

#### Post LIVE webcast

##### Sending follow up emails

1. Go to the `No shows` smart campaign and click run once to make sure the no shows get dispositioned into the correct status. Currently, no integrated exists between zoom and Marketo to automatically disposition no shows so they remain in `Registered` status until you run this smart campaign.
2. Update email `Outbound -attendees` and email `Outbound -no shows` with content with relevant copies related to the webcast.
3. On the Follow-up - Attendees and Follow up - No Shows email programs, update the `{{my.CTA..}}` tokens to point to the correct offers and use them in the hyperlinks.
4. Approve copy and send samples to Sarah Daily from digital marketing programs, the requestor, and the presenter (if different from requestor).
5. Once you get approval for the sample copy, schedule email sends within follow-up no show and follow-up attended email programs. 
 
##### Converting the webcast to an On-Demand gated asset

1. Upload the recording to our main GitLab channel, fill in the title with the webcast title, and fill in the description with a short paragraph of what the webcast is about. Make sure the video set as `Unlisted` so only people with the URL to the video can find it.
2. Once the recording has been uploaded,  click the video link on the right to navigate to the final youtube page for the webcast. 
3. Click share and click embed to get the embed url for the video (e.g: https://www.youtube.com/embed/sLB1xggtdHg).
4. Navigate to:  www-gitlab-com/data/ webcast.yml.
5. Click edit and add the following code snippet `youtube_url: [insert your youtube embed url]`under the `url` code snippet for your landing page.
6. Change the `form:` to `2076`.
7. Add commit message to name your Merge request using syntax  `Add youtube video for [webcast name] landing page` (e.g. `Add youtube video for Debunking Serverless security myths webcast landing page`).
8. Create a name for the target branch - NEVER leave it as the master (i.e. `20191130-Debunking-WC-LP`).
9. On the next screen (New Merge Request), add `WIP:` to the beginning of the title and add a quick description (`Add youtube recording to LP for [webcast name] will suffice`).
10. Assign to Jackie Gragnola and scroll down, check the box for `Delete source branch when merge request is accepted`.
11. Click Submit Merge Request.
12. You’ve now created the merge request.
13. Add the regular youtube link (non embed) to the `Pathfactory_request` issue (created during Epic creation) so the DMP team can generate the PathFactory link for this.
14. Once you get the PathFactory link from DMP, log into Marketo, go to the webcast program and update the `{{my.ondemandUrl}}` token with the PathFactory link.
15. Go to the assets folder within your webcast program and update the `On-demand Autoresponder` email with relevant copies related to the webcast. 
16. Navigate to the `Viewed On Demand` Smart campaign within your webcast program.
17. Modify the webpage link with the webcast landing page url without the https (e.g: `about.gitlab.com/webcast/securing-serverless/`), then activate the `Viewed On Demand` smart campaign.
18. Deactivate the `Attended` ,`Registration from Landing Page`, and `Registered From Zoom campaign` within your webcast program.

<iframe width="560" height="315" src="https://www.youtube.com/embed/KLfO9j_U1mo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

