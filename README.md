***(c) 2021 - 2023 RENware Software Systems***

<small>*Document control:*<br>
* last  update: 230813
* last update by: Petre Iordanescu (piu)</small>

***


**REN-SDEVEN Software Development Methodology**

[TOC]

# General information

* p/n: **8000-2300**
* name: **SDEVEN**

This methodology is copyright (C) of RENware Software Systems (REN CONSULTING SOFT ACTIVITY SRL).





# Content files

The methodology **content (last published version)** is available in **`doc_src/`** directory. Content is available as raw source in *markdown* format following mainly [Material for MkDocs rules and formatters](https://squidfunk.github.io/mkdocs-material/reference/).

Also documentation is available as `PDF` documents in generated portal. *MkDocs* assure conversion and downloading of PDF documents for each page made available.

Content history its a place where previous content versions can be found. [For more information about that please visit here](content_history/README.md).





# Versions and roadmap

* Published version: 7.p
* Next scheduled version: n/a
* Publishing directory:
    * RELEASED version: branch `publishing`, directory `/docs'
    * DEVELOPMENT version: other branches, directory `static_portal`
* Publishing URL: **`http://sdeven.renware.eu`** (hosted by GitHub repository, branch `publishing`, directory `docs/`)




# SDEVEN portal

SDEVEN has its own site as *static site*. The site is built using *mkdocs*.

Development and current / in progress work is located in `doc_src/` directory (command prompt to start: `npm start`).





## Static site publishing

Static site publishing is made through *GitHub*. `GitHub` is configured to publish the site from branch `publishing` directory `docs/` under a custom domain name (`CNAME` for `sdeven.renware.eu`).

Here are the basic rules:

* directory `docs/` has content guaranteed ONLY on branch `publishing`
* it is used by `GitHub` to publish the site (from branch `publishing` directory `docs/`, so upload can be controlled when a public release is decideded







# Changelog & Roadmap

## CHANGELOG

Changelog is available in CHANGELOG.md and can be [found here](/CHANGELOG.md).

The changelog file contains also plans, open issues, important todo actions, hot issues, publishing checklists, etc.

A history of changes is available in `versions_history` directory.


## ROADMAP

This file keeps all future intentions for SDEVEN content changes, improvements and any other such as intentions.

SDEVEN is on continuously improvement based on real practice and users (developers, product managers, etc) recommendations, but is published only after management approval for *company policy implementation*.




