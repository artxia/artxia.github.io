---
layout: handbook-page-toc
title: "GitLab Onboarding Processes"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Onboarding Processes

### Overview
This page is a guide for People Experience Associates when onboarding new team members. All onboarding tasks and guidelines for new team members, People Ops, and Managers are in the [People Ops Onboarding Issue](https://gitlab.com/gitlab-com/people-group/employment/blob/master/.gitlab/issue_templates/onboarding.md). Each onboarding issue is structured with tasks for all team members (Day 1 to Day 5-30) and below those task sections are listed department-specific and/or role-specific tasks.  In some cases, specific tasks may link to supplemental issues, created by specific teams, with in-depth training.

### Timing
People Experience Associates will create the onboarding issue, and start completing the [onboarding tasks](/handbook/general-onboarding/onboarding-issue-tasks/), no later than one week before the new team member joins. People Experience Associates require a minimum of 4 business days (with the new hire timezone as the basis) before the new hire's start date to complete all onboarding tasks. To ensure we create a smooth onboarding experience for new team members, provide enough time for the IT Ops team for laptop orders, and completing the I-9 process (for US-base hires) 4 days is the minimum amount of time needed. Should a contract not be signed prior to 4 working days from the start date, a new start date will be required. If any changes are made to the onboarding template, kindly notify team members of the People Ops team by ccing them in the MR with the `@gl-people-exp` handle. Also notify other teams if a change will impact them.

All new hires will receive invitational access to their GitLab email, GitLab accounts, and any other work-related accounts on Day 1. No access is permitted before Day 1.

### Alerts & Announcements
At 14:00 UTC every Wednesday, the `PeopleOps Bot` slack bot will send an alert in the `#peopleops-alerts` channel listing any data missing (if applicable) from the BambooHR profiles of team members joining the following week. The People Experience team will fill in these missing details as soon as possible since completeness and accuracy of BambooHR profiles is necessary for all automation.

At 16:00 UTC every Thursday, the bot will send another alert in the `#peopleops-alerts` channel with a list of all new team members joining the following week. This list includes names, email addresses, joining dates, and job titles of the new hires along with links to a Sisense graph showing the hiring progress over time. After a final and quick round of verification of the details, the People Experience team will then copy and post in the `#team-member-updates` channel with an announcement listing and welcoming all new team members who will be starting the upcoming week.

### Pre-Onboarding Issue I-9 Tasks (US Only)
- **I-9 and E-Verify**<a name="I-9"></a>

For all GitLab Inc. and GitLab Federal LLC US-based employees, GitLab complies with all USCIS requirements and laws, including the I-9 and E-Verify process. GitLab uses an online I-9 portal called [Fragomen](https://gitlab.i9servicecenter.com/Login.aspx?) where the process is completed and documents are saved electronically and securely. Only US-based People Experience team members who are US Citizens have administrative access to this portal.

There are two sections in the I-9 process (Section 1 and Section 2). GitLab requests that team members complete the I-9 process at least two business days prior to their start date. Please note the `two business days prior to the new hire's start date` timeline pertains to GitLab's internal policy, not USCIS legal requirements. GitLab requires the process to be completed earlier than USCIS to ensure there is no delay in adding the new team member to payroll and other important systems.

* Section 1 → Employee personal details. New team members fill out this section online personally.
* Section 2 → Employee assigns a “Designated Agent” to view, verify and document their government-issued official document(s). The Designated Agent completes this section online personally, but with the new team member and their documents physically in hand next to the Designated Agent.

_Note: You can reference what are considered to be “Acceptable Documents” [here](https://www.uscis.gov/i-9-central/acceptable-documents/acceptable-documents)._

If a GitLab team member has not completed Section 1 by EOD on their first day of work (their start date), all access is paused. Their GSuite account is Suspended, as well as their Okta account, as well as their 1Password account and Slack account if these have been created. Access will be resumed as soon as Section 1 is completed.

If a GitLab team member has completed Section 1 but their Designated Agent has not completed Section 2 by the EOD of the team members fourth day of work (3 business days after start date), all access is paused. Their GSuite account is Suspended, as well as their Okta account, as well as their 1Password account and Slack account. Access will be resumed as soon as Section 2 is completed.

The steps below serve as a guide for the People Experience team completing the I-9 process:

1. Check the [GitLab Onboarding Tracker](https://docs.google.com/spreadsheets/d/1L1VFODUpfU249E6OWc7Bumg8ko3NXUDDeCPeNxpE6iE/edit?ts=5def8e7c#gid=1721125348) for your assigned US-based new team members in the `assigned to` column.
2. Send your assigned new team member(s) an [email](https://docs.google.com/document/d/1uWbIfAZrEbf7JTM4zR0PSbG_3eq4jrt_jIIrV_CorfM/edit) with instructions on GitLab's I-9 process at least one week (ideally two weeks) before their start date, to account for holidays/vacations.
3. New hires are instructed to complete Section 1, and to designate an agent for Section 2, as outlined in the email template.
4. The People Experience team will monitor responses to the [I-9 Designated Agent](https://docs.google.com/spreadsheets/d/16vUt2P6Rz1kXtmdWsmOolQzjDV8RmybqYSUykeDqSZU/edit?ts=5df93c0f#gid=841432954) form several times daily.
5. Once the new team member shares designated agent information in the sheet above, the People Experience Associate will review the following steps to designate the agent in the I-9 portal:
  * Go to the [Fragomen](https://gitlab.i9servicecenter.com/Login.aspx?) I-9 portal
  * Search for the new hire's name
  * Click on the _eye_ icon to ***"View/Edit this I-9"*** in the "Incomplete I-9s" section at the top of the page
  * Select `Designate an Agent` at the top of the page
  * Type the agent’s first name, last name, and email address
  * Click `Assign Agent`
  * Check the _“Send Password Email?"_ box
  * Click `Send`

_Note: Once Section 2 is completed by the designated agent, all access is automatically disabled to both the new hire and designated agent._

6. After the designated agent uploads documents on the new team member's behalf, the PEA audits the I-9 by reviewing the following steps:
* People Ops will _generally_ receive an email titled ***“[employee name]/E-Verify Photo Matching Required”*** to prompt the PEA to perform the audit. However, it is necessary to frequently check the 1-9 profiles of your assigned new hires to ensure the process is not delayed should you not receive the email.
* Verify that the new hire and their agent uploaded correct, high-resolution, uncropped images or scans of their designated I-9 documents. If the documents are missing or unacceptable, the PEA must communicate with the new hire so that the PEA may upload the correct documents into the portal manually.
* Using the documents uploaded to the portal to review the 1-9, the PEA should audit:<br>
_*Section 1*_: Employee name and birth date<br>
_*Section 2*_: Document number and expiration date<br>
* If there are any discrepancies or incorrectly entered information, the PEA `corrects the error in the 1-9`.

7. _(If not completed automatically)_ The PEA completes the photo match process by scrolling down on the new team member’s profile in the I9 platform to the `EVerify Employment Verification` section:
* Click `photo match`
* Select the appropriate option ("Yes, "No", or "No Photo") after verifying the photo
* Press `continue`
* After the photo match is complete, the E-Verify process outlined below will often be automatically triggered. If it is, you may ignore step number 8 below.

8. _(If not completed automatically)_ The PEA needs to complete the E-Verify process by selecting the _E_ icon in the “Incomplete I9s” section at the top of the page to `manually submit this I-9 to E-verify`
9. Be sure to screenshot the `Electronic Signature Receipt!` page
10. Once the process is complete, upload the Electronic Signature Receipt screenshot and the employee document scans to the `Verification Documents` folder in the employees BambooHR profile.
11. Check the tasks listed in the onboarding issue related to the I-9 process to indicate completion
12. Notify the People Operations Analyst by commenting in the onboarding issue _no earlier_ than the new hire's first day that the process has been completed. ***Notifying the People Operations Analyst is very important, as it is what will trigger adding the new hire to payroll.***

### Pre-Onboarding Issue Creation Tasks
The People Experience Associate will create the GSuite account first.

- **Google Suite Account Creation**<a name="Google"></a>

1. Log into the Google Admin console and click on the Users tile.
1. People Experience Associates create email addresses for new team members using the convention of `firstinitiallastname@gitlab.com`. To make sure that we create new GitLab.com GSuite emails according to the new team member's preferred first and last name, we first look at the team member's resume & relevant communications to find their preferred name.
1. Before creating the email account, verify that the proposed email is not conflicting with a current account. If it is, add a letter for their middle name or ask the team member for their choice in preferred letter addition to their email address.

Examples:
  * If a team member's legal name is "Joseph D. Doe" but their application and emails are signed "Joe Doe", then we create the GitLab email as Joe Doe, `jdoe@gitlab.com`.
  * If a team member's legal name is "Nina Fernandez Kola" but their resume and emails are signed "Nina Fernandez", then we communicate with the team member in advance and create the GitLab email as `nfernandez@gitlab.com` with confirmation from them that is their preferred name.
  * If a team member's legal name is "Li Ju Zhang" but their resume and emails are signed "Joanna Zhang", then we communicate with the team member in advance and create the GitLab email as `jzhang@gitlab.com` with confirmation from them that is their preferred name.

- **BambooHR Profile Data**

As part of [onboarding](/handbook/general-onboarding/), People Experience Associates will process new hires in BambooHR. Aside from the steps listed in the onboarding issue, this is a description of how to add the proper information into BambooHR.

***Note:*** If all of the necessary tabs in the new team member's BambooHR profile do not automatically populate, please go to the `Job` tab, scroll down to the `Job Information` section, click the pencil icon on the righthand side of the section, and ensure that the `Department` and `Division` fields are correctly populated. Save you changes and refresh the new team member's profile. All necessary tabs should now appear.

Personal Tab

1. Enter the team member's full legal name (as much as it is known before seeing legal ID) and preferred name if known.
1. Enter full address, including Street address, City, Region, Zip/Post Code and Country.
1. Enter the locality ([geo area](/handbook/people-group/global-compensation/#geographical-areas), country). This information should be visible in the offer details. If you have any questions, please reach out to the compensation team.
  * Please note the formatting must be entered exactly as outlined in the [location factor file](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/data/location_factors.yml) with "area, country" or the integration outside BambooHR will fail. Please only choose a locality from the already created fields in BambooHR. Do not create any new localities.
1. Enter the relevant Region. The three options are Americas, EMEA, or JAPAC.
1. Add the GitLab email created previously in the Work Email field.
1. After verifying the work email entered and saved, go to top right corner, and set access level to "Employee Self-Service".

Jobs Tab

1. Hire Date - enter in the correct hire date.
1. Role
   * Leader - if director or above
   * Manager - if has any direct reports
   * Individual Contributor - all others
1. Cost Center - Choose the same cost center as their manager.
1. Payroll Type
   * Employee - paid through Payroll
   * Contractor: IND - Independent Contractor agreement
   * Contractor: C2C - Contractor Company agreement
   * Employee-PEO - Employe employed via a Professional Employer Org
   * Contractor-PEO - Contractor contracted via a Professional Employer Org
1. Exception to IP Agreement
   * Enter Yes if they answered Yes in the PIAA section of their contract. Send the entered information listed by the team member in an email to the VP of Engineering and VP of Product for approval. File the approved email in the Contracts & Changes folder in the Documents tab in BambooHR. No need to share the doc.
   * Enter No if the team member answered No or None.
1. Enter the Candidate ID. This is the candidate's ID in Greenhouse, and is found by looking at the URL for the candidate. It is an 11-digit number listed between /people/ and the ? symbol.
1. Compensation Table
   * Use the BambooHR Calculator in Google Drive to do the following steps. Reach out to an Analyst if you need access.
   * Effective Date - Hire Date
   * Pay Rate - Entered as if it were a payroll amount. For example, a US employee would be entered as their yearly amount divided by 24 payrolls in a year. A contractor would have their monthly contract amount listed.
   * Pay Per - Monthly for contractors and employees paid once per month, Pay Period for all other employees
   * Pay Type - Use either Salary or Hourly for employees, or Contract for contractors.
   * Pay Schedule - Select the pay period. Currently we have twice a month for the US, and monthly for all others.
   * Overtime - This is the FLSA Code - This will either be exempt or non-exempt depending on how the role is classified. If there are questions on the classification, please ask the People Ops Analyst.
   * Change Reason - Hire
   * Comment - Please add any comments that are relevant from the contract terms.
1. Pay Frequency (Note: Pay Frequency times times pay rate should equal annual compensation)
   * 12.96 for GitLab B.V. employees in the Netherlands
   * 13.92 for GitLab B.V. employees in Belgium
   * 24 for GitLab Inc. employees in the United States
   * 26 for GitLab Canada Corp employees in Canada (paid every other week)
   * 12 for everyone else paid monthly
1. On Target Earnings
   * If the team member does not have any variable compensation, do not enter any information. If yes, continue.
   * Add the effective date, annual amount of the variable component in local and USD, and the OTE in local and USD. OTE is base + variable.
   * Lastly, add the frequency at which the variable component is paid out.
1. Currency Conversion
   * The effective date is either January 1 or July 1, whichever is more recent. Every January and July, the People Ops Analyst will conduct a currency conversion for all team members.
   * Use [Oanda](https://www.oanda.com/currency/converter/) for the currency conversion. Always convert the currency from local currency into USD so that we remain consistent.
   * Enter the currency conversation factor from Oanda with all 5 decimal places.
   * Enter the Local Annual Salary with the appropriate currency code and the converted salary in USD.
1. Job information
   * Effective Date - Hire Date
   * Location - Which entity the new team member is contracted through.
   * Division - Enter the appropriate division from the dropdown.
   * Department - Enter the appropriate department from the dropdown.
   * Job Title - Choose the job title. The title should read as Level Benchmark. If the position is at the Manager or Director level it should read as "Manager, Description". If the title does not exist already, scroll to the bottom, click "Add New", create and save the new job title.
   * Reports To - Select their manager.
   * Job Title Speciality - If there is a specialty (this would be seen in the contract as titling reads Level Benchmark, Specialty, but region alignment is not considered a specialty), use the drop down to select the appropriate specialty. If the specialty is not listed in the drop down menu, create a new one. The Job Title Specialty field has no restrictions except that time zone or territory alignment do not qualify as specialties.
         (Examples of a Specialty: Growth, Commercial, DoD.
         Examples of what is not a Specialty: Americas East, EMEA, APAC)
   * Enter whether the team member is part-time or full-time. Any comments? Add them to the compensation table.
1. Bonus
   * Enter a bonus date, amount and type if applicable.
1. Employment Status
   * Enter the hire date and set the status to Active. Also leave a comment if there is anything of note in the contract. Except;
   * Hires in the Netherlands should have 5 entries;
        1. `Temporary Contract` with date marked as the start date
        2. `Temporary Contract Ending` with the date marked as exactly **12 months** from their start date
        3. `Probationary Period` with the date marked as the start date
        4. `End of Probationary Period` with the date marked as exactly one **month** from their start date
        5. `Active` with the date marked as exactly **12 months and one day** from their start date (AKA: One day after the Temporary Contract ends)
   * New team members from GitLab LTD (UK), CIIC(China), Safeguard Hungary, and Safeguard Spain all have a three-month probation period.
   * Team members from GitLab GmbH (Germany), GitLab PTY (Australia),  Lyra (India),  Safeguard in countries Italy, Nigeria, South Africa, Ireland will have a six month probation period.
1. If applicable, set the status to probation period. This sets up an alert for the manager and People Ops automatically, 2 weeks, 1 week, and a day before the probation period expires. Details of the probation period process can be found on the [contracts page](/handbook/contracts/#probation-period). Please use these probation periods in BambooHR for team  members in these specific groups.
1. For employees of HRSavvy, LYRA, and CIIC, email the Employee ID number to our contact to align our systems.

Notes Tab

1. Referral
   * Add a Note stating "Referred by Jane Doe" if team member was referred. Search in multiple places in their offer details to make sure that you find information if they were referred.
   * If referrer is their direct or indirect manager, we cannot pay the referral bonus.
   * If the referrer is not in a direct/indirect manager role to the team member, enter their Bonus information in their BambooHR profile. Read the specific information about [Referral bonuses](https://about.gitlab.com/handbook/incentives/#referral-bonuses) for more information.

Benefits Tab

1. Stock Options
   * Effective date: Enter the start date.
   * Enter the respective Entity.
   * Employee or Contractor (This should match Payroll Type on the Jobs Tab).
   * Enter the number of shares from the contract.
   * Do not enter information in any other fields.

### Onboarding Issue Creation
The People Experience Associate will then create an onboarding issue with a ChatOps command in Slack 4-5 business days prior to the new team member's start date.

1. Before creating the onboarding issue, ensure that all information entered BambooHR is accurate and complete.
1. In Slack, go to your profile as if you were going to send a Slack message to yourself. Type the command `/pops run onboarding BambooHR_ID_number` (not Employee ID #). This number is found in the team member's BambooHR profile URL, after `id=`. It is a 5-digit number. An example of the command would be `/pops run onboarding 00000`. If BambooHR's API is down, this ChatOps command will fail and will need to be created manually.
1. You will be pinged in Slack once the onboarding issue is created, which usually takes 30 seconds or so. The ping will include a link to the new onboarding issue.
1. Check and update if applicable the Name from Legal to Preferred name.
1. Update if applicable the title with the Specialty as the bot does not add the Specialty so it must be manually added.
1. If the manager is not automatically assigned and listed in the issue, add them. It could be because the employee's manager uses a name in GitLab that is very different from the one in BambooHR, and they don't use their `@gitlab.com` email ID as the primary email ID in GitLab. They will then manually need to be assigned.
1. Copy and paste the link into the Google sheet [GitLab Onboarding Tracker](https://docs.google.com/spreadsheets/d/1L1VFODUpfU249E6OWc7Bumg8ko3NXUDDeCPeNxpE6iE/edit?usp=sharing) in the team member's specific column on their line. Please note that this document is only viewable to the People Experience team and ITOps to protect personal information.
1. If you are part of the People Experience team, IT Ops team, or are the new hire's manager or onboarding buddy please note there are additional steps to complete directly in the new hire's onboarding issue in the 'Before Starting at GitLab' section.

### Day 1 Onboarding Tasks

- **Send password reset email**<a name="request-code"></a>

<i><b>Important:<b><i> This email can only be sent a maximum of 48 hours prior to the new team member's start date/time. If it is sent more than 48 hours prior the link will no longer be valid. (I.E. If a new team member is starting on Monday, the earliest the People Experience Associate can send this email is on Saturday).

1. The assigned People Experience Associate should access the [Google Admin Console](https://admin.google.com/ac/users) and search for the new team member's GitLab email address.
1. Once on the new team member's profile, click `reset password` on the lefthand side of the page.
1. Click `reset`
1. Click `email password`
1. The People Experience Associate should insert their email address and click `send` (do not insert the new team member's email address here).
1. Once the email is received, the People Experience Associate should forward to the new team member's `personal email address`. Please add the new team member's GitLab email address in the body of the email where it says "Hello [new team member name], [_____@gitlab.com].


- **Request Signature for Code of Conduct Acknowledgment document**<a name="request-code"></a>

Each assigned People Experience Associate will send their new team members our Code of Conduct Acknowledgment for review and signature.

1. In BambooHR, go to the Files section.
1. Be sure you are in the Signature Templates section.
1. To the right of the Code of Conduct Acknowledgment, click on the triangle to the right of the gear icon and click Request Signature.
1. Choose "Send a signature request to: Only some people"
1. Type in the name of your assigned team members. Please note that an employee must have access to BambooHR in order for us to request a signature, and our team members only get access Day 1.
1. Message to Signers: Dear new team member, we are so happy you are part of the GitLab team. Please take a moment to sign this document. Thank you!
1. Click Send Request.
1. On a bi-weekly basis, set a reminder to go to the Signed Documents link of the Reports section in BambooHR.
1. Click on Code of Conduct Acknowledgment.pdf and notice the team members who were sent the document and have still not signed.
1. If a team member was sent the document for signature or reminder over 2 weeks in the past, click the Bell icon on their line at the far right. Clicking on the bell will send them a notification to sign.

- **Invite to swag store**<a name="swag-store"></a>

Send the "New Hire Swag" email to new hire. It must state that they need to access the [GitLab Swag Store](https://shop.gitlab.com/), choose goods and use the new hire discount code provided in the email at checkout. New hires must use their GitLab email at checkout.

1. Each People Experience Associate is responsible for sending the [swag store invitation email](https://gitlab.com/gitlab-com/people-group/employment/blob/master/.gitlab/issue_templates/swag_email.md) to their assigned new team members.
1. Verify the new hire discount code in the People Ops 1Password vault by searching `New Hire Swag code`.
1. Update the swag code in the email prior to sending to the new team member.

- **Add to Moo**<a name="moo"></a>

We expect every team member to be an advocate for GitLab and we offer every team member the opportunity to have business cards, to make GitLab feel real to people around them despite not having an office.
1. Every week, the People Operations DRI creates a Report in BambooHR containing all Active Employees in three columns: their First Name, their Last Name, their GitLab work email. People Ops adds this data to the [GitLab : Moo](https://docs.google.com/spreadsheets/d/1O6sLITOKDAEumFY9hB42ZVBZeHaq0l6uoA69JNmu1v8/edit#gid=665635414) spreadsheet in a new weekly tab titled that Tuesday's date so that our Moo Rep can grab this data and send out email invitations to new team members from the Moo platform. Business cards should be ordered by the team member themselves using the Moo platform. Self-help instructions are [here](/handbook/people-group/#business-cards).

- **Confirm in 1Password**<a name="moo"></a>

1. Access [1Password](https://gitlab.1password.com/vaults/bdtcoqe5qetyjesywc4adx763e/allitems/dvm46psrlqj2cfeght6s3ziiwu) via your desktop.
1. The bell icon in the upper righthand corner will have a number inside of it indicating how many new team members are pending account confirmation.
1. Click the bell to view new team members names and select `confirm` to verify each user individually.

All PEAs are responsible for checking to make sure that their team members are eventually confirmed, but we all confirm any team members who are in the Pending stage as we log into 1Password multiple times on Day 1 & 2.

- **Create Interview Training Issue**

1. This task is _only applicable for new team members that are people managers_. 
2. Go to the GitLab [training project](https://gitlab.com/gitlab-com/people-group/Training)
3. On the lefthand side of the page, click into the `issues` section
4. On the upper righthand side on the page select the green `new issue` button
5. Choose the `interview_training` template
6. Proceed with the steps in the README:
* Title this issue with `Interview Training: [Team Member Name]`.
* This issue should be remain confidential after creation, as the STAR interviewing training video linked below should be kept internal to GitLab as it contains confidential information. 
* Assign this issue to the person training.
7. In the `People Manager` job specific section of the new team member's onboarding issue add a `New team member` task with the Interview Training issue linked and state "New team member: Complete interview training."
8. In the `People Manager` job specific section of the new team member's onboarding issue, mark the `People Experience` task _"If applicable, create an interviewing training issue in the People Ops Training project and assign it to the new team member."_ as complete.

## Ordering Supplies

If a GitLab team-member is in need of supplies and is unable to purchase the items themselves, People Experience Associates can place the order, per [Spending Company Money](/handbook/spending-company-money/). Use the Amazon business account for all Amazon links. In order to see what is available to ship in each country, use the Amazon site specific to a new team member's location.

## People Operations Analyst Onboarding Tasks

1. Audit the BambooHR Entry. Download a copy of the contract from the Documents Tab. Verify the information (start date, title, stock, etc) matches the entries in BambooHR as outlined in [Adding a New Team Member to BambooHR](/handbook/general-onboarding/onboarding-processes/#adding-a-new-team-member-to-bamboohr).
1. If all the information is correct, mark the new hire as complete on the "Payroll Changes Report" in BambooHR.
1. At the end of each week a People Operations Analyst will review all data entered into BambooHR through the Payroll Change Report for audit purposes. Once a month an audit should be conducted from all payroll providers to ensure the salary information matches BambooHR
1. Add to the compensation calculator
  * Add the Employee ID, First Name, Last Name
  * All other items in Blue are to be entered. Columns in black are formulas that need to be carried down.
  * Ensure the Locality follows the criteria for [geo areas](/handbook/people-group/global-compensation/#geographical-areas).
  * If the team member is over range for their compensation, the Metrics column will read as false. Please copy the formula down to generate the adjusted location factor for metrics reporting. For Sales, the Benchmark will need to be manually input based on the Sales Comp spreadsheets.
  * Audit the locality in BambooHR under the personal tab to ensure it matches to the comp calc.
1. Create a new profile in Lumity (if a US team member)
  * Login to Lumity
  * Click your name and then switch to admin view
  * Under employees, select manage.
  * Click Hire Employee and enter information as prompted.
  * Benefits plans are dependent on the state the new hire lives in. OOS stands for Out of State and should be selected if the new team member does not reside in California, Hawaii, or Colorado.
1. Create a new profile in Betterment
  * Login to Betterment's Business Account (this is different than the personal account)
  * Click Employees
  * Click add an Employee
  * Enter all information as prompted
  * All new team members in the US are primary, not part of a union, able to access a computer, and eligible to participate (except interns).

## Onboarding for Independent Contractors

From a legal/onboarding perspective, an independent contractor should be treated like a 1099 vendor. The Business Partner that is engaging with the contractor needs to fill out a standard [vendor contract issue](https://gitlab.com/gitlab-com/finance/-/blob/master/.gitlab/issue_templates/vendor_contracts.md) in the [Finance project](https://gitlab.com/gitlab-com/finance/issues) and they will need a contract and/or SOW and start the process. Once it goes to the approval stage, the Accounting team will get a ping and send the independent contractor an onboarding request in Tipalti so they can create an account and supply their tax information to ensure we supply them with a 1099 at the end of the year. In order to process the onboarding issue from the People Ops side, peopleops@gitlab.com requires the information indicated below:

*  Full legal name
*  Preferred name
*  Job title
*  Manager
*  Department/division
*  (Ideal) start date
*  Personal email address
*  Address

**1. 1-9 Process:** 

US Independent Contractors are [not required](https://www.e-verify.gov/supplemental-guide-for-federal-contractors-60-subcontractors-independent-contractors-and-1) to go through the I9 E-Verify process per: _"Employers are not required to complete Forms I-9 and use E-Verify for their independent contractors."_

**2. Onboarding Issue:**

As Independent Contractors **do not have BambooHR profiles**, onboarding issues will need to be created manually by going to the [GitLab Employment project](https://gitlab.com/gitlab-com/people-group/employment), clicking `issues` on the lefthand side, the green `new issue` button, and selecting the `onboarding_independent_contractor` [template](https://gitlab.com/gitlab-com/people-group/employment/-/blob/master/.gitlab/issue_templates/onboarding_independent_contractor_.md).
**3. IT/Office Supplies: **

IT Ops **does not** provide [laptops](https://about.gitlab.com/handbook/business-ops/it-ops-team/#laptops) to Independent Contractors nor are independent contractors eligibile to purchase and expense Office Supplies. Independent contractos are provided with a @gitlab.com email and through their onboarding issues, create 1Password accounts. Independent contractors are not provided with Okta accounts.

**4. Payroll/Expenses:**

Independent Contractors do not require Expensify access. All payments must go through Accounts Payable after manager approval; GitLab Payroll will not handle invoices.


## Hiring Manager Onboarding Tasks

### Add blank entry to team page <a name="blank-entry"></a>
1. Go to the [GitLab.com / www-gitlab-com](https://gitlab.com/gitlab-com/www-gitlab-com/) project.
1. Click on the `data` folder, then on the next page click on the `team.yml` file.
1. Click on the button labeled `Web IDE` between the `Edit` and `Replace` buttons.
1. Find the vacancy entry for the new team member's position, and replace with some of the new employee details:
  * **DO NOT** change slug, unless you are copying template then use `jobabbreviation-firstname-lastinitial` (ex. `mpm-agnes-o`). If you do not have a place holder, create a slug by using a unique naming convention such as `jobabbreviation-firstname-lastinitial`.
  * Type = change `vacancy` to `person`
  * Name = `First Name` `Last Initial` *only*
  * **Remove** placeholder line.
  * Location Factor = `0.7` (PeopleOps will update at future date)
  * **Role** = *UPDATE* URL to correct [`/job-family`](/job-families/). **Must be relative link, do not include `https://about.gitlab.com`** Make sure `Title` is accurate & matches onboarding issue using proper capitalization
  * Reports to = Manager `slug`
  * **Picture** = `../gitlab-logo-extra-whitespace.png` team member is tasked to update
  * **Departments** = *REMOVE* `Vacancy`; Add main department (i.e. Marketing or Sales).
  * Story = `Joins on Month XXth` team member is tasked to update.
  * Expertise = *REMOVE* `Recruiter` and `Application Link` lines
1. If no vacancy entry is found for this position, create an entry and make sure the information above is correct. Also:
  * Create a temporary slug, made up of shortened title / abbreviation. Search to be sure that no other team member already has this slug. If the team member will manage team members, make sure that the direct hires have the slug listed in the reports_to section.

#### Template for New Team Member entry
{:.no_toc}

```
- slug:
  type: person
  name:
  start_date:
  location_factor: 0.7
  locality:
  country: Remote
  role: <a href="#update-link">ADD TITLE</a>
  reports_to:
  picture: ../gitlab-logo-extra-whitespace.png
  twitter:
  gitlab:
  pronouns:
  departments:
    - Vacancy
  story:  |
          Joins on ...
```
