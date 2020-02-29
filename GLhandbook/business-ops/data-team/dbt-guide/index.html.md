---
layout: handbook-page-toc
title: "dbt Guide"
description: "data build tool (dbt) Guide"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .toc-list-icons .hidden-md .hidden-lg}

{::options parse_block_html="true" /}

----


## Quick Links
[Primary Project](https://gitlab.com/gitlab-data/analytics/){:.btn .btn-purple-inv}
[dbt docs](https://dbt.gitlabdata.com/){:.btn .btn-purple-inv}

## What and why
[🌎💡](/handbook/business-ops/data-team/documentation)

dbt, short for [data build tool](https://www.getdbt.com/), is an [open source project](https://github.com/fishtown-analytics/dbt) for managing data transformations in a data warehouse. Once data is loaded into a warehouse, dbt enables teams to manage all data transformations required for driving analytics. It also comes with built in testing and documentation so we can have a high level of confidence in the tables we're generating and analyzing.

The following links will give you an excellent overview of what dbt is:

* [What, exactly, is dbt?](https://blog.getdbt.com/what--exactly--is-dbt-/) - This is a less technical overview for understanding the tool
* [What is dbt?](https://docs.getdbt.com/docs/introduction) - This is a bit more technical and comes straight from the docs

But why do we use dbt? There are several reasons. 

First is that it is an open source tool with a vibrant community. 
Choosing an open source tool enables us to collaborate with the larger data community and solve problems faster than had we gone with a proprietary solution.

Second, it was built with version control in mind.
For GitLab, this is essential since we use the product for building and running the company.

Third, it speaks the language of analysts - SQL. 
This increases the number of people that can contribute since SQL is becoming such a critical part of many people's jobs.

Finally, it enables teams to move faster by integrating [testing and documentation](https://docs.getdbt.com/docs/testing-and-documentation) from the start. 

For even more information about the basics of dbt, see our [data analyst onboarding issue template](https://gitlab.com/gitlab-data/analytics/blob/master/.gitlab/issue_templates/Data%20Onboarding.md#what-is-dbt)

At times, we rely on dbt packages for some data transformation.
[Package management](https://docs.getdbt.com/docs/package-management) is built-in to dbt.
A full list of packages available are on the [dbt Hub site](https://hub.getdbt.com).

## Running dbt

If you're interested in using dbt, the [dbt documemtation has a great tutorial](https://tutorial.getdbt.com/tutorial/setting-up/) on getting setup to work on data from a fictional business called Jaffle Shop.

If you wish to use dbt and contribute to the data team project, you'll need to gain access to our Snowflake instance, which can be done via an [access request](/handbook/business-ops/it-ops-team/access-requests/).

### Configuration

* Ensure you have access to our Snowflake instance
* Ensure you have [Docker installed](https://docs.docker.com/docker-for-mac/)
* Ensure you have [Make](https://en.wikipedia.org/wiki/Make_(software)) installed (should be installed on new Macs and with XCode)
* Create a folder in your home directory called `.dbt`
* In the `~/.dbt/` folder there should be a `profiles.yml`file that looks like this [sample profile](https://gitlab.com/gitlab-data/analytics/blob/master/admin/sample_profiles.yml)
* The smallest possible warehouse should be stored as an environment variable. Our dbt jobs use `SNOWFLAKE_TRANSFORM_WAREHOUSE` as the variable name to identify the warehouse. The environment variable can be set in the `.bashrc` or `.zshrc` file as follows:
  * `export SNOWFLAKE_TRANSFORM_WAREHOUSE="ANALYST_XS"`
  * In cases where more compute is required, the variable can be overwritten by adding `--vars '{warehouse_name: analyst_xl}'` to the dbt command
* Clone the [analytics project](https://gitlab.com/gitlab-data/analytics/)

Note that many of these steps are done in the [onboarding script](https://gitlab.com/gitlab-data/analytics/-/blob/master/admin/onboarding_script.sh) we recommend new analysts run. 

### Docker Workflow
{: #docker-workflow}
[🛠🏁](/handbook/business-ops/data-team/documentation)

To facilitate an easier workflow for analysts, and to abstract away some of the complexity around handling `dbt` and its dependencies locally, the main [analytics project](https://gitlab.com/gitlab-data/analytics/) supports using `dbt` from within a `Docker` container.
We build the container from the [`data-image`](https://gitlab.com/gitlab-data/data-image) project.
There are commands within the `Makefile` to facilitate this, and if at any time you have questions about the various `make` commands and what they do, use `make help` to get a list of the commands and what each of them does.

Before your initial run (and whenever the containers get updated) make sure to run the following commands:

1. `make update-containers`
1. `make cleanup` 

These commands will ensure you get the newest versions of the containers and generally clean up your local `Docker` environment.

#### Using dbt

* Ensure you have the `DBT_PROFILE_PATH` environment variable set. This should be set if you've used the [onboarding_script.sh](https://gitlab.com/gitlab-data/analytics/blob/master/admin/onboarding_script.sh), but if not, you can set it in your `.bashrc` or `.zshrc` by adding `export DBT_PROFILE_PATH="/<your_root_dir/.dbt/"` to the file or simply running the same command in your local terminal session
* To start a `dbt` container and run commands from a shell inside of it, use `make dbt-image`
* This will automatically import everything `dbt` needs to run, including your local `profiles.yml` and repo files
  * You may see some WARNINGS about missing variables (`GIT_BRANCH`, `KUBECONFIG`, `GOOGLE_APPLICATION_CREDENTIALS`, etc.). Unless you are developing on Airflow this is ok and expected.
* To see the docs for your current branch, run `make dbt-docs` and then visit `localhost:8081` in a web-browser. Note that this requires the `docs` profile to be configured in your `profiles.yml`
* Once inside of the `dbt` container, run any `dbt` commands as you normally would
* Changes that are made to any files in the repo will automatically be updated within the container. There is no need to restart the container when you change a file through your editor!

#### Command line cheat sheet

This is a simplified version of the [primary command reference](https://docs.getdbt.com/docs/command-line-interface). 

dbt specific:
 * `dbt compile` - compiles all models
 * `dbt run` - regular run
 * Model selection syntax ([source](https://docs.getdbt.com/docs/model-selection-syntax)). Specifying models can save you a lot of time by only running/testing the models that you think are relevant. However, there is a risk that you'll forget to specify an important upstream dependency so it's a good idea to understand the syntax thoroughly:
   * `dbt run --models modelname` - will only run modelname
   * `dbt run --models +modelname` - will run modelname and all parents
   * `dbt run --models modelname+` - will run modelname and all children
   * `dbt run --models +modelname+` - will run modelname, and all parents and children
   * `dbt run --models @modelname` - will run modelname, all parents, all children, AND all parents of all children
   * `dbt run --exclude modelname` - will run all models except modelname
 * `dbt run --full-refresh` - will refresh incremental models
 * `dbt test` - will run custom data tests and schema tests; TIP: `dbt test` takes the same `--model` and `--exclude` syntax referenced for `dbt run`
 *  `dbt seed` - will load csv files specified in the `data-paths` [directory](https://gitlab.com/gitlab-data/analytics/-/tree/master/transform/snowflake-dbt/data) into the data warehouse. Also see the [seeds section of this guide]((/handbook/business-ops/data-team/dbt-guide/#seeds)) 
 
 Works only if you've run the [onboarding script](https://gitlab.com/gitlab-data/analytics/-/blob/master/admin/onboarding_script.sh):
 * `dbt_run_changed` - a function we've added to your computer that only runs models that have changed (this is accessible from within the docker container)
 * `cycle_logs` - a function we've added to your computer to clear out the dbt logs (not accessible from within the docker container)
 * `make dbt-docs` - a command that will spin up a local container to serve you the `dbt` docs in a web-browser, found at `localhost:8081`

### Configuration for contributing to dbt project
[🛠🏁](/handbook/business-ops/data-team/documentation)

If you're interested in contributing to dbt, here's our recommended way of setting up your local environment to make it easy.

* Fork the [dbt project](https://github.com/fishtown-analytics/dbt) via the GitHub UI to your personal namespace
* Clone the project locally
* Create a virtual environment (venv) for dbt following these commands

    ```bash
    cd ~
    mkdir .venv # This should be in your root "~" directory
    python -m venv .venv/dbt
    source ~/.venv/dbt/bin/activate
    pip install dbt
    ```
* Consider adding `alias dbt!="source ~/.venv/dbt/bin/activate"` to your `.bashrc` or `.zshrc` to make it easy to start the virtual environment
* Navigate to the dbt project in the same terminal window - you should see `(dbt)` at the start of the command prompt
* Run `pip install -r editable_requirements.txt`. This will ensure when you run dbt locally in your venv you're using the code on your machine. 
* Run `which dbt` to ensure it's pointing to the venv
* Develop code locally, commit your changes as you would, and push up to your namespace on GitHub

When you're ready to submit your code for a PR, ensure you've [signed their CLA](https://github.com/fishtown-analytics/dbt/blob/dev/0.15.1/CONTRIBUTING.md#signing-the-cla).

## Production Runs

<iframe class="dashboard-embed" src="https://app.periscopedata.com/shared/06101b50-9610-48e4-b1bd-2200eb488f41?embed=true" height="400"> </iframe>


## Style and Usage Guide

### Model Structure
As we transition to a more Kimball-style warehouse, we are improving how we organize models in the warehouse and in our project structure. 
The following sections will all be top-level directories under the `models` directory, which is a dbt default. 
This structure is inspired by how Fishtown Analytics [structures their projects](https://discourse.getdbt.com/t/how-we-structure-our-dbt-projects/355).

<div class="panel panel-warning">
**Legacy Structure**
{: .panel-heading}
<div class="panel-body">

Prior to our focus on Kimball dimensional modeling, we took inspiration from the BEAM* approach to modeling introduced in ["Agile Data Warehouse Design" by Corr and Stagnitto](https://books.google.com/books/about/Agile_Data_Warehouse_Design.html?id=TRWFmnv8jP0C&source=kp_book_description). 
Many of the existing models still follow that pattern. 
The information in this section is from previous iterations of the handbook.

* The goal of a (final) `_xf` dbt model should be a `BEAM*` table, which means it follows the business event analysis & model structure and answers the who, what, where, when, how many, why, and how question combinations that measure the business.
* `base models`- the only dbt models that reference the source table; base models have minimal transformational logic (usually limited to filtering out rows with data integrity issues or actively flagged not for analysis and renaming columns for easier analysis); can be found in the `analytics_staging` schema; is used in `ref` statements by `end-user models`
* `end-user models` - dbt models used for analysis. The final version of a model will likely be indicated with an `_xf` suffix when it’s goal is to be a `BEAM*` table. It should follow the business event analysis & model structure and answer the who, what, where, when, how many, why, and how question combinations that measure the business. End user models are found in the `analytics` schema.

</div>
</div>

#### Sources
All raw data will still be in the `RAW` database in Snowflake.
These raw tables are referred to as `source tables` or `raw tables`.
They are typically stored in a schema that indicates its original data source, e.g. `netsuite`

Sources are defined in dbt using a `sources.yml` file. 
* We use a variable to reference the database in dbt sources, so that if we're testing changes in a Snowflake clone, the reference can be programmatically set
*    When working with source tables with names that don't meet our usual convention or have unclear meanings, use identifiers to override source table names when the original is messy or confusing. ([Docs on using identifiers](https://docs.getdbt.com/docs/using-sources#section-configuring-sources))

     ```yaml
     # Good
     tables: 
       - name: bizible_attribution_touchpoint
         identifier: bizible2__bizible_attribution_touchpoint__c
     
     # Bad
     tables: 
       - name: bizible2__bizible_attribution_touchpoint__c
     ```

##### Source Models

We are enforcing a very thin source layer on top of all raw data. 
These are "base" models that pull directly from the raw data and should do _only_ the following:

* Rename fields to user-friendly names
* Cast columns to appropriate types
* Minimal transformations that are 100% guaranteed to be useful for the forseeable future. An example of this is parsing out the Salesforce ID from a field known to have messy data.

Even in cases where the underlying raw data is perfectly cast and named, there should still exist a source model which enforces the formatting. 
This is for the convenience of end users so they only have one place to look and it makes permissioning cleaner in situations where this perfect data is sensitive.

The following should not be done in a source model:

* Removing data
* Joining to other tables
* Transformations that fundamentally alter the meaning of a column

For all intents and purposes, the source models should be considered the "raw" data for the vast majority of users. 

Key points to remember:

* These models will be written to the `analytics.analytics_source` schema
* These models should be organized by source - this will usually map to a schema in the raw database
* Only source models should select from source/raw tables
* Source models should not select from the `raw` database directly. Instead, they should reference sources with jinja, e.g. `FROM {{ source('bamboohr', 'job_info') }}`
* Only a single source model should be able to select from a given source table
* Source models should be placed in the `/models/sources/<data_source/` directory
* Source models should perform all necessary data type casting, using the `::` sytax when casting (You accomplish the same thing with fewer characters, and it presents as cleaner). 
  * Ideally, source models should cast every column. Explicit is better than implicit. Test your assumptions
* Source models should perform all field naming to force field names to conform to standard field naming conventions
* Source fields that use reserved words must be renamed in Source models
* Source models for particularly large data should always end with an ORDER BY statement on a logical field (usually a relevant timestamp). This essentially defines the cluster key for the warehouse and will help to take advantage of [Snowflake's micro-partitioning](https://docs.snowflake.net/manuals/user-guide/tables-clustering-micropartitions.html).

#### Staging
This directory is where the majority of source-specific transformations will be stored. 
These are the models that do the prep work required to make facts and dimensions. 
Prior to our implementation of Kimball modeling, most all of our models would have fallen into this category. 

The key feature of this directory is that the transformations should stick to data-source structure. 
This means Zuora, Salesforce, etc. will have their own directory in here that maps to what exists in `sources`. 
These initially may seem redundant, but we're optimizing for the analyst and data consumers, not the data/analytics engineers.
Consolidating all sources into a single directory and schema enables simpler configuration, permissioning, and logical explanations.
Having all source-specific transformations in `staging` encourages better organization and collaboration.

#### Marts
This directory is where facts, dimensions, and OLAP cubes will be stored. 
When a model is in this directory it communicates to business stake holders that the data is cleanly modelled and is ready for querying. 
All of these models should have documentation and testing associated with them.

### General

* Model names should be as obvious as possible and should use full words where possible, e.g. `accounts` instead of `accts`.
* Documenting and testing new data models is a part of the process of creating them. A new dbt model is not complete without tests and documentation.
*    Follow the naming convention of `analysis type, data source (in alpha order, if multiple), thing, aggregation` 

     ```sql
     -- Good
     retention_sfdc_zuora_customer_count.sql
     
     -- Bad
     retention.sql
     ```

* All `{{ ref('...') }}` statements should be placed in CTEs at the top of the file. (Think of these as import statements.)
  * This does not imply all CTE's that have a `{{ ref('...') }}` should be `SELECT *` only. It is ok to do additional manipulations in a CTE with a `ref` if it makes sense for the model
* If you want to separate out some complex SQL into a separate model, you absolutely should to keep things DRY and easier to understand. The config setting `materalized='ephemeral'` is one option which essentially treats the model like a CTE. However, if you need to materialize it as a table for performance reasons, consider setting the schema config to `temporary`. This will build the table to a temporary schema which is then dropped at the end of the run. This way you get the performance benefits of a table but it won't be available for querying by end users. Note that you cannot use `temporary` if there are view models downstream. Also, you will not be able to test the model because it won't exist.

Schema References (aka What goes where)

| Purpose | Production | Dev | Config |
|---|---|---|---|
| For querying & analysis                  | analytics                   | emilie_scratch_analytics                   | None |
| For modeling marts                       | analytics_staging           | emilie_scratch_staging                     | {{  config({ "schema": "staging"}) }} |
| For modeling, but SENSITIVE              | analytics_sensitive         | emilie_scratch_analytics_sensitive         | {{  config({ "schema": "sensitive"}) }} |
| Intermediate tables that are dropped     | analytics_temporary         | emilie_scratch_temporary                   | {{  config({ "schema": "temporary"}) }} |
| Source models used to build other models | analytics_source            | emilie_scratch_temporary                   | {{  config({ "schema": "source"}) }} |

#### Model Configuration

There are multiple ways to provide configuration definitions for models. 
The [dbt docs for configuring models](https://docs.getdbt.com/docs/configuring-models) provide a concise explanation of the ways to configure models. 

Our guidelines for configuring models:

* The default materialization is `view`
* The default schema is `analytics`
* Disabling any model should always be done in the `dbt_project.yml` via the `enabled: false` declaration
* Configs should be applied in the smallest number of locations:
  * If <50% of models in a directory require the same configuration, then configure the individual models
  * If >=50% of models in a directory require the same configuration, strongly consider setting a default in the `dbt_project.yml`, but think about whether that setting is a sensible default for any new models in the directory

### Seeds
{: #seeds}

Seeds are a way to load data from csv files into our data warehouse ([dbt documentation](https://docs.getdbt.com/docs/seeds)). 
Because these csv files are located in our dbt repository, they are version controlled and code reviewable. 
This method is appropriate for loading static data which changes infrequently. 
A csv file that’s up to ~1k lines long and less than a few kilobytes is probably a good candidate for use with the `dbt seed` command.

#### Organizing columns

When writing a base model, colummns should have some logical ordering to them. 
We encourage these 4 basic groupings:
  - Primary data
  - Foreign keys
  - Logical data - This group can be subdivided further if needed
  - Metadata

Primary data is the key information describing the table. The primary key should be in this group along with other relevant unique attributes such as name.

Foreign keys should be all the columns which point to another table.

Logical data is for additional data dimensions that describe the object in reference. For a Salesforce opportunity this would be the opportunity owner or contract value. Further logical groupings are encouraged if they make sense. For example, having a group of all the variations of contract value would make sense. 

Within any group, the columns should be alphabetized on the alias name.

An exception to the grouping recommendation is when we control the extraction via a defined manifest file. A perfect example of this is our [gitlab.com manifest](https://gitlab.com/gitlab-data/analytics/blob/master/extract%2Fpostgres_pipeline%2Fmanifests%2Fgitlab_com_db_manifest.yaml) which defines which columns we extract from our application database. The base models for these tables can be ordered identically to the manifest as it's easier to compare diffs and ensure accuracy between files.

-   Ordered alphabetically by alias within groups

     ```sql
     -- Good 
     
     SELECT
       id                    AS account_id,
       name                  AS account_name,
     
       -- Foreign Keys
       ownerid               AS owner_id,
       pid                   AS parent_account_id,
       zid                   AS zuora_id,
     
       -- Logical Info
       opportunity_owner__c  AS opportunity_owner,  
       account_owner__c      AS opportunity_owner_manager,
       owner_team_o__c       AS opportunity_owner_team,
     
       -- metadata
       isdeleted             AS is_deleted,
       lastactivitydate      AS last_activity_date
     FROM table
     ```

-   Ordered alphabetically by alias without groups

     ```sql
     -- Less Good 
     
     SELECT
       id                    AS account_id,
       name                  AS account_name,
       isdeleted             AS is_deleted,
       lastactivitydate      AS last_activity_date,
       opportunity_owner__c  AS opportunity_owner,  
       account_owner__c      AS opportunity_owner_manager,
       owner_team_o__c       AS opportunity_owner_team,
       ownerid               AS owner_id,
       pid                   AS parent_account_id,
       zid                   AS zuora_id
     FROM table
     ```

-   Ordered alphabetically by original name

     ```sql
     -- Bad 
     
     SELECT
       account_owner__c      AS opportunity_owner_manager,
       id                    AS account_id,
       isdeleted             AS is_deleted,
       lastactivitydate      AS last_activity_date
       name                  AS account_name,
       opportunity_owner__c  AS opportunity_owner,  
       owner_team_o__c       AS opportunity_owner_team,
       ownerid               AS owner_id,
       pid                   AS parent_account_id,
       zid                   AS zuora_id
     FROM table
     ```

### Testing
- Every model should be tested in a `schema.yml` file
- At minimum, unique, not nullable fields, and foreign key constraints should be tested (if applicable)
- The output of dbt test should be pasted into MRs
- Any failing tests should be fixed or explained prior to requesting a review

### Snapshots
{: #snapshots}
Snapshots are a way to take point-in-time copies of source tables. dbt has [excellent documentation](https://docs.getdbt.com/docs/snapshots) on how the snapshots work. 
Take note of how we [talk about and define snapshots](https://about.gitlab.com/handbook/business-ops/data-team/#snapshots-definition).

#### Create snapshot tables with `dbt snapshot`

Snapshot definitions are stored in the [snapshots folder](https://gitlab.com/gitlab-data/analytics/tree/master/transform/snowflake-dbt/snapshots) of our dbt project. 
We have organized the different snapshots by data source for easy discovery.

The following is an example of how we implement a snapshot:

```sql
{% snapshot sfdc_opportunity_snapshots %}

    {{
        config(
          unique_key='id',
          strategy='timestamp',
          updated_at='systemmodstamp',
        )
    }}
    
    SELECT * 
    FROM {{ source('salesforce', 'opportunity') }}
    
{% endsnapshot %}
```

Key items to note:
* The database and schema are configured in `dbt_project.yml`. The database is an environmental variable while the schema is set to `snapshots`.
* _Always_ select from a source table. Even if some deduplication is required, a source table must be selected from, as selecting from a downstream dbt model is prone to failure
* As snapshots are stored in `RAW`, your role will need to be explicitly granted access to the schema or tables
* Follow the naming convention `{source_name}_{source_table_name}_snapshots` for your file name 
* Avoid any transformations in snapshots aside from deduplication efforts. Always clean data downstream
* Unless you don't have a reliable `updated_at` field, always prefer using `timestamp` as a strategy (over `check`). Please find [documentation about strategy here](https://docs.getdbt.com/docs/snapshots#section-how-does-dbt-know-which-rows-have-changed-)

##### Testing Snapshots

Testing of a snapshot can be done in a merge request using the `snapshots` CI job.
Engineers should test locally using Airflow, as the proper environment variables are handled based on the git branch.
Testing should NOT be done while on the master branch.
It is not recommended to test locally by setting the `SNOWFLAKE_SNAPSHOT_DATABASE` environment variable. 
This should never be set to `RAW` as it will overwrite production data.


#### Make snapshots table available in analytics data warehouse

Once a snapshot is taken, it becomes, and should be treated as, a [data source](/handbook/business-ops/data-team/dbt-guide/#sources).

We currently follow the legacy method for generating models based on snapshots. 
This means we don't have source models.
Base models for snapshots are available in the folder /models/snapshots of our dbt project. 
Key items to note:

* Before writing a snapshot base model, don't forget to add it in the [sources.yml file](https://gitlab.com/gitlab-data/analytics/blob/master/transform/snowflake-dbt/models/snapshots/sources.yml) (keep this file sorted)
* The name of the table in the data warehouse should be consistent with our data warehouse design guideline. Ideally we would like to stick to `{source_name}_{source_table_name}_snapshots` as our naming convention. But dbt doesn't allow duplicated file names in projects. In order to avoid this the snapshot and the snapshot base model having the same name, we follow this pattern:
  * The name of the base model file will be the name of the source snapshot table to which we suffix `_base`. Ex: we have a `gitlab_dotcom_members_snapshots` snapshot file [here](https://gitlab.com/gitlab-data/analytics/blob/master/transform/snowflake-dbt/snapshots/gitlab_dotcom_members_snapshots.sql) and a base model of this snapshot [here](https://gitlab.com/gitlab-data/analytics/blob/master/transform/snowflake-dbt/models/snapshots/gitlab_dotcom_members_snapshots_base.sql) named `gitlab_dotcom_members_snapshots_base`. 
  * We use the [dbt config alias argument](https://docs.getdbt.com/docs/using-custom-aliases#section-usage) to rename the table by removing the `_base` suffix and keep the table name clean
* If a base model built upon the snapshotted source table exists, please re-use the query that has been already written and apply the following modifications:
  * Remove the deduplication process, it is not necessary.
  * Always add `dbt_scd_id` as a primary key to your snapshot base model and rename it to something more explicit (documentation about snapshot meta-fields can be found [here](https://docs.getdbt.com/docs/snapshots#section-snapshot-meta-fields))
  * Add columns `dbt_valid_from` and `dbt_valid_to` to your query
  * Good example [here with the snapshot base model](https://gitlab.com/gitlab-data/analytics/blob/master/transform/snowflake-dbt/models/snapshots/gitlab_dotcom_gitlab_subscriptions_snapshots_base.sql) and [the base model](https://gitlab.com/gitlab-data/analytics/blob/master/transform/snowflake-dbt/models/gitlab_dotcom/base/gitlab_dotcom_gitlab_subscriptions.sql)


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
