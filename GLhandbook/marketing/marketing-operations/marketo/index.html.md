---
layout: handbook-page-toc
title: "Marketo"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

### Tools Uses  

### Forms   
Nearly all the forms on our website (`about.gitlab.com`) are Marketo embedded forms. Marketing Operations is responsible for maintaining existing forms and creating any new forms.   

All forms should follow these guidelines:  
- Field labels are always ALL CAPS
- Label width = 150 / Field width = 300
- Fields should be stacked in a vertical line
- `State/Province` only visible when `Country` = `United States` or `Canada`; the visibility rule dynamically displays `Province` when `Canada` selected or `State` when `United States` selected 
- Generally `City` is only visible when `Country` = `Ukraine`
- Forms should all contain a checkbox for the acceptance of the privacy policy
- When `Country` = `Ukraine` there is an additional checkbox for the submitter to confirm they do not belong to the Crimean region of the Ukraine  

### Smart Campaigns - Operational 

#### Standardization of Country &/or State values

There are several workflows that clean the `Country` &/or `State` fields to ensure the value meets required Salesforce format. All of the standardization smart campaigns are contained in:  

`00 Master Setup` -> `01 Operational - Don't change` -> `01_Data Management` -> `01 Data Management` -> `04-Normalize Data`   

If a `Country` &/or `State/Province` standardization is needed, please open an issue in the [Marketing Operations project](https://gitlab.com/gitlab-com/marketing/marketing-operations/issues/new?issue%5Bassignee_id%5D=&issue%5Bmilestone_id%5D=).


#### Scoring Workflows
##### Visited Booth - Field / Conference / Virtual Sponsorship   

This [smart campaign](https://app-ab13.marketo.com/#SC7097A1) is only triggered when the **Program Status** of *ANY* program is changed IN MARKETO to:  
- `Virtual Sponsorship > Visited Booth`
- `Field Event > Visited Booth`
- `Conference > Visited Booth`

When the workflow runs it adds **30 points** to the `Person Score`. A person record can flow through this smart campaign workflow **every time** it is triggered.

##### Follow Up Requested - Field / Owned / Conference / Speaking Session / Virtual Sponsorship

This [smart campaign](https://app-ab13.marketo.com/#SC7098A1) is only triggered when the **Program Status** of *ANY* program is changed IN MARKETO to: 
- `Virtual Sponsorship > Follow Up Requested`
- `Speaking Session > Follow Up Requested`
- `Owned Event > Follow Up Requested`
- `Field Event > Follow Up Requested`
- `Conference > Follow Up Requested`

When the workflow runs it adds **40 points** to the `Person Score`. A person record can flow through this smart campaign workflow **every time** it is triggered.


### Geographic DMA List   

The Geographic DMA (direct marketing area) were built for the Field Marketing and Marketing Program team to target & sends emails/invitations related to Field &/or Corporate marketing events. 
The **MktgOps** team is responsible for creating & maintaining these lists. 

If a new DMA list is needed, please open an issue in the Marketing Operations project & utilize the [DMA_request issue template](https://gitlab.com/gitlab-com/marketing/marketing-operations/issues/new?issuable_template=dma_request). 

#### AMER
##### East
- Atlanta, Geogia
- Baltimore, Maryland
- Boston, Massachusetts 
- Charlotte, North Carolina
- Chicago, Illinois
- Cincinnati, Ohio
- Dallas, Texas
- District Of Columbia
- Houston, Texas
- Montreal, Quebec, Canada
- New York City
- Quebec City, Quebec, Canada
- Raleigh, North Carolina
- San Antonio, Texas
- Tampa, Florida
- Toronto, Ontario, Canada

##### West
- Boise, Idaho
- Calgary, Alberta, Canada
- Denver, Colorado
- Des Moines, Iowa
- Irvine, California
- Los Angeles, California
- Minneapolis, Minnesota
- Phoenix, Arizona
- Portland, Oregon
- Salt Lake City, Utah
- San Diego, California
- San Francisco, California
- San Jose, California
- Seattle, Washington
- St. Louis, Missouri
- Vancouver, British Columbia, Canada

#### APAC
- Adelaide, Australia
- Auckland, New Zealand
- Bangalore, India
- Bangkok, Thailand
- Beijing, China
- Brisbane, Australia
- Busan, South Korea
- Canberra, Australia
- Chennai, India
- Christchurch, New Zealand
- Darwin, Australia
- Guangzhou, China
- Hanoi, Vietnam
- Ho Chi Minh City / Saigon, Vietnam
- Hobart, Australia
- Hong Kong
- Kolkata, India
- Kowloon, Hong Kong
- Kuala Lumpur, Malaysia
- Manila, Philippines
- Melbourne, Australia
- Mumbai, India
- New Delhi, India
- Oksaka, Japan
- Perth, Australia
- Quezon City, Philippines
- Seoul, South Korea
- Shanghai, China
- Shenzen, China
- Singapore
- Sydney, Australia
- Tianjin, China
- Tokyo, Japan
- Wellington, New Zealand
- Yokohama, Japan

#### EMEA
- All Netherlands
- All of United Kingdom
- Amsterdam, Netherlands
- Barcelona, Spain
- Berlin, Germany
- Cape Town, South Africa
- Helsinki, Finland
- London, United Kingdom
- Manchester, United Kingdom
- Munich, Germany
- Stockholm, Sweden
- Stuttgart, Germany
- Toulouse, France
- Vienna, Austria
