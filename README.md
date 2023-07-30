***(c) 2021 - 2023 RENware Software Systems***

<small>*Document control:*<br>
* last  update: 230723
* last update by: piu (Petre Iordanescu)</small>

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

* Published version: -n/a-
* Next scheduled version: 7.0 (wip)
* Publishing directory:
    * RELEASED version: branch `publishing`, directory `/docs'
    * LAST work version: other branches, directory `static_portal`
* Publishing URL: **`http://sdeven.renware.eu`** (through GitHub repository, branch `publishing`)





# Some rules

* current work / scratch is supposed to be in `wip_crt` directory (if exists)
* last version of published content can stay in a directory named `content[_nnn]`, where nnn is optional and can be a version identifier
* content for static site building is duplicated in *static site generator*; for this reason ***NEVER CHANGE A PUBLISHED VERSION, EVEN FOR HOT FIXES - ALWAYS OPEN A NEW VERSION***
* publishing directory name is imposed thorough `GitHub` policy






# SDEVEN portal

SDEVEN has its own site as *static site*. The site is built using *mkdocs*.

Development and current / in progress work is located in `doc_src/` directory (command prompt to start: `npm start`).





## Static site publishing

Static site publishing is made through *GitHub*. `GitHub` is configured to publish the site from branch `publishing` directory `docs/` under a custom domain name (`sdeven.renware.eu`).

Here are the basic rules:

* directory `docs/` has content ONLY on branch `publishing`
* it is used by `GitHub` to publish the site (from branch `publishing` directory `docs/`) and is upload when a public release is decideded







# Changelog & Roadmap

## CHANGELOG

Changelog is available in CHANGELOG.md and can be [found here](/CHANGELOG.md).

The changelog file contains also plans, open issues, important todo actions, hot issues, publishing checklists, etc.

A history of changes is available in `versions_history` directory.


## ROADMAP

This file (if exists) keeps all future intentions for SDEVEN content changes, improvements and any other such as intentions.

SDEVEN is on continuously improvement based on real practice and users (developers, product managers, etc) recommendations, but is published only after management approval for *company policy implementation*.




