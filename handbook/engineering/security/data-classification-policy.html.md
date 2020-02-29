---
layout: handbook-page-toc
title: "GitLab Data Classification Policy"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

# GitLab Data Classification Policy

Data classification provides a way to categorize organizational data based on levels of sensitivity. This includes understanding what data types are available, where the data is located, and access levels and protection of the data (for example, through encryption and access control). By carefully managing an appropriate data classification system along with each tier's protection requirements, you can map the controls and level of access/protection appropriate to the data. For example, public-facing content is available for anyone to access, whereas critical content is encrypted and stored in a protected manner that requires authorized access to a key for decrypting the content.

## Scope 

The GitLab Data Classification Policy applies to all data handled, managed, stored, or transmitted by GitLab and GitLab team members, including that which is submitted to GitLab Support as part of a support request.

## Data Classification levels

### RED

Data that falls in this category is restricted and must remain confidential. This is our most sensitive data and access to it should be considered as privileged. Red information includes, but is not limited to, personally identifiable information, sensitive information, trade secrets, heightened confidential information, third party confidential information, Government classified information, proprietary information, and non-public financial information. Exposure of this data to unauthorized parties could cause extreme loss to GitLab and/or its customers. In the gravest scenario, exposure of this data could trigger or cause a business extinction event. 

**Access:**
Requests for access to this type of data should be reviewed based on the principle of "need-to-know" and approved by appropriate data owner. Once approved, access should be logged and monitored. Additional security measures should be put in place to ensure immediate response to access that seems unexpected or inappropriate. These measures should include a formalized and documented review of access on a recurring basis, during which appropriateness of access and access entitlements are re-certified. Strong access controls should be put in place to ensure that this type of data is not publicly exposed.

Vendor and/or contractor access is not permitted without formal approval and verification that they have signed an approved confidentiality agreement or non-disclosure agreement.

Systems, applications and/or integrations containing Red information must have a DPIA on file.

**Marking/ Labeling:**
Mark each document or removable media containing this data as “Red” or Restricted.

**Reproduction:**
Do not reproduce or share Red information in an application lacking the appropriate level of security. 
Never share in a public forum.
 
**Distribution/Disclosure:**
Do not send Red information over a public network unless encrypted.
Do not store or use on an unprotected portable device. 
Encrypt when stored and not in use on a laptop or portable device.  
Documents and computer screens should be positioned to prevent inadvertent disclosure of information.
Do not leave screens unattended or unsecured in any location.
Discuss only when complete privacy is available.  

