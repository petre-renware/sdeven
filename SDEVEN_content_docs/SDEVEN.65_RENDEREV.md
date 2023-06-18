*RENware Software Systems*    
**Software Development Methodology**

Version: 0.4.10    
Last update: 220415

***

# Design approaches and review (SDEVEN.65-RENDEREV)

**Table of Content**

[TOC]

## Preliminaries

This SDEVEN section is intended to present some common design approaches (also used as review objective) practiced in RENware and supposed "to be known and understood" by development team.

The review process is (and should be) strongly correlated with design approach followed in projects and to check conformity to standards and recommendations for that models.

## Audience

Targeted audience is:

* designers / architects - to practice the ideas and guidelines of here
* developers, team leaders, product managers - to understand the design issues and impact on development

## Introductory and Approach Models

In SDEVEN there are 2 (two) kind of classic paradigms used for DESIGN:

* *waterfall paradigm* (aka sequencing) - design is a step that must be finished before development
* *incremental paradigm* (aka evolutionary) - design and development are made continosly, in small steps with returns from one to the other step

## SDEVEN Approach. Introductory

In SDEVEN both paradigms are used and combined, and when make ***a mix of them*** the predominant one is mainly dependent of nature of product and nature of intended change.

The **Product Manager** is responsible to decide what approach to be used in a particular situation. Here some basic recommendations:

* if a waterfall approach is decided, then a **minor or major version** should be considered and NOT only a patch version or just a build
* an incremental approach can update thd version in any relevant mode
* for completely new features on a product implemented using an incremental approach is better to be preceding by a research and a pilot stage

## SDEVEN Approach. Type of design changes

The following type of **design changes** must be considered related to **Design Review process**:

* **MA design change** - this is considered a MAJOR change and it is happening when a **completely new feature** needs to be implemented, by completely new meaning there is no background relative to that feature. A ***full analysis*** shoud be made and ***some related supplementary research*** could be needed. 
And all of these can generate collateral unexpected problems, even a design takes place. IN FACT THERE IS NOT EXPERIENCE REF NEW FEATURE.
* **CR design changes** - these chages appear as usually customers want some features but "staying in product scope / universe" (attn, in product scope does not necessarily mean in contract scope) 
* **WIS design changes ** - these are kind of changes, out of project scope and that could present some important features (wishes, nice to have) regardless they are a customer request or an internal idea; 
the experience to approach these changes exists but should be placed on peoduct road map

--- ooo ---