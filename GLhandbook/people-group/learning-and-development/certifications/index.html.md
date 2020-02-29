---
layout: handbook-page-toc
title: Certifications
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Introduction

Welcome to the certifications page! Here you will find links to our current certifications.

## Current Certifications 

* [GitLab Values](/handbook/values/#gitlab-values-certification)
* [GitLab Communication](/handbook/communication/#communication-certification)
* [Being an Ally](/company/culture/inclusion/ally-training/#ally-certification)

## Upcoming

In FY21-Q1 we plan to roll out the additional certification(s) listed below. 

* Inclusion

## Sharing your Certifications 

### LinkedIn 

The video below shows you how to add your GitLab Certification to your LinkedIn Profile. 

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/_u9DImCd2OM" frameborder="0" allowfullscreen="true"> </iframe>
</figure>

## How to Create a Certification 

### Step 1: Google Forms 

1. Go to the Shared L&D folder and go into the “Certifications” sub-folder. 
1. Select the “+ New” button on the top left and select “More” and then select “Google Forms” 
1. Create a google form with quiz questions for the topic. The quiz should have between 5-8 questions. 
1. In the Info section at the top: This certification quiz is based on information found on our {name of page} page (including the video): {insert link to page}. To complete the {name} Certification at GitLab, you will need to read through the content on the page linked above and watch the video on the page (if you did not attend the live session) as well as complete this quiz and earn at least an 80%.
1. Settings → 
    1. General → Uncheck "collect email addresses" - we have a separate box on the form for that. Uncheck the “Restrict to users in GitLab and its trusted organizations” box. This ensures that internal team members as well as external people can complete our certifications. 
    1. Presentation → Set up the Confirmation Message that participants will see after filling out the form. Use the following template:Thank you for completing the GitLab {Name} Certification! Please take this time to review your score. If you scored at least an 80%, you will receive your certificate via email. Please note this may take up to an hour to hit your inbox. If you did not score high enough to receive a certificate, you can take the quiz again. Please reach out to our team with any questions - learning@gitlab.com. Thanks! GitLab Learning & Development
    1. Quizzes → toggling “on” the the “Make this a quiz” button at the top. You can also uncheck “Point Values”
    1. Click “Save” when complete updating all three sections. 
1. Go back through the questions and make them all required (including name & email) as well as set up the “Answer Key” along with assigning points per question.  
1. Quizzes have a pass % of >=80% to receive a certification
1. Once the form is set up, complete the quiz (and pass it) - you will need at least 1 entry in the “passing_results” sheet to see the Sheet work and get Zapier set up.

### Step 2: Google Sheets 

1. Once the form is set up, toggle to the “Responses” tab on the top of the form. Once there, select the green icon in the top right to “Create Spreadsheet” 
1. Once in the google sheet, the first sheet will be auto named “Form Responses 1” 
1. Create a second sheet and title it `passing_results` 
   1. In box A1 type “Quiz Name”
   1. In box A2 type `=IF(ISBLANK(B2)=False, "Values", "")` 
      1. Replace “Values” with what this certification is for 
      1. Copy formula in all cells in Column A to A:1000
   1. In box B1 type `=QUERY(IMPORTRANGE("https://docs.google.com/spreadsheets/d/1bh0hZZNcsEmecEJPEnFeBl3dspv24eHbRjcOwFItkes/edit", "Form Responses 1!A1:M10000"), "Select * WHERE Col9>=10")` 
      1. Where the link is for the sheet, update that to link to the Form Responses 1 Sheet 
      1. Where it says “Col9>=10, update the “9” with the number the column is with the scores (ex. A=1, B=2, C=3, etc.). Where the 10 is, update this number to the lowest score someone could get to score at least an 80% on the quiz. 

### Step 3: Zapier (Create New Zap)

1. Log in to Zapier with the credentials in 1Password 
1. Go to the “Certifications” folder in Zapier  
1. In the top right, click “Make a Zap!” 
1. On the top left, click “Name your Zap” to name
1. 1 - When this happens…
   1. Select “Google Sheets” 
   1. Trigger Event = New Spreadsheet Row 
   1. Choose an Account = Your account
   1. Customize Spreadsheet Row 
   1. Spreadsheet = search for the name of the spreadsheet you created above 
   1. Worksheet = “passing_results” 
   1. Test and Continue 
1. 2 - Do This..
   1. Select “Google Slides” 
   1. Choose Action Event = Create Presentation from Template 
   1. Choose Account - “+ add new account” to connect your account 
   1. Title of New Presentation: GitLab {Title} Certification 
   1. Is Shared? = Yes 
   1. Template Presentation = search for the template 
   1. It will populate fields that need to be filled in in the slides (i.e. name and date) 
   1. Name: click the “insert field” button on the right, and search for the “First & Last Name” field on the spreadsheet 
   1. Date: click the “insert field” button on the right, and search for the “Timestamp” field on the spreadsheet 
   1. Click “Test and Continue” = this should make a test presentation in the same folder where the Google Slides Template is 
1. Select the “+” at the bottom of the current Zap 
   1. Select “Email by Zapier” 
   1. Select “Continue” 
   1. Customize Outbound Email: 
   1. 1. To: click the “insert field” button on the right, and search for the “email address” field under the new spreadsheet row option
   1. Subject: Congratulations! Your GitLab Ally Certificate is Inside!
   1. Body: Thank you so much for completing the {Title} Certification through GitLab. Your certificate is attached! Add it to your LinkedIn Profile or share it on Twitter. We'd love to see it! Please reach out to our team if you have any questions! GitLab Learning & Development
   1. In the body, with your cursor on a blank link at the very bottom of the text box, you will also need to go to the “insert field button on the right. Select “Create Presentation from Template in Google Slides” - select “Export Links Application/pdf” 
   1. From Name: GitLab Learning & Development 
   1. Reply to: learning@gitlab.com
   1. Cc: learning@gitlab.com 
   1. Select Test & Review 
   1. Check your Email inbox for the test certificate 

### Step 4: Add to the Handbook 

1. There should be a handbook page with the content for the certification. If there isn’t already, please create a handbook page first. 
1. At the bottom of the page, but the below template with information on how to access the certification 
1. Here is an example:

```
## {Title} Certification

Anyone can become certified in {insert cert name here}. To obtain certification, you will need to complete this [quiz](insert link to quiz) and earn at least an 80%. Once the quiz has been passed, you will receive an email with your certification that you can share on your personal LinkedIn or Twitter pages. If you have questions, please reach out to our L&D team at `learning@gitlab.com`.
``` 
