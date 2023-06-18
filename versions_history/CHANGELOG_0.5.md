(c) 2021 RENware Systems (REN CONSULTING SOFT ACTIVITY)

**SDEVEN**

***

[TOC]

# CHANGELOG of v0.5

<small>

* For version code structure meaning see SDEVEN methodology document (*sic !*) :).
* with (F) are marked those changes that are features in order to be copied in a RELNOTE file
</small>v

## 0.5 (closed 220419 06:15)

### 0.5.6-release (220419 06:00)

* 220419d **published** 0.5.5 site

### 0.5.5-preview (220419 05:45)

* 220419c **cleaned** blog content from files (without deleting them)
* 220418d **home page change** the 3 elements under buttons are from main `src/pages/index` that imports `src/components ... HomePageFeatures`
* 220419b **improve** logo: remake as png (or svc), get the color or put REN clue color

### 0.5.4-preview (220418 07:40)

* 220418c **published** the new site on deployment server
* 220418b **build** a new static site (as `static_site_0.5.4.zip`)
* 220417g **publish** about incl ref to manual (pdf full) address it in site first page
* 220417d **sign & lock** pdf manual (full pdf)
* 220417h **made
*  about** - an About_SDEVEN.md doc which has: [x] about & copyright, [x] contributions (semver & appendix D), [x] ref to SDEVEN manual (pdf full version)

### 0.5.3-beta (220418 06:15)

* 220418a **open a new** content 0.5 version
* 220417c **moved** static built img archive into `content_0.4` directory
* 220417g **archive** content 0.4
* 220417f **new entry navbar**: Code of Conduct 75 RENCC
* 220417e **new entry navbar**: SDEVEN Index
* 220417b **renamed** content archive to `static_site_0.4.zip`

### 0.5.2-prerelease (220417 07:25)

* 220416i (@docusaurus) **restored** blog directory as it is referenced somewhere and must clean all places
* 220417a (@static-site) **published** static site: **`http(s)://static.renware.eu/sdeven/index.html`**
* 220416f (@static-site) **nginx** update in static server to point to `sdeven` directory. final url: `http://static.renware.eu/sdeven/index.html`
* 220415f (@static-site) **build** static site - also made a local archive as `static_site_image.zip`

### 0.5.1-02.alpha (220416 16:32)

* 220416h (@docusaurus) **cleaned** directory and add to git build for static site build
* 220416e (@static-site) **url** where site will go and can let base url as `/` (code of kv is `url: string,`)
* 220416c (@static-site) **base url** put it how it will be at final

### 0.5.1-01.alpha (220416 09:33)

* 220416d (@static-site) let it **stable** as `npm start`
* 220416d (@static-site) ok to **build** static site; there are problems with base url (`A very common reason is a wrong site baseUrl configuration`) open iss 220416c
* 220416b (@static-site) **dropped** blog refs and sections
* 220416a (@static-site) **copied** content (v0.4) to docusaurus location

> *see version history directory  for previous releases track*

--- ooo ---