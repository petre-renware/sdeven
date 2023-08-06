<small>(c) 2021 - 2023 RENware Software Systems</small>

**SDEVEN**

* Last published version: 7.0 beta

***

[TOC]

# CHANGELOG

<small>

* For version code structure follows SDEVEN methodology
* items targeted on RELNOTE docs:
    * with (F) are marked those changes that are features in order to be copied in a RELNOTE file
    * with (B) are marked relevant bugfixes (fixed in a released version different that where happened)
* -#NOTE ____ PUBLISHING IS MADE FROM `PUBLISHING` BRANCH, so wheen publish checkout it or upload from git
</small>


## 7.0 SDEVEN 7.0

#### [ start of #TODO_PLAN section ]=========================

* tbd... rework `readthedocs` but just refer `sdeven.renware.eu` and should work AND IS PRESENT ON READ_THE_DOCS

#### [ end of #TODO_PLAN section ]=========================



### 7.0.13-beta TESTing procedure (#NOTE wip)

* tbd... write content to `SDEVEN.25_SYTEST.md`

* wip...

* 230806piu_a `SDEVEN.25_SYTEST.md` new section ref to "Testing and working environments"
* 230805piu_j write content to `SDEVEN.25_SYTEST.md`, section _Preliminaries_
* 230805piu_i `SDEVEN.00_INDEX.md` facelift of structure for a better TOC and doc readability
* 230805piu_h refer test procedure in `SDEVEN.00_INDEX.md`
* 230805piu_g refer test procedure in `mkdocs.yml`
* 230805piu_f started a draft (toc & ideas ref sections content) testing procedure, doc `SDEVEN.25_SYTEST`, name *System Software Testing*











### 7.0.12-beta standardize & clean "Appendix (B) DSGN..." procedure (230805 09:15)

* 230805piu_e update `Appendix_B_DSGN_Content_Index.md`,  updated for documents should "indent" for Heading 1 (`#`) entries and left just 1 representing the doc tile
* 230805piu_d appendices title ("Appendix" like) release dates, versions for following files:
    * [x] `Appendix_A_Semantic_versioning.md`
    * [x] `Appendix_B_DSGN_Content_Index.md`
    * [x] `Appendix_C_Status_Report.md`
    * [x] `Appendix_D_ROADMAP_template.md`
    * [x] `Appendix_E_RELNOTE_template.md`
    * [x] `Appendix_Q_faq.md`
* 230805piu_c `Appendix_B_DSGN_Content_Index.md` updated for documents should "indent" for Heading 1 (`#`) entries and left just 1 representing the doc tile (((up to "# 900-OPS Operations", exclusive)))
* 230805piu_b review of 00.INDEX ref order
* 230805piu_a installed `markdown-exec` and use `tree` feature to update `SDEVEN.62_PSTR.md`, section "Example of project full directory structure"




### 7.0.11-beta RELNOTE template (230804 19:45)

* 230804piu_h update `00-INDEX`, `55-TRACE` and `60-RELM` procedures ref `Appendix_E_RELNOTE_template.md` document (resulted from 230804piu_f)
* (B) 230804piu_g
    * updated `mkdocs.yml` ref `Appendix_E_RELNOTE_template.md` document (resulted from 230804piu_f)
    * updated `Appendix_C_Status_Report.md` set code-name as `STATUSR`
* 230804piu_f make a new doc for `Appendix_E_RELNOTE_template.md`
* (B) 230804piu_e fixed bug in `SDEVEN.55-TRACE`, section `Taxonomy`, first paragraph, there is wrong link (has no name and no link address like text `[]...`)




### 7.0.10-beta SDEVEN Status_report (230804 13:10)

* 230804piu_d updated `SDEVEN.55_TRACE.md` ref section where "Status_report..." is referred to address new file resulted from 230804piu_b
* 230804piu_c fixed 230804piu_b resulted  doc as: *updated date & version as 7.0.10* 
* 230804piu_b `Appendix_C_Status_Report.md` update content and set a target reason according to **45.OPME** (usually for one of `devREVW` & `prodREVW` meeting types)
* 230804piu_a created `.readthedocs.yaml` for integration with and publish on *Read the docs* - experimental, need more work
* 230803piu_c fixed bugs ref `SDEVEN.62_PSTR.md` directories representation
* 230803piu_b reviewed and closed `RMAP.001` in ROADMAP file
* 230803piu_a `SDEVEN.62_PSTR.md` facelifts - improved organization and readability




