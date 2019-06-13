---
title: 'ELIXIR DRS Implementation: RDSDS'
date: 2019-06-11
layout: default
author: "@susheel"
excerpt_separator: <!--more-->
www_link: https://github.com/EMBL-EBI-TSI/RDSDS
category:
  - products
tags:
  - DRS
---

## {{ page.title }}

<img style="float: right; width: 30px;" src="{{ 'assets' | relative_url }}/img/DSDS.png" />

<figure>
<img src="{{ 'assets' | relative_url }}/img/RDSDS-High-Level-Architecture.png" alt="RDSDS High-Level Workdlow"/>
</figure>

The Reference Data Set Distribution Service (RDSDS) is offered as a component in the [ELIXIR Compute Platform](https://www.elixir-europe.org/platforms/compute) to distribute reference data sets from the ELIXIR Data Platform and from individual researchers from where the data sets originate to where the data sets are to be analysed. This service holds technical metadata relating to the data stored in the Reference Data Set and the files that comprises a dataset release version. Once a release has been made, the files will be transferred to sites subscribing to releases of this Reference Data Set using existing services and file transfer protocols and services (e.g. FTS3, Globus Online and GridFTP).

<figure>
<img src="{{ 'assets' | relative_url }}/img/RDSDS-Code-Architecture.png" alt="RDSDS Code Architecture"/>
</figure>

<!--more-->
