---
layout: handbook-page-toc
title: "Vacancies"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Introduction

For a listing of open vacancies, please see the [vacancies section on the Jobs page](/jobs/apply). Vacancies are maintained in Greenhouse based on our [job families](/handbook/hiring/job-families). A vacancy is a temporarily open position. A job family is a permanent description that also applies to existing people with that title. Don't use vacancy and job family interchangeably. The relevant parts of a job family are copy-pasted to Greenhouse to open a vacancy.

## Vacancy Creation Process

To create a vacancy, a Hiring Manager will work with their Recruiting Manager or Recruiting Lead, as outlined in the steps below. For simplicity, this person will be referred to as a Recruiting Manager throughout this process. To note, a vacancy can only be created by a Recruiting Manager before it can be submitted for approval in Greenhouse. This process enables us to ensure Greenhouse the single source of truth for hiring metrics.

### No Pooling Requirements within Greenhouse or Advertised 

We will only create vacancies that are in plan and for specific teams, this means that will not create vacancies for the sole purpose of pooling candidates in one place. 

### Adding Vacancies to the Hiring Plan

The hiring manager carries the responsibility to ensure vacancies in Greenhouse align to what is included in the rolling 4Q forecast. Therefore, the Hiring Manager, Finance, and Recruiting can stay in sync on what was planned and track towards those goals.

### Create or Review the Job Family