**Storage/Disposal:**
Removable media must be stored in a locked enclosure when not in use.
Proper technological controls must be in place to monitor and prevent unauthorized access or attacks.
Information must not be stored on publicly accessible systems.
Electronic storage media must be irretrievably erased, degaussed and disposed of in a secure fashion.
Electronic storage media should be irretrievably destroyed when no longer legally required and as set forth in the [Record Retention Policy](https://about.gitlab.com/handbook/people-group/code-of-conduct/#sts=Record%20Retention%20Policy).

**Government Handling**
Please refer to the [GitLab Public Sector Rules of Engagement](https://about.gitlab.com/handbook/sales/public-sector/) for more information about handling government information.

### ORANGE

This classification applies to data and information that should not be made generally available.  Orange information includes, but is not limited to Security audits and logs, unpublished internally generated market research, Sales strategies, Sales statistics and Marketing plans. Unauthorized access or disclosure could break contractual obligations, and/or adversely impact GitLab, its partners, employees, and customers. 

**Access**
As with data within the RED classification, access to this data must be approved by appropriate owner prior to being granted, and once provisioned, access should be logged and monitored. Strong access controls should be put in place to ensure that this type of data is not publicly exposed.

Access to ORANGE data is limited to those with a business need-to-know, including third parties and customers, as defined by GitLab Security.

Third party access to confidential information is granted only on a need to know basis and providing appropriate confidentiality agreement or non-disclosure agreement is in place.

**Marking/Labeling:**
Mark each document or removable media containing trade secrets, heightened confidential information, third party confidential information, personally identifiable information, sensitive information as “Orange”.

**Reproduction:**
May be reproduced for Internal Use.

**Distribution/Disclosure:**
May be sent internally on a need to know basis, but discretion should be used.
May not be sent over a public network unless encrypted.
Must use the standard GitLab email statement regarding sensitive information.
Information must be encrypted or otherwise electronically protected when sent to a recipient outside the company.
Must be encrypted or otherwise protected when stored and not in use on a laptop or portable device.
Documents and computer screens should be positioned to prevent inadvertent disclosure of information.
“Orange” markings should be applied to all presentation materials to identify sensitive information.  

**Storage/Disposal:**
Electronic storage requires access controls, access control lists, and directory as well as file permissions, and other protection mechanisms. 
Information must be encrypted if necessary to store on publicly accessible systems.
Electronic storage media must be irretrievably erased, degaussed and/or disposed of in a secure fashion.
When information is no longer valid or necessary, it should be completely and permanently destroyed in accordance with the [Record Retention Policy](https://about.gitlab.com/handbook/people-group/code-of-conduct/#sts=Record%20Retention%20Policy).

### YELLOW

This classification covers non-public data that is not classified as ORANGE or RED. Disclosure of this data could violate privacy policies, and/or adversely impact GitLab, its partners, employees, and customers. 

**Access:**
Access to this data should be approved prior to being provisioned and should be logged. Strong access controls should be put in place to ensure that this type of data is not publicly exposed.

Access to YELLOW data is limited to those with a business need-to-know, including third parties and customers, as defined by GitLab Security.

**Marking/Labeling:**
Each document, removable media, emails, etc. should be appropriately and conspicuously labeled “Yellow”. 

**Reproduction:**
May be reproduced for internal use only
May be distributed to vendors and contractors on a need-to-know basis.
Basic access controls must be configured on the device(s) storing such information

**Distribution/Disclosure:**
Whenever possible, do not leave screens unattended or unsecured in public locations.
Conversations must be limited to other GitLab employees or individuals covered by a non-disclosure agreement.
Appropriate care must be taken to prevent disclosure or theft.

**Storage/Disposal:**
Normal deletion commands or utilities with operating systems are sufficient for online files.
When information is no longer valid or necessary, it should be completely and permanently destroyed.

### GREEN

Data and information that are publicly shareable, and do not expose GitLab or its partners to any harm are classified as Green.  

Public Information requires no special handling.  

## Credentials and access tokens are classified at the same level as the data they protect

Credentials such as passwords, encryption keys, and session cookies derive their importance from the data they protect. For example, authentication cookies for GitLab.com super users are classified as RED because anyone who gains access to them will have access to customer content, which is RED data.

## Systems must be protected at a level appropriate for the volume of data they process.

A system that processes a single data element at a time still processes many over time and must therefore be protected at a level appropriate for systems processing bulk data.

Typically only client applications are considered to be handling "A single customer's" data. Data on hosts/services is typically always "more than one customer". (example of hosts running "client applications" would likely be runner hosts)

## Combinations of data types may result in a higher classification level

An example of this would be a single customer's encrypted content (ORANGE) that is stored on the same system as a GitLab employee'ss credentials (ORANGE). If this user has permission to access to secrets that decrypt the customer's encrypted content, this elevates the classification (to RED).

## Determining the appropriate classification is at the discretion of GitLab Security and/or Leadership

GitLab Security should be contacted for all requests to review data classification of new data types.

If you have data that is not specified in the [Data Classification Index (internal only)](https://docs.google.com/spreadsheets/d/1eNuSLuBcZWQe13SV1TfEjtNdCOZw7G7ofY9A42Y0sPA/edit#gid=0) or does not fit the current classification and handling guidelines, please contact GitLab Security.

The following guidelines are used to determine the classification of data. Until GitLab Security makes a formal determination of classification, use these guidelines to self-classify your data:
* If the data could cause a business extinction event or other irreparable loss or harm to the company if lost or exposed to unauthorized parties, it should be classified as RED. You must contact GitLab Security for a review and approval for any critical data.
* If the data could cause significant or financially material loss or risk of harm to GitLab if exposed to unauthorized parties, it should be classified as ORANGE.
* If the data would cause minimal risk of loss or harm to GitLab if exposed, it should be classified as YELLOW.
* If the data does not expose GitLab to any harm and can or should be made available to the public, it may be classified as GREEN.

If you cannot identify the data element in the [Data Classification Index (internal only)](https://docs.google.com/spreadsheets/d/1eNuSLuBcZWQe13SV1TfEjtNdCOZw7G7ofY9A42Y0sPA/edit#gid=0), or are uncertain of the risk associated with the data and how it should be classified and handled, please contact GitLab Security.
