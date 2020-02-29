---
layout: handbook-page-toc
title: "Education Program"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Overview

- GitLab's top tiers (self-hosted Ultimate and cloud-hosted Gold) are [free for education](/solutions/education/)

## Requirements

- Any institution whose purposes directly relates to learning, teaching, and/or training may qualify. Educational purposes do not include commercial, professional, or any other for-profit purposes. The education license is only for the purposes of educating students and can be used by students and the teachers providing the education.
- See our [full terms](/terms/#edu-oss) regarding this program
- For more examples, please see the [FAQ section](/solutions/education/#FAQ)

## Workflows

- Community Advocacy [workflow](/handbook/marketing/community-relations/community-advocacy/workflows/education-oss-startup/)

## Metrics
The steps below will generate the Education Program metrics including: opportunity close date, tier, number of seats, billing city and billing country. These metrics are used in the Community Relations Group Conversation and for the Education Program Handbook. 

1. Log into SFDC. 
1. Navigate to Reports. 
1. Open the 'Education Opportunities' [SFDC Report](https://gitlab.my.salesforce.com/00O61000004hfne). 
1. Click on `Customize` and drag `Close date` from the `Opportunity Information` folder as a new column.
1. Click on Filters > Add > Field Filter:
    - Opportunity Information: `Type` equals `New Business` 
1. Click `Run Report` to generate the report. 
1. Click `Export Details`. Choose `Unicode (UTF-8)` for the Export File Encoding and `.csv` for the Export File Format. Then click `Export` and save the file. 
1. Download the [Eduoss](https://gitlab.com/gitlab-com/marketing/community-relations/community-advocacy/general/blob/master/tools/edoss/edoss.rb) script. 
1. Open a command prompt and change to the directory where you have the script and .csv file. 
1. Run the Edoss script with the exported csv file as input to generate the final csv file. 
       `./edoss.rb -i <exported_file>.csv -o <output_file>.csv`
1. Update the [GitLab for Education Graphs](https://docs.google.com/spreadsheets/d/18zudgYDeL1Zy90mEIO_Xi8X-ZyE86N-eQ1Nluyrh1hY/edit#gid=1612197101) for the Community Relations Group Call by importing the results of the script and updating the figures. 
Notes: 
     - You may need to make the file executable by using the following command:
       `chmod 755 edoss.rb`
- Additionally, the processor script can provide the data in `yaml` and `json` formats. 


SFDC Opportunities by Stage for EDU campaign - SFDC [report](https://na34.salesforce.com/00O61000004hfnt)
