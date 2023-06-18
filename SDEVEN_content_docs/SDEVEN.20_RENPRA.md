*RENware Software Systems*    
**Software Development Methodology**

Version: 0.6.4    
Release date: 220724

***

# Practices (SDEVEN.20-RENPRA)

**Table of Content**

[TOC]

## Preamble

This procedure is about best practices as software development in company, aimed to assure a good level of communication, exchange information, synchronizing activities and work, presenting results and obtain best benefits.

## General (common) aspects

Here is a list which present the most common and frequent situations (but probably does not covers all situations; those aspects that need more details have dedicated section):

* never change ANYTHING ref a version declared as *work in progress*. Better is to create a new issue instead of changing the existing one.
* organize dev in *sprints* as small chunks of changes that have clear objective sand specs
* when work and make a dedicated branch, just MAKE STRICTLY WHAT YOU PROPOSED TO DO / WHAT IS REQUIRED TO DO; otherwise so it will be difficult to revert / drop that branch in case of you need because something is wrong with too high impact to analyses it - DOING MORE THINGS YOU'LL LOOSE ALL WORK THAT IT IS INTENDED TO BE PRESERVED, usual have nothing too much to do with current / work issue scope and objectives

## Branches and repository

* always made a branch for each change / sprint, even is a short one (will allow you to quickly rollback work)
this branch should be locally on your dev machine but is not mandatory, it could be remote and devops engineer notified
* try to *avoid mixing with other branches* even if they're still yours (as work in progress)

## Releases check list

Here is a check list regarding most important issues that need attention before closing a release:

* check for still open / in work sections; look for specific text like: wip, ..., todo, fixme, bug, need review, etc
* check release notes: if exists as separated file or there are marked in a clear way, not mixed with things intended or in work for other versions
* check for version code (at least major, minor, patch) to be in according with roadmap
* check technical documentation: specs for usage, notes for developers
* check for end user documentation: updates, references that released features are available from version x, "how to use features", etc
* check the language used in end user intended documents to be as most as possible IMPARTIAL and avoid misinterpretations
* check for other elements with impact on branding, such as logos, colors, fonts, etc

## Technical issues regarding syncing and distributed execution

* for sync subject objects it is recommended to be accompanied by some metadata at least with a key ref to *last sync* as date time stamp
* for multi systems sync (more than 2 involved in sync process), every system should have its own list with targeted systems to be synced; this list itself is subject to sync
* generally ref syncing it is recommended to use standard components and technologies, like `rsync` or derivate but largely enough used and maintained by producer; clearly should be avoided solutions that are available only on Windows based systems
* ref distributed execution it is recommended to use already known components that have enough support as community and are dependent only of other known components, for example for queues and pub / sub systems, Rabbit MQ, redis, AMPQ, can be used; proprietary closed systems must be avoided (can be used only in custom / dedicated / turn key systems if the beneficiary want strictly a component)
* with risk of repeating, please do not use in file names intended as code modules / parts / chunks the character dash (`-`). Replace it with underscore (`_`). In many languages the including of the other files in code is made using some pre-processor directives (as `include`, `import`, `require`, and so on) and these directives does not accep always strings but directly filenames and often the dash character is treated as ***minus arithmetical operator*** which can lead to many *"hard to detect"* problems.

More information, techniques and practices can be find in template of [Software Design document](Appendix_B_DSGN_Content_Index.md).

## Tool stacks components versions

* a new version of a toolstack component must be avoided if a feature intended to be used is not backward compatible (is accessible as new from that version); before doing that must be checked: the impact to already developed or in development code by any member and the adoption of this version in standard operating systems

## Function parameters

<small>This is subject to *optional* recommended practices.</small>

* always make a local (in function) copy of received parameters. This is to minimizing risk of generating unwanted side effects
* except you really want to change their value and this change to be "seen" by caller
* if the language force to specify parameters behavior (in, out or inout) there is no need for this, but many languages do not; even you want to clearly modify them and this is known, make anyway a copy to have the original value
* *PAY ATTENTION THAT MAKING A COPY IS NOT ENOUGH TO AVOID SIDE EFFECTS*; for an address param (aka pointer) its reference update will update it as side effect

--- ooo ---