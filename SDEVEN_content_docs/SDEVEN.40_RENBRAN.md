*RENware Software Systems*    
**Software Development Methodology** 

Version: 0.4.10    
Release date: 220415

***

# Branches (SDEVEN.40-RENBRAN)

**Table of Content**

[TOC]

## Preamble

This section refers the current policies regarding *git repository* branches.

## Classification

The branches are classified like that:

* *mandatory* (always required). As example is the **master** (or *main*) branch. The name *master* is preferred (as it is already used in automation scripts), but sometimes the name main can be found (as with best practices recommendations starting with spring of 2021 year). 

* with a *long life cycle* (aka just *development*). In this category is **development** branch which is required up to a minor release, then the name can be changed if needed to reflect versioning policy. Another example could be *release* beach intended for documentation review and finalizing and packaging of system. 

* *test* branches which are created usually from an *alpha* or *beta* tag and kept until the required tests are passed. This kund of branches can return (merge) back to *development* corresponding branch or to a **release** branch if tests passed for preparing a potential release. In both cases, after test finalizing and branch merge, it will be deleted. 

* *developer dedicated* branches local kept on remote git for a quick reference for all developers without requiring a git client 

* local reflecting current work for developers that have a git client installed or remote for developers use mobile devices without a git client installed. For remote kept such as branches, the name of developer and syntagma as "dev" or "phone" aso and they need to be requested before in order to get enough rights for them and not to be (automatically) dropped by admins. 

## Branches used and their names

Usually, as not stated otherwise in a project, the following branches should be used:

* *development* - consolidates development of all team. Branch is *permanent and default.*

* *master* - current version of system in production. Branch is *permanent*.

* *xxx-dev* - work branch for team member `xxx`. Branch is *temporary* and should be administered by `Repository / GIT Admin`. This kind of branch is made for work from different devices where a git client cannot be used and files must be individually uploaded or edit using the git system web interface. The person for who the branch is create can receive full rights on this branch.

* *qa_test* / *test* - used according to classification. Branch is *temporary*.

* *release* / *vvv-rel* - used according to classification. Branch is *temporary*.

## Example of branch / tag names

Here are some cases of branch names, just for a better understanding:

* names containing "**`dev`**" are used to signify a "local" developer work. These should not be confused with *`development`* branch which has already an explained purpose. They are used by people that need a repository for their current work and cannot install a local client.

* names containing "**`rel`**"  or "**`tst`**" or "**`qa`**" are intended for test purposes. Situation could appear for own tests, for tests done by other people or for test before a release. Also, instead of making "release or test branches" and if intention is for example to not commit work but have a kind of snapshot with ***"AS IS NOW"***, a tag can be created and transformed latter in a branch. This method is STRONGLY RECOMMENDED for any kind of snapshots are needed. Just pay attention with these tags and DO NOT EXPECT a long life cycle for them as at a time can be dropped by a *devops* that remarks they are out of used conventions and policies - a better option is just to communicate the intention.

## Tagging recommendations

* for consistency, long term and reference tags should be named using **RENVER** conventions
* working tags should contain words like "dev" or "adev" *(from alpha dev)* if not an *alpha* release is intended. 
This will help fir a right alphabetically sort, normally their preceding an *alpha* or upper release.

--- ooo ---