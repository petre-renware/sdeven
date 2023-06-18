***(c) 2021, 2022 RENware Software Systems***

<small>*Document control:*<br>
* last  update: 230617
* last update by: piu (Petre Iordanescu)</small>

***

**REN-SDEVEN Software Development Methodology**

[TOC]

# General information

* p/n: **8000-2300**
* name: **SDEVEN**

This methodology is copyright (C) of RENware Software Systems (REN CONSULTING SOFT ACTIVITY SRL).

# Content files

The methodology **content (last published version)** is available in **`SDEVEN_content_docs/`** directory. Content is available as raw / source in *markdown* format following mainly [Material for MkDocs rules and formatters](https://squidfunk.github.io/mkdocs-material/reference/).

Also documentation is available as `PDF` documents in generated portal. *MkDocs* assure conversion and downloading of PDF documents for each page made available.

Content history its a place where previous content versions can be found. [For more information about that please visit here](content_history/README.md).

# Versions and roadmap

* Published version: 0.6
* Next scheduled version: 0.7 (wip)

# Some rules

* current work / scratch is supposed to be in `wip_crt` directory (if exists)
* last version of published content can stay in a directory named `content[_nnn]`, where nnn is optional and can be a version identifier
* content for static site building is duplicated in *static site generator*; 
for this reason ***NEVER CHANGE A PUBLISHED VERSION, EVEN FOR HOT FIXES - ALWAYS OPEN A NEW VERSION***






# SDEVEN portal

SDEVEN has its own site in two versions:

* **static**, which means only classic static routes (equivalent of directories) which can be published as is using web servers like Apache or Nginx
* **dynamic** (_THIS IS FUTURE INTENDED_), which is able to have forms and other kind of modern sites features; this need a WSGI web server to be published, like gunicorn or Apache

*Static site* is built using *Docusaurus*. 
Development is located in `docusaurus.../` directory (command prompt to start: `npm start`).

*Dynamic site* is built using *Flask* python framework. 
Development is located in `sdeven_site/` directory (command prompt to start: `runserver.sh`).



## Static site

### Organization

Root of development of static site resides under `docusausurus_portal` as being *Docusaurus* installed directory.

Built static site image (as deployable under a HTTP server) resides in an archive file: `static_site[_version].zip` located in repository root. 
Name may contain ***content version*** to easly identify what content version resides inside.

Also, in (together with) `content_xx`, usually will stay as archived the whole development directory for an easy restore as it was at deployment. 
*Please treat this carefully as it possible for missing or unusable as being too old software version no longer runnable on current operating systems.*

### Development organization

The following directories and files are of interest and relevant for proposed usage & objectives:

* **portal root** -  `docusaurus.config.js` portal / site visual configuration: titles, links, etc
* **src** - `src/pages/index.js` is the main (landing) page; format `HTML` with `REACT` controls
* **docs/SDEVEN_content** - the methodology content (copy or why not link !)


# Changelog

Changelog is available in CHANGELOG.md and can be [found here](/CHANGELOG.md).

The changelog file contains also plans, open issues, important todo actions, hot issues, publishing checklists, etc.

A history of changes is available in `versions_history` directory.




