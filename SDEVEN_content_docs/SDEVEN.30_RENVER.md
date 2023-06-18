*RENware Software Systems*    
**Software Development Methodology**

Version: 0.6.4    
Release date: 220724

***

# Versioning (SDEVEN.30-RENVER)

**Table of Content**

[TOC]

## Preamble

This section is about versioning scheme used by the RENware.

Mainly this scheme has at base the *semantic versioning* as described [here](https://semver.org/) or n document *Appendix A Semantic versioning* as appendix to this methodology.

RENware has been adapted this specifications to its own use, *regarding the qualification part, NOT major, minor and patch*.

## Version Structure

**`M.m[.p][-buildno][.qual]`**

><small>NOTE: default patch, build and release are latest (biggest, see semantic versioning appendix)</small>

* `M`, `m` and `p` are not explained here being exactly like accepted practices ref "*Semantic versioning*"
* `buildno` is the build number with internal applicability and uniqueness identify any build regardless of other version elements / parts
* `qual` is a qualifier and can be one of: `alfa | beta | preview | prerelease | release`; ***NOTE***: preview is just a prerelease but just with a "more commercial" name

**Examples:**

* *1.1.0-548.preview* major 1, minor 1, patch 0, build 058, preview qualifier version 
* *2.1.1-621* major 2, minor 1 patch 1, build 621, last qualifier version
* *3.7* major 3, minor 7, last patch, last build, last qualifier version

## Versioning and tagging rules

The most desired situation is when branch names inherits some (at least in part) of versioning principles.

To achieve the best part of this, the following rules must happen:

* always close a tag (version) of minimum "prerelease" qualifier at least from *top development* branch
* always close a tag of minimum "release" qualifier from *top master* branch
* when you have (or just needs) to stage / tag the work (and a repository admin is not available to do things that only him can do) then ***just tag an "alpha"*** and continue your work on the same branch or on another (depends on your context) and somebody which is admin (maintainer) will make a release branch from it

## Versioning by branches map

This map shows the most desired actions in frequent and current situations regarding branches and tagging.

So it is organized by branches and shows what kind of version **qualifiers** are recommended for each one.
With bold was marked the **normal** / usual qualifiers practiced for that kind of branch.

### master branch

Accepted qualifiers are:

* **release**
* prerelease
* preview

### development branch

Accepted qualifiers are:

* **beta**
* prelease

### other branches

* **alpha**

Accepted qualifiers are:


--- ooo ---