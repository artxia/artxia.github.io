---
layout: handbook-page-toc
title: "GitLab SOC2 - Description of the System"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .hidden-md .hidden-lg}

## Purpose of this page

This page is a collection of other information that exists throughout the [GitLab handbook](/handbook) packaged together into a format commonly used in SOC2 reports. This information will define the systems involved in an external SOC2 examination and bring clarity to the environment to which we will be applying our [security controls](/source/handbook/engineering/security/sec-controls.html).

## Company Overview and Background

GitLab is an open core company which develops software for the software development lifecycle used by more than 100,000 organizations and has an active community of more than 2200 contributors. GitLab openly shares more information than most companies and is public by default, meaning our projects, strategy, direction and metrics are discussed openly and can be found within our website. Our values are Collaboration, Results, Efficiency, Diversity & Inclusion, Iteration, and Transparency (CREDIT) and these form our culture.

GitLab as a company was founded in 2015 and employs a fully remote workforce. Our [team page](https://about.gitlab.com/company/team/) has the most recent information about our number of team-members and the various countries in which those team-members live.

Additional information about GitLab can be found [here](https://about.gitlab.com/company/).

## Overview of Products and Service Commitments

GitLab is a single application for the entire DevOps lifecycle which enables Concurrent DevOps. GitLab provides visibility, efficiency, and comprehensive governance. The GitLab product consists of ten major [feature categories](https://about.gitlab.com/product/):
1. Manage
1. Plan
1. Create
1. Verify
1. Package
1. Secure
1. Release
1. Configure
1. Monitor
1. Defend

These above features are all part of the GitLab software. GitLab.com is built on the same GitLab software used by our on-premises customers by is hosted by GitLab primarily on the Google Cloud Platform. This hosting consisting of the follow components:

### NGINX

NGINX has an Ingress port for all HTTP requests and routes them to the appropriate sub-systems within GitLab. We are bundling an unmodified version of the popular open source webserver.

Additional information about NGINX can be found [at the project page](https://github.com/kubernetes/ingress-nginx/blob/master/README.md).

### Unicorn (GitLab Rails)

Unicorn is a Ruby application server that is used to run the core Rails Application that provides the user facing features in GitLab. Often process output you will see this as `bundle` or `config.ru` depending on the GitLab version.

Additional information about Unicorn can be found [at the project page](https://gitlab.com/gitlab-org/gitlab/blob/master/README.md).

### Sidekiq

Sidekiq is a Ruby background job processor that pulls jobs from the Redis queue and processes them. Background jobs allow GitLab to provide a faster request/response cycle by moving work into the background.

Additional information about Sidekiq can be found [at the project page](https://github.com/mperham/sidekiq/blob/master/README.md).

### Gitaly

Gitaly is a service designed by GitLab to remove our need for NFS for Git storage in distributed deployments of GitLab (think GitLab.com or High Availability Deployments). As of 11.3.0, this service handles all Git level access in GitLab.

Additional information about Gitaly can be found [at the project page](https://gitlab.com/gitlab-org/gitaly/blob/master/README.md).

### GitLab Workhorse

GitLab Workhorse is a program designed at GitLab to help alleviate pressure from Unicorn. It’s designed to act as a smart reverse proxy to help speed up GitLab as a whole.

Additional information about GitLab Workhorse can be found [at the project page](https://gitlab.com/gitlab-org/gitlab-workhorse/blob/master/README.md).

### GitLab Shell

GitLab Shell is a program designed at GitLab to handle SSH-based git sessions, and modifies the list of authorized keys. GitLab Shell is not a Unix shell nor a replacement for Bash or Zsh.

Additional information about GitLab Shell can be found [at the project page](https://gitlab.com/gitlab-org/gitlab-shell/blob/master/README.md).

### GitLab Pages

GitLab Pages is a feature that allows you to publish static websites directly from a repository in GitLab.

You can use it either for personal or business websites, such as portfolios, documentation, manifestos, and business presentations. You can also attribute any license to your content.

Additional information about GitLab pages can be found [at the project page](https://docs.gitlab.com/ee/administration/pages/index.html).

### Registry

The registry is what users use to store their own Docker images. The bundled registry uses NGINX as a load balancer and GitLab as an authentication manager. Whenever a client requests to pull or push an image from the registry, it will return a 401 response along with a header detailing where to get an authentication token, in this case the GitLab instance. The client will then request a pull or push auth token from GitLab and retry the original request to the registry. Learn more about token authentication.

An external registry can also be configured to use GitLab as an auth endpoint.

Additional information about Registry can be found [at the project page](https://github.com/docker/distribution/blob/master/README.md).

### Redis

Redis is a place to store:

* session data
* temporary cache information
* background job queues

Additional information about Redis can be found [at the project page](https://github.com/antirez/redis/blob/unstable/README.md).

### PostgreSQL

GitLab packages the popular Database to provide storage for Application meta data and user information.

Additional information about PostreSQL can be found [at the project page](https://github.com/postgres/postgres/blob/master/README).

### PgBouncer

PgBouncer is a lightweight connection pooler for PostgreSQL.

Additional information about PgBouncer can be found [at the project page](https://github.com/pgbouncer/pgbouncer/blob/master/README.md).

### Consul

Consul is a tool for service discovery and configuration. Consul is distributed, highly available, and extremely scalable.

Additional information about Consul can be found [at the project page](https://github.com/hashicorp/consul/blob/master/README.md).

### Prometheus

Prometheus is a time-series tool that helps GitLab administrators expose metrics about the individual processes used to provide GitLab the service.

Additional information about Prometheus can be found [at the project page](https://github.com/prometheus/prometheus/blob/master/README.md).

### Alertmanager

Alert manager is a tool provided by [Prometheus](#prometheus) that "handles alerts sent by client applications such as the Prometheus server. It takes care of deduplicating, grouping, and routing them to the correct receiver integration such as email, PagerDuty, or OpsGenie. It also takes care of silencing and inhibition of alerts.” You can read more in [issue #45740](https://gitlab.com/gitlab-org/gitlab-foss/issues/45740) about what we will be alerting on.

Additional information about Alertmanager can be found [at the project page](https://github.com/prometheus/alertmanager/blob/master/README.md).

### Grafana

Grafana is an open source, feature rich metrics dashboard and graph editor for Graphite, Elasticsearch, OpenTSDB, Prometheus and InfluxDB.

Additional information about Grafana can be found [at the project page](https://github.com/grafana/grafana/blob/master/README.md).

### Sentry

Sentry fundamentally is a service that helps you monitor and fix crashes in realtime. The server is in Python, but it contains a full API for sending events from any language, in any application.

Additional information about Sentry can be found [at the project page](https://github.com/getsentry/sentry/blob/master/README.rst).

### Redis Exporter

Redis Exporter is designed to give specific metrics about the Redis process to Prometheus so that we can graph these metrics in [Grafana](#grafana).

Additional information about Redis Exporter can be found [at the project page](https://github.com/oliver006/redis_exporter/blob/master/README.md).

### Postgres Exporter

Postgres-exporter is the community-provided Prometheus exporter that will deliver data about [Postgres](#postgresql) to [Prometheus](#prometheus) for use in [Grafana](#grafana) Dashboards.

Additional information about Postgres Exporter can be found [at the project page](https://github.com/wrouesnel/postgres_exporter/blob/master/README.md).

### PgBouncer Exporter

[Prometheus](#prometheus) exporter for [PgBouncer](#pgbouncer). Exports metrics at 9127/metrics.

Additional information about PgBouncer Exporter can be found [at the project page](https://github.com/stanhu/pgbouncer_exporter/blob/master/README.md).

### GitLab Exporter

GitLab Exporter is a process designed in-house that allows us to export metrics about GitLab application internals to [Prometheus](#prometheus).

Additional information about GitLab Exporter can be found [at the project page](https://gitlab.com/gitlab-org/gitlab-exporter).

### Node Exporter

Node Exporter is a [Prometheus](#prometheus) tool that gives us metrics on the underlying machine (think CPU/Disk/Load). It’s just a packaged version of the common open source offering from the Prometheus project.

Additional information about Node Exporter can be found [at the project page](https://github.com/prometheus/node_exporter/blob/master/README.md).

### MinIO

MinIO is an object storage server released under Apache License v2.0. It is compatible with Amazon S3 cloud storage service. It is best suited for storing unstructured data such as photos, videos, log files, backups and container / VM images. Size of an object can range from a few KBs to a maximum of 5TB.

Additional information about MinIO can be found [at the project page](https://github.com/minio/minio/blob/master/README.md).

### Runner and CI

GitLab Runner runs tests and sends the results to GitLab. GitLab CI is the open-source continuous integration service included with GitLab that coordinates testing.

Additional information about Runner and CI can be found [at the project page](https://gitlab.com/gitlab-org/gitlab-runner/blob/master/README.md).

### Certificate Management

GitLab certificate management is handled by certbot which is a client for the Let's Encrypt CA which automates the certification management process.

Additional information about certbot can be found [at the project page](https://github.com/certbot/certbot/blob/master/README.rst).

### Geo

Geo allows you to replicate a whole GitLab instance. Customers use this for
Disaster Recovery, as well as to offload read-only requests to secondary
instances.

Additional information about Geo can be found [at the Geo handbook page](/solutions/geo/).

### HAProxy

HAProxy handles high availability, load balancing, and proxying for TCP and HTTP-based communication with GitLab.com.

Additional information about HAProxy can be found [at the project page](http://www.haproxy.org/).

### Camo

Camo is an SSL image proxy which prevents mixed content warnings on secure pages.

Additional information about Camo can be found [at the project page](https://github.com/atmos/camo).