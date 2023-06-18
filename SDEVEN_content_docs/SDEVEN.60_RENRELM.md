*RENware Software Systems*    
**Software Development Methodology**

Version: 0.6.4    
Release date: 220724

***

# Release Management (SDEVEN.60-RENRELM)

**Table of Content**

[TOC]

## Preamble

This section refers exclusively to those releases that are **made public** known also as *Deployments* (kits, packages).

It should be clear that (from software products perspective) **A RELEASE** is a consequence of a development process and **most** (even **all**) of the "content" that is found in a release is the result of the development process. So, the *structure* of a release content and the *content itself* comes from all previous stages, THE **RELEASED PRODUCT** being an "image" of that deliverables at that point in time - **THE RELEASE**.

For a better understanding of releases as general development issue please consult the [SDEVEN.90 RENBLU document](SDEVEN.90_RENBLU.md), section *880-RLSE System Releases*.

## Applicable policies

Any public release should follow these minimum requirements:

* the version number format must be in strict accordance with specs from  **Versioning** section of this document (SDEVEN.30)
* must have a **Release note** document
* the product package must be available in min 2 standard largely known and used **formats** (`zip`, `tar`, `bz2`, etc).
* the product must have been passed all tests requited for its version qualification
* the **product documentation** must be made available in the package or referred if there is no reason to duplicate it
* the product should have an **installation procedure** or a reference to it if has to be found in other place
* any known issues (as non conformities) from testing report must be placed in a dedicated section in release notes or a README document under a clear section named ***Known issues***

## Release coding

Usual release section code is **`880 RLSE`** but is not mandatory to be followed being often too technical for consumers market. But "inside" development can be used and will offer a common understanding (and a better possibility to create some *automatization tools* usable for that product in documentation generation, for example).

A good and recommended approach is to have these sections already in development directories (ie, in repository.)

## Release content structure

A release should contain the following sections:

* **`880.20-ELPRI`** - Editions, Licenses and Pricing
* **`880.30-EUMA`** - End User Manuals
* **`880.30-ADMA`** - Administration Manuals - *optional* and can be used the same `30-EUMA`, except the situations where administration doc is complex and big enough to need a dedicated directory
* **`880.40-SKIT`** - Sales Kits
* **`880.50-TKIT`** - Training Kits - training programmes, schedules, books, cheat sheets, etc
* **`880.60-SRVC`** - Service - service procedures, manuals, technical specific diagrams, product parts and codes (aka BOMs)
* **`880.90-SCA`** - Source Code Archives - published releases for downloading, organized by versions

All sections are "*self explanatory*" by names and comes from already existing information in design and development phases. What is ***REALLY DIFFERENT*** is the fact that **THESE DELIVERABLES WILL GO TO FINAL CLIENTS** and *should conform to all rules in respect to that*.

>NOTE 1: as in all methodology, the codes are presented hierarchically and with characters that are not necessarily "best option" for file names. The same thing is applicable for letters case. As consequence they can be adapted to project rules, the most important (and that should be respected) being the "***literal part***" of code.

>NOTE 2: the structure presented here is also described in [SDEVEN.90 RENBLU document](SDEVEN.90_RENBLU.md).

--- ooo ---