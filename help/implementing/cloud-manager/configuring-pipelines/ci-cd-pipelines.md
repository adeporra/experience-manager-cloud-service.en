---
title: CI-CD Pipelines
description: CI-CD Pipelines
index: no
---

# Cloud Manager CI-CD Pipelines {#intro-cicd}

In Cloud Manager, there are two types of Pipeline:

* [Production Pipeline](#prod-pipeline)
* [Non-Production Pipeline](#non-prod-pipeline)

## Production Pipeline {#prod-pipeline}

A Production pipelines is a purpose built pipeline that includes a series of orchestrated steps to take source code all the way into production. The steps include building, packaging, testing, validating, and deploying into all Stage environment first. Needless to say, a Production Pipeline can only be added once a production and stage environment set is created.

>[!NOTE]
>Refer to Configuring Production Pipeline for more details.


## Non-Production Pipeline {#non-prod-pipeline}

A Non-Production Pipeline aims to run code-quality scans or to deploy source code into a development environment. 

>[!NOTE]
>Refer to Non-Production & Code Quality Only Pipelines for more details.

The Deployment and Code Quality supported in Production and Non-Production pipeline in Cloud Manager are categorized into two different types:

* Front End
* Full Stack

The following table summarizes the pipelines:


>[!NOTE]
>A CI/CD pipeline in Cloud Manager is triggered by an event, such as a pull request from a source code repository that is, a code change, or a regular schedule to match a release cadence. 
>
>To configure your pipeline, you must:
>* define the trigger that will start the pipeline
>* define the parameters controlling the production deployment
>* configure the performance test parameters