### 7.0.9-beta RMAP.001 - OPME (230802 15:30)

* 230802piu_d `SDEVEN.45_OPME.md` described OPME _`prodREVW`_ meeting
* 230802piu_c `SDEVEN.45_OPME.md` updated meetings type with property ref TYPE (plan, review) and recommended FREQUENCY
* 230802piu_b `SDEVEN.45_OPME.md` described OPME _`devREVW`_ meeting
* 230802piu_a updated `About_SDEVEN.md` ref contributors
* 230801piu_e `SDEVEN.45_OPME.md` described OPME _`devOPER`_ meeting
* 230801piu_d updated `SDEVEN.55_TRACE.md` ref where the `sprint` comes from
* 230801piu_c updated `Appendix_D_ROADMAP_template.md`
* 230801piu_b updated `About_SDEVEN.md` ref contributors
* 230801piu_a update navigation menu for entry names (SDEVEN instead of Methodology)
* 230731piu_k `SDEVEN.45_OPME.md` prepared renaming meeting sections with RAW text that must be reviewed and make clean and relevant to SDEVEN
* 230731piu_j `SDEVEN.45_OPME.md` described OPME _`devPLAN`_ meeting
* 230731piu_i `SDEVEN.45_OPME.md` described `sprint` process / event and classified meetings + prepared place fo detailed description + updated `mkdocs.yml` for OPM name (dropped incoming acronym)
* 230731piu_h made a draft skeleton with TOC and todo-s, notes, ideas for each section of `SDEVEN.45_OPME.md` - needs refinement of each meeting types
* 230730piu_g updated `mkdocs.yml` to accommodate Markdown in HTML and to set `HTML attributes`
* 230730piu_f updated procedure `SDEVEN.45_OPME.md` ref release version, date and where to search for information
* 230730piu_e "gross" review & update of `95-RENCOCL.md` + `mkdocs.yaml` entry + refactor code from `RENCOCL` to `COCL` (including document filename)




### 7.0.8-beta (230730 09:00)

* 230730piu_d "gross" review & update of `90.RENBLU` + `mkdocs.yaml` entry
* 230730piu_c set a CNAME file in `doc_src/` directory with domain name as `sdeven.renware.eu`
* 230730piu_b install and include plugin `git-revision-date-localized` (`https://henrywhitaker3.github.io/mkdocs-material-dark-theme/plugins/revision-date/`)
* 230730piu_a procedure `SDEVEN.10-ADM` item `Last update: ...` must be called `Released date: ...`
* 260726piu_a fixed RENware portal access
* 230723piu_b changed theme color to `teal` as new color for RENware internal resources
* 230723piu_a changed top navbar **logo** to a SDEVEN logon instead of RENware logo
* 230721piu_a upload `Scrum-Guide-2020-US.pdf` in directory `wk_crt_proposals/`
* 230720piu_a fixed copyright text in `mkdocs.yml`




### 7.0.7-beta (230718 11:30)

* 230718piu_c set `site_author: 'xxx'` & `copyright: 'xxx'` in `mkdocs.yml` - these configs are KV entries at root level
* 230718piu_b update `SDEVEN.62_PSTR.md` procedure for:
    * `docs` as publishing static site (is finalized at a release from `static_portal`),
    * `doc_src` as source directory
    * `static_portal` as generation and test of static portal
