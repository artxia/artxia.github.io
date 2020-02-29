---
layout: handbook-page-toc
title: "Sales Operations Go To Market"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Welcome to The Sales Operations GTM Page! 

The purpose of this page is to centralize and document all key Go To Market policies & links for ease of use.

## **Account Ownership Rules of Engagement**
https://about.gitlab.com/handbook/business-ops/resources/#account-ownership-rules-of-engagement

## **Territory Tables**
https://about.gitlab.com/handbook/sales/territories/ 

## **Territory Success Planning (TSP)**
TSP is a combination of Salesforce Automation and business processes to help us manage our ever growing Account database. They allow us to ensure our territories are accurately reflected in SFDC as well as give visibility into "where this account is going next."" TSP fields are designed to be real time reflections of the best data we have, not necessarily the current Go To Market approach. 

For instance, an account currently marked as Sales Segment = SMB is found to have more than 100 employees, the "TSP Segment" field will automatically reflect "MidMarket." This in and of itself does not change the Segment of the account, but allows us to track the "true" Segment of the Account and support future clean up.

LeanData compares TSP fields against [Territories Live Gsheet](https://docs.google.com/spreadsheets/d/1PYU8oQJQEPpi8K-SHuqSgPeSpLcWeSQd9FuwKtgD048/edit#gid=1172192878) and **automatically determines the account's Territory and Territory Owner**.

**Firmographic TSP Fields**
*  **TSP Sales Segment**: Segment of the account based on the MAX employee count in that account's hierarchy (regardless if MAX is parent or child).
*  **TSP MAX Employees Account**: Link to specific MAX employee account in hierarchy
*  **TSP MAX Family Employees**  MAX employee count (number) in hierarchy
*  **TSP Account Employees** Number of employees ***for this specific account*** 
*  **TSP Address (Street, City, State, etc)**: Location of Ultimate Parent Account based on the TSP data hierarchy. 
*  **TSP Geo Story**: Source of address data from TSP Data Hierarchy

**Ownership TSP Fields**
*  **TSP Requested Owner**: Lookup to SFDC User, filled in by sales per Account Ownership Change Process
*  **TSP Requested Rationale**: Free text field for rationale for ownership change request, filled in by sales per Account Ownership Change Process
*  **TSP Next Owner**: Owner of territory det on [Territories Live Gsheet](https://docs.google.com/spreadsheets/d/1PYU8oQJQEPpi8K-SHuqSgPeSpLcWeSQd9FuwKtgD048/edit#gid=1172192878)
*  **TSP Next Owner Date**: Date when account ownership will change to **TSP Next Owner**

**TSP Data Hierarchy**: Many TSP fields rely on a hierarchy of data to come to one final answer (ie, multiple address fields are combined into one). The first non-blank answer is selected based on the data sources below
1. Manual Override - Admin
2. Datafox 
3. DiscoverOrg 
4. SFDC standard field (in case of Address: Shipping then Billing)
6. Manual Override - User

**Cadence of Changes**: On a quarterly basis, Sales Operations will update account Ownership and Segmentation based on the output of the TSP system in accordance with our Rules of Engagement.

**Reporting** for pending moves in/out of your name here: REPORT LINK

## **Account ownership change request process**
To request an account ownership change (to you or to someone else), please follow the below process:

1.  **Request**
*  Enter your desired owner into “Requested Owner Name” field on Account. If request is for entire hierarchy, please make request on Ultimate Parent Account.
*  Enter your rationale for move (please be as detailed as possible) in “Requested Owner Rationale” Field
2.  **Sales Operations Review**: On a weekly basis, Sales Operations will review all account change requests. 
3.  **Sales Operations Response**
*  ***Approved***: “Next Account Owner” & “Next Owner Date” will be filled in by Sales Ops. 
*  ***Rejected***: Based on the Rules of Engagement, this request cannot be completed, rejection rationale will be included. If you find this incorrect, please escalate to your direct sales manager.
*  ***Needs Approval/More Information***: Rationale is incomplete or requires input from other party (current owner or Sales Management)
4.  **Account Ownership Updated**: SFDC will automatically change ownership of the Account, child Accounts & related contacts to new owner on the “Next Owner Date.”