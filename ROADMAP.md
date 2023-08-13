<small>**SDEVEN Software Development & Engineering Methodology**</small>


***

***Document control***

* updated at: 230810<br>
* updated by: Petre Iordanescu



***Table of contents***

[TOC]


# ROADMAP



## RMAP.004 - convert to Word (docx) format the full document - (temp closed @ 230810)

* **Objective:** convert to Word (docx) format the full document
* **Recorded at:** 230810
* **Updated at**:
    * 230810 [Petre Iordanescu] tested locally, generated `DOCX` from `HTML` & `PDF` ok, resulted document has "protection" footers and banners (ie, undesired, unwanted text) that can be manually dropped or by using a paid license (price magnitude 1.5 - 3 kUSD), genration time ~10sec for source full SDEVEN HTML and ~1min for full SDEVEN PDF
    * 230810 [Petre Iordanescu] **resolution**: not to be used except a licence is paid by client, can be kept as optional feature included in site generation only with paid license
* **Recorded by:** Petre Iordanescu (piu)
* **Detailed  description:**
    * convert to Word (docx) format the full document
    * _Aspose_ offer multiple variants for output file (`doc` & `docx`) - choose the _free commercially licensed one_
* **Recommendations:**
    * use _Aspose_ tool (see refs)
    * make a _Python script_ that is execute ***after*** `mkdocs build` finish execution (in order to have the full doc generated as HTML and PDF)
    * create a script (`bash` and `cmd / bat` types) that "integrates" final build (by running Word generator after mkdocs build)
* **Known dependencies:** -
* **Assigned to:** Petre Iordanescu
* **References & notes:**
    * _Aspose_ tool details @ `https://pypi.org/project/aspose-words/` 






# Closed and archived issues

* [RMAP.003 - integrate old version in new ones](versions_history/RMAP_003.md)
* [RMAP.002 - 25_SYTEST templates](versions_history/RMAP_002.md)
* [RMAP.001 - OPME](versions_history/RMAP_001.md)







# Templates & other misc...

``` #NOTE: TEMPLATE section use for future

## RMAP.item_code - #NOTE...give a hort description name of item

* **Objective:** -#NOTE...the item objective...
* **Recorded at:** -#NOTE...date of recording this item...
* **Updated at**: n/a
* **Recorded by:** -#NOTE...who registered this item - this should identify that person as mail and phone, otherwise these should be written here...
* **Detailed  description:**
    * -#NOTE...here different items of description...
    * -#NOTE...here different items of description...
* **Recommendations:**
    * -#NOTE...here different items of hints / recommendations...
    * -#NOTE...here different items of hints / recommendations...
* **Known dependencies:** -#NOTE...if there are knwon dependencies of INTERNAL system components or other open / wip issues...
* **Assigned to:** -#NOTE...the person nominated to respond for this roadmap item...
* **References & notes:**
    * -#NOTE...more notes... (if use footnote like `[^xxx]: ...`, please do not mark as list entry because will appear at foonotes)

```









