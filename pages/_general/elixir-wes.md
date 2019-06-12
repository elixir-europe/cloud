---
title: 'ELIXIR WES Implementation: WES-ELIXIR'
date: 2019-06-11
layout: default
author: "@susheel"
excerpt_separator: <!--more-->
www_link: https://github.com/elixir-europe/WES-ELIXIR
category:
  - products
tags:
  - WES
---

## {{ page.title }}

<img style="float: right;width: 30px;" src="{{ 'assets' | relative_url }}/img/WES-ELIXIR.png" />

Provides a Flask microservice implementing the [Global Alliance for Genomics and Health (GA4GH) Workflow Execution Service (WES)](https://github.com/ga4gh/workflow-execution-service-schemas) API specification.

<!--more-->

WES-ELIXIR is an implementation of the [GA4GH WES OpenAPI specification](https://github.com/ga4gh/workflow-execution-service-schemas) based on [Flask](http://flask.pocoo.org/) and [Connexion](https://github.com/zalando/connexion). It allows clients/users to send workflows for execution, list current and previous workflow runs, and get the status and/or detailed information on individual workflow runs. It interprets workflows and breaks them down into individual tasks, for each task emitting a request that is compatible with the [GA4GH Task Execution Service](https://github.com/ga4gh/task-execution-schemas) (TES) OpenAPI specification. Thus, for end-to-end execution of workflows, a local or remote instance of a TES service such as [TESK](https://github.com/EMBL-EBI-TSI/TESK) or [funnel](https://ohsu-comp-bio.github.io/funnel/) is required.

The service is backed by a [MongoDB](https://www.mongodb.com/) database and optionally uses [JWT](https://jwt.io/introduction/) token-based authorization, e.g. through [ELIXIR AAI](https://www.elixir-europe.org/services/compute/aai). While currently only workflows written in the [Common Workflow Language](https://www.commonwl.org/) are supported (leveraged by [CWL-TES](https://github.com/common-workflow-language/cwl-tes), we are planning to abstract workflow interpretation away from API business logic on the one hand and task execution on the other, thus hoping to provide an abstract middleware layer that can be interfaced by any workflow language interpreter in a pluggable manner.

Note that the project is currently still under active development. Nevertheless, a largely [**FUNCTIONAL PROTOTYPE**](http://193.167.189.73:7777/ga4gh/wes/v1/ui/) is available as of October 2018, hosted at the [CSC](https://www.csc.fi/home) in Helsinki.

WES-ELIXIR is part of [ELIXIR](https://www.elixir-europe.org/), a multinational effort at establishing and implementing FAIR data sharing and promoting reproducible data analyses and responsible data handling in the Life Sciences. Infrastructure and IT support are provided by ELIXIR Finland at the [CSC](https://www.csc.fi/home), the [TESK](https://github.com/EMBL-EBI-TSI/TESK) service is being developed and maintained by ELIXIR UK at the [EBI](https://www.ebi.ac.uk/) in Hinxton, and WES-ELIXIR itself is being developed by ELIXIR Switzerland at the [Biozentrum](https://www.biozentrum.unibas.ch/) in Basel and the [Swiss Institute of Bioinformatics](https://www.sib.swiss/).

(TBC)

<!--more-->
