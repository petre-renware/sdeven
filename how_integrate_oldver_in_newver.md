
# How integrate prev content versions into new versions


action plan to integrate old version (`v6.0` in example) in current (new future) version:

1. save `doc_src/` ==> `doc_src_v6.0/

2. save `static_portal/`==> `static_portal_v6.0/`

3. create `doc_src/v6.0/` directory with an empty `index.md` text file (just to exists when used as reference, if feel better can write a comment inside it as it will never be generated as html)

4. update `mkdocs.yml` to ignore directory `doc_src/v6.0/` by mkdocs builder (but will keep it as is)

5. create `docs/v6.0/` directory

6. at least in `publishing` branch copy the old version saved site to dir from step (2), ie `static_portal_v6.0/` --> `docs/v6.0/`

* *Take care of:*
    * update new version `index.md` to reference previous version (`v6.0/index.md`)
    * do not drop from `docs/` directory `v6.0/` when you're publishing actual / current version



