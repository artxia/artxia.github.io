---
layout: markdown_page
title: "104 - Epic Templates - Repeatable sets of issues"
---
## Objective:

 Often you need to manage a set of consistently repeating events, where multiple issues are used to track the combined activity of a team.  This page describes how to utilize [GitLab Issue Import](https://docs.gitlab.com/ee/user/project/issues/csv_import.html) and a few spreadsheet tricks to make it possible to create a repeatable set of issues for future projects.

 The Issue `Import CSV` button is at the top of the GitLab project issue list.  This feature can be very useful for repeating projects with similar groups of issues / work.

  ![0 - Import CSV](/handbook/marketing/product-marketing/images/0-import-issue-button.png)

### Please read the "Tips and Tricks" section before you import issues into your projects:

### Assumptions:

1. You're familiar with the GitLab structure of how projects, groups, epics, milestones, issues, and labels work.  If not, please review [GitLab 101- No Tissues with Issues](https://about.gitlab.com/handbook/marketing/product-marketing/getting-started/101/)

2. You're comfortable working in a spreadsheet and using formulas to [concatenate](https://support.google.com/docs/answer/3093592) text into a cell.  note: In my examples, I use the `&` operator, which is the same as the `concat` function.

3. You have Developer permission level or higher in your project. (required to do issue import)

---

### Background:

1. Issue `Import CSV` is **really simple**.  It requires only two columns,
  - title
  - description
<br>
<br>Where the issues are in a coma delimited file. The first row is the header and the subsequent rows include the data.

2. Issue `Import CSV`  is **really powerful**. It allows you to use the [/Quick Actions](https://docs.gitlab.com/ee/user/project/quick_actions.html) to do cool things to your new issues like:
- add labels
- set due dates
- add to milestones
- add to epics
- set weights
- set effort estimates
- assign issues to individuals
<br>
<br> note: See the GitLab documentation for [Importing issues from CSV](https://docs.gitlab.com/ee/user/project/issues/csv_import.html)

---

### Steps

#### 1. Build Issue spreadsheet

Decide what project structure will be for your set of issues.  Specifically,
  - what `labels` will be used for the project,
  - what `epics` and `sub-epics` will be used to track the work, and
  - what `milestones` will you use for this work effort.

If these structures do do not already exist in GitLab, **configure them now**.

#### 1.1 Spreadsheet setup

1. Configure a spreadsheet with four columns `raw title`, `raw description`, `title`, and `description`
 ![1 - four columns](/handbook/marketing/product-marketing/images/1-four-columns.png)
2. In the `Raw Title Cells`, you will enter the text for the titles of your issues.
4. In the `Raw Description` cells, will be the text of the issue descriptions (NO LABELS or Quick quick_actions)
5. The `Title` and `Description` cells will be where you use a formula to create the actual **title** and **description** of your issues.
6. You will probably use several columns to the right of these four basic columns so you can apply different `quick actions` to issues, depending on your needs.
7. Last step: Insert at least 1 row **ABOVE** your title/description row.  You will use this for common labels terms.  You will use these cells for any text or quick actions that you want to apply to ALL you issues.
 ![2- insert row](/handbook/marketing/product-marketing/images/2-insert-row.png)

#### 1.2 Build your Issue titles

|---|---|
| 1. In the first cell **below** the `Raw title` header, draft your first issue title. <br> In this case, I've drafted a title: *Market Research - Persona* as the title of my first issue.| ![3- first title](/handbook/marketing/product-marketing/images/3-write-first-title.png)_____________________________________________________________________________________________________ |   
| 2. In the cell **Above** the `Title` cell. (remember, you inserted a row), add ANY text that you want to use in EVERY title.  In this case, I wanted "SCM" to preface all my issues.  This will typically be the name of the event or activity that all these issues are related to. | ![4- first title](/handbook/marketing/product-marketing/images/4-common-title-text.png) |

| 3. In the first `Title` cell, write a formula that combines the text in the `Raw Title Cell` AND the common content from the cell **Above** the `Title` cell that we described in step 2.   |
|  ![5- title formula](/handbook/marketing/product-marketing/images/5-title-formula.png)  |
| In this case the formula that pulls together the two cells is `=N$1&": "&L3`, which combines the top cell, with some text `: ` and then the raw title.   |
| 4. Now, just write new raw titles, and then copy the formula in the `Title` cell down... and you have a new title with the same prefix.    |

#### 1.3 Build your Issue Descriptions.

1. In the cell **Above** the `Description` cell.  Add ANY quick action commands apply to EVERY issue.  
In my example. I wanted to do the following `quick actions` for **EVERY ISSUE**
  - add the following labels "usecase-gtm", "sm-request", "sm_req::triage", "usecase-SCM"
  - add every issue to a specific epic.
![6- common actions](/handbook/marketing/product-marketing/images/6-common-actions.png)
 - **TIP**: In order to type the correct `/quick actions`, go to an existing issue in your project and type the quick action in an issue comment.  The autocomplete will help you correctly write the `quick action`.  Simply copy and paste the quick action from the Gitlab comment into your spreadsheet.
2. Depending on your situation, you **might** want to have individual issues have unique labels for *teams*, or specific *due dates* or *weights*, etc.   In order to accommodate that, add additional columns to the RIGHT of the four initial columns.
  - In my example, I have added four columns, one for *team*, *due date*, *effort estimate*, and *weight*
  - ![7- issue actions](/handbook/marketing/product-marketing/images/7-issue-actions.png)
3. In the `Raw Description` cell, using Markdown, write the issue description how you want it to appear.
![8- raw description](/handbook/marketing/product-marketing/images/8-raw-description.png)
  - **Note 1**:  This is actually a **FORMULA**, where it starts with an `=` equals sign and then everything is in quotes so that the spreadsheet treats the entire block of text as a string.
  - **Note 2**:  I have found it more efficient and effective to make edits in the **formula bar** at the top of the spreadsheet, rather than in the specific cell.  You can expand the height of the formula bar to make it easier to edit.

4. In the first `Description` cell, write the formula that will bring together the `Raw Description` and the **common actions** and the **issue actions**
![9- description formula](/handbook/marketing/product-marketing/images/5-description-formula.png)
In this example, the formula is:
> =M3&"
> "&O$1&"
> "&Q3&"
> "&R3&"
> "&S3&"
> "&T3`

See this [working spreadsheet example](https://docs.google.com/spreadsheets/d/1i77cJwenb7x34nJ3pT-eYEtD4S8rdZyjpQSQyAO7jVA/edit?usp=sharing).


### 2. Import Your Issues

1. Select the `title` and `description` cells (including the column headers) and copy the contents.
2. Go to a new empty spreadsheet and `paste as values`.   This will eliminate the formulas, but will keep the actual values.
3. Save the new spreadsheet as a CSV file.  The file should **only** be the two columns `title` and `description`
4. Go to your project issue list and click on the `Import CSV` button:
![0 - Import CSV](/handbook/marketing/product-marketing/images/0-import-issue-button.png)
5. In the dialogue box, click on the file name button and select the CSV file.
  ![10 - Import issue screen](/handbook/marketing/product-marketing/images/10-import-issue-screen.png)
6. Click the `Import Issues` button and wait for the magic to happen.
  ![10 - Import issue message](/handbook/marketing/product-marketing/images/10-import-issue-message.png)

### IMPORTANT - Tips, Tricks, and Hints - READ THIS FIRST

1. Create a separate project to TEST your import file.  There is **NO WAY TO DELETE ISSUES** in GitLab.   You can **CLOSE** issues, but you cannot delete them.   So, if you are importing 20 issues and you make a mistake, depending on where your test project is in your GitLab hierarchy, you will need to:
  - Remove all the labels, milestones, epics, etc  (labels and epics roll up to higher level groups)
  - Un-assign any issues that were assigned to individuals
  - Close the issues
1. Use a **real issue** in your GitLab project to write your `Quick Action` codes.  Then, copy and paste the `quick actions` to your spreadsheet.  That way your `quick actions` will not have typos or errors.
1. The Issue **ORDER** will be sequential starting at the first row then working to the last. That means your first row in the your spreadsheet will show up LAST in GitLab (when sorted by the default `issue created date`).  However, if you list your spreadsheet in the reverse order, then your last issues will be loaded first.  That means they will be OLDER, and therefore listed last in GitLab issue lists.
