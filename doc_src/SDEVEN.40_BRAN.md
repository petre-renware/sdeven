<small>**SDEVEN Software Development & Engineering Methodology**</small>

Version: 7.0.14<br>
Release date: 230812

***

# Branches (SDEVEN.40-BRAN)

**Table of Content**

[TOC]



## Preamble

This section refers the current policies regarding *git repository* branches.



## Classification

The branches are classified like that:

* *mandatory* (always required). As example is the **master** (or *main*) branch. The name *master* is preferred (as it is already used in automation scripts), but sometimes the name main can be found (as with best practices recommendations starting with spring of 2021 year).

* with a *long life cycle* (aka just *development*). In this category is **development** branch which is required up to a minor release, then the name can be changed if needed to reflect versioning policy. Another example could be *release* beach intended for documentation review and finalizing and packaging of system.

* *test* branches which are created usually from an *alpha* or *beta* tag and kept until the required tests are passed. This kind of branches can return (merge) back to *development* corresponding branch or to a **release** branch if tests passed for preparing a potential release. In both cases, after test finalizing and branch merge, it will be deleted.

* *developer dedicated* branches local kept on remote git for a quick reference for all developers without requiring a git client

* *personal* branches reflecting current work for developers that: <sup>(i)</sup> have a `git` client installed or <sup>(ii)</sup> remote for developers using mobile devices without a `git` client installed. For such as branches open on public remote[^public_remote] `git`, the name of developer and phrase "`dev`" or "`phone`" and these branches *need to be requested from DevOps person* in order to crete them, give them enough rights and not to be (automatically) dropped.


[^public_remote]: the internal `git` used by team




## Branches used and their names

Usually, as not stated otherwise in a project, the following branches should be used:

* **development** - consolidates development of all team. Branch is *permanent* and set as *default*

* **master** - current version of system in production. Branch is *permanent*

* **xxx-dev** - work branch for team member `xxx`. Branch is *temporary* and should be administered by the DevOps person. This kind of branch is made to work from different devices where a `git` client cannot be used and files must be individually uploaded or edit using the `git` system web interface. The person for whom it was created can receive full rights on this branch

* **qa_test** / *t*est* - used according to classification. Branch is *temporary*

* **release** / **`version_string`-rel** - used according to classification. Branch is *temporary*

!!! warning "master branch name"
    starting from 2022 new git systems are default configured to name default base branch as **`main`** instead of `master`. Please check to avoid mistakes due to branch name *use in different automation / configuration* `yaml` scripts.



## Frequent mistakes

* names containing "**`dev`**" are used to signify a "local" developer work. These should not be confused with *`development`* branch which has already an explained purpose. They are used by people that need a repository for their current work and cannot install a local client.

* names containing "**`rel`**"  or "**`tst`**" or "**`qa`**" are intended for test purposes. This situation could appear <sup>(i)</sup> for own tests, <sup>(ii)</sup> for tests done by other people or <sup>(iii)</sup> for tests made before a release. Also, instead of making "release or test branches" when intention is for example not commit work but have a kind of snapshot with *"AS IS NOW"*, a tag can be created and transformed latter in a branch. This method is *STRONGLY RECOMMENDED* for any kind of snapshots that are needed. Just pay attention with these tags and DO NOT EXPECT a long life cycle for them as anytime can be dropped by a `DevOps` that remarks they are out of used conventions and policies - a better option is just to communicate the intention.



## Tagging recommendations

* for consistency, long term and reference tags should be named using *[RENVER](SDEVEN.30_RENVER.md)* conventions

* working tags should contain words like `dev` or `adev` *(from alpha dev)* if not an *alpha* release is intended. This will help for a right alphabetically sort, normally their preceding an *alpha* or upper release.




## Graphic basic flow

This diagram shows the basic flow for `master (main)`, `development` and one `xxx-dev` branch. Also on graphic the practices ref tagging are shown.

**Example for git 1<sup>st</sup> organization by issues**

``` mermaid
---
title: git flow org by issues
---
gitGraph
    commit id: "init repo"
    branch "development"
    commit id: "start of iss A"
    branch "iss-A"
    commit
    commit
    commit id: "alpha rdy to test"
    branch "qa-iss-A"
    commit id: "test of iss A"
    commit id: "beta PASSED"
    checkout "development"
    merge "qa-iss-A" tag: "beta of iss-A"
    commit id: "prep for release"
    branch "qa-release"
    commit id: "documentation Ok"
    commit id: "deployment kit OK"
    commit id: "release PASSED"
    checkout "main"
    merge "qa-release" tag: "M.m.p-release"
```

**Example for git 1<sup>st</sup> organization by developers**

``` mermaid
---
title: git flow org by developer
---
gitGraph
    commit

    branch "development"
    commit id: "review and close development"

    branch "personA-dev"
    commit id: "work iss 001"
    commit
    commit

    checkout "development"
    branch "personX-dev"
    commit id: "work to iss 002"
    commit
    
    checkout "personA-dev"
    commit id: "finished iss 001" tag: "ALPHA tag for iss-001"
    branch "test-QA-check"
    commit
    commit id: "test work for iss 001"
    commit id: "passed"
    checkout "development"
    merge "test-QA-check" id: "get iss 001" tag: "BETA tag for iss-001"
    checkout "personA-dev"
    merge "development"
    commit

    branch "release-QA"
    merge "development"
    commit "...checks for release iss 001"
    checkout "main"
    merge "release-QA" tag: "RELEASE tag for iss-001"
```

Names and codes used in diagram:

* `iss-001` is an issue that needs to be closed (and coded)
* `personA-dev` is a _personal_ branch created for "person A" to work (in example for issue 001)
* `personX-dev` is a _personal_ branch created for another developer (persona X)

Also diagram shows different tags created as occasioned by "issue 001".