Once the vacancy is approved, the Hiring Manager will review the position description in the `/job-families` folder and update it, if needed, by making a merge request and assigning it to the Executive to review and merge. If there is no existing job family, follow the steps to [create a new job family](/handbook/hiring/job-families/#new-job-family-creation), then continue. Please note that new job families require approval from the CEO. The Recruiting Manager will use the relevant elements from this job family to open the vacancy in Greenhouse. The job family should include:

  - Responsibilities
  - Specialties (e.g. Gitaly, Backend)
  - Levels (e.g. intern, junior, senior, staff, manager)
  - Location (e.g. Anywhere, EMEA, Americas)
  - Requirements
  - Hiring Process, also update the internal [hiring process repo](https://gitlab.com/gitlab-com/people-ops/hiring-processes)

A compensation benchmark for the role should be set by working with the Compensation & Benefits team.

### Opening Vacancies in Greenhouse

For positions that are included in the Rolling 4 Quarter Forecast, the Recruiting Manager will create and open all approved vacancies simultaneously.

1. The Recruiting Manager will [log in](/handbook/hiring/greenhouse/#how-to-join-greenhouse) to [Greenhouse](https://gitlab.greenhouse.io/users/sign_in) and hover over the plus sign in the top right corner of their dashboard, and then click ["Create a Job"](https://app2.greenhouse.io/plans/new).

1. Click on ["Start from a copy of an existing job"](https://gitlab.greenhouse.io/get_started/show_existing_jobs). From there, you can choose to clone a vacancy, which is ideal if you are opening a vacancy that has been opened before, or something very similar has been opened before. If there is no close match, select `Any Status` at the top bar, select "Draft", and choose the template for the division. Please note: when creating a vacancy, the "Start from scratch" option should not be used, as important elements needed in a vacancy will not be included.

1. Once you've selected a vacancy to copy, the first screen will ask for **basic job info**.

1. The "Internal job name" is only viewable within Greenhouse, and the "External job name" is what appears on the jobs page. Enter in the vacancy name in these fields, including the specialty if applicable. These two fields should almost always be the same, but if you have questions on this, please reach out to the Compensation & Benefits team.

1. "Department" is the department this role will fall under. Always choose a department and **not** a division (e.g. for a Security Engineer vacancy, choose the "Security" department underneath the "Engineering" division, and do not choose "Engineering"). If you are unsure of what department to choose, reach out to the Compensation & Benefits team.

1. If a vacancy can be located anywhere where GitLab hires, check "Anywhere" next to "Office". If a vacancy is dedicated to a certain region or time zone, uncheck the "Anywhere" button and select any of the predetermined regions or time zones. If you need a region or time zone not represented in the list, please reach out to the recruiting operations team. In addition to the region or time zone you've selected, it's recommended to also choose "Remote" so that it's clear to applicants that the vacancy is both located in a particular area but also still remote.

1. Input the number of openings you want to hire for this role.

1. Click `Generate IDs` to create a requisition ID and opening IDs for your vacancies.

1. Under "Employment Type", select if your vacancy is a full-time, part-time, intern, or contract role. We strongly advise offering both full-time and part-time options for most of the vacancies. Please note: "contract" here refers to true independent contractors who work on short-term projects and is rarely used.

1. "Salary" can be found on the job family page for roles where the compensation calculator is public.
   - Take the `benchmark x level x 0.25` for the low end and `benchmark x level x 0.8` on the high end.
   - For roles not in the compensation calculator (Sales/Director/Exec): Leave blank if not known. The Compensation & Benefits team will edit as the first level of approval. The Compensation & Benefits Manager team will pull survey data in San Francisco for this role then apply the same formula for `0.25` on the low end and `0.8` on the high end. 

1. If this vacancy is eligible for a bonus, input the range of the bonus amount under the "Bonus" field. If there are no bonuses associated with this vacancy, enter zero, it is a required field.

1. If this vacancy is eligible for stock options, input the [range of offered stock options](/handbook/stock-options/) under the "Options" field. If you may be hiring various levels for this vacancy, input the range (e.g. if you may hire anywhere from Junior to Senior input a range), but if you only want to hire Seniors, then input the number of stock options associated with that level in both fields. If there are no stock options associated with this vacancy, enter zero.

1. Under "Type" choose if this is a new hire or a backfill.

1. Select if you'd like to be signed up for weekly recruiting emails or new candidate emails. You'll also be able to configure your notifications later, so don't worry if you're not sure yet.

1. On the right hand side, you'll be able to add optional background information for interviewers and advice on how to sell this vacancy. This is not required but gives great context for the interviewers and is recommended.

1. Click "Create Job & Continue".

1. The next page consists of all of the **attributes** interviewers will be evaluating for candidates in their scorecards across the full interview process. These may not be known until after the intake call. The attributes are typically split up into various categories, such "Requirements" (copied from the job family), "Responsibilities" (copied from the job family), "Skills", "Traits", and "Values" (standard across all roles, see additional info in the next step). 
   - These can be adjusted as needed, but **every** attribute listed should be a must-have and not a nice-to-have. 
   - If you want to include nice-to-haves in the scorecard, please create a new category called "Nice-to-haves" and add any applicable attributes there, making sure that your entire interview team knows that if a candidate does not meet any of those attributes it is not a negative against them.

1. To create a new category, scroll to the bottom of the screen and select "Add a Category", and add the name of the category. In the category you can add additional attributes.  

1. To remove a category, hover over the category, and click "Delete Category". 

1. The only required category is "Values", which should never be deleted. The values are listed in such a way to match how the values listed on our contracts.
   - Collaboration: Helping others, even when it is not immediately related to the goals that I am trying to achieve. Similarly, I will rely on others for help and advice.
   - Results: Doing what I promise for my fellow team members, our customers, our users, and our investors.
   - Efficiency: Caring about working on the right things, not doing more than needed, and not duplicating work. Dogfooding: Willingness to work with git and GitLab, using GitLab workflows within the team. (this attribute falls under the efficiency value and is called out separately, not as an additional value, but as an important key to success)
   - Diversity: Fostering an environment where everyone can thrive and feel included.
   - Iteration: Doing the smallest thing possible and get it out as quickly as possible.
   - Transparency: Being as open about as many things as possible.
   
1.  To edit the attributes within a category, click "Edit" next to the category. You can then change the name of attributes, delete attributes, add brand new ones, or choose existing attributes from other vacancies. Keeping the attribute names the same and choosing existing attributes from other vacancies is recommended so that the attribute choices remain streamlined. However, if you have a particular attribute for this role that needs to be evaluated, don't hesitate to add it. 

1. Click "Save" once you've configured your attributes and categories. If you don't want to save your changes after you've clicked "Edit" under a category, click "Cancel". 

1. Once the scorecard is finished, click "This looks good, NEXT" at the right of your screen.

1. The "Interview Plan", is where you'll craft the hiring process and scorecards for each step in the process.

1. Every vacancy should have an "Application Review" stage. Typically no edits are needed on this stage.

1. There is an optional stage called "Qualified" for those recruiters who would like to use it as a holding place before Screening. Especially with high-volume roles, this step can be used to sort through all the applications, mark the ones who meet the qualifications and want to reevaluate before the qualified pool before screening.

1. Some vacancies have an "Assessment" as the second stage in the process.
   - If your vacancy requires an assessment but there is no assessment stage already added, scroll to the bottom of the page and click "Add a Stage".
   - From there, you can either click "Copy from another job?" at the bottom of the pop-up and select a vacancy you know has an assessment. Click on "Assessment", then "Add."
   - If you're not sure of another vacancy that has an assessment, you can scroll to the bottom of the pre-populated list and select "Take Home Test", then "Add". 
   - Once added, hover over the new stage and click the pencil next to the stage name and change the text from `Take Home Test` to `Assessment`. Then hover over the second "Take Home Text" on the right of the stage and change the text again.
   - The assessment stage **must** be added using one of the two methods above, or it will not work properly. If you have any questions about this, please reach out to the recruiting operations team.
   - Once your assessment stage is created, or if it is already included, click "Edit" in the stage. You'll then want to select any attributes you want the grader of the assessment to focus on. This will typically be more technical in nature, but select whatever seems appropriate.
   - Scroll down to "Email to Candidate". This is where you'll include the actual assessment questions. The "From" should be `{{MY_EMAIL_ADDRESS}}` and "Subject" `GitLab Application - {{CANDIDATE_NAME}} - {{JOB_NAME}} Questionnaire`. In the Body, craft an email and insert your assessment questions. Below the body, make sure that the "link for candidates to submit tests" is **ON**. You can also add any attachments below that field if necessary.
   - Scroll down to "Grading Instructions" and include any specific items you want your graders to look out for when they review the candidates' answers. You can copy this section over from another job if applicable.
   - Under "Custom Questions", be sure that there is either a "Full Notes" custom question or that you add one. To add it, simply click "Add Custom Question", title it "Full Notes", choose "Text" as the answer type, and click "Add Custom Question". If there are any other specific questions you want your graders to answer when reviewing the assessment, feel free to add them here. They can be required or not, depending on your preference.
   - Under "Graders and Notifications", search for members of your team who can grade the assessments. You can select multiple people at this point, and when the assessments are actually sent out to candidates, each grader will appear and the person sending the assessment can delete extras so it is only sent to one person. You can also select who you want to be notified when the test is received; the test graders should absolutely be selected, and it's recommended for the recruiter to be notified as well. You can select any additional people to be notified as well if desired.
   - Finally, under "Additional Settings", check "This interview requires scorecards to be submitted" and leave unchecked "Hide candidate name and details from grader."
   - Then click "Save".

1. The next stage is the "Screening" call stage, which should be standard across the organization. Click "Edit" on this stage, scroll to the bottom, and choose the recruiter as the default interviewer and set interview duration to 30 minutes. It is important for this stage to be named the same across the organization for reporting purposes.

1. The next stage is "Team Interview", where the candidates will meet with peers and the hiring manager. Under this stage, you should see multiple interviews. They are typically called 1 - Hiring Manager, title (name), 2 - Peer Interview, title (name), 2 - Peer Interview, title (name)", etc. You can also add additional interviews such as 3 - Director Interview, title (name), 4 - Demo with Panel, titles (names), or other names that work for your interview plan.
   - The Team Interview stage should be laid out according to steps, indicated by the 1, 2, 3, etc. There can be more than 1 interview in a step to help speed up the interview process and reduce our apply to accept KPI. 
   - The interview plan should be defined during the intake call to include what attributes from the scorecard each interviewer is addressing as well as standard questions each interview should ask. 
   - The interview plan should be duplicated in the [hiring process repo](https://gitlab.com/gitlab-com/people-ops/hiring-processes). 
   - The interview plan should also be defined on the job family page under the Hiring Process section.

1. For each interview, click "Edit".
   - Select the appropriate attributes to focus on in that interview.
   - To the right of "Interview Prep", choose how long the interview should take (e.g. 30 minutes, 45 minutes, 50 minutes, etc.). 
   - Include the purpose of the call and questions the interviewer should ask. You can copy this over from another vacancy if applicable.
   - Under "Custom Questions", be sure that there is a "Full Notes" custom question in addition to the interview specific questions. 
   - To add additional questions, click "Add Custom Question", title it "Full Notes", choose "Text" as the answer type, and click "Add Custom Question". 
   - Choose default interviewers. If you have multiple team members that can interview, feel free to input all of their names, and the CES will choose one interviewer when scheduling the interview. This gives visibility to everyone who is trained and ready to perform interviews for this vacancy.
   - The two "Additional Settings" should both be checked.
   - Click "Save".

1. Some teams prefer to have the hiring manager stage broken out separate from "Team Interview" stage and in that case, a stage labeled "Hiring Manager Interview" should be added.

1. To add a new interview in a stage, hover over the stage and click "Add Interview", then you can copy over an interview from another job or create a new one. You can also move the interviews around within the stage and change the interview names.

1. The next stage (if applicable) is the "Executive Interview" stage. Depending on the level of the role the executive interviews may be conducted during the team interview stage. In this case, the executive interview section would be reserved for the CEO interview, if applicable. You can customize as needed following the guidelines for the team interview, including selecting attributes, adding custom questions, setting the interview length and selecting a default interviewer.

1. The next stage is "Reference Check", with at least three sections; a former manager and two former peers. These can be customized as needed. For executive-level roles, it is suggested you include the following; two former managers, two former peers, two former direct reports, and back-channel. The [background check](/handbook/people-group/code-of-conduct/#background-checks) is performed during the Reference Check stage.

1. There is an optional "Justification" section. This section should include three questions:
   - In what specific way(s) does this candidate make the team better?
   - What flags were raised during the interview process? 
   - How do we intend on setting this candidate for success?

1. The last stage is the "Offer" stage and cannot be edited or removed. Some important notes about the interview plan:
   - Every interview should be evaluating values add in the attributes section.
   - On occasion, there may be additional or fewer stages than represented here, but these stages should be consistent as much as possible in order to maintain data integrity for reporting. The interviews within the stages can be adjusted as needed.
   - If a candidate will have more interviews in a stage than predetermined, you can add additional interview events as long as the candidate is in the stage where you need to add the additional event.

1. Once your interview plan is complete, click "This looks good, NEXT" at the right.

1. The "Hiring Team" is where you select who will be working on this vacancy and what access they should have.
   - Scroll to the "Who's responsible for this job?" to assign the Hiring Managers, [Recruiter(s)]((https://about.gitlab.com/handbook/hiring/recruiting-alignment/), Coordinator(s) and Sourcer(s). If any of these are unknown leave blank. 
   - Scroll to the "Who can see this job?" section to set permissions to the team members who will need access. Search for someone's name click the pencil and select the correct access level from the drop-down.
   - Search for every person who will be in the hiring process, whether they will be grading assessment, reviewing new applications, or performing interviews.
   - You may need to go back to the interview plan to add the interviews if it did not let you add them before completing this step.

1. Click "This looks good, NEXT" at the right.

1. Approvals section is where you can add any notes here for the vacancy where it says "Leave a note". 
   - You must include the job family url to the Approval Note section.
   - If you were unable to determine the compensation information tag the Compensation and Benefits team in the Approval Notes section with an @ mention.

1. Scroll to the bottom of the page and click "Request Approval".

1. You'll be redirected to the vacancy in Greenhouse, where you can review the vacancy, make any changes, or make any updates. 
^

#### Intake Call

1. While pending [approval](/handbook/hiring/greenhouse/#approval-flows), the recruiter assigned to the req should contact the hiring manager to setup a REQ intake session. 

1. The REQ intake session should include the Recruiter, the Hiring Manager, the assigned Candidate Experience Specialist (optional) and Sourcer (optional). 

1. Ahead of the call, Recruiter must create a REQ Intake Issue by using the [REQ Intake Issue Template] (https://gitlab.com/gl-recruiting/req-intake/issues/new?issue%5Bassignee_id%5D=&issue%5Bmilestone_id%5D=). The Recruiter, Hiring Manager, CES, and Sourcer should all be added to the issue so they can contribute ahead of the REQ Intake Session.  

1. The Hiring Manager should come prepared to discuss the interview team, what is each interview assessing for so we can update/create the scorecard, time zone or location requirements (please note some of the job boards we post to requires a specific town even if the position can be located anywhere). The [REQ Intake Issue Template] (https://gitlab.com/gl-recruiting/req-intake/issues/new?issue%5Bassignee_id%5D=&issue%5Bmilestone_id%5D=) should be attached to the calendar invite so the hiring manager can fill out the form prior to the meeting.

1. When the REQ intake session is complete and the job is ready to be posted, the Recruiter notifies the assigned CES by an @ mention in the approval notes.

#### Publishing the Job

The [Candidate Experience Specialist](/job-families/people-ops/candidate-experience-specialist/) who is the coordinator for that vacancy should follow the below steps once they receive notice from the recruiter to post the new vacancy.

1. Go to the vacancy and under "Job Setup", review the configurations the Recruiting Manager has made and ensure everything is correct; reach out to them to ask clarifying questions if there is anything you don't understand or if there is anything missing.

1. The interview plan, scorecard(s), hiring team should be updated from the Intake Call notes. Each req is different on which stages are included and the order of those stages, however ensure each stage is labeled correctly for reporting purposes:
    - Application Review
    - Qualified
    - Screening
    - Assessment
    - Hiring Manager Interview
    - Team Interview
    - Technical Interview
    - Executive Interview
    - Justification
    - Reference Check
    - Background Check
    - Offer

1. Confirm each person in the hiring process has appropriate access and upgrade if necessary in [Greenhouse](/handbook/hiring/greenhouse/#how-to-upgrade-access-levels).

1. Confirm each interviewer has a personal Zoom link.

1. Confirm each interviewer is listed on the [Zoom Cheat Sheet](https://docs.google.com/spreadsheets/d/1D8praKd3Vc1gMTTUzONAGkqNKxyYHd3_nzqsq2OYjeA/edit?usp=sharing).

1. Confirm each interviewer has completed an [Interview Training Issue](https://gitlab.com/gitlab-com/people-ops/Training/issues/new).

1. The CES may choose to send the following email to each member of the interview team:

   Subject: Interview Training Issue, Zoom Personal Room and Google Office Hours

   Body: xxx, in order to have you scheduled for interviews I needed to create a zoom personal "room" for you. Please note this link can be joined by anyone at any time if they already have the link so it's a good idea to turn on the [waiting room function](https://support.zoom.us/hc/en-us/articles/115000332726-Waiting-Room?mobile_site=true#PMI). You can even customize the waiting room message with a GitLab logo and custom text! These steps are done in a web browser, not the app.

   Your personal zoom link: https://gitlab.zoom.us/my/gitlab.

   Also can you please make sure you have your office hours set up in your calendar? This will help me schedule the interview right the first time and save you and the candidate time and frustration. You can learn how [here](https://support.google.com/calendar/answer/7638168?hl=en).

   And one final thing, if this is your first time conducting interviews on behalf of GitLab I will need to create an interview training issue for you. Please let me know if that is the case. 

   As always, If you have any questions let me know! 
   Thanks, xxx

1. Confirm email notifications for the hiring team under "Job Setup".
   - Weekly Recruiting Report:
      - Hiring Manager
   - New Internal Applicants:
      - Hiring Manager
      - Recruiter
   - New Referrals:
      - Hiring Manager
      - Recruiter
   - New Agency Submissions:
      - Hiring Manager
      - Recruiter
   - Approved to Start Recruiting:
      - Hiring Manager 
      - Executive 
      - Recruiter
      - Sourcer
      - Candidate Experience Specialist
   - Offer Fully Approved:
      - Hiring Manager, 
      - Executive, 
      - Recruiter, 
      - Recruiting Managers, 
      - People Business Partner according to [business alignment](https://about.gitlab.com/handbook/people-group/how-to-reach-us/#people-business-partner-alignment-to-groups)
   - Stage Transitions:
      - Recruiter (all stages)
      - Candidate Experience Specialist (all stages)
      - Hiring Manager:
        -  Reference and Background Check 
        -  Justification 
        -  Offer 
   - New Scorecards:
      - Recruiter
      - Candidate Experience Specialist

1. Create or update the "Job Post" under "Job Setup", which will hold the vacancy description and application questions. Next to the name of the vacancy, click the pencil icon to edit the job post.
   - `Job Name`
   - `Post To` should always be `GitLab`.
   - `Location` always keep "Remote" listed in addition to any location requirement.
   - `Application Language` should always be `English`.
   - `Description` should be the copy/pasted from the job family on GitLab.com with the relevant information for the level/specialty/etc.
   - Be sure to add the Compensation section as a header and hyperlink the "view our handbook" to the correct job family link: 
   Compensation

   To view the full job description and its compensation calculator, view our handbook (insert job family url). The compensation calculator can be found towards the bottom of the page.

   Additional details about our process can be found on our [hiring page](/handbook/hiring/interviewing/).

1. If there are any links in the description, click on the link, then click the link icon in the text box toolbar, then change `Target` to `New Window`, then click "Ok" and repeat for any other links in the description; this will ensure all links work properly. 

1. To make sure this role is added to LinkedIn, you'll need to add a job wrapping code to the source code.
   - Click on the `< >` on the menu bar in the description text box to open the source code
   - Scroll to the bottom of the pop up
   - Paste the following text `<div><span style="font-size: xx-small;"><span style="color: white">Remote-Global</span></span></div>` at the bottom, and change the letters in `Remote-XXX` to the appropriate code for the current [available LinkedIn job wrapping locations](https://docs.google.com/spreadsheets/d/1JrKLyMlrNgUpNEvEolM1YwvUGY7qm-J_CmJhW8sIDDE/edit#gid=186847216) (ensure to copy exactly from the sheet as spaces matter). Default should be the Remote-Global tag.
   - Click "Ok"
  
  1. `Basic Application Questions`:
     - "Location" is **required**, and 
     - "Phone", "Resume", "Cover letter" are  optional. 
     - Almost always hide "Education", but discuss this with the Hiring Manager/Recruiter; if they want to include it, make sure it is **optional** and not required.
  
1. `Additional Questions` must include:
   - What's the name you'd prefer us to use throughout the interview process? - **Optional**
   - LinkedIn Profile - **Optional** (should link to the candidate's profile)
   - Please choose the country in which you are located. - **Required**
   - Are you legally eligible to work for GitLab where you are currently located? - **Required** (should link to the candidate's profile)
   - Were you referred by a current GitLab team-member? If so, please write their name below. - **Optional** (should link to the candidate's profile)
   - Are you subject to any employment agreements and/or post-employment restrictions with your current employer or a past employer? - **Required**
   -  What are your pronouns for others to use when referring to you? (ex: she/her, he/him, they/them, ze/zir/hir, etc.) **Optional**
   -  It is important to us to create an accessible and inclusive interview experience. Please let us know if there are any adjustments we can make to assist you during the hiring and interview process. **Optional**
   - Why did you decide to apply for a role at GitLab? - **Required** (should link to candidate's profile) 
  
1. You can add additional custom application questions as needed to help sort through required qualifications or to replace the information asked in the assessment stage. 

1. `Settings` 
   - Send Confirmation Email to Candidates: select the "Default Candidate Auto Reply" from the drop-down list
   - Application Confirmation Page: Default
   - Uncheck "Include Custom Demographic Questions"
   - Check "Include EEOC Questions"
   - Uncheck "Include 'Apply with SEEK' button"

1. Choose a city to index the vacancy on Glassdoor and Indeed. Please reference the [GitLab Country Guidelines](/jobs/faq/#country-hiring-guidelines) to ensure you are not posting to a location where we cannot hire. The location should have been identified by the Hiring Manager during the Intake Call.

1. Click "Save" at the bottom of the screen.

1. Click the red button to publish the vacancy to our external job board.

1. On the Job Post you just edited click the three dots next to the pencil and click "Duplicate".

1. The `Job Name` automatically puts "Copy of" at the front of the title; remove this.

1. Select "INTERNAL" from the drop-down list under "Post To".

1. Do not edit `Location`, `Application Language`, `Description`, and `Basic Application Questions`.

1. `Additional Questions` section should only include the following questions:
    - LinkedIn Profile - **Optional**
    - GitLab Username - **Optional**
    - Have you notified your current manager that you are applying to this role?  Please note that if you make it to the end of the interview process the Hiring Manager will speak with your current manager. **Required**
    - What are your pronouns for others to use when referring to you? (ex: she/her, he/him, they/them, ze/zir/hir, etc.) - **Optional**
    -  It is important to us to create an accessible and inclusive interview experience. Please let us know if there are any adjustments we can make to assist you during the hiring and interview process. **Optional**

1. ``Settings` 
   - Send Confirmation Email to Candidates: select the "Internal Auto-Reply after Application" from the drop-down list
   - Application Confirmation Page: Default
   - Uncheck "Include Custom Demographic Questions"
   - Uncheck "Include EEOC Questions"
   - Uncheck "Include 'Apply with SEEK' button"

1. Click "Save".

1. Click the red button to publish the vacancy to our internal job board.

1. After publishing, announce on Slack in `#new-vacancies` for team members to apply or send in referrals. Slack message template:
  New Job Alert: TITLE
  Apply internally: LINK
  You can share this opening with your network: LINK
  Review how to make a referral: https://about.gitlab.com/handbook/hiring/greenhouse/#making-a-referral

1. Please note, updates from the [Greenhouse jobs page](https://boards.greenhouse.io/gitlab) to the [GitLab jobs page](/jobs/apply/) generally happen within 30 minutes. Though, it can take up to 1 business day.

### Add a Video

Adding a video to your job post is a great way for candidates to get to know the role, hiring manager, and GitLab before they even apply. 
Hiring managers, if there's not already a video created for your job family or role, consider recording one. Check out the [job family video issue](https://gitlab.com/gitlab-com/people-group/recruiting/issues/237) for guidance or support, or record your own role-specific video.

Examples: 
1. [Sales Development Representative job family](https://www.youtube.com/watch?v=A4lMjhNfX9s)
1. [Product Manager job family](https://youtu.be/DVLOyaRbAoM)
1. [Senior Product Manager, Manage (Analytics) vacancy](https://youtu.be/-BT9-xhk9as)
1. [All-Remote Integrated Marketing Campaign Manager vacancy](https://youtu.be/BOeXgGu1Vco)
1. [Senior Product Manager, Create (Gitaly) vacancy](https://youtu.be/5TGixSUXbk0)

Learn more about [uploading to GitLab Unfiltered within the Communication section of the Handbook](/handbook/communication/youtube/). If you're unable to create a video, please add a video about life at GitLab, like [this one](https://youtu.be/V2Z1h_2gLNU).

To add an embedded video to a job posting:
1. Inside Greenhouse, click the "Job Setup" tab in the navigation top bar while viewing the relevant job.
1. Click "Job Posts" in the left sidebar and click the small pencil to edit the relevant job description.
1. In the editing area for the job description, click the small "Insert/edit media" button.
1. Click the "Embed" tab and insert the embed code from YouTube. 
   * You can retrieve this code by clicking "Share" on the relevant video in YouTube, then clicking "Embed". Copy and paste the code.

## Screening, and Resume Review

1. The Recruiter may conduct a calibration exercise with the Hiring Manager by presenting 2-3 unscreened resumes to make sure they are identifying the right skills and will adjust accordingly.

1. The Recruiter conducts direct sourcing efforts, reviews resumes, maintains the status of applicants, sets dispositions, and will screen on average 8-10 candidates per opening.

1. Once candidates have been identified and screened, the Recruiter will submit the top 4-5 qualified applicants to the Hiring Manager or designee for review.

1. The Hiring Manager will select which candidates they are interested in interviewing.

### Sourcing Support

For difficult or hard-to-fill positions, the hiring team will use the available tools to source for additional candidates. Please communicate with the hiring team if sourcing is needed for a strategic, specialized, or difficult to fill position. In addition, Managers should also reach out to their own network for candidates and referrals. It is common for candidates to respond more frequently to those who they know are the hiring manager. One superpower of great Managers is having a strong network of talent from which to source.

Recruiters use various tools to identify talent by proactively reaching out to candidates for opportunities. In addition, they will partner with hiring managers to participate in sourcing to ensure they are targeting the right skillsets.

The Hiring Manager should always ask the team for passive referrals for open positions. GitLab team-members can refer candidates through our [referral program](/handbook/incentives/#referral-bonuses).

The hiring team should publicize the vacancy through the following means:
   - Tweet about the new vacancy, help can be provided by the content marketing manager and team.
   - Request "soft” referrals by encouraging all GitLab team-members to post links to the jobs site on their LinkedIn profiles.
   - [Who's Hiring](https://news.ycombinator.com/ask): On the first of the month (or closest business day), include a comment for GitLab in the Hacker News thread of "Who's Hiring". Template text:
`GitLab | Remote only | Full time - It’s an exciting time to join GitLab. As a fast-growing, all-remote company, GitLab is a place where you can contribute and make an impact from anywhere in the world. You’ll be part of an ambitious, productive team that values transparency and collaboration. We’re hiring solutions architects, engineering managers, security engineers, recruiters, support engineers, product managers, strategic account leaders, and more roles in every department. Here’s our full list of vacancies: https://about.gitlab.com/jobs/ Here’s an inside look at GitLab’s interview process from one of our new team members: https://about.gitlab.com/blog/2019/03/28/what-its-like-to-interview-at-gitlab/ Want to learn more? Check out our company handbook: https://about.gitlab.com/handbook/`[Example comment](https://news.ycombinator.com/item?id=19543942)
   - [Alumni post](https://news.ycombinator.com/jobs) as a Y Combinator alumni we can post directly to the front page of Hacker News. We do this for all engineering functions, including the management ones. The PeopleOps vault has credentials under Hacker news. Go to [Alumni post](https://news.ycombinator.com/jobs) and click submit job. For the title use: `GitLab (YC W15, All-remote) is hiring XXX`. And the URL links to the vacancy. [Example posting](https://news.ycombinator.com/item?id=19586072)
   - [LinkedIn](https://www.linkedin.com/) (Able to post 40 vacancies simultaneously, please ask the recruiting operations team if you want your role listed here and it is not already)
   - [RemoteBase](https://remotebase.io/) (Free; position descriptions are synced directly to our respective position description sites)
   - [WeWorkRemotely](https://weworkremotely.com) ($200 for 30 days, per position, used infrequently)
   - [RemoteOK](https://remoteok.io) ($200 for 90 days, per position, used infrequently)
   - [Indeed Prime](http://www.indeed.com/) (Primarily used for non-engineering roles)
   - [Ruby Weekly](https://rubyweekly.com) ($199 per slot per newsletter, for engineering roles)

When using vacancy links to spread the word about our current vacancies, in order to keep data accurate, we can create specific tracking links through Greenhouse in order to include the specific source of different job boards, etc. To learn more about how to create the tracking links for jobs, please [see the Greenhouse help article](https://support.greenhouse.io/hc/en-us/articles/201823760-Create-a-Tracking-Link-for-Your-Job-Board).

All vacancies must be posted on our jobs page for at least 3 business days before we can close it externally or make an offer; this includes all new positions and [promotions](/handbook/people-group/promotions-transfers/#promotions). If a vacancy has been opened for at least 3 business days and has 50 or more applicants, the recruiting team may close the role to new applicants at that time and reopen if and when we need more applicants. Generally the job will remain published on the Internal job board to stay open for additional referrals.  

### Closing a Requisition

1. The Recruiter will clear the pipeline of candidates in all stages of application and notify the candidates that the position has been either filled or closed. 

1. Consider rejecting promising candidates with the reason `Future Interest` and making them a prospect so we can reconsider them in the future. 

1. You can also add various tags to the candidates, which makes it easier to find them in Greenhouse later on if you are recruiting for the same or a similar position. 

1. You can also set a reminder for a candidate if you anticipate reopening the role at a later date.

1. The Recruiter will close the position in Greenhouse. Please note that upon closing the vacancy this will cancel interviews but not remove them from calendars. It is best to manually delete any inflight interviews before closing the role.
