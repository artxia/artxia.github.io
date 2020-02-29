---
layout: handbook-page-toc
title: "Financial Planning & Analysis"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Financial Planning & Analysis @ GitLab

## Common Links

 * [Finance Issue Tracker](https://gitlab.com/gitlab-com/finance/issues)
 * [Analtyics Issue Tracker](https://gitlab.com/gitlab-data/analytics) for all data, dashboard, or reporting requests
 * [Slack Channel](https://gitlab.slack.com/archives/fpanda)
 * [Hypergrowth Rule](https://about.gitlab.com/handbook/finance/financial-planning-and-analysis/hypergrowth-rule)

## How to work with us

### On issues

Issues the FP&A team works on have the `~"FP&A"` label.  This applies to both the Finance and Analytics Issue Trackers. This will ensure that expectations are set accordingly and the work gets delievered in a timely and professional way.

The Analytics part of the FP&A team focuses on delivering project based works and at times will assist with ad-hoc analysis.

### Async Status Updates

Since we are a [remote](/company/culture/all-remote/) company, we utilize a Slack plugin called [Geekbot](https://geekbot.io/) to coordinate various status updates. There is currently 1 status update configured in Geekbot:

#### Weekly Status Update
The **Weekly Status Update** is configured to run at noon on Fridays, and contains three questions:

1. ***What progress was made on your deliverables this week?*** (MRs and Closed Issues are good for this)

    The goal with this question is to show off the work you did.

2. ***What do you plan to work on next week?*** (think about what you'll be able to merge or close by the end of the week)

    Think about what the next most important thing is to work on, and think about what part of that you can accomplish in one week. If your priorities aren't clear, talk to your manager.

3. ***Who will you need help from to accomplish your plan for next week?*** (tag specific individuals so they know ahead of time)

    This helps to ensure that the others on the team know you'll need their help and will surface any issues earlier.

#### Retrospectives

The FP&A Team holds a quarterly planning [retrospective](https://docs.google.com/document/d/1XeaPpMRskohFPLvevhPGETiIsMyXzCAdHJkAbdEFJZs/edit?ts=5d8a8dcf#) to discuss what went well and what didn't go well. The team will take action items away from the Retrospective to improve the planning process and overall efficiency at GitLab.

The FP&A Team uses GitLab's Engineering methodology to hold the Retrospectives, which are detailed on the [Team Retrospectives](/handbook/engineering/management/team-retrospectives/) page.

## What is purpose of FP&A @ GitLab?
1. Help drive GitLab’s business value
2. Facilitate execution of GitLab's [strategy](/company/strategy/)
3. Ensure financial and operational goals of GitLab are defined, documented and achieved
4. Evangelize awareness of strategy and each departments role in achieving it
5. Ensure sound decision support

## How GitLab’s FP&A plans to get there….
1. Manage the budget and planning processes for GitLab's [operating plan](/handbook/finance/financial-planning-and-analysis/#operating-plan)
2. Build and maintain an [integrated financial model](/handbook/finance/financial-planning-and-analysis/#gitLab-integrated-financial-model) that projects performance into the future
3. Measure, track and report on GitLab’s [KPIs](/handbook/business-ops/data-team/metrics/)
4. Constantly look for opportunities to improve performance
    - Process Improvements
    - Analytics
    - Education

## Where to find our Models?
1. GitLab Financial Model:  Google Drive -- FP&A >> Models >> GitLab Financial Model
2. Revenue Model: Google Drive -- FP&A >> Models >> Revenue Model
3. Capacity Model(s): Google Drive -- FP&A >> [FBP - Function Owner Folder, i.e S&M] >> Planning >> Capacity Model
4. Rolling 4 Quarter Forecast sheets: Google Drive -- FP&A>> Planning >> [Current Fiscal Year] >> [Current Fiscal Year] Plan >> [Quarter-Year thru Quarter-Year]]
5. Rolling 4 Quarter Forecast Feed sheets for Program Spend & Team: Google Drive -- FP&A>> Planning >> Financial Model >> Feed Sheet
6. Budgets vs. Actuals: Google Drive -- FP&A>> [FBP - Function Owner Folder, i.e S&M]>>  Budget vs. Actuals >> [Current Fiscal Year] >> Dashboard File

## How To Add A New Department into Models
1. Create new departments in each of the R4QF spreadsheets (Programs & People) feed
2. Make sure the new department is rolled up into [Department] tab onto both of the feeds. Right now, you would need to add ’New Department’A5:AF! to the [Department] tab because currently it’s only referring to current departments
3. Add new department to Headcount rollup
4. Make sure the new department is in the Compensation, Base Salary, Benefits, and T&E tabs of the Capacity model
5. The New Department needs to be added to the Account Based Department Budgets tab
6. Ping Financial Analyst in order for the new department to be added in the Allocation Accounts tab and Department Post Allocated Budgets tab in GitLab Financial Model
7. Everything else should flow through after that

For new department approvals and more detail on the process, please reach out on the #fpanda channel in Slack for desktop procedures.

## GitLab's Operating Plan vs Integrated Financial Model

#### Operating Plan

GitLab's operating plan is a guideline to understand how much capital it needs and how the capital will be consumed. The operating plan helps GitLab answer questions like "how fast can we hire and when?" The operating plan consists of three main components: the revenue model, the rolling 4 quarter forecast and the budget. The operating plan can also be considered a bottom-up plan.

- The revenue model predicts new business based on the [growth persistence model](/handbook/finance/financial-planning-and-analysis/#forecasting-growth-using-a-growth-persistence-model) and growth from existing business based on net retention assumptions. Understanding how much revenue is anticipated determines how much capital will be needed for growth in the foreseeable future.

- The [rolling 4 quarter forecast](/handbook/finance/financial-planning-and-analysis/#rolling-4-quarter-forecast) builds off of the revenue projected in the revenue model. During the rolling 4 quarter, departments build out plans to help meet their strategic goals. Understanding the departmental plans determines how much of the capital will be consumed for foreseeable future.

- The [budget](/handbook/finance/financial-planning-and-analysis/#budgeting-@-gitLab) looks to GitLab's [long term profitiablity goals](/handbook/finance/financial-planning-and-analysis/#long-term-profitability-targets) and incorporates plans made during the rolling 4 quarter forecast in addition to revenue forecasts from the revenue model. In order to have a budget, GitLab must have a forecast(s) for it's operating plan. Therefore, the revenue and rolling 4 quarter forecasts are critical to set budgets. Budgets help GitLab understand how it's spends its cash and help predict long term targets, but ultimately budgets are a guideline.

#### Integrated Financial Model

GitLab's [integrated financial model](/handbook/finance/financial-planning-and-analysis/#gitlab-integrated-financial-model) is synonymous to its operating plan, but the integrated financial model is based soley on [business drivers](/handbook/finance/financial-planning-and-analysis/#business-drivers). The integrated financial model dynamcially answers questions like “What are our limits in comparison to the total addressable market?” and provides "What-if" scenarios. The integrated financial model also helps set the long term profitablity goals. GitLab has established business drivers in each function of the business and continues to refine them to ensure its tracking accordingly. The integrated financial model can also be considered a top-down plan.

## Operating Plan

### Forecasting Growth Using a Growth Persistence Model

Scale Venture Partners developed a [Growth Persistence Model](https://www.scalevp.com/blog/predictable-growth-decay-in-saas-companies) based on research on private and public software companies. The Persistence Model shows that ARR growth rates typically decline year over year, with each year’s growth being, on average 85% to that of the preceding year. We use this methodology to set our growth targets.

### Operating Plan Diagram
![alt text](/handbook/finance/financial-planning-and-analysis/financial-workflow.png "Operating Model")

### Planning @ GitLab

****

### Making Changes to the Plan to Optimize for Growth

Our Plan is intended to ensure that the Company has sufficiently considered what is required to support the Company's financial goals. The Plan ensures that there is accountability across all divisions that can be measured. The Plan is not intended to represent a cap on what we can invest in support of maximizing the growth of the Company.  We encourage our team members to actively seek opportunities that will help us grow faster. Those growth initiatives will be evaluated, as follows:

1. If the investment will allow us to exceed our IACV plan by at least an equal amount in the current year we will do it. The e-group will be informed of the increased spend and anticipated impact.
1. If the increased spend will allow us to exceed our IACV targets next year then we will quantify the impact and raise our financial guidance for the following year. The e-group will review these investments and will, in some cases, request board approval for relief against current year planning targets.
1. If we need to exceed spend to achieve our current plan we should review as an e-group and inform the board. We won't necessarily get plan relief unless there are extenuating circumstances but we will do what is right for the business.

####  Rolling 4 Quarter Forecast

GitLab creates an annual Plan which establishes our financial objectives for the coming [fiscal year](/handbook/finance/#fiscal-year) and is used for measurement of the Company's ability to achieve goals. Things move quickly and our forecast needs to iterate quickly to keep up with the business. Accordingly, we run a rolling 4 quarter forecast process. This means that we are always looking out a minimum of 12 months when projecting revenue and expenses, and we update those forecasts at least once per quarter.  We plan our expenses at a high level (e-group) and we expect this group to make prioritizations and trade-offs while remaining accountable against the plan parameters. By reforecasting quarterly, we can quickly evaluate and incorporate new initiatives into our forecasting model. That being said, we do follow an annual plan to set our goals and measurement for our top-level targets of revenue, profitability and expense management.

#### Tips - Rolling 4 Quarter Forecast

- Meeting each department and function leader prior to the planning cycle is a must and useful for building long term relationships. Set up a coffee chat to do an informal intro.
- Having a Rolling 4 Quarter Forecast kickoff helps everyone know that the planning cycle is about to begin.
    - This should generally occur 3-4 weeks out before the planning cycle starts and should be communicated through as many channels as possible (Slack, Team Calls, Company Call, etc)
- Scheduling invites 3-4 weeks out with department and function leaders around the same time as the kickoff is important. This helps get on everyone's calendar and ensure topics are not rushed
    - Having a templated calendar invite helps save time. There will be multiple folks involved in the process, broken out by each function.
    - It also helps if the Rolling 4 Quarter Forecast models are up to date prior to meeting. This would include the current team, planned hires, and program spend so leaders have a clear guide during the meeting. It won't be perfect and will inevitablty change during or shortly after the meetings, but this is an efficient way to make the meetings productive.
    - Meeting with the function leads after the department leads help tie everything together. However, if possible, it can be beneficial to meet with the function leads before and after to ensure buy in and close any gaps.
- When applicable, it is important to always include the function operation leads to the meetings so they can help faciliate any work or changes during or after the meetings.
- Continously gather feedback from stakeholders on what can be done more efficient
- Planning is a team sport. It requires effort and communication on all sides to make it work well. Build the relationships, be patient, and be humble as some folks have less experience with planning while others have a lot of experience.

**Note: During the last quarter of the year, GitLab runs a 5 quarter forecast that aligns with it's annual planning efforts.**
### Updating Budget vs. Actuals
****

1. Open file: FP&A > Templates > Corporate F&A > Open 'Budget vs. Actual' Blank File GSheet
*  Please note that Budget vs. Actuals for all departments already exist within the FP&A Shared Drive
2. Open Netsuite and go to Budget vs. Actual report
*  Download the spreadsheet and copy & paste into the relevant month (e.g. For March 2019, paste into the March 2019 BvA Tab)
3. Open Netsuite and go to 'Income Statement Detail with JE name data' report
*  Copy / paste spreadsheet into the relevant month (e.g. For March 2019, paste into the March 2019 Detail Tab)
4. Once these spreadsheets are loaded in the spreadsheet, the numbers should auto-populate for the relevant months

### Campaign Finance Tag Verification Process
****

The Finance Business Partner for Marketing will review transactions within the general ledger accounts for marketing program expense (6100’s) on a weekly basis to ensure that campaign tags are present. An exception report will be delivered to the Marketing Operations team either validating that all tags are present, or pointing out those transactions where the tag is missing. Marketing Operations will then work with the Marketing team to add back the missing tags.

A live dashboard to assist in identifying these transactions can be found in Sisense, but it is not linked here due to the sensitive nature of this data. The weekly desktop procedures for this process are as follows:
1. Monday morning- the financial analyst will use the Sisense dashboard to pull transactions from the 6100 Marketing account without campaign tags. This data will be transferred to a Google Spreadsheet and the link will be shared in the ongoing issue.
1. Wednesday- the Marketing Operations team will update the Google doc with the appropriate tags
1. Friday- the Accounting team will will work through the new tags and get them appropriately accounted for


### Monthly Investor Update

****

Each month we send to our investors an update no later than the 10th day following the end of the month. For further reference see our [blog post](/blog/2018/10/17/how-we-keep-investors-in-the-loop/).
#### Format
1. Thanks
1. Asks
1. Key Metrics
1. Lowlights
1. Highlights
1. Expectations (next month)

#### Process
1. On the 1st day of the month, the FinOps lead prepares a draft of the previous months investor update in a google document and posts in the #investor-update slack channel.
1. On the same day the draft is added to the #investor update slack channel, the FinOps lead will `@mention` e-group members with asks for topics related to the investor update agenda.
1. The e-group members will have no later than the 9th of each month to review and add input.
1. No later than the 10th of each month the will CEO send the update to the investor mailing list.
1. Once the investor update is sent to the investor mailing list, the FinOps lead will add the current investor update to the #investor-update slack channel, along with highlight commentary on GitLab's operating metrics.

#### Relevant Locations for Investor Update Process

##### Revenue Model & Metrics Tab within the Financial Model

**1: Sales Metrics 2019 Monthly Metrics**
* Gross New IACV → New IACV (Revenue Model)
* Gross Growth IACV → Growth IACV (Line 14 Revenue Model)
* Expiring Subscriptions gets updated once every 3 months
* Won Renewal ACV → Renewal ACV (Line 8 Revenue Model)
* Lost Renewals ACV + Growth Downgrade IACV + Growth Refund IACV + New Refund IACV + New Downgrade IACV → Lost Renewals, Credits, Downgrades (Line 11 Revenue Model)
* Update new month with % of Lost Renewals, Credits, Downgrades
* TCV --> filter out Professional Services, sum all relevant information, & in Revenue Model paste number in Line 34 for TCV
* Double check to see if Revenue model Net IACV = Net IACV in Sales Metrics Sheet
* Note: ACV on Sales Metrics Sheet will not equal ACV on Revenue Model because of Professional Services in the Sales Metrics Sheet

**2: Sisense**
* Exit ARR --> Filter data by current MRR month & then sum using (=subtotal(109, ARR column))
* Retention
* Licensed Users --> Make sure EDU & OSS are excluded
* Active Hosts
* Customer Count By ARR

**3: Metrics Report (SFDC)**
* Gives an overview of what happened within the stated month

**4: All Pipeline Report (SFDC)**
* Relevant number is the Grand Total Sum
* Make sure the month is correct

**5: Late Stage Report (SFDC)**
* Relevant number is the Grand Total Sum
* Make sure the month is correct

**6: Orders Processed Report (SFDC)**
* Ensure that closed deals are updated for the month (Bottom of Funnel Forecast Line 56 - 64)

**7: Revenue Spreadsheet sent from Controller**
* Non-GAAP Revenue -> Pull grand total and input into Line 29 in Revenue Model

**8: Cash Flow Forecast (Accounting Will Send Over -- typically within the 4th of the Month)**
* Step 1: Find Ending Balance for Latest Month (Line 60)
* Step 2: Add to Financial Model Balance Sheet

**9: Pingdom**
* GitLab.com Availability, Response Time

**10: LTV for Metrics**
* LTV with DCF Tab (Line 116)
* Go back to the Metrics Tab (Current Month and 2 Months Prior -- get the average)
* Put that average number * .90 (GM) in Line 116
* Pull LTV number into Line 123 & input into Financial Model

**11: BambooHR**
* To get updated team members number -- check Income Statement Monthly
* If not updated within IS Monthly, go to BambooHR and pull actuals --> Put new numbers into IS Monthly (Lines 47 - 51)

**12: Zendesk**
* Step 1: Reporting --> Insights
* Step 2: Corp Dash - OKR Overview should have the relevant information for Customer Support
* Put them in the metrics tab (Line 8,9,& 10)

**13: Snowflake**
* Get GitLab.com Licensed Users --> Filter down by product category (Bronze, Silver, & Gold) --> Get grandtotal of each category and overall
* Additionally, Add Revenue for each Product in the GitLab.com Model --> Information comes from Revenue spreadsheet listed above (Number 7)

**14: Sales Pipeline Analysis**
* Model is being updated & TBD

#### Once Metrics & Financial Model Are Completed for Investor Update Process
* Add relevant numbers to the GitLab.com & GitLab Allocation Model
* Copy All of Metrics Tab in the Financial Model & Paste it in Static Metrics Sheet
* *Note:* Remember to remove forecast, format new month to actual (from orange to light blue), copy/paste hyperlinks for names within static sheet, & anything in the previous month that was italicized needs to be back to normal.

### Budgeting @ GitLab

GitLab uses several different methods to budget specific revenue and expenses. During the Rolling 4 Quarter Forecast planning process GitLab may use one of the following methods to allocate revenue or expenses.

#### Spreading

Recording activities based on the percentages across a certain time period. This can either be on a percentage spread or an amount spread

#### One Time Adjustments

Recording activities based on a one time basis across a certain time period. These activities are geared toward, but not limited to, marketing expenses.

#### Headcount Growth (+/-)

Recording activities based on headcount growth across a certain time period.

****

### Out of Budget Business Case

In the event an organization is asking to spend money outside either the [Annual Plan](/handbook/finance/financial-planning-and-analysis/) or [Quarterly Forecast](/handbook/finance/financial-planning-and-analysis/), you should develop a business case showcasing what the spend is for and how Gitlab can benefit from spending it.

This business case should be completed in conjunction with your [Finance Business Partner (FBP)](/handbook/finance/financial-planning-and-analysis/) to articulate the financial impact of the request.  Below are a few examples of the question you should be trying to answer:
* What is the purpose of the spend?
* How much is the spend?
* What kind of spend is it? (One time, contract, utility-based, etc..)
* What is the Return on Investment?
* If the ROI cant be measured what KPI are we trying to move?
* Can we measure the impact in terms of ROI or KPI improvement?
* Have we investigated any other options?

Together with your FBP , this analysis should be presented to your leader for approval.

### Monthly Finance Planning Meeting

#### Purpose

Each month after the financials have been published, GitLab reviews department spend data in detail. The goal of this analysis is to compare department budgets with actual results and examine any material discrepancies between budgeted and actual costs. These costs are reviewed at the divisional department level, allowing GitLab to measure progress in meeting its plan, forecast, and operating model. During the meeting, the Finance Business Partners will review GitLab results in addition to a detailed overview. Each division can expect to review the following during the monthly meetings:

1. Company results
   -  Bookings IACV, TCV
   -  Spending OpEx vs Plan
1. Divisional level review
  - Last month and last fiscal quarter (once per quarter)
1. Department level review
  - Last month and last fiscal quarter (once per quarter)
1. Review next 4 quarters vs Plan for the Division and for each department

#### Process
Following the month-end close, the Finance Business Partners will distribute department income statements to the related budget owners and the e-group members. Each department is then responsible for comparing these reports, which contain actual costs, to the budget. Departments, with guidance from the Finance Business Partners, should analyze their data and if necessary, discuss items of interest and take appropriate action. Any questions regarding the cost data should be discussed with the Finance Business Partner.

#### Timing
1. The Accounting Manager will send the income statements on or before the 15th of each month.
1. The Finance Business Parters will prepare a templated budget vs actual reporting package for distribution to the divisional and departmental leaders.
1. With guidance from the Finance Business Partners, each division and department leader will review the budget vs actuals in the same month.

#### Expense Controls and Improving Efficiency
1. The primary mechanism to ensure efficient spend of company assets is the [Procure to Pay](https://about.gitlab.com/handbook/finance/procure-to-pay/#procure-to-pay-process) process, and specifically completion of the [vendor and contract approval workflow](https://about.gitlab.com/handbook/finance/procure-to-pay/#vendor-and-contract-approval-workflow) prior to authorization. The procurement team or your finance business partner can assist with questions related to this process.  

1. The second mechanism is the budget vs actual review to determine reasons for variances vs plan.

##### Vendor and Contracts Approvals Tracking for Marketing Programs Spend
1. The Marketing FP&A team maintains a status document containing the finance issues submitted by the marketing organization for approvals.
1. This dynamic list contains links to the issues, start dates, budgeted amount, approval status (y/n), and other pertinent details such as department. The list is kept current with updates on a weekly basis.
1. Please contact the Finance Business Partner for Marketing with questions concerning this information.
***

#### Variance Analysis
The study of differences between budgetary and expected cost. At GitLab, different measures of materiality thresholds are measured during the variance analysis process, including the Monthly Finance Planning Meeting. During the variance analysis processs the GitLab FP&A team analyzes and isolates any variance in question to the lowest level possible. The team reviews detailed items in order to identify the root cause of the variance. This could include transaction date, cost center, vendor, location, department or additional low level details.

At GitLab, analysts begin the variance analysis process with trended data to understand if there is a recognizable pattern. This helps determine if the variance was caused by incremental change or driven by one particular event and helps identify the root path quickly.

The FP&A team takes the following into consideration while evaluating variances in relation to materiality thresholds:

- The percentage size of the misstatement (i.e. what was the overall varinace by percentage)
- The intent of the misstatement (i.e. did something stand out as deceptive)
- The correlation to other misstatements (i.e. did a immaterial difference in one place cause a material difference in another)
- The inherent character of the mistake (i.e. does the expense correlate to the traits of the business)

#### Marketing Specific Monthly Variance Analysis
In partnership with Marketing Operations and Accounting, we set out to improve the timing and accuracy of budget vs. actuals tracking for marketing programs opex and to provide data driven insights to these teams during the close process by BD3 at the beginning of a new monthly accounting period. 

The utilization of [campaign finance tagging](https://about.gitlab.com/handbook/marketing/marketing-operations/#campaign-cost-tracking) for marketing program spend enables month-end reconciliation of expense actuals, prepaids, and accruals at the budget line item level. The components of this analysis are as follows:

1. **Actuals:**
    - Prepaids provided by accounting on BD2 in a new monthly accounting period, grouped by campaign finance tag
    - Transactional ledger detail of expenses grouped by campaign finance tag. This can be pulled using the Marketing Campaigns Tagging Dashboard in Sisense, or an income statement in NetSuite.
1. **Budget totals:**
    - Using the Marketing_Non-HC_R4QF_FY21 budget document, join the datasets based on campaign finance tagging to pull the relevant line items from the budget. 

Once these components are in place, a comparison showing the difference between budget vs. actuals may indicate the need for an accrual or indicate a budget overage. The finance business partner can then take appropriate action with the accounting team or the business to resolve. The basic structure of this analysis should resemble the following:

| Campaign Finance Tag | A: Expense | B: Prepaid (GL Acct# 1150) | C: Total (A+B) | D: Budget line item | E: Variance (D-C = Potential Accrual/Overage) |
| ------ | ------ | ------ |------ | ------ | ------ |
| ISOdate_CampaignShortName | $000's | $000's | $000's | $000's | $000's |

### Campaign Finance Tag Verification Process
****

The Finance Business Partner for Marketing will review transactions within the general ledger accounts for marketing program expense (6100’s) on a weekly basis to ensure that campaign tags are present. An exception report will be delivered to the Marketing Operations team either validating that all tags are present, or pointing out those transactions where the tag is missing. Marketing Operations will then work with the Marketing team to add back the missing tags.

A live dashboard to assist in identifying these transactions can be found in Sisense, but it is not linked here due to the sensitive nature of this data. The weekly desktop procedures for this process are as follows:
1. Monday morning- the financial analyst will use the Sisense dashboard to pull transactions from the 6100 Marketing account without campaign tags. This data will be transferred to a Google Spreadsheet and the link will be shared in the ongoing issue.
1. Wednesday- the Marketing Operations team will update the Google doc with the appropriate tags
1. Friday- the Accounting team will will work through the new tags and get them appropriately accounted for

### Types of Threshold

Generally accepted accounting principles (GAAP) does not provide definitive guidance in distinguishing material information from immaterial information. Therefore, GitLab uses a percentage based approach for defining materiality thresholds and can be found below. The [Plan vs Actuals vs Forecast](https://app.periscopedata.com/app/gitlab/525851/Plan-vs-Actuals-vs-Forecast) Sisense dashboard provides the data for the threshold analysis via a color coded legend.

#### Revenue Thresholds

The total is inclusive of all Revenue activities including subscription, professional services, swag shop and other revenue streams.

- `< 5% of plan OR < $0 is considered immaterial`
- `> 10% AND > $10,000 of plan is considered material`
- `5-10% OR $0 - $9,999 of plan is subject to judgement and review`

#### Cost of Goods Sold Total Threshold

The total is inclusive of all COGS activities including Customer Support, Professional Services, and other allocation expenses.

- `< 5% of plan OR < $0 is considered immaterial`
- `> 10% AND > $10,000 of plan is considered material`
- `5-10% OR $0 - $9,999 of plan is subject to judgement and review`

#### Operating Expense Total Threshold

The totals are exclusive of the sum of operating expenses. Each operating expense line item (i.e. Sales, Marketing, R&D, G&A) should be measured on a line item basis

- `< 5% of plan OR < $0 is considered immaterial`
- `> 10% AND > $10,000 of plan is considered material`
- `5-10% OR $0 - $9,999 of plan is subject to judgement and review`

#### Individual GL Accounts

- `< 5% of plan OR < $0 is considered immaterial`
- `> 10% AND > $10,000 of plan is considered material`
- `5-10% OR $0 - $9,999 of plan is subject to judgement and review`

### Logging Threshold Differences
1. As part of closing tasks, Financial Analyst will create issue for [Threshold Analysis](https://gitlab.com/gitlab-com/finance/blob/master/.gitlab/issue_templates/threshold_analysis.md) for the current month.
2. Finance Business Partners will need to enter expenses that have exceeded thresholds within the created issue.
3. Finance Business Partners will also need to add commentary to expenses that did exceed our thresholds as well.
4. Once issue is completed, Financial Analyst will apply Threshold Analysis label to each completed issue. This will help us keep track of all our threshold analysis issues through the months.

***

## Calendar of Events

We follow the cadence below in our planning process:

Throughout the year the Executive Business Partner team puts together a calendar of events for board members and other events associated with planning. Those events can be found in the [GitLab Board Calendar](https://docs.google.com/spreadsheets/d/1GW59GiT0MLXEgMxy2bN0ZVcbMs_wssOkP2c59f19YTk/edit?usp=sharing) sheet.

## Monthly Update
* Hold Departmental Metrics Meetings to review how well the departments are operating.
* Send out Investors Update
* Update our Budget vs Actual model with revenue, expense and headcount actuals.
* Perform an actuals vs  budget and forecast variance analysis and generate variance package.
* Distribute monthly results to budget owners.

###### Monthly Important Dates
* **10th of the Month** - Update Metrics Report
* **10th of the Month** - Update Revenue Model
* **10th of the Month** - Send out Investors Update
* **15th of the Month** - Update Financial Models
* **15th of the Month** - Distribute monthly results to budget owners

****

### Quarterly Forecast
* All of the activities in the Monthly Forecast.
* Budget owners update headcount planning templates and non-headcount expenses.
* Revenue model updated and signed off by CMO and CRO.
* Generate locked rolling forecast for the quarter for variance

###### Quarterly Important Dates
* **14th of the Last Month in Fiscal Quarter** - Send out calender invites to review non-headcount & headcount expenses
* **22th of the Last Month in Fiscal Quarter** - Finalize non-headcount & headcount planning with departments
* **22th of the Month** - Finalize Revenue Model signoff from CMO and CRO

****

### Annual Plan
* All of activities above.
* Revise and update the annual sales compensation plan.
* Set annual quota assignments for revenue producing roles.
* Review product investments vs expected revenue generation.
* Set expected amount for annual compensation increases.
* Set targets for any contributors on a company based performance plan.
* Set company targets for board, investors and creditors.
* Our Annual Plan is viewable internally as a google slide presentation.  Search on "[current year e.g. 2018] Plan" to view.
* Build out bottoms up integrated sales and marketing financial model with key assumptions documented so they can be tracked
* Generate a financial plan based on a headcount list, tbh list, vendor level spend list
* Headcount list communicated to recruiting, proposed vendor list communicated to procurement (future with Purchase Orders in place for existing vendors)

###### Annual Planning Important Dates
* **28th of October** - Five quarter rolling forecast kick-off
* **22nd of November** - Five quarter rolling forecast completed
* **22nd of November** - Sales Compensation Direction
* **2nd of December** - Preliminary outlook reviewed at Board of Directors
* **16th of December** - Plan iteration and discussion at egroup meeting
* **18th of December** - Product Roadmap and Investments (board review)
* **17th of January** - Go to market planning deep dive (board review)
* **24th of January** - Plan sent to Board for async commentary
* **31st of January** - FY21 Plan Approved by Board
* **7th of February** - Sales compensation plans distributed to sales team

### Terminology
* Plan is the term we used for the current plan of record which has been approved by the Board.  Typically this is set at the beginning of the year.
* Forecast is a dynamic assessment based on current expectations of financial performance.
* Target is a goal or objective that may be higher or lower than the Plan or Forecast. Targets are typically used in conjunction with setting OKRs, compensation plans or other performance objectives.
* Baseline is a measurement of actual expense or revenue that relates to a certain point in time (i..e month, quarter or year). We use baselines to measure progress of improvement against actual results. The progress can be stated in monthly, quarterly or annualized terms.
* Actuals are results that have been reported or exist in a system that is designated as a single source of truth for the item that is being measured.

## GitLab Integrated Financial Model

### Business Drivers (also known as Gearing Ratios)

At GitLab, planning starts with long term goals. GitLab uses business drivers to forecast out long term goals by division. By using division specific business drivers that tie into the long term goals, GitLab is able to quickly and dynamically shift priorities based on external or internal changes.

Business drivers are the key inputs and activities that drive the operational and financial results of a business.[^3]

## Long Term Profitability Targets

Our long term profitability target for EBITA (Earnings Before Interest Taxes and Amortization) is 20% of revenue.
Our long term gross margin target is 85% but is dependent on the revenue mix between products - self managed and [gitlab.com](/handbook/product/#long-term-financial-success-criteria-for-gitlabcom) and [professional services](/handbook/customer-success/professional-services-engineering/#long-term-profitability-targets). Gross margin is defined as total revenue less cost of revenues as defined by GAAP and reported in the Company's financial statements. This analysis can be found on the [Finance Dashboard](https://app.periscopedata.com/app/gitlab/483606/Finance-KPIs).
Other financial planning targets are described in the divisional area (e.g. sales, marketing, development, etc.) in this handbook. We plan to achieve our long term profitability target as our revenue growth rate approaches 30%.
The long term target for operating expenses as a percentage of revenue for G&A is 10%.

| Division | Long Term Target  |
|---|---|
| Cost of Sales  |15% of Revenue   |
| R&D  | 20% of Revenue  |
| Marketing  | 12.5% of Revenue  |
| Sales   | 22.5% of Revenue  |
| G&A  | 10% of Revenue  |
| **Total**  | **80% of Revenue**  |

### FY20 Financial Planning Goals

| Division | FY20 Expense Target  |
|---|---|
| Customer Support  |10% of ARR   |
| Customer Solutions  | 80% of PS Recognized Revenue  |
| Engineering  | 70% of IACV  |
| Sales  | 75% of IACV  |
| Marketing   | 45% of IACV  |
| G&A  | 10% of Total Operating Expense  |

## <i class="fas fa-users fa-fw icon-color font-awesome" aria-hidden="true"></i> FP&A Team Responsibilities

### Manager, Financial Planning & Analysis

###### Responsibilities

1. Coordinates Monthly Investor Update
1. Coordinates Rolling 4 Quarter Process
1. Coordinates Annual Planning Process
1. Ensures GitLab's financial model and forecast is accurate
1. Partners with Business Operations to ensure Financial Systems & Integration Roadmap
1. Develops data processes in partnership with the Data team
1. Responsible for financial and mechanical integrity of the operating model and street model

#### Performance Indicators

##### Budget, Forecast Creation Cycle Time

Measures the number of days from Rolling Forecast Kickoff to Quarterly Board Meeting. The time period is quarterly. The target is 30 days.

##### Team Morale Score

Measures the team morale by using the tool [Lead Honeslty]( https://leadhonestly.com/).  The time period is monthly, but will use a weekly average based on weekly 1:1s. The target is 9 on a scale from 1-10.

[Position Description](/job-families/finance/finance-planning-and-analysis/){:.btn .btn-purple}

### Finance Business Partner

###### Responsibilities

1. Reviews BvsA Analysis with e-group member (or designee)
1. Responsible for leading the Rolling 4Q forecast process
1. Building integrated financial model with gearing ratios for business.
1. Coordinates Monthly KPI and OKR prep
1. Maintain and develop KPI definitions for divisional business units
1. Develops and maintains cost and efficiency benchmarking
1. Develops and maintains Unit economic analysis
1. Partners with division leaders to ensure financial and key metric forecast accuracy of supported division
1. Provides Adhoc Analysis to supported division leaders
1. Helps business group negotiate Vendor Contracts
1. Develops and maintains compensation modeling

#### Performance Indicators

##### Number of days to release variance analysis to business leaders
Measures the number of days from [month end close](/handbook/finance/accounting/#average-days-to-close-kpi-definition) to release variance analysis to business leaders. The target is five business days.

##### Plan vs Actual
Measures the percentage deviation between the actual costs and the planned costs over the same time period. The time period may be monthly, quarterly, or yearly. The target deviation percentage is +/- 1.5%.

Percentage Deviation= (actual expenses-planned expenses)/planned expenses * 100

[Position Description - Engineering Specific](/job-families/finance/finance-business-partner/){:.btn .btn-purple}

[Position Description - Sales Specific](/job-families/finance/finance-business-partner-sales/){:.btn .btn-purple}

### Financial Analyst

###### Responsibilities

1. Reviews BvsA Analysis - G&A Division
1. Partners with Recruiting on hiring plan
1. Develops and maintains contract & renewal projections
1. Develops and maintains monthly audit projects
1. Develops and maintains planned vs actuals GitLab Team analysis
1. Reviews BambooHR to ensure GitLab Team are in the correct divisions and departments

#### Performance Indicators

##### Time to compile variance analysis reporting
Measures the days from Accounting Close to distrubtion of Budgets vs Actuals to Finance Business Partners. The time period is monthly. The target is 1 day after Accounting close.

##### Time to complete investor update reporting
Measures the days from 1st of month to release of the investor update. The time period is monthly. The target is 1 day after Accounting close. The target is 5 days from 1st of the month.

[Position Description](/job-families/finance/financial-analyst/){:.btn .btn-purple}

### Data Analyst, Finance

###### Responsibilities

1. Support the FP&A team in driving financial and operational initiatives by analyzing data and discovering insights
1. Focus on financial and operational specific data
1. Priorities will be set by the Financial and Operations Lead but will collaborate with and report into the Data Team
1. Expand our data warehouse with clean data, ready for analysis
1. Understand and document the full lifecycle of data from numerous sources and how to model it for easy analysis
1. Build reports and dashboards to help teams identify opportunities and explain trends across data sources
1. Follow and improve our processes for maintaining high quality data and reporting
1. Implement the DataOps philosophy in everything you do
1. Build upon and document our common data framework so that all data can be connected and analyzed

#### Performance Indicators

##### Adoption of Data Team BI Charts Throughout the Company

Measurements can be found under the Data Teams [Performance Indicators](/handbook/business-ops/metrics/#adoption-of-data-team-bi-charts-throughout-company)

[Position Description](/job-families/finance/data-analyst/){:.btn .btn-purple}


## Department Structure

### Creating New Departments
Successfully creating new departments require that various company systems be updated to capture newly defined department structures. Once the need for a new department arises, follow these steps:

1. Create an issue using the *dept_change* template.
2. In the issue, add the appropriate team members from each department included in the checklist.
3. Disclose the nature of the new department. Is the new department simply a name change, or there is a structural modification?
4. Provide all detail necessary to ensure team members are assigned to the newly created departments.

Below is a table showing the structure of GitLab departments as they exist in BambooHR and netsuite. Please [check out the Team Page](/company/team/org-chart) to see our org chart.

## Cost & Reporting Structure

At GitLab, the lowest level of tracking reporting structure starts with departments. For reporting and accounting purposes, departments are assigned both a cost center and a division.  In certain cases, a department may span multiple cost centers based on GitLab's allocation methodology.

The cost center, divison, and department reporting structure can be found in the Data Team repo located below. In efforts to keep a single source of truth for organizational and reporting purposes, the Data Team maintains any changes implemented by the FP&A team as a result of an organizational change.

[Cost & Reporting Structure](https://gitlab.com/gitlab-data/analytics/blob/master/transform/snowflake-dbt/data/cost_center_division_department_mapping.csv)

#### 1. Cost Center

A grouping of departments within GitLab to which costs may be charged for accounting purposes.

#### 2. Division

A grouping of departments in which specific activities are carried out within GitLab. Aligning specific departments to divisions ensure the proper operations and efficiency for supporting and creating value for GitLab's customers.

#### 3. Department

An area of special expertise or responsibility within a GitLab division.

## Allocation Methodology

GitLab allocates cost items based on consumption of resources or headcount. Below are the workflow and diagrams that illustrate how various cost items are allocated:

### Workflow

#### Pre-Allocation P&Ls

The grid highlighted as `Pre-Allocation P&Ls` in the diagram below highlights what GitLab P&L structure would look like if there were no allocation methodology. The grid represents Cost Centers and Departments that fall within those Cost Centers. In order to support different dimensional P&Ls and ensure expenses are flowing to the proper Cost Center, GitLab applies an allocation methodology. Therefore, the `Pre-Allocation P&Ls` is meant to provide clarity and be a starting point to the allocation methodology process.

#### Allocation Methodology

The grid highlighted as `Allocation Methodology` in the diagram below highlights the specifc processes that occur in order to achieve proper expense allocations to their respective Cost Centers.

###### Step 1: Yellow Process

The allocation methodology is applied to the G&A Company Allocation department. Items that are recorded to the G&A Company Allocation department are software expenses and one off expenses. The software expenses are for software used by the entire company (examples include gmail and slack). At times one off expenses are also recorded to the G&A Company Allocation department (examples include Contribute, payroll service fees, etc).

While credit card processing fees are not allocated company wide, it is important to call out the distinction of applying credit card processing fees to Sales. GitLab does not consider credit card processing a cost to it's product or service. GitLab believes that its credit card processing fees are more appropriately classified as marketing and selling expense because these fees are related to the cash collection process for completing customer orders, which supports sales and marketing classification.

**Note:** One thing to note during the Yellow Process is the Infrastructure expenses are removed. Infrastructure is allocated during the next phase of the allocation cycle. Therefore no shared expenses will hit the Infrastructure P&L.

###### Step 2: Red Process

The allocation cycle for GitLab's SaaS offering [GitLab.com](https://gitlab.com) starts. The Finance Business Parter for R&D maintains an allocation model to provide Accounting with an allocation breakout of expenses as well as a P&L based on allocation. The model can be found by searching My Drive > GitLab.com Model. The allocation for GitLab.com is broken out into two different methods.


1. Free vs Paid Users
   - Infrastructure
   - 3rd Party Expenses [i.e. Hosting Services]

1. Percentage of Revenue
   - Customer Support

- Allocation for Infrastructure and 3rd Party expenses are based off of usage from free, paid and internal users of GitLab.
- Allocation of Customer Support are based off of expected revenue from GitLab's self hosted and SaaS offerings.

These allocation breakouts will be documented in the GitLab.com model and will flow into the Post Allocation P&Ls. GitLab allocates these expenses to 3 Cost Centers

1. Marketing - Free users
1. R&D - Internal users
1. Cost of Sales - Paid users


###### Step 3: Blue Process

The Blue Process, which encapsulates the Yellow and Red process, is meant to bring the full allocation cycle together before the Post Allocation P&Ls are rendered.

#### Post Allocation P&Ls

The grid highlighted as `Pre-Allocation P&Ls` in the diagram below highlights the final process during the allocation cycle. As a result, new P&Ls are generated to show the breakout of the Infrastructure team across Cost Centers as well as GitLab.com.

### Diagram

[![alt text](/handbook/finance/financial-planning-and-analysis/allocate.png "P&L Breakout")](https://drive.google.com/drive/folders/1hPZll6nWRk5waMTATJV9f4TojCSTxpCI)

## Misc

### Creating & Updating Models

If you create and/or update to a model that materially impacts it, please make sure to make a quick note of what you did in the [ChangeLog](https://gitlab.com/gitlab-com/finance/blob/master/changelog.md). This is important because it keeps us on all the same page.

**Note: At this time, GitLab use's the term `Division` to describe the makeup of its internal structure. In the future, the plan is to use the term `Function` to describe it's internal structure.**