* 230718piu_a refactor `SDEVEN_content_docs` according to procedure `SDEVEN.62_PSTR.md`
* 230717piu_f `SDEVEN.45_OPME.md` add some useful comments ref SCRUM Events as subjects to cover in procedure
* 230717piu_e prepare an empty doc for `45-OPME` procedure (just as empty under construction document) & updated all references (mkdocs.yml & 00-INDEX)
* 230717piu_d the FULL SITE html document make "Download PDF" link in `index.md` as now the PDF exists on normal path for all PDF docs (`_site_dir_/pdfs/...`); updated left navigation bar to have an entry for full PDF manual
* 230717piu_c in order to have `/print_page/` directory created, move `pdf-with-js` plugin AFTER `print-site` plugin
* 230717piu_b included a `print_page.md` as empty doc that serve as reference for final generation of `print_page.html` (generation is delayed and is based on final result of site navigation structure)
* 230717piu_a fixed `About_SDEVEN.md` link entry at text "A complete SDEVEN manua..."
* 230716piu_f add `RMAP.001 OPME` and prepared "all places" where will be placed (SDEVEN 00 index & mkdocs.yml for navogation entry)
* 230716piu_e implemented PDF BUTTON FOR FULL DOC in `mkdocs.yml`, `print-site` plugin, option `path_to_pdf` - TEST FAILED, reverted file to previous version
* 230716piu_d rebuild portal and publish for new version updated in procedures
* 230716piu_c refactored `50-RENCHGM` to `50-CHGMNG`
* 230716piu_b add a ROADMAP file to log future improvements and intentions
* 230716piu_a updated SDEVEN logo with minor version number resulting "7.0"
* 230715piu_c to change version in all docs to 7.0.7 (search for `0.7.` and change to `7.0.`)




### 7.0.6-alpha (230626 12:00)

* 230715piu_b made a template for `ROADMAP_template` document and ref it in `55-TRACE` procedure
* 230715piu_a "gross" review & update of `80.RENCOPRI` + `mkdocs.yaml` entry + refactor code from `RENCOPRI` to `COPRI` (including document filename)
* 230712piu_b "gross" review & update of `75.RENCC` + `mkdocs.yaml` entry + refactor code from `RENCC` to `CCEP` (including document filename)
* 230712piu_a installed "Full PDF" generation and printing option & activated in site navigation
* 230711piu_b dropped the doc `Appendix_D_Fundamentals_of_Test_Management.pdf` as being too "book" and, anyway, a TESTING procedure should be described...
* 230711piu_a updated SDEVEN logo with majpr version number (to be able to visualize to version "at first sight" of manual cover)
* 230702piu_c updated README with GitHub URL for public SDEVEN static site
* 230703piu_b renamed `published_site` to `/docs` & updated README (rule imposed by GitHub platform)
* 230702piu_a created `published_site` as **publishing directory** and copied current content in (partial publishing)
* 230628piu_a put in portal RENware logo & updateded (just prepared) SDEVEN logo with a small one for docs inside
* 230626piu_d "gross" review & update of `70.RENLIP` + `mkdocs.yaml` entry + refactor code from `RENLIP` to `LIP` (including document filename)
* 230626piu_c "gross" review & update of `68.RENCOREV` + `mkdocs.yaml` entry + refactor code from RENCOREV` to `COREV` (including document filename)




### 7.0.5-alpha (230626 12:00)

* 230626piu_b "gross" review & update of `65.RENDEREV` + `mkdocs.yaml` entry + refactor code from `RENDEREV` to `DEREV` (including document filename)
* 230626piu_a update of `62.PSTR` with a very short reference to project root directory for a README.md & project.toml files
* 230622piu_a "gross" review & update of `62.PSTR` + `mkdocs.yaml` entry + refactor code from `RENSTR` to `PSTR` (including document filename)
* 230621piu_a "gross" review & update of `60.RELM` + `mkdocs.yaml` entry + refactor code from `RENRELM` to `RELM` (including document filename)
* 230620piu_c "gross" review & update of `55.TRACE` + `mkdocs.yaml` entry + refactor code from `RENTRACE` to `TRACE` (including document filename)
* 230620piu_b update `40.BRAN` with a Git diagram ref basic flow of master, development, xxx-dev and allowed tags (tagging policy)
* 230620piu_a update `40.BRAN` with proposals made in January 2023 + clean doc and change code from RENBRAN to `BRAN`
* 230619piu_g "gross" review & update of `50.CHGM` + `mkdocs.yaml` entry
* 230619piu_f "gross" review & update of `40.BRAN` + `mkdocs.yaml` entry
* 230619piu_e "gross" review & update of `30.VER` + `mkdocs.yaml` entry
* 230619piu_d "gross" review & update of `20.PRA` + `mkdocs.yaml` entry
* 230619piu_c clean directories, update version on all changed documents and updated shorts actions plan
* 230619piu_b finish and closed 10.ADM




### 7.0.4-alpha (230619 06:30)

* 230619piu_a minor updates in 10.ADM ref section names to have a more administrative and staffing impact
* 230618piu_f closed `index.md` as cover with 2 links: About SDEVEN & Start book here
* 230618piu_e adjust picture background to make @ picture dimensions
* 230618piu_d update SDEVEN logo (generate a SVG, change directory in `SDEVEN_content_docs/pictures/`)
* 230618piu_c created a remote repository and sync all SDEVEN repository
* 230618piu_b:
    * `SDEVEN.00_INDEX.md` clear useless `#` headings to make more readable the document
    * reorganized site navigation menu to follow readability created in `SDEVEN.00_INDEX` change
