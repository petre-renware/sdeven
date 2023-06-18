*RENware Software Systems*    
**Software Development Methodology** 

Version: 0.4.10    
Release date: 220415

***

# Conventions & Principles (SDEVEN.80-RENCOPRI)

**Table of Content**

[TOC]

## Preliminaries

Generally speaking, this section is about terminology, standards and conventions used in RENware. The company try to keep aligned to international most used terms, conventions and "quickly" adopts standards. But is necessary that people who work on software company structures to keep aligned with terms and conventions in order to have **A COMMON LANGUAGE AND UNDERSTANDING ABOUT THINGS**. Seems easy but, sometimes, when need to write things to be used by someone else (don't know who will be but will be !) in the other process steps or in the future after a while, so especially in these cases it is important that things to be **recognized** at destination as they was thought at origin by those team that produced them !.

## Files

* the files that have the name beginning with `xxx` (case is not important) are so marked for a ***future deletion or discontinuing***; this method allows to mark them in a way in that to "remember" to be deleted but to still keep the information available enough time to assure an acceptable and as smooth as possible change management; also this practice will allow that in usual sorting of files, these to appear grouped at the beginning or at the end of the list (of files)
* files that have the name beginning with `_WIP` or simply `WIP` (normally case doesn't matter but should be a sign to pay more attention) are known (announced) as ***being in work and not in a stable state***, so they should be used carefully
* any other "traditional" conventions should be respected and treated in consequence; the most of them comes from `Linux` systems, for example files begining with dot (`.`) are hidden (for normal users), backup files have extension `bck`, files with extension `tmp` are temporary and subject to be deleted (by users or operating system) without notice, and so on
* the character `-` (dash) will be avoided as much as possible in file names (in different programs should be sourec of errors by confusing with arithmetic minus operator) and replaced with `_` (underscore); if this is not possible, A WARNING must in a way noticed best in the file content or in a README

## Calendar dates

* these should respect the convention as they will be written as `YYYYMMDD` at least, simply doing so will assure a right ordering in about all situations by using the operating system standard sorting procedures and not requiring some special order methods; the year could be only from 2 characters if there is no doubt regarding the year (should use standard conventions and practices from *SQL ANSI*)

## Datastores

The preferred datastore is the repository.

On the other hand, there are cases when other type of stores are required. Generally these stores are required in development process (stores for other processes are not subject if this methodology) and specific to project. They can be permanent (as stores where kits resides or stores for sales materials) or temporary allocated for project.

In any cases the dev infrastructure admin should be contacted.

Normally these stores will be allocated from file servers pool, which means that without any notice will act as "simple shared drives". If there are some other protocols required, such as access by http, https, rsync daemons started and so on, *these issues must be notified*.

Also you should expect always for such stores there are some limitations such as maximum capacity allowed, number of files, lifetime of files, file foemats allowed, etc. If this could be issues or you concern about them, please ASK and do not make other assumptions.

## "In code" names & identifiers

These issues should follow the programming language standards (as PEP for Python) or best practices if there are no such as standards. A *linter* and / or code formatter should be used like *Blake* for Python, but better is to ASK the team leader or project technical manager and NOT TO USE your own standards by supposing they are good and should be used (if this is the case, please discuss this with technical stuff before putting it in practice).

Some of recommended practices in any cases are:

* always mark protected or private attributes with underscore character in front of their names, regardless the programming language used

* always comment the code; as frequently as better; do not worry about readability or other concerns; somebody will take care to ask for cleaning if seems to be too much "spam"

* use UPPER CASE for identifiers used or intended to use as constants

* comment the functions or class methods with a large comment block and specify at least: a description of max 2 lines, the argument types and what are good for, the returns type and when is happening

--- ooo ---