
## 1. CONTENT directory

- [x] think to a directory where all documents will reside - now is **`content_0.6`/** but this was something usable then...
- [x] this directory should accommodate all docs incl images
- [x] proposal: **`SDEVEN_content_docs/`**



## 2. prepare `mkdocs` environment

- [x] prepare `mkdocs.yaml` **nav** section
- [x] move `.wenv` & `requirements.txt` in root
- [x] check in environment can be activated & `mkdocs` & `mkdocs build` run



## 3. final generated portal directory

- [x] decide how will be called - maybe **`static_portal/`** ?
- [x] OPTIONAL: protect it in `.gitignore`
- [ ] archive `content_0.6/` directory with manual generated PDFs (in `content_history/`) - #NOTEsee if keep FULL PDF DIRECTORY !
- [ ] check for left issues & drop myself (this directory)

## 4. Documents that have more than 1 `#` entry

This documents should "indent" for Heading 1 (`#`) entries and left just 1 representing the doc tile (otherwise mkdocs will not generate "right side" navigation as TOC):

- [ ] Appendix_B_DSGN_Content_Index.md
- [ ] Appendix_C_Status_Report.md



## 5. Other issues

- see how to automatically generate a "FULL PDF":
    - make SDEVEN index.md doc to include all docs (not very good solution, tried in `clusterCS` project and the TOC entries will recursively mirror generatic an unreadable document)
    - there is a `mkdocs` extension that generate PDFs (that which does not render mermaid) - maybe take a look in code to make a customization in `mkdocs`



