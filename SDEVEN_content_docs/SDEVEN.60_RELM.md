<small>**SDEVEN Software Development & Engineering Methodology**</small>

Version: 0.7.5<br>
Release date: 230621

***

# Release Management (SDEVEN.60-RELM)

**Table of Content**

[TOC]


## Preamble

This procedure refers to releases that are **made public** known also as *Deployments* (aka kits, packages).

A RELEASE is a consequence of a successful development process and the **RELEASE** is the **physical image** of what a customer **will get to install and use** (also consult the [SDEVEN.90 RENBLU document section *880-RLSE System Releases*](SDEVEN.90_RENBLU.md#880-rlse-system-releases)).

!!! info "Release section in Software Design document"
    Release section has code **`880 RLSE`** in [Software Design document section System Release](Appendix_B_DSGN_Content_Index.md#880-rlse-system-release)

## Applicable policies

Any public release should follow these minimum requirements:

* the **version number** format must be strictly in accordance with [*Versioning* scheme of SDEVEN](SDEVEN.30_RENVER.md)
* must have a **Release note** document (`RELNOTE_version`)
* the product package must be available in a standard **format**: `zip`, `tar`, `bz2`
* the product must have been **passed all requited tests**: unit tests, integration tests, documentation QA, installation tests, code review tests
* the **product documentation** has been made available or a note with reference to a public place where is available (in release package)
* the product should have an **installation procedure** or a reference to it if has to be found in other place
* any known issues (as non conformities) from testing report must be placed in a dedicated section in release notes document (`RELNOTE`) in section **Known issues**

!!! warning "Releases content language"
    All released documentation **WILL GET TO FINAL CLIENTS** and *should conform to all rules* in respect to that (especially used language).


## Release directory content and structure

A `880-RLSE/` releases directory should contain the following items / sections:

* **`880.20-ELPRI`** - Editions, Licenses and Pricing
* **`880.30-EUMA`** - End User Manuals
* **`880.30-ADMA`** - Administration Manuals - *optional* and can be used the same `30-EUMA`, except the situations where administration documentation is complex enough to need to be structured and placed a dedicated directory
* **`880.40-SKIT`** - Sales Kits
* **`880.50-TKIT`** - Training Kits - training programmes, schedules, books, cheat sheets, etc
* **`880.60-SRVC`** - Service - service procedures, manuals, technical specific diagrams, product parts and codes (aka BOMs)
* **`880.90-SCA`** - Source Code Archives - published releases for downloading, organized by versions

!!! note "RLSE sections content source"
    All sections content comes from information "produced" in design and development phases.

Related procedure: [SDEVEN.90 RENBLU document](SDEVEN.90_RENBLU.md#880-rlse-system-releases).




