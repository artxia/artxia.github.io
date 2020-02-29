---
layout: handbook-page-toc
title: "Marketing Metrics"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Marketing Metrics Dashboard

The [Marketing Metrics Dashboard](https://app.periscopedata.com/app/gitlab/431555/Marketing-Metrics) is the centralized hub of all major marketing metrics and [marketing KPIs](/handbook/marketing/revenue-marketing/#revenue-marketing-kpi-definitions). It is an evergreen source of information brought in from Salesforce that is comprised of numerous individual graphs/charts (defined below) and allows the viewer to quickly filter results using pre-defined filters on the dashboard itself.


### Marketing Metric Charts - Base Fields and Base Data Filters

#### New Unique Emails AddedBase
**Base Fields**
1. Salesforce `Leads` and `Contacts` - sum of unique SFDC IDs
1. `Created Date` - SFDC System field - grouped by Month
1. [Net New Source Categories](https://docs.google.com/spreadsheets/d/1s0n1vrcROrG7qjJ55hz3qs5UyOLvSO-ljEx4IT5ENf4/edit?usp=sharing) - using the [Lead's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Lead&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DLead%26setupid%3DLeadFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DLead&setupid=LeadFields) or [Contact's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Contact&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DContact%26setupid%3DContactFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DContact&setupid=ContactFields) - By Default `DiscoverOrg` is removed, but can be added in with a Sisense filter.   

**Base Filter**
`Email` is not NULL.

### MQLs by Date by Initial Source
**Base Fields**
1. Salesforce `Leads` and `Contacts` - sum of unique SFDC IDs
1. `MQL Date` - [Lead MQL Date](https://gitlab.my.salesforce.com/00N6100000CJuLB?setupid=LeadFields) or [Contact MQL Date](https://gitlab.my.salesforce.com/00N4M00000IW0Jx?setupid=ContactFields) - grouped by Month
1. [Source Buckets](https://docs.google.com/spreadsheets/d/1s0n1vrcROrG7qjJ55hz3qs5UyOLvSO-ljEx4IT5ENf4/edit?usp=sharing) - using the [Lead's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Lead&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DLead%26setupid%3DLeadFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DLead&setupid=LeadFields) or [Contact's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Contact&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DContact%26setupid%3DContactFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DContact&setupid=ContactFields)

**Base Filter**
`MQL Date` is not from `2018-12-03 08:00:00` to `2018-12-04 07:00:00` (UTC)

### MQLs by Date by Segment
**Base Fields**
1. Salesforce `Leads` and `Contacts` - sum of unique SFDC IDs
1. `MQL Date` - [Lead MQL Date](https://gitlab.my.salesforce.com/00N6100000CJuLB?setupid=LeadFields) or [Contact MQL Date](https://gitlab.my.salesforce.com/00N4M00000IW0Jx?setupid=ContactFields) - grouped by Month
1. `Sales Segment` - [Lead Sales Segment](https://gitlab.my.salesforce.com/00N6100000HHdoa?setupid=LeadFields) or [Contact/Account UPA Sales Segment](https://gitlab.my.salesforce.com/00N6100000IOi8o?setupid=AccountFields) - using the [Lead's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Lead&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DLead%26setupid%3DLeadFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DLead&setupid=LeadFields) or [Contact's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Contact&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DContact%26setupid%3DContactFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DContact&setupid=ContactFields)

**Base Filter**
`MQL Date` is not from `2018-12-03 08:00:00` to `2018-12-04 07:00:00` (UTC)

### Converted MQLs by Converted Date
**Base Fields**
1. Salesforce `Leads` - sum of unique SFDC IDs
1. `Converted Date` - SFDC System Field - grouped by Month
1. [Source Buckets](https://docs.google.com/spreadsheets/d/1s0n1vrcROrG7qjJ55hz3qs5UyOLvSO-ljEx4IT5ENf4/edit?usp=sharing) - using the [Lead's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Lead&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DLead%26setupid%3DLeadFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DLead&setupid=LeadFields)

**Base Filter**
`MQL Date` is not from `2018-12-03 08:00:00` to `2018-12-04 07:00:00` (UTC)
`MQL Date` is not NULL
`Is Converted` - SFDC System Field - is not `False`

### Opportunity Creation - Count by Source
**Base Fields**
1. Salesforce `Opportunities` - sum of unique SFDC IDs
1. `Created Date` - SFDC System Field - Grouped by Month
1. [Source Buckets](https://docs.google.com/spreadsheets/d/1s0n1vrcROrG7qjJ55hz3qs5UyOLvSO-ljEx4IT5ENf4/edit?usp=sharing) - Using the [Opportunity Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields)

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`

### Opportunity Creation - IACV by Segment
**Base Fields**
1. [Opportunity's IACV](https://gitlab.my.salesforce.com/00N6100000HJpyB?setupid=OpportunityFields) - sum of IACV
1. `Created Date` - SFDC System Field - Grouped by Month
1. `Sales Segment` - Using the [Account UPA Sales Segment](https://gitlab.my.salesforce.com/00N6100000IOi8o?setupid=AccountFields)

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`

### XDR Opportunity Creation by XDR
**Base Fields**
1. Salesforce `Opportunities` - sum of unique SFDC IDs
1. `Created Date` - SFDC System Field - Grouped by Month
1. `XDR` - by User Name -  Using the [SDR](https://gitlab.my.salesforce.com/00N6100000HmyBe?setupid=OpportunityFields) or [BDR](https://gitlab.my.salesforce.com/00N6100000HmyBZ?setupid=OpportunityFields) fields on the Opportunity.

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`
`XDR` is not NULL or `Sales Admin`

### XDR Opportunity Creation by Source
**Base Fields**
1. Salesforce `Opportunities` - sum of unique SFDC IDs
1. `Created Date` - SFDC System Field - Grouped by Month
1. [Source Buckets](https://docs.google.com/spreadsheets/d/1s0n1vrcROrG7qjJ55hz3qs5UyOLvSO-ljEx4IT5ENf4/edit?usp=sharing) - using the [Opportunity's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields)

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`
`XDR` is not NULL or `Sales Admin` - by User Name - Using the [SDR](https://gitlab.my.salesforce.com/00N6100000HmyBe?setupid=OpportunityFields) or [BDR](https://gitlab.my.salesforce.com/00N6100000HmyBZ?setupid=OpportunityFields) fields on the Opportunity.

### XDR Pipeline Creation - IACV
**Base Fields**
1. [Opportunity's IACV](https://gitlab.my.salesforce.com/00N6100000HJpyB?setupid=OpportunityFields) - sum of IACV
1. `Created Date` - SFDC System Field - Grouped by Month
1. `Sales Segment` - Using the [Account UPA Sales Segment](https://gitlab.my.salesforce.com/00N6100000IOi8o?setupid=AccountFields)

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`
[Sales Qualified Source](https://gitlab.my.salesforce.com/00N6100000HZPjd?setupid=OpportunityFields) is `SDR Generated` or `BDR Generated`

### XDR SAOs by XDR
**Base Fields**
1. Salesforce `Opportunities` - sum of unique SFDC IDs
1. [Sales Accepted Date](https://gitlab.my.salesforce.com/00N6100000HmPaK?setupid=OpportunityFields) - Grouped by Month
1. `XDR` - by User Name - Using the [SDR](https://gitlab.my.salesforce.com/00N6100000HmyBe?setupid=OpportunityFields) or [BDR](https://gitlab.my.salesforce.com/00N6100000HmyBZ?setupid=OpportunityFields) fields on the Opportunity.

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`
`XDR` is not NULL or `Sales Admin`

### XDR SAOs by Source
**Base Fields**
1. Salesforce `Opportunities` - sum of unique SFDC IDs
1. [Sales Accepted Date](https://gitlab.my.salesforce.com/00N6100000HmPaK?setupid=OpportunityFields) - Grouped by Month
1. [Source Buckets](https://docs.google.com/spreadsheets/d/1s0n1vrcROrG7qjJ55hz3qs5UyOLvSO-ljEx4IT5ENf4/edit?usp=sharing) - using the [Opportunity's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields)

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`
`XDR` is not NULL or `Sales Admin`

### XDR SAOs - Opp per XDR
**Base Fields**
1. Salesforce `Opportunities` - sum of unique SFDC IDs
1. [Sales Accepted Date](https://gitlab.my.salesforce.com/00N6100000HmPaK?setupid=OpportunityFields) - Grouped by Month
1. Salesforce `XDR`s - count of unique users in that role
1. count of `Opportunities` / count of `XDR`s as - Opps per XDR

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`
`XDR` is not NULL or `Sales Admin` - by User Name - Using the [SDR](https://gitlab.my.salesforce.com/00N6100000HmyBe?setupid=OpportunityFields) or [BDR](https://gitlab.my.salesforce.com/00N6100000HmyBZ?setupid=OpportunityFields) fields on the Opportunity.

### XDR Closed Won by Segment - Count
**Base Fields**
1. Salesforce `Opportunities` - sum of unique SFDC IDs
1. [Closed Date](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=CloseDate&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields) - Grouped by Month
1. `Sales Segment` - Using the [Account UPA Sales Segment](https://gitlab.my.salesforce.com/00N6100000IOi8o?setupid=AccountFields)

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is 'Closed Won' or '7-Closed Won'
`XDR` is not NULL or `Sales Admin` - by User Name - Using the [SDR](https://gitlab.my.salesforce.com/00N6100000HmyBe?setupid=OpportunityFields) or [BDR](https://gitlab.my.salesforce.com/00N6100000HmyBZ?setupid=OpportunityFields) fields on the Opportunity.

### XDR Closed Won by Segment - IACV
**Base Fields**
1. [Opportunity's IACV](https://gitlab.my.salesforce.com/00N6100000HJpyB?setupid=OpportunityFields) - sum of IACV
1. [Closed Date](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=CloseDate&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields) - Grouped by Month
1. `Sales Segment` - Using the [Account UPA Sales Segment](https://gitlab.my.salesforce.com/00N6100000IOi8o?setupid=AccountFields)

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is 'Closed Won' or '7-Closed Won'
`XDR` is not NULL or `Sales Admin` - by User Name - Using the [SDR](https://gitlab.my.salesforce.com/00N6100000HmyBe?setupid=OpportunityFields) or [BDR](https://gitlab.my.salesforce.com/00N6100000HmyBZ?setupid=OpportunityFields) fields on the Opportunity.

### Converted MQLs by Converted Date - daily
**Base Fields**
1. Salesforce `Leads` - sum of unique SFDC IDs
1. `Converted Date` - SFDC System Field - grouped by Day
1. [Source Buckets](https://docs.google.com/spreadsheets/d/1s0n1vrcROrG7qjJ55hz3qs5UyOLvSO-ljEx4IT5ENf4/edit?usp=sharing) - using the [Lead's Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Lead&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DLead%26setupid%3DLeadFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DLead&setupid=LeadFields)

**Base Filter**
`MQL Date` is not from `2018-12-03 08:00:00` to `2018-12-04 07:00:00` (UTC)
`MQL Date` is not NULL
`Is Converted` - SFDC System Field - is not `False`

### MQL Goals
**Base Fields**
1. Salesforce `Leads` and `Contacts` - sum of unique SFDC IDs
1. `MQL Date` - [Lead MQL Date](https://gitlab.my.salesforce.com/00N6100000CJuLB?setupid=LeadFields) or [Contact MQL Date](https://gitlab.my.salesforce.com/00N4M00000IW0Jx?setupid=ContactFields) - grouped by Month 
1. [MQL Goal](https://docs.google.com/spreadsheets/d/15GDBF9OI3WSZKO3osODafY1u6tf5OG01Za8srO85pyY/edit#gid=0) - Displayed by Month

**Base Filter**
`MQL Date` is not from `2018-12-03 08:00:00` to `2018-12-04 07:00:00` (UTC)

### IACV Pipeline Creation
**Base Fields**
1. [Opportunity's IACV](https://gitlab.my.salesforce.com/00N6100000HJpyB?setupid=OpportunityFields) - sum of IACV
1. `Created Date` - SFDC System Field - Grouped by Month
1. [Net New IACV Goal](https://docs.google.com/spreadsheets/d/15GDBF9OI3WSZKO3osODafY1u6tf5OG01Za8srO85pyY/edit#gid=0) - Displayed by Month

**Base Filter**
[Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields) is not `Duplicate` or `10-Duplicate`
[Opportunity Type](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=Type&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields) is `Net New Business`

### New Hire Location Factor - Marketing
**Base Fields**
1. `Hire Date` - Grouped by Month
1. `Location Factor` - Averaged

**Base Filter**
`Location Factor` is not NULL
`Department` is not NULL
`Division` is `Marketing`

Note: This data is from BambooHR


## Reporting Fields Source of Truth
This section captures and links the most often used fields in reporting so that anyone pulling a Salesforce report can and is using the correct fields and the same fields that are being used in Periscope reports/dashboards.    

Note: There is a current transition to move towards the [Territory Success Planning fields](https://about.gitlab.com/handbook/sales/field-operations/sales-systems/gtm-technical-documentation/)

### Lead
1. [Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Lead&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DLead%26setupid%3DLeadFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DLead&setupid=LeadFields)
1. [MQL Date](https://gitlab.my.salesforce.com/00N6100000CJuLB?setupid=LeadFields) - if this is blank, the record is *not* counted as a `MQL`
1. [Sales Segment](https://gitlab.my.salesforce.com/00N6100000HHdoa?setupid=LeadFields)

### Contact
1. [Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Contact&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DContact%26setupid%3DContactFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DContact&setupid=ContactFields)
1. [MQL Date](https://gitlab.my.salesforce.com/00N4M00000IW0Jx?setupid=ContactFields) - if this is blank, the record is *not* counted as a `MQL`
1. Sales Segment - See the Account `UPA Sales Segment` field. 

### Account
1. [UPA Sales Segment](https://gitlab.my.salesforce.com/00N6100000IOi8o?setupid=AccountFields)

### Opportunity
1. [BDR](https://gitlab.my.salesforce.com/00N6100000HmyBZ?setupid=OpportunityFields)
1. [Closed Date](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=CloseDate&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields)
1. [IACV](https://gitlab.my.salesforce.com/00N6100000HJpyB?setupid=OpportunityFields)
1. [Lead Source](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=LeadSource&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields)
1. [Sales Accepted Date](https://gitlab.my.salesforce.com/00N6100000HmPaK?setupid=OpportunityFields)
1. [Sales Qualified Source](https://gitlab.my.salesforce.com/00N6100000HZPjd?setupid=OpportunityFields)
1. [SDR](https://gitlab.my.salesforce.com/00N6100000HmyBe?setupid=OpportunityFields) 
1. [Stage Name](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=StageName&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields%26retURL%3D%252Fui%252Fsetup%252FSetup%253Fsetupid%253DOpportunity&setupid=OpportunityFields)
1. [Type](https://gitlab.my.salesforce.com/_ui/common/config/field/StandardFieldAttributes/d?id=Type&type=Opportunity&retURL=%2Fp%2Fsetup%2Flayout%2FLayoutFieldList%3Ftype%3DOpportunity%26setupid%3DOpportunityFields&setupid=OpportunityFields)








