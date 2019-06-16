---
title: 'ELIXIR TES Implementation: TESK'
date: 2019-06-11
layout: default
author: "@susheel"
excerpt_separator: <!--more-->
www_link: https://github.com/EMBL-EBI-TSI/TESK
category:
  - products
tags:
  - WES
---

## {{ page.title }}

<img style="float: right; width: 30px;" src="{{ 'assets' | relative_url }}/img/TESK.png" />

Provides an implementation of a Kubernetes based task execution engine based on the [GA4GH TES](https://github.com/ga4gh/task-execution-schemas) standard. For more details on TES, see the (very) brief [introduction to TES](https://github.com/EMBL-EBI-TSI/TESK/blob/master/documentation/tesintro.md).

<!--more-->

<figure>
<img src="{{ 'assets' | relative_url }}/img/TESK-Architecture.png" alt="TESK Architecture"/>
</figure>

The project comprises of:

[![EMBL-EBI-TSI/TESK](https://gh-card.dev/repos/EMBL-EBI-TSI/TESK.svg?fullname)](https://github.com/EMBL-EBI-TSI/TESK)

[![EMBL-EBI-TSI/tesk-api](https://gh-card.dev/repos/EMBL-EBI-TSI/tesk-api.svg?fullname)](https://github.com/EMBL-EBI-TSI/tesk-api)

[![EMBL-EBI-TSI/tesk-core](https://gh-card.dev/repos/EMBL-EBI-TSI/tesk-core.svg?fullname)](https://github.com/EMBL-EBI-TSI/tesk-core)

TESK is designed with the goal to support any Kubernetes cluster, for its deployment please refer to the [deployment](https://github.com/EMBL-EBI-TSI/TESK/blob/master/documentation/deployment.md) page, the instructions provided there can be used in heterogeneous environments, with minimal configuration.

## Description

The first pod in the task lifecycle is the API pod, a pod which runs a web server (Tomcat) and exposes the TES specified endpoints. It consumes TES requests, validates them and translates them to Kubernetes jobs. The API pod then creates a task controller pod, or taskmaster.

The taskmaster consumes the executor jobs, inputs and outputs. It first creates filer pod, which creates a persistent volume claim (PVC) to mount as scratch space. All mounts are initialized and all files are downloaded into the locations specified in the TES request; the populated PVC can then be used by each executor pod one after the other. After the filer has finished, the taskmaster goes through the executors and executes them as pods one by one. Note: Each TES task has a separate taskmaster, PVC and executor pods belonging to it; the only 'singleton' pod across tasks is the API pod.

After the last executor, the filer is called once more to process the outputs and push them to remote locations from the PVC. The PVC is the scrubbed, deleted and the taskmaster ends, completing the task.

#### Requirements
A working Kubernetes cluster version 1.8 and later.
