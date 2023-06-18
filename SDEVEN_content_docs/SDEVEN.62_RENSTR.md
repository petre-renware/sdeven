*RENware Software Systems*    
**Software Development Methodology** 

Version: 0.4.10    
Release date: 220415

***

# Project structure (SDEVEN.62-RENSTR)

**Table of Content**

[TOC]

## Preamble and goals

This procedure contains usual project structure and it is just a recommendation. The *Project Manager* will organize the project in the best possible mode in order to to be relevant in specific project situations. A common practice is to start with these recommendations and to add (or refine) elements that reflects project particular aspects.

## Basic structure - THE BACKBONE

Being in majority a software development project, those elements from RENBLU need to be highlighted as to be "visible" and clear even from the project root level (or immediately under the project root).

So immediately under project "entry" our recommendation is to reflect the most important SDEVEN phases (*see RENBLU*):

* 110-SRE System Requirements
* 120-CPTS System Concepts
* 130-SKIT Sales Kit(s)
* 810-DSGN System Design
* 830-DEV System Development
* 880-RLSE System Releases

These are the most usual items and required / used in 99.9% of software development cases. Of course, all other items from RENBLU are welcome either at topmost directory either as subdirectories.

Sure it is strongly recommended to have a dedicated directory for **Project Management** where to keep (with own organization):

* project contract
* project delivery documents
* project tests & acceptances
* project deliverables
* and so on...

## Naming conventions

As seen, phases, sub-phases, other items names aer not necessarily "in best form" to be used as directory or file names, even is possible on most operating systems, but on other IS NOT and this can induce important limitations. So it is recommended to replace spaces (` `) and dashes (`-`) wth underscores (`_`).

## Usages

* All product / system code is recommended to be kept under `830-DEV` directory.
* It is highly recommended to keep all files on RENWARE GIT / REPOSITORY, at least `830-DEV` directory or code directory.

--- ooo ---