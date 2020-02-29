---
layout: handbook-page-toc
title: "Payroll"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Introduction

Welcome to the Payroll Group handbook!  You should be able to find answers to most of your questions here.  If you't find what you are looking for then please do the following:
-  **Email** your question(s) to one of the following group email addresses:
   *   US team members: uspayroll@gitlab.com
   *   Non-US team members: nonuspayroll@gitlab.com
   *   Expenses: expenses@gitlab.com
-  **Chat channel**:  `#payroll_expenses` slack channel for questions that is not confidential.

## Legal Entity Payroll providers

- GitLab BV (Netherlands) - HR Savvy
- GitLab BV (Belgium) - B&F Consult Firm
- GitLab IT BV - iiPay payment service
- GitLab Federal (US) - ADP
- GitLab Inc (US) - ADP
- GitLab GmbH (Germany) - RPI
- Gitlab LTD (UK) - Vistra
- GitLab PTY (Australia) - iiPay
- GitLab Canada Corp (Canada) - TBD

## Pay Date

1. Employees of GitLab Inc and GitLab Federal will get pay on the 15th and the last day of the month.  The payroll schedule, pay slips, and W-2(s) are available on [ADP portal](https://workforcenow.adp.com)
1. Employees of GitLab BV (Netherlands) will get their salary wired on the 25th of every month, and can see their pay slip in their personal portal on
[HR Savvy's system](https://hr-savvy.nmbrs.nl/) towards the end of the month.
1. Employees of GitLab BV (Belgium) will get their salary wired the last day of each month and will receive their pay slip in their personal portal on [Boekfisk's system](http://www.boekfisk.be/)
1. Employees of GitLab Ltd will get their salary wired on the last day of every month, and can see their pay slip via their personal portal on [Vistra's system](https://www.vistra.com/) towards the end of the month.
1. Employees of GitLab GmbH will get their salary wired on the last day of every month, and can see their pay slip via their [person portal](https://www.datev.de/ano/) on [RPI International Payroll's system](http://roehm-international.com/) towards the end of the month.
1. Employees of GitLab PTY will get their salary on the 27th of each month, and their pay slip through [iiPay portal](https://pay.iipaysp.com/RegisterUser/GITL)
1. Employees of GitLab BV that are employed through GitLab's co-employer PE0:
   - [Lyra](http://lyrainfo.com/) (India) will get their salary wired around the last day of the month. Lyra will send pay slips electronically through their HR portal.
   - CXC (Canada) are paid bi-weekly and can see their pay slip via [CXC](https://totalaccess.adp.ca). 
   - Safeguard are paid monthly and on the last day of the month (depending on the country) with exception to Brazil, 15th of each month and last day of the month. Payslips are provided electronically by Safeguard. 
1. Contractors from Nigeria, South Africa, and the US will get pay within 15 days after they submitted their monthly invoices for services to nonuspayroll@gitlab.com. 
1. Contractors from Poland and Ukraine will get pay around 27th or 28th of each month from CXC Global.
1. All other contractors will get pay on the 22nd of the month by iiPay and remittance advice will send to their gitlab email address.
 

## US

### Adding New Hire into ADP

1. People Operations Analysts will notify Payroll when I-9 verification is completed
1. Login to ADP as Administrator
1. Select Process, HR, and Hire/Rehire
1. Select Payroll Only (System) template
1. Enter the legal name from Passport or SSN in BambooHR
1. Select SSN for the Tax ID Type
1. Enter Hire Date
1. Select Gender
1. Reason for Hire – New Position
1. Enter Birth Date
1. Company Code – 26X for GitLab Inc or JW9 for GitLab Federal
1. Select USA under the drop down under Countries
1. Enter address
1. Select Works from Home from the More Fields section on the right side
1. Select Yes for Works from Home and Use Primary Address as the Work Address
1. Select Ethnicity/Race ID Method under More Field
1. Look up the Ethnicity under Job section in BambooHR
1. Enter Job Tile and Report to Manager
1. Select FT – Full Time under Worker Category
1. Select team member’s lived in state for Location
1. Select NAICS worker comp code – be sure to use 5302 for WA residents
1. NAICS worker's comp code 8859 only to be used for CA residents
1. Enter work email address and check “Use For Notification”
1. Select Salary or hourly under Regular Pay Rate
1. Enter 86.67 hours for salary team members under Standard Hours and leave it blank for hourly members
1. Enter the Worked in State, Lived in State, and SUI/SDI tax code
1. Select Done
1. Email the ADP Registration email to the team member(s)
1. If the team member is hourly then be sure to copy the hourly template and share it with the team member via Google Sheet

### Processing Payroll

#### One time payment

1. Create a batch and name it accordingly
1. Select the Bonus paydata grid
1. Add employee
1. Enter the earning type and amount
1. Enter B pay frequency
1. Enter 2, or 3 under pay #
1. Enter W under Special Action

 
#### Updating Benefits 

Lumity will send a “Diff” payroll file to Payroll 5 days before pay date for all new enrollments along with changes.  Payroll Specialist will covert the information into an import file to update all changes in ADP.

1. Download the Diff file from Lumity secured portal
1. Make a copy of the original Diff tab and name it as "Payroll"
1. Insert 4 tabs into the workbook: ER Ded, EE Ded, ER Catchup, and EE Catchup 
1. Insert a column into the "Payroll" tab for ADP PositionID.  Use the SSN column to pull in the information via VLOOKUP formula
1. Copy the "Payroll" tab and paste onto those 4 new tabs
1. For the ER Ded tab - delete all deductions columns except for Employer deduction column
1. Sort the ER Ded tab by Benefits Plan Name and add ADP deduction code
1. For the EE Ded tab - delete all deductions columns except for Employee deduction column
1. Sort the EE Ded tab by Benefits Plan Name and add ADP deduction code
1. Add the deduction code and deduction amount onto an import template "EMP(company code)EPI".  Example - EMP26XEPI.csv or EMPJW9EPI.csv
1. A copy of this template is saved in each payroll folder on Google shared drive
1. For the ER catchup tab - delete all deduction columns and only keep ER catchup column and add ADP memo code
1. For the EE catchup tab - delete alld deduction columns and  ony keep EE catchup column and add ADP memo code
1. Add those memo codes and amounts only the Benefits adjustment template (a copy is available in the payroll folder).  Template -26XBCEPI.csv or JW9BCEPI.csv
1. Import employee data for deductions: Process - Utilities - EMP Data import
1. Import benefits adjustment: Payroll - Paydata Batch - Import batch (see one time adjustment instruction)

#### Other payroll adjustment tasks:

1. Update payroll changes
1. reconcile salary for each team member from ADP vs BambooHR
1. Review payroll department between ADP and BambooHR
1. Generate payroll reports for review:
   * Employee changes
   * Active hourly without hours
   * Inactive employees with paydata
   * Autopay cancellation
   * Payroll Summary
1. Preview payroll and accept payroll after thorough review  

#### Reports after Accept payroll

Generate the following reports and saved them on Google Shared drive for Federal and Inc:

1. GL report
1. Payroll Reports (Payroll Summary, Statistical Summary, and Payroll Register Total)
1. Commission and Bonus per check date
1. Benefits deduction for Lumity
1. MISC deductions

#### Benefits Funding Process

* H.S.A
  * Employer contributions will be funded each payroll ($50 per pay)
  * Missed ER contribution will not have a catch up (Employee enrolls late…Lumity will only fund ER contribution on the upcoming pay period. Any missed employer contributions will be disregarded)
  * Discovery will debit GitLab Bank account on each funding date
  * Max out is allowed
* FSA
  * Funds will debit from the Discovery reserve account once the employee submits a claim
  * Discovery will contact GitLab if the reserve is low on funds
* Dependent Care FSA
  * Funds will debit from the Discovery reserve account once the employee submits a claim
  * Discovery will contact GitLab if the reserve is low on funds
* Limited FSA
  * Funds will debit from the Discovery reserve account once the employee submits a claim
  * Discovery will contact GitLab if the reserve is low on funds
* Commuter
  * Employee payroll deduction will occur on the last payroll of the month and funded on the 1st of the following month
  * Funds will debit from the Discovery reserve account once the employee submits a claim
  * Discovery will contact GitLab if the reserve is low on funds
## Non-US


### Australia, UK, Belgium, Netherlands, and Germany Monthly Payroll Process

1. Payroll changes due date to the payroll providers is 15th with exception of Australia (12th).  If the 15th fall on weekend or holidays, then the due date is move to the last business day before the 15th.  
1. Compensation Team will add bonus, promotion, title changes, etc.. to the Payroll Changes template
1. Payroll changes are entered into a spreadsheet for commission, bonus, new salary, expense (only for UK) and password protected the file
1. Payroll sends the payroll changes file to the local payroll providers.
1. Local payroll providers will send the payroll report to nonuspayroll@gitlab.com for review and approval
1. Senior Payroll Specialist will review and notify Payroll Manager for final review and approval.  Once that is completed then SPS will sends the approval email to the payroll provider before the 21st.
1. Payroll save and upload the payroll report to the GoogleDrive by month and under the right entity
1. Payroll notify Financial Controller after approved payroll for Germany and Netherlands so he can queue up the ACH payments for net pay.


### Contractors

#### iiPay:
1. Team member must submit their salary invoices through BambooHR and expense through Expensify by the 8th of each month
1. To enter salary invoice in BambooHR:
   * Visit "My Info" page
   * Select "Request a Change", locate at the upper right corner in that section
   * Click "Contractor Invoice..."
   * Enter "Date Submitted" - current date
   * Enter "Invoice Number" - it should be incremental from the last invoice
     * If new team member, then it will be 1
   * Enter "Invoice Date" - it should be same as invoice date
   * Enter "Monthly Salary"
     * For new hires starting after the 1st of each month, the pro-rated calculation is: `(monthly salary / # of business days for that month) * actual work days from the hire date`
   * Change the currency to match with the currency on the employment contract
   * Enter bonus or commission according to the position. For referral or discretionary bonus, please convert it into your assigned currency by using the corresponding [exchange rate](/handbook/people-group/global-compensation/#exchange-rates).
   * Change the currency
   * Submit - there will be a message at the top of the page - "Your request was submitted successful"
   * The submitted invoice can be seen in "Sent Requests" page, locate the inbox icon at the upper right corner of the page
1.  The invoice will submit to hdelvin@gitlab.com in Payroll for approval
1.  BambooHR will send an email after the invoice was approve or reject with the reason
1.  The invoice will be visible in BambooHR at that time
1.  Note - Once Payroll approved the invoice, any corrections to that invoice must be edit by Payroll through correction request(s) email to       nonuspayroll@gitlab.com
1.  All invoices will be approve by Payroll by the 9th of each month
1.  For expense reimbursement, team member will need to submit through Expensify and report(s) must be approved by managers by the 8th of each month
1.  Payroll will approve all expense reports by the 9th of each month
1.  If the 8th fall on the holidays or weekend, then the due date will move to the last business day before the 8th.
1.  For all new hires starting after the 8th of each month, then the current month payment will be pay with the following invoice as separate payment
1.  Note - all new team members will receive a testing payment from iiPay to validate their bank details prior to th 1st live payment.  Please enter the bank details on the 1st day of employment. 
1.  The required fields for bank details in BambooHR under Bank Information tab:
    * Bank Name
    * Beneficiary Name
    * Account Number (as needed due to each country's banking requirements)
    * Routing number (as needed due to each country's banking requirements)
    * IBAN - this is international Bank Account number.  Each region will have different name for this number.  Be sure to check with your bank
    * SWIFT (as needed or available due to each country's banking requirements)
    * Account type
 

  
#### CXC Global

Team members in Poland, Ukraine, existing contractors in Hungary after to July 2019 will get pay through CXC Global.  Team members will need to submit their monthly invoice (Salary, bonus, commission, etc...) to CXC Global. Payroll will submit commission along with bonus to CXC by the 10th of each month.  For new hires starting after the 1st of each month, the pro-rated calculation is: `(monthly salary / # of business days for that month) * actual work days from the hire date`

### PEO

#### SafeGuard

- Brazil
- France
- Hungary
- Ireland
- Italy
- Japan
- Spain
- South Africa
- South Korea
- Switzerland

Payroll changes due by the 10th of each month.  Payroll will submit commission, bonus, salary adjust, expense reimbursement to SafeGuard via a password encrypted template.  SafeGuard will issue an invoice for each country no later than the 16th of each month.  Payroll Specialist will review and submit the invoice for payment with AP.

#### CXC Global

* Canada - Payroll Specialist will send payroll changes and expense reimbursement reports to Canada payroll on weekly basis.  CXC will send over an invoice for each payroll for review and submit for payment via AP.

#### Lyra

Payroll changes are due by the 14th of each month.  Lyra will send an invoice by the 15th of each month.  For any additional adjustment, payroll have until the 24th to notify Lyra.  They will invoice the adjustment on the following month invoice.

## Expenses

All team members will have access to Expensify within 2 days from their hire date.  If you didn't receive an email from Expensify for your access, then please contact expenses@gitlab.com. Expense reports are to be submitted once a month, at least. Additional information on getting started with Expensify and creating/submitting expense reports can be found [here.](https://docs.expensify.com/using-expensify-day-to-day/using-expensify-as-an-expense-submitter/report-actions-create-submit-and-close)

The procedure by which reimbursable expenses are processed varies and is dependent on contributor legal status (e.g. independent contractor, employee) and subsidiary assignment (Inc, LTD, BV, GmbH, PTY). Check with Payroll if you are unsure about either of these.

For information regarding the company expense policy, check out the section of our team handbook on [Spending Company Money](/handbook/spending-company-money). Managers and Payroll team will review the expenses for compliance with the company travel policy.  The CEO will review selected escalations at least annually.
Team members should also consider the terms and conditions of their respective contractor agreements, when submitting invoices to the company.

Team members in a US policy will be automatically reimbursed through Expensify after their report is "final approved" within 7 business days by Payroll team. For all other team members, please see the reimbursement process below based on your location or employment status.


##### SafeGuard
Team members who are employed through SafeGuard must submit their expense for reimbursement through Expensify.  All expense reports must be submitted and approved by manager by the 8th of each month to include in the current month payment.

Team members in France, Italy, and Spain must submit their expenses through:
*  Expensify
*  Safeguard in-house expense reimbursement
*  GitLab payroll send the expense approval to Safeguard after the team member's manager approved the report
*  Team members send the original receipts to Safeguard

##### CXC
- Canada:
    * Payroll will submit your approved expense report to CXC payroll for payment.  The typical processing time is about 3-4 weeks due to invoice timeline.
- Poland and Ukraine:
    * Expense reports will be reimbursed by GitLab AP team with the normal weekly Friday AP payment if the report was "final approved" by EOD Tuesday of the same week.  For all other reports, it will be reimbursed the following week.

##### Lyra

* Team members must submit their expenses through Expensify, and Payroll will approve for reimbursement within 5 business days after the approval from the manager.  The reimbursement is through GitLab AP.

##### iiPay

* All Individual contractors or C2C, with exception of Hungary, Nigeria, South Africa, and Switzerland, will be reimbursed by iiPay by the 22nd of each month.  All expense reports must be approved by manager by the 8th of each month to be include in the current month payment.  For contractor with C2C status, be sure to contact Payroll team via email at expenses@gitlab.com if you need to set up a separate bank for your expense reimbursement.

##### Legal entities

* Expense reports for GitLab Ltd (UK) must be approved by the manager on or before the 14th of each month enable for it to include in the current month payroll.
* Expense reports for GitLab BV (Belgium and Netherlands), GmbH (Germany), PTY Ltd (Australia) are reimbursed via GitLab AP within 10 business days from the approval date by their manager.
* Expense reports for GitLab Inc, Gitlab Inc Billable, and GitLab Federal reimbursed via Expensify, and Payroll will final approved the report within 5 business days after the approval from their manager.

##### Hungary, Nigeria, South Africa, Switzerland

* Please include your expenses along with receipts on your monthly salary invoice.
 

##### Non-Reimbursable Expenses

Examples of things we have not reimbursed:
1. Costume for end of summit party.
1. Boarding expense for dog while traveling.
1. Headphones costing $800 which were found to be in excess of our standard equipment guidelines.
1. Batteries for smoke detector.
1. Meals during the summit when team members opt out of the company provided meal option.
1. Cellphones and accessories.
1. Travel related expenses for family members of GitLab employees
1. Fitness equipments (treadmill, etc..) and gym membership

In accordance with [Reimbursable Expense guidelines](/handbook/finance/accounting/#reimbursable-expenses), independent contractors should note which expenses are Contribute related on their invoices, prior to submitting to the company.

**Billable Expenses**
If you have an expense report that can be billed back to a customer please make sure to check the "billable" flag in Expensify along with tagging the customer name under the "customer" field in Expensify.

## Performance Indicators

### Payroll accuracy for each check date = 100%
Payroll is paid on time and accurately for each check date. 

### Payroll journal entry reports submitted to Accounting <= Payroll date + 2 business days
Payroll journal entry reports are to be submitted to Accounting no later than two business days after the payroll date. The payroll journal entry reports submitted dates are tracked in the Monthly Closing Checklist on a monthly basis. 