* 230618piu_a drop directory `docusausurus_portal/` as this solution is no more used
* 230617piu_h more actions as:
    * change menu entries (lef navigation bar) to make the more readable
    * add Creative Commons license and linked it in `About_SDEVEN.md` file
    * created `index.md` as symbolic link to `SDEVEN.00_INDEX.md` (to assure compatibility with "old" simple HTTP servers)
    * right (as strings) qualified `mkdocs.yaml nav entries` to avoid mistakes generated by blank character
* 230617piu_g more actions as:
    * check & clean all docs for unaccepted changes for string as `<<< HEAD...` or `>>> ...`
    * archive `content_0.6/` directory with manual generated PDFs (in `content_history/`)
* 230617piu_h reinitialized full git ... and cleaned all directories and files
* 230617piu_g prepare `mkdocs.yaml` **nav** section - list of "left-out" documents [here](mkdocs_site_builder/README_CHECKLIST.md#2-prepare-mkdocs-environment)
* 230617piu_f created a doc `/xxx` with frequent / useful git commands (especially when working with large data such as books, documentation, etc)
* 230617piu_e started a clean work with mkdoc




### 7.0.3-alpha (230617 10:00)

* 230617d release 7.0.4-alpha as **SDEVEN draft 0.7 built with mkdocs**
* 230617c update project README file ref all changes by moving to `mkdocs` site generation
* 230617b cleaning & archiving history directories by moving historical generated sites to `.../880.90_SCA_Source_Code_Archives/generated_sites/` directory
* 230617a cleaning & archiving history directories by moving historical content to `.../880.90_SCA_Source_Code_Archives/content_history` directory + drop all temp `xxx*/` directories
* 230616e clean `content_history/` directory for older than v0.6 generated portals (files `dtatic_site_build_...`) and archive SDEVEN content of v0.6 and market `content_0.6/` dire tory for deletion
* 230616d prepare first mkdocs environment to generate a draft portal - DONE. generated a first site more than draft ! FACTS:
    * ---> made last released version and current working is in directory: **`SDEVEN_content_docs/`**
    * ---> generated static portal directory: **`static_portal/`**
* 230616c add more things to do in `mkdocs_site_builder/` README_CHECKLIST file (docs with more that 1 Heading1 & ideas for FULL PDF doc)
* 230616b dropped `docusaurus/` (previous solution to static portal generator) and make a temp copy out of `830-DEV/` directory
* 230617a preparations to switch to `mkdocs` static site generator (directory `mkdocs_site_builder/`)
* 230109c add `mkdocs` material admonition blocks
* 230109b add PDF exporter for `mkdocs`




###  7.0.2-alpha (230109 06:00)

* 230109a introduced a new site builder with *MkDocs* in directory `mkdocs_site_builder`




### 7.0.1-alpha (220819 19:35)

* 220819c updated `SDEVEN.40_BRAN` ref branches usage recommended techniques
* 220819b updated `Appendix_B_DSGN_Content_Index.md` ref a text from **sagaRT** project, inserted in doc a text to remember...
* 220819a updated `SDEVEN.90_RENBLU`
* 220803a updated `Appendix_B_DSGN_Content_Index.md` ref a text from git merge missed in (@BOOK.007-15.d) and 830-DEV added as no doc section but frequently asked why is missing from numbering schema :)








> *see version history directory  for previous releases track*

## History of changes log

* [SDEVEN 0.6](versions_history/CHANGELOG_0.6.md)
* [SDEVEN 0.5](versions_history/CHANGELOG_0.5.md)
* [SDEVEN 0.4](versions_history/CHANGELOG_0.4.md)
* [SDEVEN 0.3](versions_history/CHANGELOG_0.3.md)






