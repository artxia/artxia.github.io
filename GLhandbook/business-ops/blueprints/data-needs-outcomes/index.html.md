---
layout: handbook-page-toc
title: "Data Team"
description: "GitLab Data Team Handbook"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .toc-list-icons .hidden-md .hidden-lg}

{::options parse_block_html="true" /}

----

## Context
With the migration from the previous BI tool to Periscope, we took the opportunity to review
with stakeholders across the business how they were engaging with the data team and the reports it produces.

Further context and notes from each call can be found [on the relevant issue](https://gitlab.com/gitlab-data/analytics/issues/1035)


## Summary of findings

**There is no single universally accepted list of what metrics matter now**

While the KPIs Page exists, this is not 100% accurate representation of what the SLT considers their most important metrics _at the moment_ (I'd give it an 80%). 
Part of the reason behind this is that as focus/projects change so does the importance of certain metrics over others. 

**The primary use of Periscope for most of the participants was to populate their monthly metrics call**

There is(was?) an OKR being defined that all OKR tracking should be done through Periscope, but really this should be aimed towards making the _monthly metrics_ calls run from Periscope. 

**OKRs at Gitlab extend the primary stream of work instead of documenting it**

OKRs are important, but they do not generally represent what people are looking at on a day-to-day basis. 
Any work focused on reporting/dashboarding for teams should not begin from the premise that OKRs are the place to start. 

**The Data Team is larger than its official members**

As noted by @emilie, people with "Operations" in their title are generally doing Data Analyst functions, people like Francis and Robert come to mind (although there are many others across the organization). 

This brought to mind the [Spotify Squads/Tribes/Guilds](https://medium.com/productmanagement101/spotify-squad-framework-part-i-8f74bcfcd761) Framework, and that we need to work on how to better integrate with the "Extended" Data Team. 

**We should consider how to take a step closer to Salesforce** 

The sales team does *not* want people getting their data somewhere else, and will not be satisfied with a Single Source of Truth outside of SFDC. 

This comes from the need to keep people in the tool so that activities get correctly logged and data of the process is captured how it should be. 

The business also has serious problems with Data Quality on Salesforce.

While embedding Periscope into Salesforce is a good first step, we need to consider how to help the business get into a place where SFDC reports work just as well and where there is a Data Quality process.

**Everyone wants Product Usage Data related to their metrics**

The Product Team needs deeper insight into product usage, but the rest of the organization would be satisfied with feature usage. 

I could not find a place that has a full inventory of all Features tied to a Category and to a Stage. 
Getting to a place where that information exists and is tied to a "usage" definition would be a huge first step in the right direction.  

**There is a big appetite for Training, but not a lot of clarity on where to start** 

The interest and willingness to participate in training are there, but for the non-analysts the topics are daunting and there is no clear roadmap on to get from 0 to exploring data on Periscope.

## Recommendations from these calls:

* By focusing on generating a "Monthly Metrics Call" Dashboard per team we can solve two problems in one go:
    * Use this chance to have deeper conversations of what metrics matter, this collection of dashboards can become the living inventory of KPIs/Metrics.
    * Put the OKRs (as simple text will do just fine) in the Dashboard and bring the main stream of work and OKRs closer together. 
    * In my view, the order should be People Ops > Finance > Sales > Marketing > Gitlab.com > Support > Success > Alliances

* Create a formal mechanism for integrating the Extended Data Team
    * Recommend a dotted reporting line into Walter
    * Create a private "guild of data" channel and use it to socialize best practices and facilitate learning. 

* Consider re-building some the sales reports _in_ Salesforce
* Work with the new person dedicated to Salesforce on a measure and report for Data Quality
* Work with product to get clear definitions of what "usage" means for the entire Stage > Category > Feature hierarchy.

## Should-haves in the future:

* Work in Forecasting/Correlating: There was a lot of interest and appetite for forecasts (IACV/Pipeline Conversion Rate), and in correlating feature usage to conversions/retention/upgrades.
* Create consumable analyses: There are questions the business has that can work as a stand-alone report and should come with analysis/recommendations baked into it (Like how does feature usage affect the success rate of the PoC/Trial)
* Create internal training plans on SQL/dbt/Periscope
