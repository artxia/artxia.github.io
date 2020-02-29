---
layout: handbook-page-toc
title: "Job Families"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Job Families

They are [organized by function in directories in the www-gitlab-com repo](https://gitlab.com/gitlab-com/www-gitlab-com/tree/master/source/job-families).

Confused about when you need to create a new job family and when you should add a new role to an existing one?

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/5EcFz1qNj2E" frameborder="0" allowfullscreen="true"> </iframe>
</figure>


## Format

For each job at GitLab, there is job descriptions as the single source of truth for the expectations of that role. A job has the URL ``/job-families/department/title`` and contains the following paragraphs:

- Overview
- Responsibilities
- Requirements - All roles must have the ability to use GitLab as a requirement.
- [Job Grades](/handbook/people-group/global-compensation/#gitlab-job-grades)
- Performance Indicators
  Link to one or more performance indicator definitions for which this job family will be the [DRI](/handbook/people-group/directly-responsible-individuals/).
  A performance indicator can be a [KPI](/handbook/ceo/kpis/) but don't need to be, only a sub-set of performance indicators are KPIs.
- Career Paths
  - **In role levels** (i.e. junior, intermediate, senior, staff, etc.) which describe the requirements for each level. If no level is specified in the Job Family, then that is representing the intermediate level.
  - **Moving to and moving from** which describes possible current and future roles which move to the job family and which the job family might move to. Here is [an example](/job-families/product/product-manager/#moving-to-and-moving-from).
- [Specializations](/job-families/specialist) (e.g. CI/CD, distributed systems, Gitaly) relevant to that job family. Note that "specialist" job families may be created if their area of expertise and/or job responsibilities do not fit under any other, more general job families (e.g. the [candidate experience specialist job family](/job-families/people-ops/candidate-experience-specialist/)).
- Hiring process
- Apply
- About GitLab
- Compensation

The position description will be used _both_ for the [Vacancy Creation Process](/handbook/hiring/vacancies/#vacancy-creation-process), as well as serving as the requirements that team members and managers alike use in conversations around career development and performance management.

### The job family does not contain

1. Locations (EMEA, Americas, APEC), these are part of the [headline](/handbook/hiring/#headline)
1. [Expertises](/company/team/structure/#expert), since these are free form.
1. Anything that makes it look like a [vacancy](/handbook/hiring/vacancies/) like "exciting opportunity" or "we're hiring for".

## Leads and Managers

If you're working with a team lead or management job family, you should be aware of how GitLab defines these terms. Typically, team leads are individuals who oversee a specific project or area of expertise, but they *do not* manage people, which means they are not directly responsible for hiring, promoting, performance management, or termination of employees.

Manager job families are those responsible for directly managing other GitLab team-members. They *do* hire, promote, and terminate employees, and performance management is one of their key functions. Nomenclature to represent someone is a manager of people can be clarified with "Manager, Benchmark" (e.g., Manager, Marketing) The same holds true for director. Nomenclature to represent when someone manages a job function, and might not have people management responsibilites, can be clarified with "Benchmark Manager" (e.g., Marketing Manager)

## New Job Family Creation

If a hiring manager is creating a new job family within the organization, the hiring manager will need to create the job family.  If this is a job family that already exists (for example, Gitaly Developer would use the Developer position description), update the current position description to stay DRY. If the compensation for the job family is the same as one already in `job_families.yml`, you should just update the specialty, do not create a new job family.

Here is a brief [walkthrough](https://docs.google.com/presentation/d/1ZNsMLhk5ZB_NMinV4X2QPWLudnHHWapasxRz5HJCuCQ/edit#slide=id.g551bcad215_0_146) of this process.
If you use these slides please remember that the HANDBOOK is the most up to date and the slides and/or videos may be dated.

1. Create the relevant page in `/job-families/[department]/[name-of-job-family]`, being sure to use only lower case in naming your directory if it doesn't already exist, and add it to the correct department subdirectory.
1. The file type should be `index.html.md`.
1. Add each paragraph to the position description, for an example see the [backend engineer job family](/job-families/engineering/backend-engineer). All job families must have Requirements, Responsibilites, Performance Indicators, [Job Grades](/handbook/people-group/global-compensation/#gitlab-job-grades), and a Hiring Process. There is a template below that may be useful.
1. Assign the Merge Request to your manager, executive leadership, and finally the CEO to merge (also at-mention CEO in the #job-family chat channel). Also, cc `@gl-compensation` for a compensation review.
1. Once the merge request has been merged, the People Ops Analyst will reach out to the HR Business Partner who supports the function to understand the job description and job family requirements in determining the appropriate compensation benchmark.
2. Compensation Team: Compensation Benchmark data will be sourced from Comptryx, AdvancedHR, LinkedIn, Glassdoor, Paysa, Payscale and when applicable Cybercoders to determine the 50th percentile for the job family.  For benchmarking we are only looking at the intermediate level in San Francisco.
3. Compensation Team: In Comptryx, look at each position description by hovering over the title to make sure it aligns to our position description.  For a history of mapping, take a look at the "Comptryx Benchmarks SF" tab in the "Comp Data Analysis and Modeling "Google sheet.
4. Compensation Team: The level in Comptryx that aligns with intermediate is "proficiency,"except for in special cases (see the history of mapping for those cases).
5. Compensation Team: Create a google document that includes the compensation data and determine the median for the benchmark, share the document with the CEO, CPO and CFO. Document should be titled Job title Comp Benchmark.
6. Compensation Team: Create a merge request to add the benchmarks to the [job families](https://gitlab.com/gitlab-com/www-gitlab-com/blob/master/data/job_families.yml) file in GitLab and assign it to the CEO.  In the merge request refer to the job family title in the Google document that shows the compensation data sources and the proposed benchmark add the CPO, CFO and CEO to the MR for benchmark approval. Slack the CEO the MR for the new benchmark for review and approval.  The CEO will review the document and approvals in the MR and then will make the final decision to merge the new benchmark. Once the CEO approves the MR will add the benchmark to the `job_families.yml` file which will automatically cause the [Compensation Calculator](/handbook/people-group/global-compensation/#compensation-calculator) to show at the bottom of the position description page.
7. Compensation Team: Also add the benchmark to the "SF Benchmark" tab in the "Comp Data Analysis and Modeling" Google sheet, and document how you mapped this data in "Comptryx Benchmarks SF" tab if Comptryx was used.

## Why Job Families Have Performance Indicators 

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/9EJkgBRUSDA" frameborder="0" allowfullscreen="true"> </iframe>
</figure>


All job families should have performance indicators. 
Those performance indicators should tell you whether or not you’re doing your job well or correctly. 
For example, our [Sr. Director, Investor Relations](/job-families/finance/senior-director-of-investor-relations) role  has performance indicators which compare how we’re being described by analysts to how we describe ourself.

Performance indicators are important because people want to know that they’re contributing. 
Applicants want to know what success looks like in a role, and team members what to know how they're being measured for success. 

Company, functional, or department KPIs are too generic and, thus, not useful as job family performance indicators. 
Time sensitive PIs, like OKRs or weekly goals, are also not useful.
Performance indicators should be specific to the role and not dependent on anyone else's performance. 
Job Families should have three to five PIs. 

## Job Family Creation Using Web Version of GitLab
### Things You Will Need
* A written job description
* A job title
* A few minutes to get the job family merge request submitted. Note: job families need to be merged before the role is opened in greenhouse
* Note: [Job families are permanent](/handbook/hiring/#definitions) so do not use words like “we are seeking” in the job description

### Getting to the Right Place
* Go to the [www-gitlab-com](https://gitlab.com/gitlab-com/www-gitlab-com?nav_source=navbar) project on `gitlab.com`
* Select the [source](https://gitlab.com/gitlab-com/www-gitlab-com/tree/master/source) directory
* Go to the [job-families](https://gitlab.com/gitlab-com/www-gitlab-com/tree/master/source/job-families) directory
* Select the department where you will be making the new job family (i.e. Marketing, Sales, etc)

### Creating the New File
* Once you are in the correct department directory, select the `+`
* From the drop down list, select `New file`

### Title the File
* Insert the title in the format of `job-title/index.html.md` for example `marketing-program-manager/index.html.md`

### Body of the File
* Copy the [Template for New Job Family](/handbook/hiring/job-families/#template-for-new-job-family) and insert it into the body of the file
* Fill in the sections of the template by replacing everything in `{curly brackets}`
* Use [markdown formatting](/handbook/engineering/ux/technical-writing/markdown-guide/)
* Delete any unnecessary sections - for example, there may be no `Levels` or `Specialties` at this time, so those sections can be deleted

### Committing Changes
* Update the Commit message with a description of what you are doing
* Update Target Branch to an abbreviation of what you did. Note: include dashes between words instead of spaces.
* Make sure “Start a new merge request with these changes” box is checked.
* Click the Commit changes button at the bottom

### Assigning and Submitting Merge Request
* If it is an entirely new job family, our CEO will need to merge. You can also cc any necessary team members in the comments box (i.e. your manager or exec of the group)
* Check: Delete source branch when merge request is accepted.
* Click the Submit merge request button at the bottom

### Once the Merge Request is Submitted
* The pipeline will run to prepare the changes
* Once it is merged - it is pushed to master to make the changes and the pipeline will need to run again to make the changes official.
* Once the MR has been merged, you will be able to go into the directory you added to and see your newly created Job Family there.  

### Help! My pipeline is failing.

In October 2019, we added a CI Job that checks that job families have Requirements, Responsibilities, Performance Indicators, [Job Grades](/handbook/people-group/global-compensation/#gitlab-job-grades), and a Hiring Process, as per the below template.

Under requirements, every role must have `Ability to use GitLab`. This will also fail the pipeline.

## Template for New Job Family
```
---
layout: job_family_page
title: {Insert Title of Job Here}
---

{Insert brief description of the role here.}

## Job Grade
The {role name} is a [grade #](/handbook/people-group/global-compensation/#gitlab-job-grades).

## Responsibilities
* {add a bulleted list of responsibilities here}

## Requirements
* Ability to use GitLab
* {add a bulleted list of requirements here}

## Levels
### {Name of Level - i.e. Junior/Senior/Manager}
#### {Level} Responsibilities
* {add level responsibilities here}

#### {Level} Requirements
* {add level requirements here}

## Specialties
### {Name of Specialty - i.e. Security, Monitor, Create, etc.}
{Insert brief description of the specialty here.}

#### {Specialty} Requirements
* {add a bulleted list of requirements for this specialty here}

## Performance Indicators
* {add at least one KPI that this role will be the DRI for}

## Hiring Process
Candidates for this position can expect the hiring process to follow the order below. Please keep in mind that candidates can be declined from the position at any stage of the process. To learn more about someone who may be conducting the interview, find their job title on our [team page](/company/team/).
* Qualified candidates will be invited to schedule a 30 minute [screening call](/handbook/hiring/interviewing/#screening-call) with one of our Global Recruiters.
{Insert hiring process steps here.}

Additional details about our process can be found on our [hiring page](/handbook/hiring).
```

## Helpful Tips

### Creating a New Job Family from Scratch

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/x3q2KVFwMUY" frameborder="0" allowfullscreen="true"> </iframe>
</figure>

### Updating a Job Family Title

<figure class="video_container">
  <iframe src="https://www.youtube.com/embed/ArPShocikDM" frameborder="0" allowfullscreen="true"> </iframe>
</figure>
