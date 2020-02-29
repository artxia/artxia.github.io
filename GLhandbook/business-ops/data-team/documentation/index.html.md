---
layout: handbook-page-toc
title: "Data Team Documentation Guide"
description: "GitLab Data Team Handbook"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .toc-list-icons .hidden-md .hidden-lg}

{::options parse_block_html="true" /}

----

## Personas

There is a surfeit of information in the data team handbook. Not everything documented is meant for everyone who might read it. Even within the company we come from different backgrounds and are looking for different pieces of information. 

To help readers orient themselves, we've created a series of 4 personas that we believe capture the majority of user types. These are as follows:

### Builder 🛠
{: #builder}

Key attributes of a Builder:

* You have strong SQL abilities for both querying and transforming data
* Have excellent data fluency
* Direct access to data (Snowflake Raw data)
* Strong domain knowledge
* Contributor / collaborator of documentation and analysis

Typical Roles:

* Data Engineer
* Core Data Analyst

### User 💻
{: #user}

Key attributes of a User:

* Low to mid-level SQL abilities for querying data
* Basic data fluency
* Direct access to data (Snowflake Raw data)
* Strong domain knowledge

Typical Roles:

* Distributed Analyst/Engineer
* Product Manager
* Engineering Manager

### Consumer 📊
{: #consumer}

Key attributes of a Consumer:

* Limited to No SQL ability
* Limited data fluency
* Strong domain knowledge
* Limited access to data (Sisense only)

Typical roles:

* People Manager
* Business Partner
* Non-data / technical individual contributor

### Champion 👑
{: #champion}

Key attributes of a Champion:

* Limited SQL ability and limited time
* Good domain knowledge but rely on direct reports for analytic insights
* Limited Access to data

Typical roles:

* Director/VP/CXO
* Investor

### Everyone 🌎
{: #everyone}

This is our catchall grouping in case something is relevant to all personas.

## Documentation Types

The [Divio blog](https://www.divio.com/blog/documentation/) details this more than we will here, but the general idea is that there are 4 types of documentation. Each of these are different and are written with different aims in mind. They are:

### Tutorials 🔍
{: #tutorials}

A tutorial:

* is learning-oriented
* allows the newcomer to get started
* is a lesson

Analogy: teaching a small child how to cook

### How-to guides 🏁
{: #howto}

A how-to guide:

* is goal-oriented
* shows how to solve a specific problem
* is a series of steps

Analogy: a recipe in a cookery book

### Explanation 💡
{: #explanation}

An explanation:

* is understanding-oriented
* explains
* provides background and context

Analogy: an article on culinary social history

### Reference 📚
{: #reference}

A reference guide:

* is information-oriented
* describes the machinery
* is accurate and complete

Analogy: a reference encyclopaedia article

## Usage

You'll notice there are emojis next to both the persona and documentation type headers. We use the emojis in the rest of the data team portion of the handbook to help readers quickly understand the audience and purpose of different sections. For example:

* 🛠🏁 Indicates this is a how-to guide probably for somebody on the data team. An example would be how to provision somebody in Snowflake
* 💻📚 Indicates this is a reference for our user persona. An example would be the tips and tricks section for working in Sisense
* 🌎💡 Indicates this is an explanation for all personas. An example would be the charter of the data team.

Note that the emojis will not be inclusive of everyone who may in fact be interested in the section. Our aim is only to provide a quick guide to help orient the reader for what they're reading.

<!-- EXTRA STYLES APPLIED FOR THIS PAGE ONLY -->

<style>
.purple {
  color: rgb(107,79,187) !important;
}
.orange {
  color:rgb(252,109,38) !important;
}
.md-page h2 i.icon-color {
  color: rgb(107,79,187)
}
.md-page h2:nth-of-type(even) i.icon-color{
  color:rgb(252,109,38);
}
.font-awesome {
  font-size: .70em;
  vertical-align: middle;
  padding-bottom: 5px;
}
.btn-purple {
  color: rgb(107,79,187);
  background-color: #fff;
  border-color: #403366;
}
.btn-purple:hover {
  color: #fff;
  background-color: rgb(107,79,187);
  border-color: #403366;
}
.btn-purple-inv {
  color: #fff;
  background-color: rgb(107,79,187);
  border-color: #403366;
}
.btn-purple-inv:hover {
  color: rgb(107,79,187);
  background-color: #fff;
  border-color: #403366;
}
.btn-orange {
  color: rgb(252,109,38);
  background-color: #fff;
  border-color: rgb(226,67,41);
}
.btn-orange:hover {
  color: #fff;
  background-color: rgb(252,109,38);
  border-color: rgb(226,67,41);
}
.product.thumbnail img {
  display: block;
  max-width: 50%;
  margin: 20px auto;
}
.thumbnail img {
  display: block;
  max-width: 30%;
  margin: 20px auto;
}
.caption h4 {
  text-align: center;
}
.mkt-box {
  padding-bottom: 10px;
  padding-top: 10px;
  cursor: pointer;
}
.mkt-box:hover {
  /*border-radius: 5px;*/
  box-shadow:0 1px 5px rgba(0,0,0,0.3), 0 0 2px rgba(0,0,0,0.1) inset;
}
.mkt-row {
  padding-top: 20px;
  padding-bottom: 5px;
}
.mkt-row a:focus {
  outline: none;
}
.modal-header h2 {
  margin-top: 0;
}
.modal-footer p {
  margin-bottom: 0;
}
.center {
  text-align: center;
  display: block;
  margin-right: auto;
  margin-left: auto;
}
.description {
  color: #999;
}
.extra-space {
  margin-bottom: 5px;
}
.alert-purple {
  color: rgb(107,79,187);
  background-color: #fff;
  border-color: rgba(107,79,187,.5);
}
ul.toc-list-icons {
  list-style-type: none;
  padding-left: 25px;
}
ul.toc-list-icons li ul {
  padding-left: 25px;
}
ul.toc-list-icons {
  list-style-type: none;
  padding-left: 25px;
}
ul.toc-list-icons li ul {
  padding-left: 35px;
}
ul.toc-list-icons li i,
ul.toc-list-icons li ul li i {
  padding-right: 15px;
  color: rgb(107,79,187);
}
ul.toc-list-icons li:nth-of-type(even) i {
  color:rgb(252,109,38);
}
ul.toc-list-icons li ul li i.slack {
  color: rgb(224,23,101);
}
ul.toc-list-icons li ul li i.email {
  color: rgb(192,0,0);
}
</style>
