# Comparing `tmp/pypath_omnipath-0.14.48.tar.gz` & `tmp/pypath_omnipath-0.15.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypath_omnipath-0.14.48.tar", max compression
+gzip compressed data, was "pypath_omnipath-0.15.4.tar", max compression
```

## Comparing `pypath_omnipath-0.14.48.tar` & `pypath_omnipath-0.15.4.tar`

### file list

```diff
@@ -1,329 +1,343 @@
--rw-r--r--   0        0        0    35141 2016-11-05 19:50:35.500333 pypath_omnipath-0.14.48/LICENSE
--rw-r--r--   0        0        0    11492 2023-03-28 22:05:50.316062 pypath_omnipath-0.14.48/README.rst
--rw-r--r--   0        0        0     2743 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/__init__.py
--rw-r--r--   0        0        0     2057 2023-04-12 15:39:36.242305 pypath_omnipath-0.14.48/pypath/_metadata.py
--rw-r--r--   0        0        0      666 2022-12-05 01:12:34.011729 pypath_omnipath-0.14.48/pypath/biocypher/__init__.py
--rw-r--r--   0        0        0     7863 2022-12-05 01:12:34.011729 pypath_omnipath-0.14.48/pypath/biocypher/adapter.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.502224 pypath_omnipath-0.14.48/pypath/core/__init__.py
--rw-r--r--   0        0        0   174945 2023-03-29 12:47:27.521270 pypath_omnipath-0.14.48/pypath/core/annot.py
--rw-r--r--   0        0        0     4327 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/core/attrs.py
--rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/core/common.py
--rw-r--r--   0        0        0    19000 2023-03-29 12:48:22.415968 pypath_omnipath-0.14.48/pypath/core/complex.py
--rw-r--r--   0        0        0    13228 2023-03-29 23:28:02.614928 pypath_omnipath-0.14.48/pypath/core/entity.py
--rw-r--r--   0        0        0    37353 2022-11-29 10:17:12.502224 pypath_omnipath-0.14.48/pypath/core/enz_sub.py
--rw-r--r--   0        0        0    20612 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/core/evidence.py
--rw-r--r--   0        0        0    95812 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/core/interaction.py
--rw-r--r--   0        0        0    30155 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/core/intercell.py
--rw-r--r--   0        0        0   230647 2022-11-29 10:17:12.505557 pypath_omnipath-0.14.48/pypath/core/intercell_annot.py
--rw-r--r--   0        0        0   140737 2023-03-29 23:08:59.315836 pypath_omnipath-0.14.48/pypath/core/network.py
--rw-r--r--   0        0        0      138 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/data/__init__.py
--rw-r--r--   0        0        0     1300 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/embl_colors
--rw-r--r--   0        0        0      271 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/ensembl_biomart_query.xml
--rw-r--r--   0        0        0      227 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/goose_ancestors.sql
--rw-r--r--   0        0        0      712 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/goose_annotations.sql
--rw-r--r--   0        0        0      120 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/goose_terms.sql
--rw-r--r--   0        0        0      185 2023-03-30 00:53:33.672441 pypath_omnipath-0.14.48/pypath/data/licenses/afl_v3.json
--rw-r--r--   0        0        0      186 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/apache_2.0.json
--rw-r--r--   0        0        0      190 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/artistic_2.0.json
--rw-r--r--   0        0        0      199 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/biocarta.json
--rw-r--r--   0        0        0      188 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/bsd.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_2.5.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_3.0.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_4.0.json
--rw-r--r--   0        0        0      242 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc-nd_3.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc-nd_4.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_2.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_3.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_4.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_sa_3.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_sa_4.0.json
--rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nd_3.0.json
--rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nd_4.0.json
--rw-r--r--   0        0        0      224 2023-03-30 00:45:57.463174 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_sa_2.5.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_sa_3.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_sa_4.0.json
--rw-r--r--   0        0        0      233 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_zero.json
--rw-r--r--   0        0        0      196 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cellcellinteractions.json
--rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/composite.json
--rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cosmic.json
--rw-r--r--   0        0        0      194 2022-03-18 18:18:43.477819 pypath_omnipath-0.14.48/pypath/data/licenses/cytosig.json
--rw-r--r--   0        0        0      182 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/dsl.json
--rw-r--r--   0        0        0      185 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/elm.json
--rw-r--r--   0        0        0      174 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/data/licenses/embl-ebi.json
--rw-r--r--   0        0        0      212 2023-04-05 14:14:07.817106 pypath_omnipath-0.14.48/pypath/data/licenses/eul.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/gnu_gpl_v2.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/gnu_gpl_v3.json
--rw-r--r--   0        0        0      200 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/gnu_lgpl_v3.json
--rw-r--r--   0        0        0      311 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/hgnc.json
--rw-r--r--   0        0        0      150 2022-09-15 18:20:39.089511 pypath_omnipath-0.14.48/pypath/data/licenses/hpo.json
--rw-r--r--   0        0        0      139 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/hprd.json
--rw-r--r--   0        0        0      168 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/i2d.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/informal.json
--rw-r--r--   0        0        0      175 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/kegg.json
--rw-r--r--   0        0        0      174 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/kinase-com.json
--rw-r--r--   0        0        0      268 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mirecords.json
--rw-r--r--   0        0        0      184 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mirtarbase.json
--rw-r--r--   0        0        0      154 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mit.json
--rw-r--r--   0        0        0      165 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mppi.json
--rw-r--r--   0        0        0      360 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/nar.json
--rw-r--r--   0        0        0      179 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/no_license.json
--rw-r--r--   0        0        0      177 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/pathwaycommons.json
--rw-r--r--   0        0        0      351 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/pdb.json
--rw-r--r--   0        0        0      363 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/phosphonetworks.json
--rw-r--r--   0        0        0      464 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/unspecified.json
--rw-r--r--   0        0        0     5731 2023-03-29 13:56:06.759376 pypath_omnipath-0.14.48/pypath/data/settings.yaml
--rw-r--r--   0        0        0     1150 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/www/favicon.ico
--rw-r--r--   0        0        0      486 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/www/http500.html
--rw-r--r--   0        0        0      324 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/www/index.html
--rw-r--r--   0        0        0     5815 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/formats/obo.py
--rw-r--r--   0        0        0     8624 2023-03-09 00:29:38.782357 pypath_omnipath-0.14.48/pypath/formats/sqldump.py
--rw-r--r--   0        0        0     1358 2023-03-09 17:12:37.914407 pypath_omnipath-0.14.48/pypath/formats/sqlite.py
--rw-r--r--   0        0        0     7508 2023-03-13 13:39:42.775048 pypath_omnipath-0.14.48/pypath/formats/xml.py
--rw-r--r--   0        0        0     2204 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/__init__.py
--rw-r--r--   0        0        0     1075 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/abs.py
--rw-r--r--   0        0        0     3155 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/acsn.py
--rw-r--r--   0        0        0     2422 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/adhesome.py
--rw-r--r--   0        0        0     2343 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/almen2009.py
--rw-r--r--   0        0        0     5340 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/baccin2019.py
--rw-r--r--   0        0        0     6319 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/inputs/biogps.py
--rw-r--r--   0        0        0     5016 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/biogrid.py
--rw-r--r--   0        0        0    10223 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/biomart.py
--rw-r--r--   0        0        0     5365 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/biomodels.py
--rw-r--r--   0        0        0     1794 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/ca1.py
--rw-r--r--   0        0        0     2760 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/cancercellmap.py
--rw-r--r--   0        0        0     5541 2023-03-23 11:43:45.220378 pypath_omnipath-0.14.48/pypath/inputs/cancerdrugsdb.py
--rw-r--r--   0        0        0     1907 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/cancersea.py
--rw-r--r--   0        0        0     3358 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cell.py
--rw-r--r--   0        0        0     6338 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cellcall.py
--rw-r--r--   0        0        0     1551 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/cellcellinteractions.py
--rw-r--r--   0        0        0     9191 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/cellchatdb.py
--rw-r--r--   0        0        0    15036 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cellinker.py
--rw-r--r--   0        0        0     9174 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cellphonedb.py
--rw-r--r--   0        0        0     5398 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/celltalkdb.py
--rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/celltypist.py
--rw-r--r--   0        0        0    13899 2023-03-09 16:16:55.198353 pypath_omnipath-0.14.48/pypath/inputs/chembl.py
--rw-r--r--   0        0        0     3454 2023-04-07 15:34:02.552665 pypath_omnipath-0.14.48/pypath/inputs/clinvar.py
--rw-r--r--   0        0        0     5564 2023-03-30 21:50:08.109288 pypath_omnipath-0.14.48/pypath/inputs/collectri.py
--rw-r--r--   0        0        0     7920 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/common.py
--rw-r--r--   0        0        0     2656 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/compleat.py
--rw-r--r--   0        0        0     4509 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/complexportal.py
--rw-r--r--   0        0        0     4036 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/comppi.py
--rw-r--r--   0        0        0     2788 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/connectomedb.py
--rw-r--r--   0        0        0     2793 2023-03-23 12:55:34.154293 pypath_omnipath-0.14.48/pypath/inputs/corum.py
--rw-r--r--   0        0        0     4779 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/cosmic.py
--rw-r--r--   0        0        0     4234 2023-03-29 21:02:25.987565 pypath_omnipath-0.14.48/pypath/inputs/cpad.py
--rw-r--r--   0        0        0     1989 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cpdb.py
--rw-r--r--   0        0        0     3412 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/credentials.py
--rw-r--r--   0        0        0     3344 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/csa.py
--rw-r--r--   0        0        0     3547 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/cspa.py
--rw-r--r--   0        0        0     5114 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/ctdbase.py
--rw-r--r--   0        0        0     3343 2023-03-22 17:05:50.626476 pypath_omnipath-0.14.48/pypath/inputs/cytosig.py
--rw-r--r--   0        0        0     4765 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/dbptm.py
--rw-r--r--   0        0        0     2833 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/deathdomain.py
--rw-r--r--   0        0        0     4384 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/depod.py
--rw-r--r--   0        0        0     3721 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.48/pypath/inputs/dgidb.py
--rw-r--r--   0        0        0     4921 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/dip.py
--rw-r--r--   0        0        0    68257 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/disgenet.py
--rw-r--r--   0        0        0    17135 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/domino.py
--rw-r--r--   0        0        0    12715 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/dorothea.py
--rw-r--r--   0        0        0    20676 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/drugbank.py
--rw-r--r--   0        0        0     4706 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/drugcentral.py
--rw-r--r--   0        0        0     4803 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/ebi.py
--rw-r--r--   0        0        0     4929 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/elm.py
--rw-r--r--   0        0        0     2523 2023-03-28 12:11:30.004207 pypath_omnipath-0.14.48/pypath/inputs/embopress.py
--rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/embrace.py
--rw-r--r--   0        0        0     1220 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/encode.py
--rw-r--r--   0        0        0     1982 2023-04-05 00:14:36.657341 pypath_omnipath-0.14.48/pypath/inputs/ensembl.py
--rw-r--r--   0        0        0     3152 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/exocarta.py
--rw-r--r--   0        0        0     3425 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/genecards.py
--rw-r--r--   0        0        0    26086 2023-03-28 21:26:09.280054 pypath_omnipath-0.14.48/pypath/inputs/go.py
--rw-r--r--   0        0        0     2356 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/gpcrdb.py
--rw-r--r--   0        0        0     1937 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/graphviz.py
--rw-r--r--   0        0        0     8093 2023-03-28 11:43:53.797828 pypath_omnipath-0.14.48/pypath/inputs/guide2pharma.py
--rw-r--r--   0        0        0     1597 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/havugimana.py
--rw-r--r--   0        0        0     1628 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/hgnc.py
--rw-r--r--   0        0        0     3763 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/hippie.py
--rw-r--r--   0        0        0    12568 2023-03-20 14:49:33.714166 pypath_omnipath-0.14.48/pypath/inputs/hmdb.py
--rw-r--r--   0        0        0     4862 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/homologene.py
--rw-r--r--   0        0        0    10335 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/hpmr.py
--rw-r--r--   0        0        0     4781 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/hpo.py
--rw-r--r--   0        0        0     2748 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/hprd.py
--rw-r--r--   0        0        0     1491 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/htri.py
--rw-r--r--   0        0        0     1773 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/humancellmap.py
--rw-r--r--   0        0        0     2048 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/humap.py
--rw-r--r--   0        0        0     8093 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/huri.py
--rw-r--r--   0        0        0     2665 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/i3d.py
--rw-r--r--   0        0        0     6713 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/icellnet.py
--rw-r--r--   0        0        0     8076 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/ielm.py
--rw-r--r--   0        0        0     3914 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/imweb.py
--rw-r--r--   0        0        0     2242 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/innatedb.py
--rw-r--r--   0        0        0     3005 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/instruct.py
--rw-r--r--   0        0        0     5688 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/intact.py
--rw-r--r--   0        0        0     1741 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/integrins.py
--rw-r--r--   0        0        0     8866 2023-03-28 21:43:59.156468 pypath_omnipath-0.14.48/pypath/inputs/interpro.py
--rw-r--r--   0        0        0     2530 2023-03-29 19:46:17.335600 pypath_omnipath-0.14.48/pypath/inputs/intogen.py
--rw-r--r--   0        0        0     1708 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/ipi.py
--rw-r--r--   0        0        0     3630 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/iptmnet.py
--rw-r--r--   0        0        0     3192 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/italk.py
--rw-r--r--   0        0        0     2557 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/kea.py
--rw-r--r--   0        0        0    20673 2023-03-29 12:38:13.194490 pypath_omnipath-0.14.48/pypath/inputs/kegg.py
--rw-r--r--   0        0        0    14746 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/kegg_api.py
--rw-r--r--   0        0        0     1932 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/kinasedotcom.py
--rw-r--r--   0        0        0     2522 2023-03-29 14:45:43.764405 pypath_omnipath-0.14.48/pypath/inputs/kirouac2010.py
--rw-r--r--   0        0        0     4327 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/lambert2018.py
--rw-r--r--   0        0        0     2174 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/laudanna.py
--rw-r--r--   0        0        0     5633 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/li2012.py
--rw-r--r--   0        0        0     2625 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/lincs.py
--rw-r--r--   0        0        0     2926 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/lmpid.py
--rw-r--r--   0        0        0     1549 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/lncdisease.py
--rw-r--r--   0        0        0     2026 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/lncrnadb.py
--rw-r--r--   0        0        0     7887 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/locate.py
--rw-r--r--   0        0        0     3648 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/lrdb.py
--rw-r--r--   0        0        0     2907 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/macrophage.py
--rw-r--r--   0        0        0      568 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/main.py
--rw-r--r--   0        0        0     2334 2023-03-28 17:55:35.707415 pypath_omnipath-0.14.48/pypath/inputs/matrisome.py
--rw-r--r--   0        0        0     4171 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/matrixdb.py
--rw-r--r--   0        0        0     1107 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/mcam.py
--rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/membranome.py
--rw-r--r--   0        0        0     4296 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/mimp.py
--rw-r--r--   0        0        0     1365 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/mir2disease.py
--rw-r--r--   0        0        0     3865 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/mirbase.py
--rw-r--r--   0        0        0     1742 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/mirdeathdb.py
--rw-r--r--   0        0        0     1659 2023-03-29 17:59:15.511751 pypath_omnipath-0.14.48/pypath/inputs/mirecords.py
--rw-r--r--   0        0        0     2177 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/mirtarbase.py
--rw-r--r--   0        0        0     1069 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/mitab.py
--rw-r--r--   0        0        0     3166 2023-03-23 12:55:18.904569 pypath_omnipath-0.14.48/pypath/inputs/mppi.py
--rw-r--r--   0        0        0    11491 2023-04-04 23:37:06.309559 pypath_omnipath-0.14.48/pypath/inputs/msigdb.py
--rw-r--r--   0        0        0     2100 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/ncrdeathdb.py
--rw-r--r--   0        0        0     1830 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/negatome.py
--rw-r--r--   0        0        0     1758 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/netbiol.py
--rw-r--r--   0        0        0     6376 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/netpath.py
--rw-r--r--   0        0        0     2994 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.48/pypath/inputs/oma.py
--rw-r--r--   0        0        0     3600 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/ontology.py
--rw-r--r--   0        0        0     2845 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/opm.py
--rw-r--r--   0        0        0     2313 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/oreganno.py
--rw-r--r--   0        0        0     4003 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/panglaodb.py
--rw-r--r--   0        0        0     3558 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.48/pypath/inputs/pathophenodb.py
--rw-r--r--   0        0        0     4593 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/pathwaycommons.py
--rw-r--r--   0        0        0     1071 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/pazar.py
--rw-r--r--   0        0        0     6333 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/pdb.py
--rw-r--r--   0        0        0     2411 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/pdzbase.py
--rw-r--r--   0        0        0     6660 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/pepcyber.py
--rw-r--r--   0        0        0     9162 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/pfam.py
--rw-r--r--   0        0        0     6669 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/pharos.py
--rw-r--r--   0        0        0     1673 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/phobius.py
--rw-r--r--   0        0        0     2299 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/phosphatome.py
--rw-r--r--   0        0        0     3433 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/phosphoelm.py
--rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/phosphonetworks.py
--rw-r--r--   0        0        0     1299 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/phosphopoint.py
--rw-r--r--   0        0        0    37326 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/phosphosite.py
--rw-r--r--   0        0        0     9976 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/pisa.py
--rw-r--r--   0        0        0     1850 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/pro.py
--rw-r--r--   0        0        0     3189 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/progeny.py
--rw-r--r--   0        0        0     7531 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/proteinatlas.py
--rw-r--r--   0        0        0     3573 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/proteins.py
--rw-r--r--   0        0        0     3808 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/protmapper.py
--rw-r--r--   0        0        0     2463 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/pubchem.py
--rw-r--r--   0        0        0     4224 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/pubmed.py
--rw-r--r--   0        0        0     4418 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/ramilowski2015.py
--rw-r--r--   0        0        0     5426 2023-03-22 21:01:49.738609 pypath_omnipath-0.14.48/pypath/inputs/ramp.py
--rw-r--r--   0        0        0     6496 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/rdata.py
--rw-r--r--   0        0        0    40102 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/reaction.py
--rw-r--r--   0        0        0     7539 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/scconnect.py
--rw-r--r--   0        0        0     2455 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/science.py
--rw-r--r--   0        0        0     5578 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/signalink.py
--rw-r--r--   0        0        0    11727 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/signor.py
--rw-r--r--   0        0        0     5681 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/spike.py
--rw-r--r--   0        0        0     4287 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/stitch.py
--rw-r--r--   0        0        0     7315 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/string.py
--rw-r--r--   0        0        0     1579 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/surfaceome.py
--rw-r--r--   0        0        0     4412 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/switches_elm.py
--rw-r--r--   0        0        0     3225 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/talklr.py
--rw-r--r--   0        0        0     2616 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/tcdb.py
--rw-r--r--   0        0        0     2119 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/tfcensus.py
--rw-r--r--   0        0        0     7926 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/threedcomplex.py
--rw-r--r--   0        0        0    17368 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/threedid.py
--rw-r--r--   0        0        0     3692 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/topdb.py
--rw-r--r--   0        0        0     1453 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/transmir.py
--rw-r--r--   0        0        0     9902 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/trip.py
--rw-r--r--   0        0        0     5196 2023-03-19 23:05:05.810094 pypath_omnipath-0.14.48/pypath/inputs/unichem.py
--rw-r--r--   0        0        0    31311 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/uniprot.py
--rw-r--r--   0        0        0     7602 2023-03-29 16:56:14.179505 pypath_omnipath-0.14.48/pypath/inputs/wang.py
--rw-r--r--   0        0        0     2171 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/wojtowicz2020.py
--rw-r--r--   0        0        0     1619 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/zhong2015.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/__init__.py
--rw-r--r--   0        0        0    11896 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/annot_formats.py
--rw-r--r--   0        0        0    21507 2023-03-23 08:10:01.341026 pypath_omnipath-0.14.48/pypath/internals/input_formats.py
--rw-r--r--   0        0        0    43762 2023-03-27 19:06:47.600564 pypath_omnipath-0.14.48/pypath/internals/intera.py
--rw-r--r--   0        0        0     7533 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/license.py
--rw-r--r--   0        0        0     7257 2023-03-06 18:13:55.980766 pypath_omnipath-0.14.48/pypath/internals/maps.py
--rw-r--r--   0        0        0     4199 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/refs.py
--rw-r--r--   0        0        0     9673 2023-03-10 13:53:12.961501 pypath_omnipath-0.14.48/pypath/internals/resource.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.14.48/pypath/legacy/__init__.py
--rw-r--r--   0        0        0     4608 2022-11-29 10:17:12.492224 pypath_omnipath-0.14.48/pypath/legacy/db_categories.py
--rw-r--r--   0        0        0   556645 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.48/pypath/legacy/main.py
--rw-r--r--   0        0        0     1768 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/__init__.py
--rw-r--r--   0        0        0    18012 2023-02-23 11:35:21.780049 pypath_omnipath-0.14.48/pypath/omnipath/app.py
--rw-r--r--   0        0        0    16321 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.48/pypath/omnipath/bel.py
--rw-r--r--   0        0        0    16758 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/cellphonedb.py
--rw-r--r--   0        0        0     1477 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/databases/__init__.py
--rw-r--r--   0        0        0     1848 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/databases/build.py
--rw-r--r--   0        0        0     1729 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.48/pypath/omnipath/databases/builtins.json
--rw-r--r--   0        0        0      522 2022-01-24 11:42:01.191613 pypath_omnipath-0.14.48/pypath/omnipath/databases/classes.json
--rw-r--r--   0        0        0     8342 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/databases/define.py
--rw-r--r--   0        0        0    34353 2023-03-27 20:50:05.365575 pypath_omnipath-0.14.48/pypath/omnipath/export.py
--rw-r--r--   0        0        0     4180 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/legacy.py
--rw-r--r--   0        0        0     1792 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/param.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/server/__init__.py
--rw-r--r--   0        0        0   122926 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/_html.py
--rw-r--r--   0        0        0    10455 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/build.py
--rw-r--r--   0        0        0    17217 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/generate_about_page.py
--rw-r--r--   0        0        0    11122 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/legacy.py
--rw-r--r--   0        0        0    79104 2023-04-06 10:09:25.133831 pypath_omnipath-0.14.48/pypath/omnipath/server/run.py
--rw-r--r--   0        0        0     4740 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/reader/field.py
--rw-r--r--   0        0        0     1620 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/reader/network.py
--rw-r--r--   0        0        0     1013 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/resources/__init__.py
--rw-r--r--   0        0        0    14229 2023-03-30 21:45:15.125990 pypath_omnipath-0.14.48/pypath/resources/controller.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/resources/data/__init__.py
--rw-r--r--   0        0        0      139 2023-01-10 18:56:49.559042 pypath_omnipath-0.14.48/pypath/resources/data/complex_input_template.json
--rw-r--r--   0        0        0      239 2023-01-10 18:56:35.023580 pypath_omnipath-0.14.48/pypath/resources/data/enz_sub_input_template.json
--rw-r--r--   0        0        0   176408 2023-04-05 14:14:26.002955 pypath_omnipath-0.14.48/pypath/resources/data/resources.json
--rw-r--r--   0        0        0   100689 2023-03-29 23:22:52.815513 pypath_omnipath-0.14.48/pypath/resources/data_formats.py
--rw-r--r--   0        0        0   179216 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/resources/descriptions.py
--rw-r--r--   0        0        0     2817 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/resources/licenses.py
--rw-r--r--   0        0        0     5389 2023-03-20 15:20:34.662810 pypath_omnipath-0.14.48/pypath/resources/network.py
--rw-r--r--   0        0        0    72005 2023-03-29 17:58:54.799225 pypath_omnipath-0.14.48/pypath/resources/urls.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.14.48/pypath/share/__init__.py
--rw-r--r--   0        0        0     1801 2023-03-08 22:39:02.796456 pypath_omnipath-0.14.48/pypath/share/cache.py
--rw-r--r--   0        0        0    69255 2023-04-07 15:32:55.789532 pypath_omnipath-0.14.48/pypath/share/common.py
--rw-r--r--   0        0        0      852 2023-01-16 16:04:45.977246 pypath_omnipath-0.14.48/pypath/share/constants.py
--rw-r--r--   0        0        0    57036 2023-03-28 21:12:57.964394 pypath_omnipath-0.14.48/pypath/share/curl.py
--rw-r--r--   0        0        0     6176 2022-12-05 01:12:34.031728 pypath_omnipath-0.14.48/pypath/share/log.py
--rw-r--r--   0        0        0    17323 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/lookup/_manytomany.py
--rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany.py
--rw-r--r--   0        0        0     2525 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany2.py
--rw-r--r--   0        0        0     5284 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/progress.py
--rw-r--r--   0        0        0     4426 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/share/session.py
--rw-r--r--   0        0        0     9674 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/share/settings.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.492224 pypath_omnipath-0.14.48/pypath/utils/__init__.py
--rw-r--r--   0        0        0    37321 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/go.py
--rw-r--r--   0        0        0    56014 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/homology.py
--rw-r--r--   0        0        0   107424 2023-03-29 12:54:39.165798 pypath_omnipath-0.14.48/pypath/utils/mapping.py
--rw-r--r--   0        0        0     5765 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/pdb.py
--rw-r--r--   0        0        0    11855 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/proteomicsdb.py
--rw-r--r--   0        0        0   109034 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/utils/pyreact.py
--rw-r--r--   0        0        0     7265 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/reflists.py
--rw-r--r--   0        0        0     8802 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/utils/residues.py
--rw-r--r--   0        0        0    11325 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/seq.py
--rw-r--r--   0        0        0    11255 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/taxonomy.py
--rw-r--r--   0        0        0    11956 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/unichem.py
--rw-r--r--   0        0        0    17936 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/uniprot.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/visual/__init__.py
--rw-r--r--   0        0        0    26879 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/drawing.py
--rw-r--r--   0        0        0    21128 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/__init__.py
--rw-r--r--   0        0        0    13835 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/edge.py
--rw-r--r--   0        0        0     4769 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/vertex.py
--rw-r--r--   0        0        0   156771 2022-12-05 01:12:34.038395 pypath_omnipath-0.14.48/pypath/visual/plot.py
--rw-r--r--   0        0        0     2761 2023-04-12 15:39:36.242305 pypath_omnipath-0.14.48/pyproject.toml
--rw-r--r--   0        0        0    13420 1970-01-01 00:00:00.000000 pypath_omnipath-0.14.48/setup.py
--rw-r--r--   0        0        0    13585 1970-01-01 00:00:00.000000 pypath_omnipath-0.14.48/PKG-INFO
+-rw-r--r--   0        0        0    35141 2016-11-05 19:50:35.500333 pypath_omnipath-0.15.4/LICENSE
+-rw-r--r--   0        0        0    11492 2023-03-28 22:05:50.316062 pypath_omnipath-0.15.4/README.rst
+-rw-r--r--   0        0        0     2743 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/__init__.py
+-rw-r--r--   0        0        0     2056 2023-06-10 21:09:01.907500 pypath_omnipath-0.15.4/pypath/_metadata.py
+-rw-r--r--   0        0        0      666 2022-12-05 01:12:34.011729 pypath_omnipath-0.15.4/pypath/biocypher/__init__.py
+-rw-r--r--   0        0        0     7863 2022-12-05 01:12:34.011729 pypath_omnipath-0.15.4/pypath/biocypher/adapter.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.502224 pypath_omnipath-0.15.4/pypath/core/__init__.py
+-rw-r--r--   0        0        0   174945 2023-03-29 12:47:27.521270 pypath_omnipath-0.15.4/pypath/core/annot.py
+-rw-r--r--   0        0        0     4327 2022-12-05 01:12:34.015062 pypath_omnipath-0.15.4/pypath/core/attrs.py
+-rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.508891 pypath_omnipath-0.15.4/pypath/core/common.py
+-rw-r--r--   0        0        0    19000 2023-03-29 12:48:22.415968 pypath_omnipath-0.15.4/pypath/core/complex.py
+-rw-r--r--   0        0        0    13292 2023-05-17 15:00:12.465009 pypath_omnipath-0.15.4/pypath/core/entity.py
+-rw-r--r--   0        0        0    37353 2022-11-29 10:17:12.502224 pypath_omnipath-0.15.4/pypath/core/enz_sub.py
+-rw-r--r--   0        0        0    23007 2023-05-24 01:46:11.792790 pypath_omnipath-0.15.4/pypath/core/evidence.py
+-rw-r--r--   0        0        0    97985 2023-05-17 17:29:01.383941 pypath_omnipath-0.15.4/pypath/core/interaction.py
+-rw-r--r--   0        0        0    30155 2022-11-29 10:17:12.498891 pypath_omnipath-0.15.4/pypath/core/intercell.py
+-rw-r--r--   0        0        0   230647 2022-11-29 10:17:12.505557 pypath_omnipath-0.15.4/pypath/core/intercell_annot.py
+-rw-r--r--   0        0        0   141858 2023-05-24 00:32:23.382052 pypath_omnipath-0.15.4/pypath/core/network.py
+-rw-r--r--   0        0        0      138 2022-12-05 01:12:34.015062 pypath_omnipath-0.15.4/pypath/data/__init__.py
+-rw-r--r--   0        0        0     1300 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/embl_colors
+-rw-r--r--   0        0        0      271 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/ensembl_biomart_query.xml
+-rw-r--r--   0        0        0      227 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/goose_ancestors.sql
+-rw-r--r--   0        0        0      712 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/goose_annotations.sql
+-rw-r--r--   0        0        0      120 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/goose_terms.sql
+-rw-r--r--   0        0        0      185 2023-03-30 00:53:33.672441 pypath_omnipath-0.15.4/pypath/data/licenses/afl_v3.json
+-rw-r--r--   0        0        0      186 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/apache_2.0.json
+-rw-r--r--   0        0        0      190 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/artistic_2.0.json
+-rw-r--r--   0        0        0      199 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/biocarta.json
+-rw-r--r--   0        0        0      188 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/bsd.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_2.5.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_3.0.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_4.0.json
+-rw-r--r--   0        0        0      242 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nc-nd_3.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.168281 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nc-nd_4.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nc_2.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nc_3.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nc_4.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nc_sa_3.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nc_sa_4.0.json
+-rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nd_3.0.json
+-rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_nd_4.0.json
+-rw-r--r--   0        0        0      224 2023-03-30 00:45:57.463174 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_sa_2.5.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_sa_3.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_by_sa_4.0.json
+-rw-r--r--   0        0        0      233 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cc_zero.json
+-rw-r--r--   0        0        0      196 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cellcellinteractions.json
+-rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/composite.json
+-rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/cosmic.json
+-rw-r--r--   0        0        0      194 2022-03-18 18:18:43.477819 pypath_omnipath-0.15.4/pypath/data/licenses/cytosig.json
+-rw-r--r--   0        0        0      182 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/dsl.json
+-rw-r--r--   0        0        0      185 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/elm.json
+-rw-r--r--   0        0        0      174 2022-12-05 01:12:34.015062 pypath_omnipath-0.15.4/pypath/data/licenses/embl-ebi.json
+-rw-r--r--   0        0        0      212 2023-04-05 14:14:07.817106 pypath_omnipath-0.15.4/pypath/data/licenses/eul.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/gnu_gpl_v2.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/gnu_gpl_v3.json
+-rw-r--r--   0        0        0      200 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/gnu_lgpl_v3.json
+-rw-r--r--   0        0        0      311 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/hgnc.json
+-rw-r--r--   0        0        0      150 2022-09-15 18:20:39.089511 pypath_omnipath-0.15.4/pypath/data/licenses/hpo.json
+-rw-r--r--   0        0        0      139 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/hprd.json
+-rw-r--r--   0        0        0      168 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/i2d.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/informal.json
+-rw-r--r--   0        0        0      175 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/kegg.json
+-rw-r--r--   0        0        0      174 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/kinase-com.json
+-rw-r--r--   0        0        0      268 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/mirecords.json
+-rw-r--r--   0        0        0      184 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/mirtarbase.json
+-rw-r--r--   0        0        0      154 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/mit.json
+-rw-r--r--   0        0        0      165 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/mppi.json
+-rw-r--r--   0        0        0      360 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/nar.json
+-rw-r--r--   0        0        0      179 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/no_license.json
+-rw-r--r--   0        0        0      177 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/pathwaycommons.json
+-rw-r--r--   0        0        0      351 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/pdb.json
+-rw-r--r--   0        0        0      363 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/phosphonetworks.json
+-rw-r--r--   0        0        0      464 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/licenses/unspecified.json
+-rw-r--r--   0        0        0     5798 2023-06-10 18:20:35.550400 pypath_omnipath-0.15.4/pypath/data/settings.yaml
+-rw-r--r--   0        0        0     1150 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/www/favicon.ico
+-rw-r--r--   0        0        0      486 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/www/http500.html
+-rw-r--r--   0        0        0      324 2022-01-24 11:42:01.171614 pypath_omnipath-0.15.4/pypath/data/www/index.html
+-rw-r--r--   0        0        0     5815 2022-11-29 10:17:12.498891 pypath_omnipath-0.15.4/pypath/formats/obo.py
+-rw-r--r--   0        0        0    15893 2023-04-25 11:32:08.453155 pypath_omnipath-0.15.4/pypath/formats/sdf.py
+-rw-r--r--   0        0        0     8624 2023-03-09 00:29:38.782357 pypath_omnipath-0.15.4/pypath/formats/sqldump.py
+-rw-r--r--   0        0        0     1358 2023-03-09 17:12:37.914407 pypath_omnipath-0.15.4/pypath/formats/sqlite.py
+-rw-r--r--   0        0        0     7508 2023-03-13 13:39:42.775048 pypath_omnipath-0.15.4/pypath/formats/xml.py
+-rw-r--r--   0        0        0     2204 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/__init__.py
+-rw-r--r--   0        0        0     1075 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/abs.py
+-rw-r--r--   0        0        0     3155 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/acsn.py
+-rw-r--r--   0        0        0     2422 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/adhesome.py
+-rw-r--r--   0        0        0     2343 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/almen2009.py
+-rw-r--r--   0        0        0     5340 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/baccin2019.py
+-rw-r--r--   0        0        0     6319 2022-12-05 01:12:34.015062 pypath_omnipath-0.15.4/pypath/inputs/biogps.py
+-rw-r--r--   0        0        0     5016 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/biogrid.py
+-rw-r--r--   0        0        0    10223 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/biomart.py
+-rw-r--r--   0        0        0     5365 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/biomodels.py
+-rw-r--r--   0        0        0     1794 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/ca1.py
+-rw-r--r--   0        0        0     2760 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/cancercellmap.py
+-rw-r--r--   0        0        0     5541 2023-03-23 11:43:45.220378 pypath_omnipath-0.15.4/pypath/inputs/cancerdrugsdb.py
+-rw-r--r--   0        0        0     1907 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/cancersea.py
+-rw-r--r--   0        0        0     3358 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/cell.py
+-rw-r--r--   0        0        0     6338 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/cellcall.py
+-rw-r--r--   0        0        0     1551 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/cellcellinteractions.py
+-rw-r--r--   0        0        0     9191 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/cellchatdb.py
+-rw-r--r--   0        0        0    15036 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/cellinker.py
+-rw-r--r--   0        0        0     9174 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/cellphonedb.py
+-rw-r--r--   0        0        0     5398 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/celltalkdb.py
+-rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/celltypist.py
+-rw-r--r--   0        0        0    13903 2023-04-12 15:40:29.427011 pypath_omnipath-0.15.4/pypath/inputs/chembl.py
+-rw-r--r--   0        0        0     4001 2023-04-24 12:19:43.309076 pypath_omnipath-0.15.4/pypath/inputs/clinvar.py
+-rw-r--r--   0        0        0     5660 2023-05-23 23:18:53.666105 pypath_omnipath-0.15.4/pypath/inputs/collectri.py
+-rw-r--r--   0        0        0     7920 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/common.py
+-rw-r--r--   0        0        0     2656 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/compleat.py
+-rw-r--r--   0        0        0     4509 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/complexportal.py
+-rw-r--r--   0        0        0     4036 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/comppi.py
+-rw-r--r--   0        0        0     2788 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/connectomedb.py
+-rw-r--r--   0        0        0     2793 2023-03-23 12:55:34.154293 pypath_omnipath-0.15.4/pypath/inputs/corum.py
+-rw-r--r--   0        0        0     4779 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/cosmic.py
+-rw-r--r--   0        0        0     4234 2023-03-29 21:02:25.987565 pypath_omnipath-0.15.4/pypath/inputs/cpad.py
+-rw-r--r--   0        0        0     1989 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/cpdb.py
+-rw-r--r--   0        0        0     3412 2022-12-05 01:12:34.018396 pypath_omnipath-0.15.4/pypath/inputs/credentials.py
+-rw-r--r--   0        0        0     3344 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/csa.py
+-rw-r--r--   0        0        0     3547 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/cspa.py
+-rw-r--r--   0        0        0     5114 2023-02-23 11:38:30.888776 pypath_omnipath-0.15.4/pypath/inputs/ctdbase.py
+-rw-r--r--   0        0        0     3343 2023-03-22 17:05:50.626476 pypath_omnipath-0.15.4/pypath/inputs/cytosig.py
+-rw-r--r--   0        0        0     4765 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/dbptm.py
+-rw-r--r--   0        0        0     2833 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/deathdomain.py
+-rw-r--r--   0        0        0     4384 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/depod.py
+-rw-r--r--   0        0        0     3721 2022-12-05 01:12:37.954873 pypath_omnipath-0.15.4/pypath/inputs/dgidb.py
+-rw-r--r--   0        0        0     4921 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/dip.py
+-rw-r--r--   0        0        0    68257 2023-02-23 11:38:30.888776 pypath_omnipath-0.15.4/pypath/inputs/disgenet.py
+-rw-r--r--   0        0        0    17135 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/domino.py
+-rw-r--r--   0        0        0    12715 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/dorothea.py
+-rw-r--r--   0        0        0    20676 2023-02-23 11:38:30.888776 pypath_omnipath-0.15.4/pypath/inputs/drugbank.py
+-rw-r--r--   0        0        0     4706 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/drugcentral.py
+-rw-r--r--   0        0        0     4803 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/ebi.py
+-rw-r--r--   0        0        0     4929 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/elm.py
+-rw-r--r--   0        0        0     2523 2023-03-28 12:11:30.004207 pypath_omnipath-0.15.4/pypath/inputs/embopress.py
+-rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/embrace.py
+-rw-r--r--   0        0        0     1220 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/encode.py
+-rw-r--r--   0        0        0     1982 2023-04-05 00:14:36.657341 pypath_omnipath-0.15.4/pypath/inputs/ensembl.py
+-rw-r--r--   0        0        0     3152 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/exocarta.py
+-rw-r--r--   0        0        0     3425 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/genecards.py
+-rw-r--r--   0        0        0    26086 2023-03-28 21:26:09.280054 pypath_omnipath-0.15.4/pypath/inputs/go.py
+-rw-r--r--   0        0        0     2356 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/gpcrdb.py
+-rw-r--r--   0        0        0     1937 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/graphviz.py
+-rw-r--r--   0        0        0     8279 2023-05-15 15:09:25.911387 pypath_omnipath-0.15.4/pypath/inputs/guide2pharma.py
+-rw-r--r--   0        0        0     1597 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/havugimana.py
+-rw-r--r--   0        0        0     1628 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/hgnc.py
+-rw-r--r--   0        0        0     3763 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/hippie.py
+-rw-r--r--   0        0        0     1212 2023-04-25 10:57:06.360072 pypath_omnipath-0.15.4/pypath/inputs/hmdb/__init__.py
+-rw-r--r--   0        0        0     6447 2023-04-23 23:03:35.117400 pypath_omnipath-0.15.4/pypath/inputs/hmdb/common.py
+-rw-r--r--   0        0        0     5203 2023-04-23 22:57:58.110370 pypath_omnipath-0.15.4/pypath/inputs/hmdb/metabolites.py
+-rw-r--r--   0        0        0     5156 2023-04-23 22:57:25.115949 pypath_omnipath-0.15.4/pypath/inputs/hmdb/proteins.py
+-rw-r--r--   0        0        0      716 2023-04-24 00:26:08.438456 pypath_omnipath-0.15.4/pypath/inputs/hmdb/schema/__init__.py
+-rw-r--r--   0        0        0     2333 2023-04-18 23:43:51.458073 pypath_omnipath-0.15.4/pypath/inputs/hmdb/schema/common.py
+-rw-r--r--   0        0        0     5139 2023-04-18 23:26:33.780211 pypath_omnipath-0.15.4/pypath/inputs/hmdb/schema/metabolites.py
+-rw-r--r--   0        0        0     3008 2023-04-18 23:50:21.440680 pypath_omnipath-0.15.4/pypath/inputs/hmdb/schema/proteins.py
+-rw-r--r--   0        0        0     1271 2023-04-25 02:19:47.024785 pypath_omnipath-0.15.4/pypath/inputs/hmdb/structures.py
+-rw-r--r--   0        0        0     1728 2023-04-24 00:01:38.285585 pypath_omnipath-0.15.4/pypath/inputs/hmdb/visual.py
+-rw-r--r--   0        0        0     1326 2023-04-22 16:09:07.572686 pypath_omnipath-0.15.4/pypath/inputs/hmdb/xml.py
+-rw-r--r--   0        0        0     4862 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/homologene.py
+-rw-r--r--   0        0        0    10335 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/hpmr.py
+-rw-r--r--   0        0        0     4781 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/hpo.py
+-rw-r--r--   0        0        0     2748 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/hprd.py
+-rw-r--r--   0        0        0     1491 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/htri.py
+-rw-r--r--   0        0        0     1773 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/humancellmap.py
+-rw-r--r--   0        0        0     2048 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/humap.py
+-rw-r--r--   0        0        0     8093 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/huri.py
+-rw-r--r--   0        0        0     2665 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/i3d.py
+-rw-r--r--   0        0        0     6713 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/icellnet.py
+-rw-r--r--   0        0        0     8076 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/ielm.py
+-rw-r--r--   0        0        0     3914 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/imweb.py
+-rw-r--r--   0        0        0     2242 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/innatedb.py
+-rw-r--r--   0        0        0     3005 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/instruct.py
+-rw-r--r--   0        0        0     5688 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/intact.py
+-rw-r--r--   0        0        0     1741 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/integrins.py
+-rw-r--r--   0        0        0     8866 2023-03-28 21:43:59.156468 pypath_omnipath-0.15.4/pypath/inputs/interpro.py
+-rw-r--r--   0        0        0     2530 2023-03-29 19:46:17.335600 pypath_omnipath-0.15.4/pypath/inputs/intogen.py
+-rw-r--r--   0        0        0     1708 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/ipi.py
+-rw-r--r--   0        0        0     3569 2023-05-15 14:57:33.843263 pypath_omnipath-0.15.4/pypath/inputs/iptmnet.py
+-rw-r--r--   0        0        0     3192 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/italk.py
+-rw-r--r--   0        0        0     2557 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/kea.py
+-rw-r--r--   0        0        0    20673 2023-03-29 12:38:13.194490 pypath_omnipath-0.15.4/pypath/inputs/kegg.py
+-rw-r--r--   0        0        0    14746 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/kegg_api.py
+-rw-r--r--   0        0        0     1932 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/kinasedotcom.py
+-rw-r--r--   0        0        0     2522 2023-03-29 14:45:43.764405 pypath_omnipath-0.15.4/pypath/inputs/kirouac2010.py
+-rw-r--r--   0        0        0     4327 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/lambert2018.py
+-rw-r--r--   0        0        0     2174 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/laudanna.py
+-rw-r--r--   0        0        0     5633 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/li2012.py
+-rw-r--r--   0        0        0     2625 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/lincs.py
+-rw-r--r--   0        0        0      631 2023-04-25 10:58:29.696387 pypath_omnipath-0.15.4/pypath/inputs/lipidmaps/__init__.py
+-rw-r--r--   0        0        0     1383 2023-04-25 11:08:05.831573 pypath_omnipath-0.15.4/pypath/inputs/lipidmaps/structures.py
+-rw-r--r--   0        0        0     2929 2023-05-12 00:20:06.185422 pypath_omnipath-0.15.4/pypath/inputs/lmpid.py
+-rw-r--r--   0        0        0     1549 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/lncdisease.py
+-rw-r--r--   0        0        0     2036 2023-05-17 23:50:39.545164 pypath_omnipath-0.15.4/pypath/inputs/lncrnadb.py
+-rw-r--r--   0        0        0     7887 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/locate.py
+-rw-r--r--   0        0        0     3648 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/lrdb.py
+-rw-r--r--   0        0        0     2907 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/macrophage.py
+-rw-r--r--   0        0        0      568 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/main.py
+-rw-r--r--   0        0        0     2334 2023-03-28 17:55:35.707415 pypath_omnipath-0.15.4/pypath/inputs/matrisome.py
+-rw-r--r--   0        0        0     4171 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/matrixdb.py
+-rw-r--r--   0        0        0     1107 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/mcam.py
+-rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/membranome.py
+-rw-r--r--   0        0        0     4296 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/mimp.py
+-rw-r--r--   0        0        0     1365 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/mir2disease.py
+-rw-r--r--   0        0        0     3865 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/mirbase.py
+-rw-r--r--   0        0        0     1742 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/mirdeathdb.py
+-rw-r--r--   0        0        0     1659 2023-03-29 17:59:15.511751 pypath_omnipath-0.15.4/pypath/inputs/mirecords.py
+-rw-r--r--   0        0        0     2177 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/mirtarbase.py
+-rw-r--r--   0        0        0     1069 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/mitab.py
+-rw-r--r--   0        0        0     3166 2023-03-23 12:55:18.904569 pypath_omnipath-0.15.4/pypath/inputs/mppi.py
+-rw-r--r--   0        0        0    11491 2023-04-04 23:37:06.309559 pypath_omnipath-0.15.4/pypath/inputs/msigdb.py
+-rw-r--r--   0        0        0     2100 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/ncrdeathdb.py
+-rw-r--r--   0        0        0     1830 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/negatome.py
+-rw-r--r--   0        0        0     1758 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/netbiol.py
+-rw-r--r--   0        0        0     6376 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/netpath.py
+-rw-r--r--   0        0        0     2994 2022-12-05 01:12:37.954873 pypath_omnipath-0.15.4/pypath/inputs/oma.py
+-rw-r--r--   0        0        0     3600 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/ontology.py
+-rw-r--r--   0        0        0     2845 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/opm.py
+-rw-r--r--   0        0        0     2313 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/oreganno.py
+-rw-r--r--   0        0        0     4003 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/panglaodb.py
+-rw-r--r--   0        0        0     3558 2022-12-05 01:12:37.954873 pypath_omnipath-0.15.4/pypath/inputs/pathophenodb.py
+-rw-r--r--   0        0        0     4593 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/pathwaycommons.py
+-rw-r--r--   0        0        0     1071 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/pazar.py
+-rw-r--r--   0        0        0     6333 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/pdb.py
+-rw-r--r--   0        0        0     2411 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/pdzbase.py
+-rw-r--r--   0        0        0     6660 2022-12-05 01:12:34.021729 pypath_omnipath-0.15.4/pypath/inputs/pepcyber.py
+-rw-r--r--   0        0        0     9162 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/pfam.py
+-rw-r--r--   0        0        0     6669 2023-02-23 11:38:30.888776 pypath_omnipath-0.15.4/pypath/inputs/pharos.py
+-rw-r--r--   0        0        0     1673 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/phobius.py
+-rw-r--r--   0        0        0     2299 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/phosphatome.py
+-rw-r--r--   0        0        0     3433 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/phosphoelm.py
+-rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/phosphonetworks.py
+-rw-r--r--   0        0        0     1299 2022-11-29 10:17:12.515557 pypath_omnipath-0.15.4/pypath/inputs/phosphopoint.py
+-rw-r--r--   0        0        0    37326 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/phosphosite.py
+-rw-r--r--   0        0        0     9976 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/pisa.py
+-rw-r--r--   0        0        0     1850 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/pro.py
+-rw-r--r--   0        0        0     3189 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/progeny.py
+-rw-r--r--   0        0        0     7531 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/proteinatlas.py
+-rw-r--r--   0        0        0     3573 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/proteins.py
+-rw-r--r--   0        0        0     3808 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/protmapper.py
+-rw-r--r--   0        0        0     2463 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/pubchem.py
+-rw-r--r--   0        0        0     4224 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/pubmed.py
+-rw-r--r--   0        0        0     4418 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/ramilowski2015.py
+-rw-r--r--   0        0        0     5426 2023-03-22 21:01:49.738609 pypath_omnipath-0.15.4/pypath/inputs/ramp.py
+-rw-r--r--   0        0        0     6496 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/rdata.py
+-rw-r--r--   0        0        0    40102 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/reaction.py
+-rw-r--r--   0        0        0     7685 2023-05-15 15:06:31.612587 pypath_omnipath-0.15.4/pypath/inputs/scconnect.py
+-rw-r--r--   0        0        0     2455 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/science.py
+-rw-r--r--   0        0        0     5578 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/signalink.py
+-rw-r--r--   0        0        0    11727 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/signor.py
+-rw-r--r--   0        0        0     5681 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/spike.py
+-rw-r--r--   0        0        0     4287 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/stitch.py
+-rw-r--r--   0        0        0     7315 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/string.py
+-rw-r--r--   0        0        0     1579 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/surfaceome.py
+-rw-r--r--   0        0        0     4412 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/switches_elm.py
+-rw-r--r--   0        0        0     3225 2022-11-29 10:17:12.528890 pypath_omnipath-0.15.4/pypath/inputs/talklr.py
+-rw-r--r--   0        0        0     2616 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/tcdb.py
+-rw-r--r--   0        0        0     2119 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/tfcensus.py
+-rw-r--r--   0        0        0     7926 2022-12-05 01:12:34.025062 pypath_omnipath-0.15.4/pypath/inputs/threedcomplex.py
+-rw-r--r--   0        0        0    17368 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/threedid.py
+-rw-r--r--   0        0        0     3692 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/topdb.py
+-rw-r--r--   0        0        0     1453 2022-11-29 10:17:12.522224 pypath_omnipath-0.15.4/pypath/inputs/transmir.py
+-rw-r--r--   0        0        0     9902 2022-11-29 10:17:12.525557 pypath_omnipath-0.15.4/pypath/inputs/trip.py
+-rw-r--r--   0        0        0     5196 2023-03-19 23:05:05.810094 pypath_omnipath-0.15.4/pypath/inputs/unichem.py
+-rw-r--r--   0        0        0    31425 2023-06-01 01:40:55.468783 pypath_omnipath-0.15.4/pypath/inputs/uniprot.py
+-rw-r--r--   0        0        0     7602 2023-03-29 16:56:14.179505 pypath_omnipath-0.15.4/pypath/inputs/wang.py
+-rw-r--r--   0        0        0     2171 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/inputs/wojtowicz2020.py
+-rw-r--r--   0        0        0     1619 2022-11-29 10:17:12.518890 pypath_omnipath-0.15.4/pypath/inputs/zhong2015.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.508891 pypath_omnipath-0.15.4/pypath/internals/__init__.py
+-rw-r--r--   0        0        0    11896 2022-11-29 10:17:12.508891 pypath_omnipath-0.15.4/pypath/internals/annot_formats.py
+-rw-r--r--   0        0        0    23161 2023-06-10 21:02:59.831243 pypath_omnipath-0.15.4/pypath/internals/input_formats.py
+-rw-r--r--   0        0        0    43762 2023-05-17 01:29:02.152782 pypath_omnipath-0.15.4/pypath/internals/intera.py
+-rw-r--r--   0        0        0     7533 2022-11-29 10:17:12.508891 pypath_omnipath-0.15.4/pypath/internals/license.py
+-rw-r--r--   0        0        0     7259 2023-06-09 22:21:35.543174 pypath_omnipath-0.15.4/pypath/internals/maps.py
+-rw-r--r--   0        0        0     4199 2022-11-29 10:17:12.508891 pypath_omnipath-0.15.4/pypath/internals/refs.py
+-rw-r--r--   0        0        0    13323 2023-05-13 22:20:04.742847 pypath_omnipath-0.15.4/pypath/internals/resource.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.15.4/pypath/legacy/__init__.py
+-rw-r--r--   0        0        0     4608 2022-11-29 10:17:12.492224 pypath_omnipath-0.15.4/pypath/legacy/db_categories.py
+-rw-r--r--   0        0        0   556645 2022-12-05 01:12:34.028395 pypath_omnipath-0.15.4/pypath/legacy/main.py
+-rw-r--r--   0        0        0     1768 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/omnipath/__init__.py
+-rw-r--r--   0        0        0    18001 2023-05-23 23:17:40.806258 pypath_omnipath-0.15.4/pypath/omnipath/app.py
+-rw-r--r--   0        0        0    16321 2022-12-05 01:12:34.028395 pypath_omnipath-0.15.4/pypath/omnipath/bel.py
+-rw-r--r--   0        0        0    16758 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/omnipath/cellphonedb.py
+-rw-r--r--   0        0        0     1477 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/omnipath/databases/__init__.py
+-rw-r--r--   0        0        0     1848 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/omnipath/databases/build.py
+-rw-r--r--   0        0        0     1729 2022-12-05 01:12:34.028395 pypath_omnipath-0.15.4/pypath/omnipath/databases/builtins.json
+-rw-r--r--   0        0        0      522 2022-01-24 11:42:01.191613 pypath_omnipath-0.15.4/pypath/omnipath/databases/classes.json
+-rw-r--r--   0        0        0     8342 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/omnipath/databases/define.py
+-rw-r--r--   0        0        0    30966 2023-05-27 15:14:12.741178 pypath_omnipath-0.15.4/pypath/omnipath/export.py
+-rw-r--r--   0        0        0     4180 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/omnipath/legacy.py
+-rw-r--r--   0        0        0     1792 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/omnipath/param.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/omnipath/server/__init__.py
+-rw-r--r--   0        0        0   122926 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/omnipath/server/_html.py
+-rw-r--r--   0        0        0    10455 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/omnipath/server/build.py
+-rw-r--r--   0        0        0    17217 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/omnipath/server/generate_about_page.py
+-rw-r--r--   0        0        0    11122 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/omnipath/server/legacy.py
+-rw-r--r--   0        0        0    79353 2023-05-18 22:40:25.793503 pypath_omnipath-0.15.4/pypath/omnipath/server/run.py
+-rw-r--r--   0        0        0     4740 2022-11-29 10:17:12.498891 pypath_omnipath-0.15.4/pypath/reader/field.py
+-rw-r--r--   0        0        0     1620 2022-11-29 10:17:12.498891 pypath_omnipath-0.15.4/pypath/reader/network.py
+-rw-r--r--   0        0        0     1013 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/resources/__init__.py
+-rw-r--r--   0        0        0    14229 2023-03-30 21:45:15.125990 pypath_omnipath-0.15.4/pypath/resources/controller.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/resources/data/__init__.py
+-rw-r--r--   0        0        0      139 2023-01-10 18:56:49.559042 pypath_omnipath-0.15.4/pypath/resources/data/complex_input_template.json
+-rw-r--r--   0        0        0      239 2023-01-10 18:56:35.023580 pypath_omnipath-0.15.4/pypath/resources/data/enz_sub_input_template.json
+-rw-r--r--   0        0        0   176408 2023-04-05 14:14:26.002955 pypath_omnipath-0.15.4/pypath/resources/data/resources.json
+-rw-r--r--   0        0        0   104312 2023-05-23 23:18:53.666105 pypath_omnipath-0.15.4/pypath/resources/data_formats.py
+-rw-r--r--   0        0        0   179216 2022-11-29 10:17:12.512224 pypath_omnipath-0.15.4/pypath/resources/descriptions.py
+-rw-r--r--   0        0        0     2817 2022-11-29 10:17:12.508891 pypath_omnipath-0.15.4/pypath/resources/licenses.py
+-rw-r--r--   0        0        0     5794 2023-05-15 14:17:27.617532 pypath_omnipath-0.15.4/pypath/resources/network.py
+-rw-r--r--   0        0        0    72801 2023-06-10 15:53:55.683541 pypath_omnipath-0.15.4/pypath/resources/urls.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.15.4/pypath/share/__init__.py
+-rw-r--r--   0        0        0     1801 2023-03-08 22:39:02.796456 pypath_omnipath-0.15.4/pypath/share/cache.py
+-rw-r--r--   0        0        0    69958 2023-05-11 20:47:13.918886 pypath_omnipath-0.15.4/pypath/share/common.py
+-rw-r--r--   0        0        0      852 2023-01-16 16:04:45.977246 pypath_omnipath-0.15.4/pypath/share/constants.py
+-rw-r--r--   0        0        0    57422 2023-06-10 18:07:34.910855 pypath_omnipath-0.15.4/pypath/share/curl.py
+-rw-r--r--   0        0        0     6176 2022-12-05 01:12:34.031728 pypath_omnipath-0.15.4/pypath/share/log.py
+-rw-r--r--   0        0        0    17323 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/share/lookup/_manytomany.py
+-rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/share/lookup/_onetomany.py
+-rw-r--r--   0        0        0     2525 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/share/lookup/_onetomany2.py
+-rw-r--r--   0        0        0     5284 2022-11-29 10:17:12.482225 pypath_omnipath-0.15.4/pypath/share/progress.py
+-rw-r--r--   0        0        0     4498 2023-05-15 15:03:06.058489 pypath_omnipath-0.15.4/pypath/share/session.py
+-rw-r--r--   0        0        0     9674 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/share/settings.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.492224 pypath_omnipath-0.15.4/pypath/utils/__init__.py
+-rw-r--r--   0        0        0    37321 2022-11-29 10:17:12.495558 pypath_omnipath-0.15.4/pypath/utils/go.py
+-rw-r--r--   0        0        0    56106 2023-05-11 20:50:11.897243 pypath_omnipath-0.15.4/pypath/utils/homology.py
+-rw-r--r--   0        0        0   110761 2023-06-10 21:56:47.191281 pypath_omnipath-0.15.4/pypath/utils/mapping.py
+-rw-r--r--   0        0        0      742 2023-04-24 00:23:43.344869 pypath_omnipath-0.15.4/pypath/utils/metabo/__init__.py
+-rw-r--r--   0        0        0     1550 2023-04-24 00:26:32.170187 pypath_omnipath-0.15.4/pypath/utils/metabo/struct/visual.py
+-rw-r--r--   0        0        0     5765 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/utils/pdb.py
+-rw-r--r--   0        0        0    11855 2022-11-29 10:17:12.495558 pypath_omnipath-0.15.4/pypath/utils/proteomicsdb.py
+-rw-r--r--   0        0        0   109034 2022-11-29 10:17:12.498891 pypath_omnipath-0.15.4/pypath/utils/pyreact.py
+-rw-r--r--   0        0        0     7265 2022-11-29 10:17:12.495558 pypath_omnipath-0.15.4/pypath/utils/reflists.py
+-rw-r--r--   0        0        0     8802 2022-11-29 10:17:12.498891 pypath_omnipath-0.15.4/pypath/utils/residues.py
+-rw-r--r--   0        0        0    11325 2022-11-29 10:17:12.495558 pypath_omnipath-0.15.4/pypath/utils/seq.py
+-rw-r--r--   0        0        0    11255 2023-05-15 15:09:43.227271 pypath_omnipath-0.15.4/pypath/utils/taxonomy.py
+-rw-r--r--   0        0        0    11956 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/utils/unichem.py
+-rw-r--r--   0        0        0    17936 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/utils/uniprot.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.15.4/pypath/visual/__init__.py
+-rw-r--r--   0        0        0    26879 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/visual/drawing.py
+-rw-r--r--   0        0        0    21128 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/visual/igraph_drawing/__init__.py
+-rw-r--r--   0        0        0    13835 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/visual/igraph_drawing/edge.py
+-rw-r--r--   0        0        0     4769 2022-12-05 01:12:34.035061 pypath_omnipath-0.15.4/pypath/visual/igraph_drawing/vertex.py
+-rw-r--r--   0        0        0   156771 2022-12-05 01:12:34.038395 pypath_omnipath-0.15.4/pypath/visual/plot.py
+-rw-r--r--   0        0        0     3056 2023-06-10 21:09:01.904167 pypath_omnipath-0.15.4/pyproject.toml
+-rw-r--r--   0        0        0    13663 1970-01-01 00:00:00.000000 pypath_omnipath-0.15.4/PKG-INFO
```

### Comparing `pypath_omnipath-0.14.48/LICENSE` & `pypath_omnipath-0.15.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/README.rst` & `pypath_omnipath-0.15.4/README.rst`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/__init__.py` & `pypath_omnipath-0.15.4/pypath/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/_metadata.py` & `pypath_omnipath-0.15.4/pypath/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 import os
 import pathlib
 import importlib.metadata
 
 import toml
 
-_VERSION = '0.14.48'
+_VERSION = '0.15.4'
 
 
 def get_metadata():
     """
     Basic package metadata.
 
     Retrieves package metadata from the current project directory or from
```

### Comparing `pypath_omnipath-0.14.48/pypath/biocypher/__init__.py` & `pypath_omnipath-0.15.4/pypath/biocypher/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/biocypher/adapter.py` & `pypath_omnipath-0.15.4/pypath/biocypher/adapter.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/annot.py` & `pypath_omnipath-0.15.4/pypath/core/annot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/attrs.py` & `pypath_omnipath-0.15.4/pypath/core/attrs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/common.py` & `pypath_omnipath-0.15.4/pypath/core/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/complex.py` & `pypath_omnipath-0.15.4/pypath/core/complex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/entity.py` & `pypath_omnipath-0.15.4/pypath/core/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,14 +497,19 @@
 
 
     def info(self):
 
         self.entity_info(self.identifier)
 
 
+    def __bool__(self):
+
+        return bool(self.identifier)
+
+
 class EntityList(object):
 
 
     def __init__(self, entities):
 
         self._entities = (
             entities
```

### Comparing `pypath_omnipath-0.14.48/pypath/core/enz_sub.py` & `pypath_omnipath-0.15.4/pypath/core/enz_sub.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/evidence.py` & `pypath_omnipath-0.15.4/pypath/core/evidence.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 import copy
 
 import pypath.internals.refs as refs
 import pypath.share.common as common
 import pypath.share.session as session_mod
 import pypath.core.entity as entity
 import pypath.core.attrs as attrs_mod
+import pypath.resources.network as netres
 
 _logger = session_mod.Logger(name = 'evidence')
 _log = _logger._log
 
 
 class Evidence(attrs_mod.AttributeHandler):
     """
@@ -62,20 +63,22 @@
     :arg str,list,set,NoneType references:
         Optional, one or more literature references (preferably PubMed IDs).
     """
 
     __slots__ = [
         'resource',
         'references',
+        'dataset',
     ]
 
 
     def __init__(self, resource, references = None, attrs = None):
 
         self.resource = resource
+        self.dataset = getattr(resource, 'dataset', None)
         self.references = self._process_references(references)
         attrs_mod.AttributeHandler.__init__(self, attrs)
 
 
     def reload(self):
         """
         Reloads the object from the module level.
@@ -112,27 +115,32 @@
 
     def __eq__(self, other):
 
         return (
             self.resource == other or
             (
                 hasattr(other, 'resource') and
-                self.resource == other.resource
+                self.resource == other.resource and
+                (
+                    self.resource.interaction_type ==
+                    self.resource.interaction_type
+                )
             )
         )
 
 
     def __iadd__(self, other):
         """
         This will ignore if the other evidence is from different resource:
         still better than attributing wrong references to a resource.
         """
 
         if self == other:
 
+            self.dataset = netres.choose_dataset(self.dataset, other.dataset)
             self.references.update(other.references)
             attrs_mod.AttributeHandler.__iadd__(other)
 
         else:
 
             _log(
                 'Warning: attempt to merge evidences from different '
@@ -140,18 +148,21 @@
             )
 
         return self
 
 
     def __add__(self, other):
 
+        dataset = netres.choose_dataset(self.dataset, other.dataset)
+
         new = self.__class__(
             resource = self.resource,
             references = self.references | other.references,
         )
+        new.dataset = dataset
         new.update_attrs(self.attrs.copy())
         new.update_attrs(other.attrs.copy())
 
         return new
 
 
     @property
@@ -181,14 +192,19 @@
         return '<Evidence %s (%s%u references)>' % (
             self.resource.name,
             'via %s, ' % self.resource.via if self.resource.via else '',
             len(self.references),
         )
 
 
+    def __str__(self):
+
+        return self.resource.name
+
+
     def __copy__(self):
 
         return self.__class__(
             resource = self.resource,
             references = copy.copy(self.references),
             attrs = self.attrs.copy(),
         )
@@ -299,14 +315,15 @@
     def match(
             self,
             resource = None,
             data_model = None,
             interaction_type = None,
             via = False,
             references = None,
+            datasets = None,
         ):
 
         def _match(attr, value):
 
             return (
                 getattr(self.resource, attr) in value
                     if isinstance(value, common.list_like) else
@@ -367,18 +384,50 @@
             (
                 not references or
                 self.references & references
             ) and
             (
                 not data_model or
                 _match('data_model', data_model)
+            ) and
+            (
+                datasets is None or
+                _match('dataset', datasets)
             )
         )
 
 
+    def __str__(self):
+
+        return self.resource.name
+
+
+    @property
+    def pubmeds(self) -> list[str]:
+        """
+        PubMed IDs of the references supporting this evidence.
+        """
+
+        return [r.pmid for r in self.references]
+
+
+    def asdict(self) -> dict:
+        """
+        Dictionary representation of the evidence.
+        """
+
+        return {
+            'resource': self.resource.name,
+            'references': self.pubmeds,
+            'dataset': self.dataset,
+            'via': self.resource.via,
+            'attrs': self.attrs,
+        }
+
+
 class Evidences(object):
     """
     A collection of evidences. All evidences supporting a relationship such
     as molecular interaction, molecular complex, enzyme-PTM interaction,
     annotation, etc should be collected in one `Evidences` object. This way
     the set of evidences can be queried a comprehensive way.
 
@@ -710,14 +759,37 @@
 
 
     def get_data_models(self, **kwargs):
 
         return {ev.resource.data_model for ev in self.filter(**kwargs)}
 
 
+    def get_datasets(self, **kwargs):
+
+        return {
+            ds for ds in
+            (ev.dataset for ev in self.filter(**kwargs))
+            if ds
+        }
+
+
+    def has_dataset(self, dataset: str, **kwargs) -> bool:
+        """
+        Contains evidence(s) from a given dataset meeting the criteria.
+
+        Args:
+            dataset:
+                Name of the dataset.
+            kwargs:
+                Filtering criteria for evidences.
+        """
+
+        return dataset in self.get_datasets(**kwargs)
+
+
     def __isub__(self, other):
 
         if isinstance(other, self.__class__):
 
             self.evidences = dict(
                 (key, ev)
                 for key, ev in iteritems(self.evidences)
@@ -747,45 +819,49 @@
     def filter(
             self,
             resource = None,
             data_model = None,
             interaction_type = None,
             via = False,
             references = None,
+            datasets = None,
         ):
 
         return (
             ev for ev in self
             if ev.match(
                 resource = resource,
                 data_model = data_model,
                 interaction_type = interaction_type,
                 via = via,
                 references = references,
+                datasets = datasets,
             )
         )
 
 
     def match(
             self,
             resource = None,
             data_model = None,
             interaction_type = None,
             via = False,
             references = None,
+            datasets = None,
         ):
 
         return bool(
             tuple(
                 self.filter(
                     resource = resource,
                     data_model = data_model,
                     interaction_type = interaction_type,
                     via = via,
                     references = references,
+                    datasets = datasets,
                 )
             )
         )
 
 
     def __getitem__(self, key):
         """
@@ -841,7 +917,33 @@
         """
 
         return attrs_mod.AttributeHandler._serialize(
             self.simple_dict,
             top_key_prefix = top_key_prefix,
             default = lambda obj: obj.serialize(),
         )
+
+
+    @property
+    def datasets(self) -> set:
+        """
+        Datasets in this evidence set.
+        """
+
+        return {ev.dataset for ev in self}
+
+
+    @property
+    def attrs(self) -> dict:
+        """
+        Combines the custom attributes from all evidences within this set.
+        """
+
+        return common.combine_attrs([ev.attrs for ev in self])
+
+
+    def asdict(self) -> list[dict]:
+        """
+        Evidence set as a list of dictionaries.
+        """
+
+        return [ev.asdict() for ev in self]
```

### Comparing `pypath_omnipath-0.14.48/pypath/core/interaction.py` & `pypath_omnipath-0.15.4/pypath/core/interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 of the :py:class:`Interaction`` objects.
 """
 
 from __future__ import annotations
 
 from future.utils import iteritems
 
+from typing import Literal
+
 import importlib as imp
 import collections
 import operator
 import itertools
 import functools
-from typing_extensions import Literal
+import json
 
 import pypath.core.evidence as pypath_evidence
 import pypath.internals.resource as pypath_resource
 import pypath.share.session as session_mod
 import pypath.share.common as common
 import pypath.utils.mapping as mapping
 import pypath.core.entity as entity
@@ -115,17 +117,19 @@
         'b_a',
         'nodes',
         'key',
         'evidences',
         'direction',
         'positive',
         'negative',
+        'unknown_effect',
     ]
 
     _get_methods = {
+        'datasets',
         'entities',
         'evidences',
         'references',
         'curation_effort',
         'resource_names',
         'resources',
         'data_models',
@@ -149,14 +153,15 @@
         'references',
         'resources',
         'resources_via',
         'resource_names',
         'resource_names_via',
         'data_models',
         'interaction_types',
+        'datasets',
     )
 
     _by_methods = (
         'resource',
         'reference',
         'data_model',
         'interaction_type',
@@ -272,14 +277,18 @@
             self.a_b: pypath_evidence.Evidences(),
             self.b_a: pypath_evidence.Evidences(),
         }
         self.negative = {
             self.a_b: pypath_evidence.Evidences(),
             self.b_a: pypath_evidence.Evidences(),
         }
+        self.unknown_effect = {
+            self.a_b: pypath_evidence.Evidences(),
+            self.b_a: pypath_evidence.Evidences(),
+        }
 
         attrs_mod.AttributeHandler.__init__(self, attrs)
 
 
     def reload(self):
         """
         Reloads the object from the module level.
@@ -301,14 +310,15 @@
         setattr(self, '__class__', new)
 
         for evs in itertools.chain(
             (self.evidences,),
             self.direction.values(),
             self.positive.values(),
             self.negative.values(),
+            self.unknown_effect.values(),
         ):
 
             evs.__class__ = evsnew
 
             for ev in evs:
 
                 ev.__class__ = evnew
@@ -424,15 +434,15 @@
         return direction is not None and direction != 'undirected'
 
 
     def add_evidence(
             self,
             evidence,
             direction = 'undirected',
-            effect = 0,
+            effect = None,
             references = None,
             attrs = None,
         ):
         """
         Adds directionality information with the corresponding data
         source named. Modifies self attributes :py:attr:`dirs` and
         :py:attr:`sources`.
@@ -493,14 +503,18 @@
 
                 self.positive[direction] += evidence
 
             elif effect in {-1, 'negative', 'inhibition'}:
 
                 self.negative[direction] += evidence
 
+            elif effect in {0, 'unknown'}:
+
+                self.unknown_effect[direction] += evidence
+
 
     def __hash__(self):
 
         return hash(self.key)
 
 
     def __eq__(self, other):
@@ -564,18 +578,30 @@
 
             one.positive[eff_key] += other.positive[eff_key]
 
         for eff_key in one.negative.keys():
 
             one.negative[eff_key] += other.negative[eff_key]
 
+        for eff_key in one.unknown_effect.keys():
+
+            one.unknown_effect[eff_key] += other.unknown_effect[eff_key]
+
 
     def __repr__(self):
 
-        return '<Interaction: %s %s=%s=%s=%s %s [%s]>' % (
+        return '<Interaction: %s [%s]>' % (
+            self.__str__(),
+            self.evidences.__repr__().strip('<>'),
+        )
+
+
+    def __str__(self):
+
+        return '%s %s=%s=%s=%s %s' % (
             self.a.label or self.a.identifier,
             '<' if self.direction[self.b_a] else '=',
             (
                 '(+-)' if (
                     self.positive[self.b_a] and
                     self.negative[self.b_a]
                 ) else
@@ -590,18 +616,16 @@
                 ) else
                 '(+)=' if self.positive[self.a_b] else
                 '(-)=' if self.negative[self.a_b] else
                 '===='
             ),
             '>' if self.direction[self.a_b] else '=',
             self.b.label or self.b.identifier,
-            self.evidences.__repr__().strip('<>'),
         )
 
-
     def __contains__(self, other):
 
         return (
             other == self.a or
             other == self.b or
             self.evidences.__contains__(other) or
             attrs_mod.AttributeHandler.__contains__(self, other)
@@ -618,14 +642,28 @@
 
         return {
             ev.resource.data_model
             for ev in self.evidences
         }
 
 
+    def has_dataset(
+            self,
+            dataset: str,
+            direction: str | tuple = None,
+            effect: Literal['positive', 'negative'] = None,
+            **kwargs,
+        ) -> bool:
+
+        return (
+            self.get_evidences(direction = direction, effect = effect).
+            has_dataset(dataset, **kwargs)
+        )
+
+
     def get_direction(
             self,
             direction,
             resources = False,
             evidences = False,
             sources = False,
             resource_names = False,
@@ -832,14 +870,18 @@
 
             return 'positive'
 
         if effect in {'negative', 'inhibition', 'inhibitory'}:
 
             return 'negative'
 
+        if effect in {'unknown'}:
+
+            return 'unknown'
+
 
     def _resources_set(self, resources = None):
 
         return common.to_set(resources)
 
 
     def unset_direction(
@@ -869,15 +911,15 @@
         direction = self.direction_key(direction)
 
         if direction is not None:
 
             attrs = (
                 (self._effect_synonyms(only_sign),)
                     if only_sign else
-                ('direction', 'positive', 'negative')
+                ('direction', 'positive', 'negative', 'unknown_effect')
             )
             resource = resource or source
 
             for attr in attrs:
 
                 if resource is not None:
 
@@ -2080,14 +2122,15 @@
             direction = None,
             effect = None,
             resources = None,
             data_model = None,
             interaction_type = None,
             via = None,
             references = None,
+            datasets = None,
         ):
 
         effect = self._effect_synonyms(effect)
 
         evidences = (
 
             # any signed
@@ -2135,14 +2178,15 @@
             pypath_evidence.Evidences(
                 evidences.filter(
                     resource = resources,
                     interaction_type = interaction_type,
                     via = via,
                     data_model = data_model,
                     references = references,
+                    datasets = datasets,
                 )
             )
         )
 
 
     def get_entities(
             self,
@@ -2150,14 +2194,15 @@
             direction = None,
             effect = None,
             resources = None,
             data_model = None,
             interaction_type = None,
             via = None,
             references = None,
+            datasets = None,
             return_type = None,
         ):
         """
         Retrieves the entities involved in interactions matching the criteria.
         It either returns both interacting entities in a *set* or an empty
         *set*. This may not sound so useful at the level of this object but
         becomes more useful once we want to collect entities having certain
@@ -2296,14 +2341,15 @@
             data_model = None,
             interaction_type = None,
             via = None,
             references = None,
             entity_type = None,
             source_entity_type = None,
             target_entity_type = None,
+            datasets = None,
         ):
         """
         Returns one or two tuples of the interacting partners: one if only
         one direction, two if both directions match the query criteria.
         The tuple will be empty if no evidence matches the criteria.
 
         :arg NontType,bool,tuple direction:
@@ -2377,14 +2423,15 @@
                     direction = direction,
                     effect = effect,
                     resources = resources,
                     data_model = data_model,
                     interaction_type = interaction_type,
                     via = via,
                     references = references,
+                    datasets = datasets,
                 )
             )
 
         )
 
 
     def evaluate_evidences(
@@ -2393,14 +2440,15 @@
             direction = None,
             effect = None,
             resources = None,
             data_model = None,
             interaction_type = None,
             via = None,
             references = None,
+            datasets = None,
         ):
         """
         Selects the evidence collections matching the direction and effect
         criteria and then evaluates if any of the evidences in these
         collections match the evidence criteria.
         """
 
@@ -2416,14 +2464,15 @@
             direction = None,
             effect = None,
             resources = None,
             data_model = None,
             interaction_type = None,
             via = None,
             references = None,
+            datasets = None,
         ):
         """
         Selects the evidence collections matching the direction and effect
         criteria and yields collections matching the evidence criteria.
         """
 
         for evs in self.iter_evidences(
@@ -2434,14 +2483,15 @@
 
             if evs.match(
                 resource = resources,
                 data_model = data_model,
                 interaction_type = interaction_type,
                 via = via,
                 references = references,
+                datasets = datasets,
             ):
 
                 yield evs
 
 
     def iter_evidences(
             self,
@@ -3209,21 +3259,49 @@
                             type = interaction_type,
                             dmodel = data_model,
                             sources = sources,
                             references = refs,
                         )
 
 
-    def serialize_attrs(self, direction = None):
+    def asdict(self, direction: tuple) -> dict:
+        """
+        Dictionary representation of the evidences.
+        """
+
+        direction = self.a_b if self.a_b == direction else self.b_a
+
+        return {
+            'id_a': str(direction[0].identifier),
+            'id_b': str(direction[1].identifier),
+            'positive': self.positive[direction].asdict(),
+            'negative': self.negative[direction].asdict(),
+            'directed': self.unknown_effect[direction].asdict(),
+            'undirected': self.direction['undirected'].asdict(),
+        }
+
+
+    def serialize_attrs(self, direction: tuple | str | None = None) -> str:
+        """
+        Serialize the resource specific attributes into a JSON string.
+        """
 
         evs = self.evidences if not direction else self.direction[direction]
 
         return evs.serialize_attrs()
 
 
+    def serialize_evidences(self, direction: tuple) -> str:
+        """
+        Serialize the evidences into a JSON string.
+        """
+
+        return self._serialize(self.asdict(direction = direction))
+
+
     def _get_attr(self, resource, key, direction):
 
         if resource in self.direction[direction]:
 
             return self.direction[direction][resource][key]
```

### Comparing `pypath_omnipath-0.14.48/pypath/core/intercell.py` & `pypath_omnipath-0.15.4/pypath/core/intercell.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/intercell_annot.py` & `pypath_omnipath-0.15.4/pypath/core/intercell_annot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/core/network.py` & `pypath_omnipath-0.15.4/pypath/core/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 #  Website: http://pypath.omnipathdb.org/
 #
 
 from __future__ import annotations
 
 from future.utils import iteritems
 
+from typing import Mapping
+
 import importlib as imp
 import re
 import os
 import sys
 import collections
 import itertools
 import functools
@@ -52,14 +54,15 @@
 import pypath.share.settings as settings
 import pypath.share.cache as cache_mod
 import pypath.share.constants as constants
 import pypath.utils.mapping as mapping
 import pypath.inputs.pubmed as pubmed_input
 import pypath.share.curl as curl
 import pypath.internals.refs as refs_mod
+import pypath.internals.resource as resource_mod
 import pypath.utils.reflists as reflists
 import pypath.resources.network as network_resources
 import pypath.inputs as inputs
 
 # Py 2/3
 try:
     input = raw_input
@@ -499,14 +502,19 @@
 
 
     def __len__(self):
 
         return len(self.interactions)
 
 
+    def __bool__(self):
+
+        return bool(self.interactions)
+
+
     def __iter__(self):
 
         for ia in self.interactions.values():
 
             yield ia
 
 
@@ -578,17 +586,17 @@
             'first_n': first_n,
         }
 
         exclude = common.to_set(exclude)
 
         resources = (
             (resources,)
-                if not isinstance(resources, (list, dict, tuple, set)) else
+                if not isinstance(resources, (list, Mapping, tuple, set)) else
             resources.values()
-                if isinstance(resources, dict) else
+                if isinstance(resources, Mapping) else
             resources
         )
 
         for resource in resources:
 
             if (
                 isinstance(resource, common.basestring) and
@@ -686,15 +694,16 @@
         total_attempts = settings.get('network_load_resource_attempts')
 
         for attempt in range(total_attempts):
 
             try:
 
                 self._log(
-                    f'Loading network data from resource `{resource.name}`; '
+                    f'Loading network data from resource `{resource.name}`'
+                    f' (dataset: {resource.dataset}); '
                     f'attempt {attempt + 1} of {total_attempts}.'
                 )
 
                 self._read_resource(
                     resource,
                     reread = reread,
                     redownload = redownload,
@@ -711,24 +720,15 @@
             except Exception as e:
 
                 exc = sys.exc_info()
                 self._log(
                     'Failed to read interactions '
                     f'from resource `{resource.name}`:'
                 )
-                self._log_traceback()
-
-                try:
-
-                    traceback.print_tb(e.__traceback__, file = sys.stdout)
-
-                except:
-
-                    self._log('Failed to handle exception.')
-                    self._log_traceback()
+                self._log_traceback(console = True)
 
                 if attempt == total_attempts - 1:
 
                     self._log(
                         f'Not loading `{resource.name}`: giving up after '
                         f'{total_attempts} attempts.'
                     )
@@ -1291,14 +1291,15 @@
 
                     _resources_secondary = tuple(
                         network_resources.resource.NetworkResource(
                             name = sec_res,
                             interaction_type = _resource.interaction_type,
                             data_model = _resource.data_model,
                             via = _resource.name,
+                            dataset = _resource.dataset,
                         )
                         for sec_res in resource
                         if sec_res != _resource.name
                     )
 
                     resource.add(networkinput.name)
 
@@ -1325,15 +1326,15 @@
                     )
 
                     # 11) creating the Evidence object
                     evidences = evidence.Evidences(
                         evidences = (
                             evidence.Evidence(
                                 resource = _res,
-                                references = refs,
+                                references = None if _res.via else refs,
                                 attrs = attrs_edge,
                             )
                             for _res in
                             _resources_secondary + (_resource,)
                         )
                     )
 
@@ -2177,14 +2178,22 @@
 
             interaction.add_evidence(
                 evidence = evidences,
                 direction = (entity_a, entity_b),
                 effect = -1,
             )
 
+        if is_directed and not positive and not negative:
+
+            interaction.add_evidence(
+                evidence = evidences,
+                direction = (entity_a, entity_b),
+                effect = 0,
+            )
+
         self.add_interaction(
             interaction,
             attrs = extra_attrs,
             only_directions = only_directions,
         )
 
 
@@ -2954,14 +2963,15 @@
 
 
     def extra_directions(
             self,
             resources = 'extra_directions',
             use_laudanna = False,
             use_string = False,
+            dataset = 'directionextra',
         ):
         """
         Adds additional direction & effect information from resources having
         no literature curated references, but giving sufficient evidence
         about the directionality for interactions already supported by
         literature evidences from other sources.
         """
@@ -2981,41 +2991,53 @@
                 network_resources.pathway_bad['laudanna_directions']
             )
 
         if use_string:
 
             pass
 
+        resources = resource_mod.NetworkDataset(
+            name = dataset,
+            resources = resources,
+        )
+
         self.load(resources = resources, only_directions = True)
 
 
     @staticmethod
     def omnipath_resources(
             omnipath = None,
             kinase_substrate_extra = False,
             ligand_receptor_extra = False,
             pathway_extra = False,
             old_omnipath_resources = False,
             exclude = None,
-        ):
+        ) -> list[network_resoruces.resource.NetworkResource]:
+
 
+        def reference_constraints(resources, data_model, relax = True):
 
-        def reference_constraints(resources, data_model, relax):
+            result = []
 
             resources = (
                 resources.values()
                     if isinstance(resources, dict) else
                 resources
             )
 
+            resources = copy_mod.deepcopy(resources)
+
             for res in resources:
 
                 if res.data_model == data_model:
 
                     res.networkinput.must_have_references = not relax
+                    result.append(res)
+
+            return result
 
 
         omnipath = omnipath or copy_mod.deepcopy(network_resources.omnipath)
         exclude = common.to_set(exclude)
 
         if old_omnipath_resources:
 
@@ -3031,35 +3053,35 @@
 
         else:
 
             omnipath['huri'] = copy_mod.deepcopy(
                 network_resources.interaction_misc['huri']
             )
 
-        reference_constraints(
-            omnipath,
-            'activity_flow',
-            pathway_extra,
-        )
-        reference_constraints(
-            omnipath,
-            'ligand_receptor',
-            ligand_receptor_extra,
-        )
-        reference_constraints(
-            omnipath,
-            'enzyme_substrate',
-            kinase_substrate_extra,
-        )
-
-        omnipath = dict(
-            (key, resource)
-            for key, resource in iteritems(omnipath)
-            if resource.name not in exclude
-        )
+        omnipath = list(omnipath.without(exclude))
+
+        for dataset, data_model, enabled in (
+            ('pathwayextra', 'activity_flow', pathway_extra),
+            ('ligrecextra', 'ligand_receptor', ligand_receptor_extra),
+            ('kinaseextra', 'enzyme_substrate', kinase_substrate_extra),
+        ):
+
+            if enabled:
+
+                extra = list(
+                    resource_mod.NetworkDataset(
+                        name = dataset,
+                        resources = reference_constraints(
+                            omnipath,
+                            data_model,
+                        ),
+                    )
+                )
+
+                omnipath.extend(extra)
 
         return omnipath
 
 
     def load_omnipath(
             self,
             omnipath = None,
@@ -3093,31 +3115,29 @@
             pathway_extra = pathway_extra,
             old_omnipath_resources = old_omnipath_resources,
             exclude = exclude,
         )
 
         self.load(omnipath, exclude = exclude, allow_loops = allow_loops)
 
-        if kinase_substrate_extra:
-
-            self._log('Loading extra enzyme-substrate interactions.')
-
-            self.load(network_resources.ptm_misc, exclude = exclude)
 
-        if ligand_receptor_extra:
-
-            self._log('Loading extra ligand-receptor interactions.')
-
-            self.load(network_resources.ligand_receptor, exclude = exclude)
+        for dataset, label, enabled in (
+            ('pathwayextra', 'activity flow', pathway_extra),
+            ('ligrecextra', 'ligand-receptor', ligand_receptor_extra),
+            ('kinaseextra', 'enzyme-PTM', kinase_substrate_extra),
+        ):
 
-        if pathway_extra:
+            if enabled:
 
-            self._log('Loading extra activity flow interactions.')
+                self._log(f'Loading extra {label} interactions.')
 
-            self.load(network_resources.pathway_noref, exclude = exclude)
+                self.load(
+                    getattr(network_resources, dataset).rename(dataset),
+                    exclude = exclude,
+                )
 
         if extra_directions:
 
             self.extra_directions()
 
         if remove_htp:
 
@@ -3353,37 +3373,45 @@
         if make_df:
 
             cls.make_df()
 
         return new
 
 
-    def load_dorothea(self, levels = None, expand_levels = None, **kwargs):
+    @staticmethod
+    def dorothea_resources(levels = None, expand_levels = None):
 
         expand_levels = (
             expand_levels
                 if isinstance(expand_levels, bool) else
             settings.get('dorothea_expand_levels')
         )
 
-        dorothea_resource = copy_mod.deepcopy(
-            network_resources.transcription_dorothea['dorothea']
-        )
+        dorothea = copy_mod.deepcopy(network_resources.transcription_dorothea)
 
         if levels:
 
-            dorothea_resource.networkinput.input_args['levels'] = levels
+            dorothea['dorothea'].networkinput.input_args['levels'] = levels
 
         dorothea = (
-            network_resources.dorothea_expand_levels(
-                dorothea_resource,
-                levels = levels,
-            )
+            network_resources.dorothea_expand_levels(dorothea, levels = levels)
                 if expand_levels else
-            dorothea_resource
+            dorothea
+        )
+
+        dorothea = dorothea.rename('dorothea')
+
+        return dorothea
+
+
+    def load_dorothea(self, levels = None, expand_levels = None, **kwargs):
+
+        dorothea = self.dorothea_resources(
+            levels = levels,
+            expand_levels = expand_levels,
         )
 
         self.load(dorothea, **kwargs)
 
 
     @classmethod
     def dorothea(cls, levels = None, ncbi_tax_id = 9606, **kwargs):
@@ -3458,15 +3486,15 @@
             )
 
         if original_resources:
 
             transcription = (
                 original_resources
                     if not isinstance(original_resources, bool) else
-                network_resources.transcription_onebyone
+                network_resources.transcription_onebyone.rename('tf_target')
             )
 
             self.load(
                 resources = transcription,
                 reread = reread,
                 redownload = redownload,
                 exclude = exclude,
@@ -3514,15 +3542,17 @@
         return new
 
 
     def load_mirna_target(self, **kwargs):
 
         if 'resources' not in kwargs:
 
-            kwargs['resources'] = network_resources.mirna_target
+            kwargs['resources'] = (
+                network_resources.mirna_target.rename('mirnatarget')
+            )
 
         self.load(**kwargs)
 
 
     @classmethod
     def mirna_target(
             cls,
@@ -4761,18 +4791,19 @@
 def init_db(use_omnipath = False, method = None, **kwargs):
 
     method_name = (
         'load_omnipath'
             if use_omnipath else
         (method or 'load')
     )
-    n = Network()
-    getattr(n, method_name)(**kwargs)
 
-    globals()['db'] = n
+    new_network = Network()
+    maybe_network = getattr(new_network, method_name)(**kwargs)
+
+    globals()['db'] = maybe_network or new_network
 
 
 def get_db(**kwargs):
 
     if 'db' not in globals():
 
         init_db(**kwargs)
```

### Comparing `pypath_omnipath-0.14.48/pypath/data/embl_colors` & `pypath_omnipath-0.15.4/pypath/data/embl_colors`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/data/goose_annotations.sql` & `pypath_omnipath-0.15.4/pypath/data/goose_annotations.sql`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/data/settings.yaml` & `pypath_omnipath-0.15.4/pypath/data/settings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,17 @@
 small_molecule_pickle: small_molecule.pickle
 
 # Internet settings
 server_annotations_full_download: false
 mapping_use_cache: true
 mapping_uniprot_static: false
 use_intermediate_cache: true
-uniprot_uploadlists_chunk_size: 10000
+uniprot_uploadlists_chunk_size: 100000
+uniprot_idmapping_timeout: 180
+uniprot_idmapping_poll_interval: 3
 timestamp_dirs: true
 uniprot_info_maxlen: 500
 uniprot_datasheet_connect_timeout: 10
 uniprot_datasheet_timeout: 20
 genecards_datasheet_connect_timeout: 10
 genecards_datasheet_timeout: 20
 curl_connect_timeout: 10
```

### Comparing `pypath_omnipath-0.14.48/pypath/data/www/favicon.ico` & `pypath_omnipath-0.15.4/pypath/data/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/formats/obo.py` & `pypath_omnipath-0.15.4/pypath/formats/obo.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/formats/sqldump.py` & `pypath_omnipath-0.15.4/pypath/formats/sqldump.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/formats/sqlite.py` & `pypath_omnipath-0.15.4/pypath/formats/sqlite.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/formats/xml.py` & `pypath_omnipath-0.15.4/pypath/formats/xml.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/__init__.py` & `pypath_omnipath-0.15.4/pypath/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/abs.py` & `pypath_omnipath-0.15.4/pypath/inputs/abs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/acsn.py` & `pypath_omnipath-0.15.4/pypath/inputs/acsn.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/adhesome.py` & `pypath_omnipath-0.15.4/pypath/inputs/adhesome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/almen2009.py` & `pypath_omnipath-0.15.4/pypath/inputs/almen2009.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/baccin2019.py` & `pypath_omnipath-0.15.4/pypath/inputs/baccin2019.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/biogps.py` & `pypath_omnipath-0.15.4/pypath/inputs/biogps.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/biogrid.py` & `pypath_omnipath-0.15.4/pypath/inputs/biogrid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/biomart.py` & `pypath_omnipath-0.15.4/pypath/inputs/biomart.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/biomodels.py` & `pypath_omnipath-0.15.4/pypath/inputs/biomodels.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ca1.py` & `pypath_omnipath-0.15.4/pypath/inputs/ca1.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cancercellmap.py` & `pypath_omnipath-0.15.4/pypath/inputs/cancercellmap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cancerdrugsdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/cancerdrugsdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cancersea.py` & `pypath_omnipath-0.15.4/pypath/inputs/cancersea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cell.py` & `pypath_omnipath-0.15.4/pypath/inputs/cell.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cellcall.py` & `pypath_omnipath-0.15.4/pypath/inputs/cellcall.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cellcellinteractions.py` & `pypath_omnipath-0.15.4/pypath/inputs/cellcellinteractions.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cellchatdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/cellchatdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cellinker.py` & `pypath_omnipath-0.15.4/pypath/inputs/cellinker.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cellphonedb.py` & `pypath_omnipath-0.15.4/pypath/inputs/cellphonedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/celltalkdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/celltalkdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/celltypist.py` & `pypath_omnipath-0.15.4/pypath/inputs/celltypist.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/chembl.py` & `pypath_omnipath-0.15.4/pypath/inputs/chembl.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,21 +452,21 @@
         fileobj = open(c.fileobj.name, encoding='utf-8')
         page_dct = json.loads(fileobj.read())
 
         indication_lst.extend(
             ChemblIndication(
                 efo_id = ind['efo_id'],
                 efo_term = ind['efo_term'],
-                max_phase = int(ind['max_phase_for_ind']),
+                max_phase = float(ind['max_phase_for_ind']),
                 mesh_heading = ind['mesh_heading'],
                 mesh_id = ind['mesh_id'],
                 molecule_chembl = ind['molecule_chembl_id'],
             )
             for ind in page_dct['drug_indications']
-            if int(ind['max_phase_for_ind']) > max_phase_threshold and max_phase_threshold != 0 \
+            if float(ind['max_phase_for_ind']) > max_phase_threshold and max_phase_threshold != 0 \
                 or max_phase_threshold == 0
         )
     
     return indication_lst
 
 
 def chembl_mechanisms() -> list[tuple]:
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/clinvar.py` & `pypath_omnipath-0.15.4/pypath/inputs/clinvar.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,19 +53,24 @@
             [
                 'allele',
                 'type',
                 'variant',
                 'entrez',
                 'genesymbol',
                 'clinical_significance',
+                'review_status',
                 'rs',
                 'phenotype_ids',
                 'phenotypes',
+                'otherids',
                 'origin',
                 'variation_id',
+                'assembly',
+                'chromosome',
+                'chromosome_accession',
             ],
             defaults = None
         )
 
     url = urls.urls['clinvar']['url']
     c = curl.Curl(url, large = True, silent = False)
     c.gzfile.seek(1) # get rid of a stray `#` character
@@ -75,29 +80,35 @@
         dialect = 'excel-tab',
     )
 
     result = set()
 
     for row in response:
 
-        phenotype_ids = tuple(row['PhenotypeIDS'].replace('|', ';').split(';'))
-        phenotypes = tuple(row['PhenotypeList'].replace('|', ';').split(';'))
+        phenotype_ids = tuple(row['PhenotypeIDS'].replace('|', ';').replace(',', ';').split(';'))
+        phenotypes = tuple(row['PhenotypeList'].replace('|', ';').replace(',', ';').split(';'))
+        otherids = tuple(row['OtherIDs'].replace('|', ';').replace(',', ';').split(';'))
 
         variant = Variant(
             allele = row['AlleleID'],
             type = row['Type'],
             variant = row['Name'],
             entrez = row['GeneID'],
             genesymbol = row['GeneSymbol'],
             clinical_significance = row['ClinicalSignificance'],
+            review_status = row['ReviewStatus'],
             rs = row['RS# (dbSNP)'],
             phenotype_ids = phenotype_ids,
             phenotypes = phenotypes,
+            otherids = None if otherids[0] == '-' else otherids,
             origin = row['OriginSimple'],
-            variation_id = row['VariationID']
+            variation_id = row['VariationID'],
+            assembly = row['Assembly'],
+            chromosome = row['Chromosome'],
+            chromosome_accession = row['ChromosomeAccession'],
         )
         result.add(variant)
 
     return list(result)
 
 
 def clinvar_citations() -> list[tuple]:
@@ -139,8 +150,8 @@
             nsv = row['nsv'],
             citation_source = row['citation_source'],
             citation_id = row['citation_id']
         )
 
         result.add(citation)
 
-    return list(result)
+    return list(result)
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/collectri.py` & `pypath_omnipath-0.15.4/pypath/inputs/collectri.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         (
             'tf',
             'target',
             'effect',
             'tf_category',
             'resources',
             'pubmed',
+            'sign_decision',
             'target_type',
         ),
     )
 
     url = urls.urls['collectri']['url']
     c = curl.Curl(
         url,
@@ -145,14 +146,15 @@
             CollectriRecord(
                 tf = l[0],
                 target = target_id,
                 effect = int(l[2]),
                 tf_category = l[3],
                 resources = l[4].replace('DoRothEA_A', 'DoRothEA-A'),
                 pubmed = l[5],
+                sign_decision = l[6],
                 target_type = 'mirna' if mmirna else 'protein',
             )
         )
 
     return result
 
 
@@ -179,14 +181,15 @@
         (
             'tf',
             'target',
             'effect',
             'tf_category',
             'resources',
             'pubmed',
+            'sign_decision',
             'target_type',
         ),
     )
 
 
     def process_complex(name):
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/common.py` & `pypath_omnipath-0.15.4/pypath/inputs/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/compleat.py` & `pypath_omnipath-0.15.4/pypath/inputs/compleat.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/complexportal.py` & `pypath_omnipath-0.15.4/pypath/inputs/complexportal.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/comppi.py` & `pypath_omnipath-0.15.4/pypath/inputs/comppi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/connectomedb.py` & `pypath_omnipath-0.15.4/pypath/inputs/connectomedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/corum.py` & `pypath_omnipath-0.15.4/pypath/inputs/corum.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cosmic.py` & `pypath_omnipath-0.15.4/pypath/inputs/cosmic.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cpad.py` & `pypath_omnipath-0.15.4/pypath/inputs/cpad.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cpdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/cpdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/credentials.py` & `pypath_omnipath-0.15.4/pypath/inputs/credentials.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/csa.py` & `pypath_omnipath-0.15.4/pypath/inputs/csa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cspa.py` & `pypath_omnipath-0.15.4/pypath/inputs/cspa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ctdbase.py` & `pypath_omnipath-0.15.4/pypath/inputs/ctdbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/cytosig.py` & `pypath_omnipath-0.15.4/pypath/inputs/cytosig.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/dbptm.py` & `pypath_omnipath-0.15.4/pypath/inputs/dbptm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/deathdomain.py` & `pypath_omnipath-0.15.4/pypath/inputs/deathdomain.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/depod.py` & `pypath_omnipath-0.15.4/pypath/inputs/depod.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/dgidb.py` & `pypath_omnipath-0.15.4/pypath/inputs/dgidb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/dip.py` & `pypath_omnipath-0.15.4/pypath/inputs/dip.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/disgenet.py` & `pypath_omnipath-0.15.4/pypath/inputs/disgenet.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/domino.py` & `pypath_omnipath-0.15.4/pypath/inputs/domino.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/dorothea.py` & `pypath_omnipath-0.15.4/pypath/inputs/dorothea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/drugbank.py` & `pypath_omnipath-0.15.4/pypath/inputs/drugbank.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/drugcentral.py` & `pypath_omnipath-0.15.4/pypath/inputs/drugcentral.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ebi.py` & `pypath_omnipath-0.15.4/pypath/inputs/ebi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/elm.py` & `pypath_omnipath-0.15.4/pypath/inputs/elm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/embopress.py` & `pypath_omnipath-0.15.4/pypath/inputs/embopress.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/embrace.py` & `pypath_omnipath-0.15.4/pypath/inputs/embrace.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/encode.py` & `pypath_omnipath-0.15.4/pypath/inputs/encode.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ensembl.py` & `pypath_omnipath-0.15.4/pypath/inputs/ensembl.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/exocarta.py` & `pypath_omnipath-0.15.4/pypath/inputs/exocarta.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/genecards.py` & `pypath_omnipath-0.15.4/pypath/inputs/genecards.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/go.py` & `pypath_omnipath-0.15.4/pypath/inputs/go.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/gpcrdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/gpcrdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/graphviz.py` & `pypath_omnipath-0.15.4/pypath/inputs/graphviz.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/guide2pharma.py` & `pypath_omnipath-0.15.4/pypath/inputs/guide2pharma.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,23 @@
 #  Distributed under the GPLv3 License.
 #  See accompanying file LICENSE.txt or copy at
 #      http://www.gnu.org/licenses/gpl-3.0.html
 #
 #  Website: http://pypath.omnipathdb.org/
 #
 
+from __future__ import annotations
+
 import csv
 import collections
 import itertools
 
 import pypath.share.curl as curl
 import pypath.share.common as common
+import pypath.share.constants as constants
 import pypath.resources.urls as urls
 import pypath.utils.mapping as mapping
 import pypath.utils.taxonomy as taxonomy
 import pypath.internals.intera as intera
 
 
 def guide2pharma_download(
@@ -47,15 +50,19 @@
     Args:
         organism
             Name of the organism, e.g. `human`.
         endogenous
             Whether to include only endogenous ligands interactions.
     """
 
-    get_taxid = taxonomy.ensure_ncbi_tax_id
+    get_taxid = lambda x: (
+        constants.NOT_ORGANISM_SPECIFIC
+            if x in {'', 'None'} else
+        taxonomy.ensure_ncbi_tax_id(x)
+    )
     organism_ = None
     ncbi_tax_id = None
 
     if isinstance(organism, common.basestring):
 
         ncbi_tax_id = get_taxid(organism)
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/havugimana.py` & `pypath_omnipath-0.15.4/pypath/inputs/havugimana.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/hgnc.py` & `pypath_omnipath-0.15.4/pypath/inputs/hgnc.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/hippie.py` & `pypath_omnipath-0.15.4/pypath/inputs/hippie.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/hmdb.py` & `pypath_omnipath-0.15.4/pypath/utils/unichem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,521 +1,425 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
 #  This file is part of the `pypath` python module
 #
 #  Copyright
-#  2014-2023
+#  2014-2022
 #  EMBL, EMBL-EBI, Uniklinik RWTH Aachen, Heidelberg University
 #
 #  Authors: Dénes Türei (turei.denes@gmail.com)
 #           Nicolàs Palacio
 #           Sebastian Lobentanzer
 #           Erva Ulusoy
 #           Olga Ivanova
 #           Ahmet Rifaioglu
-#           Sebastian Lobentanzer
 #
 #  Distributed under the GPLv3 License.
 #  See accompanying file LICENSE.txt or copy at
 #      http://www.gnu.org/licenses/gpl-3.0.html
 #
 #  Website: http://pypath.omnipathdb.org/
 #
 
 from __future__ import annotations
 
-"""
-Access the Human Metabolome Database.
-"""
-
-from typing import Any, Literal
+from future.utils import iteritems
+from past.builtins import xrange, range
 
-import itertools
+import json
+import os
+import sys
+import textwrap
 
-from lxml import etree
-import pandas as pd
+import bs4
 
-import pypath.resources.urls as urls
+import pypath.share.progress as progress
 import pypath.share.curl as curl
 import pypath.share.common as common
-import pypath.share.session as session
-import pypath.formats.xml as xml
+import pypath.inputs.unichem as unichem_input
 
-_log = session.Logger(name = 'hmdb_input')._log
 
+class Unichem(object):
+    """
+    Client for the UniChem drug compound identifier translation service
+    (https://www.ebi.ac.uk/unichem/).
+    """
 
-XMLNS = '{http://www.hmdb.ca}'
+    def __init__(self):
 
+        sys.stdout.write(
+            '\n\tType `Unichem_instance.usage()` to get help.\n\n'
+        )
+        sys.stdout.flush()
 
-def hmdb_xml(dataset: Literal['metabolites']) -> etree.iterparse:
-    """
-    Download and open the XML file of a dataset from the HMDB.
-    """
+        # from unichem id to db name
+        self.uc_dict = unichem_input.unichem_sources()
+        # from db name to unichem id
+        self.name_dict = common.swap_dict(self.uc_dict)
+        self.url_stem = 'https://www.ebi.ac.uk/unichem/rest/src_compound_id'
+        self.inchi_stem = 'https://www.ebi.ac.uk/unichem/rest/inchikey/%s'
+        self.chembl_url = (
+            'http://www.ebi.ac.uk/chemblws/compounds/smiles/{0}.json'
+        )
+        self.cpd_search = 'http://www.ebi.ac.uk/unichem/rest/{0}/{1}/{2}{3}'
+        self.result = {}
 
-    url = urls.urls['hmdb'][dataset]
-    c = curl.Curl(
-        url,
-        large = True,
-        silent = False,
-        slow = True,
-        default_mode = 'rb',
-    )
-
-    return etree.iterparse(
-        c.result['hmdb_metabolites.xml'],
-        tag = f'{XMLNS}metabolite',
-    )
 
 
-def hmdb_iter_metabolites():
-    """
-    Itertate over metabolite records from HMDB.
-    """
+    def usage(self):
+        """
+        Prints usage information and examples to the standard output.
+        """
 
-    for _, element in hmdb_xml('metabolites'):
+        msg = '''
+        List of identifier types can be read above.
+        To query UniChem, give either names or numbers of the
+        ID types you wish to translate from and to.
+        E.g.
+        >>> u = unichem.Unichem()
+        >>> u.translate('pubchem', 'chembl', list_of_pubchems)
 
-        yield element
+        For example, the PubChem CID of Aspirin is 2244. Translate it to
+        ChEMBL:
+        >>> u.translate('pubchem', 'chembl', '2244')
+        >>> u.result
+        {'2244': ['CHEMBL25']}
 
+        We can translate multiple identifiers the same way:
+        >>>
+        >>> u.translate('pubchem', 'chembl', ['2244', '4091'])
+        >>> u.result
+        {'2244': ['CHEMBL25'], '4091': ['CHEMBL1431']}
 
-def _ref_chunk(container: str = 'references') -> tuple:
+        Additional ways of translation are from SMILEs to ChEMBL IDs, and
+        from InChiKeys to any ID. These are translated not by the UniChem,
+        but by the ChEMBL webservice.
+        >>> u.translate('smiles', 'chembl', list_of_smiles)
+        >>> u.translate('inchikey', 'chembl', list_of_inchikeys)
 
-    return (
-        container,
-        ('reference', 'findall'),
-        'pubmed_id',
-        None,
-    )
-
-
-ONTOLOGY_FIELDS = xml._simple_fields((
-    'term',
-    'definition',
-    'parent_id',
-    'level',
-    'type',
-))
-
-
-def _ontology(descendant: etree._Element) -> dict:
-
-    path = (
-        dict(
-            **ONTOLOGY_FIELDS,
-            **{
-                'descendants': (
-                    'descendants',
-                    ('descendant', 'findall'),
-                    _ontology,
-                ),
-            },
-        ),
-    )
-
-    return xml.fetch(descendant, path, namespaces = XMLNS)
-
-
-ONTOLOGY = (
-    'ontology',
-    ('root', 'findall'),
-    _ontology,
-)
-
-SIMPLE_FIELDS = {
-    'accession',
-    'name',
-    'version',
-    'status',
-    'description',
-    'chemical_formula',
-    'average_molecular_weight',
-    'monisotopic_molecular_weight',
-    'iupac_name',
-    'traditional_iupac',
-    'cas_registry_number',
-    'smiles',
-    'inchi',
-    'inchikey',
-    'state',
-    'synthesis_reference',
-}
-
-ID_FIELDS = {
-    'chemspider',
-    'drugbank',
-    'foodb',
-    'pubchem_compound',
-    'pdb',
-    'chebi',
-    'phenol_explorer_compound',
-    'knapsack',
-    'kegg',
-    'biocyc',
-    'bigg',
-    'wikipedia',
-    'metlin',
-    'vmh',
-    'fbonto',
-}
-
-SIMPLE_FIELDS.update(xml._simple_fields(f'{f}_id' for f in ID_FIELDS))
-
-ARRAY_FIELDS = {
-    ('secondary_accessions', 'accession'),
-    ('synonyms', 'synonym'),
-}
-
-TAXONOMY = (
-    'taxonomy',
-    dict(
-        **xml._simple_fields((
-            'description',
-            'direct_parent',
-            'kingdom',
-            'class',
-            'sub_class',
-            'molecular_framework',
-        )),
-        **xml._array_fields((
-            ('alternative_parents', 'alternative_parent'),
-            ('substituents', 'substituent'),
-        )),
-    ),
-)
-
-EXPERIMENTAL_PROPERTIES = (
-    'experimental_properties',
-    ('property', 'findall'),
-    {'kind', 'value', 'source'},
-)
-
-PREDICTED_PROPERTIES = (
-    'predicted_properties',
-    ('property', 'findall'),
-    {'kind', 'value', 'source'},
-)
-
-SPECTRA = (
-    'spectra',
-    ('spectrum', 'findall'),
-    {'type', 'spectrum_id'},
-)
-
-BIOLOGICAL_PROPERTIES = (
-    'biological_properties',
-    {
-        'cellular_locations': (
-            'cellular_locations',
-            ('cellular', 'findall'),
-            None,
-        ),
-        'biospecimen_locations': (
-            'biospecimen_locations',
-            ('biospecimen', 'findall'),
-            None,
-        ),
-        'tissue_locations': (
-            'tissue_locations',
-            ('tissue', 'findall'),
-            None,
-        ),
-        'pathways': (
-            'pathways',
-            ('pathway', 'findall'),
-            {'name', 'smpdb_id', 'kegg_map_id'},
-        ),
-    }
-)
-
-NORMAL_CONCENTRATIONS = (
-    'normal_concentrations',
-    ('concentration', 'findall'),
-    dict(
-        **xml._simple_fields((
-            'biospecimen',
-            'concentration_value',
-            'concentration_units',
-            'subject_age',
-            'subject_sex',
-            'subject_condition',
-        )),
-        **{'references': _ref_chunk()},
-    ),
-)
-
-ABNORMAL_CONCENTRATIONS = (
-    'abnormal_concentrations',
-    ('concentration', 'findall'),
-    dict(
-        **xml._simple_fields((
-            'biospecimen',
-            'concentration_value',
-            'concentration_units',
-            'patient_age',
-            'patient_sex',
-            'patient_information',
-        )),
-        **{'references': _ref_chunk()},
-    ),
-)
-
-DISEASES = (
-    'diseases',
-    ('disease', 'findall'),
-    dict(
-        **xml._simple_fields((
-            'name',
-            'omim_id',
-        )),
-        **{'references': _ref_chunk()},
-    ),
-)
-
-GENERAL_REFERENCES = _ref_chunk('general_references')
-
-PROTEIN_ASSOCIATIONS = (
-    'protein_associations',
-    ('protein', 'findall'),
-    {
-        'protein_accession',
-        'name',
-        'uniprot_id',
-        'gene_name',
-        'protein_type',
-    },
-)
-
-SCHEMA = {
-    'taxonomy': TAXONOMY,
-    'spectra': SPECTRA,
-    'biological_properties': BIOLOGICAL_PROPERTIES,
-    'experimental_properties': EXPERIMENTAL_PROPERTIES,
-    'predicted_properties': PREDICTED_PROPERTIES,
-    'normal_concentrations': NORMAL_CONCENTRATIONS,
-    'abnormal_concentrations': ABNORMAL_CONCENTRATIONS,
-    'diseases': DISEASES,
-    'general_references': GENERAL_REFERENCES,
-    'protein_associations': PROTEIN_ASSOCIATIONS,
-    'ontology': ONTOLOGY,
-}
-SCHEMA.update(xml._simple_fields(SIMPLE_FIELDS))
-SCHEMA.update(xml._array_fields(ARRAY_FIELDS))
+        Other option to search is connectivity search from UniChem.
+        A-G parameters can be defined optionally. See description at
+        https://www.ebi.ac.uk/unichem/info/widesearchInfo
+        >>> u.connectivity_search(list_of_zincs, 'zinc', parameters=[1,0,0,0,0,1,0])
 
+        InChiKeys can be used in connectivity search too:
+        >>> u.connectivity_search(list_of_inchikeys, 'inchikey', parameters=[1,0,0,0,0,1,0])
 
-def hmdb_metabolites_raw(schema: dict = None, head: int | None = None) -> list:
-    """
-    Parse metabolite data from HMDB.
+        You can also call directly functions accessing ChEMBL webservice, with the
+        same result as you would call `translate()` or `connectivity_search()`:
+        >>> u.smiles2chembl(list_of_smiles)
+        >>> u.inchikey2anything('chembl', list_of_inchikeys)
 
-    Args:
-        schema:
-            The schema defines the fields to be parsed. By default, a schema
-            covering nearly all fields in the HMDB metabolites XML is used.
-            Likely you don't need all the fields within one task: in this
-            case see `pypath.inputs.hmdb.SCHEMA` to see the full schema,
-            and create your own that is restricted to your fields of interst.
-        head:
-            Process the first N records only. Useful for peeking into
-            the data.
-
-    Returns:
-        A list of dicts, each dict containing the data extracted from
-        one metabolite record. These dicts might be deeply nested, and
-        the structure depends on the schema used.
-    """
+        Find the dict in `u.result`. Untranslated items have value `None`.
+        Every call overwrites previous result!
 
-    result = []
-    schema = schema or SCHEMA
+        For an up to date list of identifier types see
+        https://www.ebi.ac.uk/unichem/ucquery/listSources or
+        call `Unichem.info(<source>)`:
+        >>> Unichem.info('chembl')
+        '''
 
-    for i, met in enumerate(hmdb_iter_metabolites()):
+        sys.stdout.write(os.linesep)
 
-        yield xml.fetch(met, schema, XMLNS)
+        id_types = sorted(
+            self.uc_dict.items(),
+            key = lambda x: int(x[0])
+        )
 
-        met.clear(keep_tail = True)
+        if len(id_types) % 2:
 
-        if i == head:
+            id_types.append(('',) * 2)
 
-            break
+        nrows = len(id_types) // 2
 
-    return result
+        for i in xrange(nrows):
 
+            sys.stdout.write(
+                ''.join((
+                    ' ' * 8,
+                    id_types[i][0].rjust(2),
+                    ' ' * 3,
+                    id_types[i][1].ljust(20),
+                    id_types[i + nrows][0].rjust(2),
+                    ' ' * 3,
+                    id_types[i + nrows][1].ljust(20),
+                    os.linesep,
+                ))
+            )
 
-class Field:
+        sys.stdout.write(msg + os.linesep)
+        sys.stdout.flush()
 
-    def __init__(self, name, *definition):
 
-        if isinstance(name, Field):
+    @staticmethod
+    def info(source):
+        """
+        Print information about one source.
 
-            name, definition = name.name, name.definition
+        Args
+            source (int,str): The numeric or string ID of one source.
+        """
 
-        self.name = name
-        self.d = definition or (name,)
+        unichem_input.info(source)
 
 
-    def process(self, record) -> tuple[tuple[Any]]:
+    def translate(self, source, target, lst):
+        """
+        Translate one drug compound identifier to another identifier type
+        using the UniChem web service. For an up to date list of identifier
+        types see https://www.ebi.ac.uk/unichem/ucquery/listSources.
 
-        value = ((record,),)
-        name = common.to_tuple(self.name)
+        Args
+            source (str,int): The source ID type, either as a string label
+                or as a number, as used in UniChem.
+            target (str,int): The target ID type, either as a string label
+                or as a number, as used in UniChem.
+            lst (str,set): One or more identifiers to translate.
 
-        for d in self.d:
+        Returns
+            Returns None, the results are stored in the `result` attribute
+            of this object.
+        """
 
-            if d == '@':
+        lst = common.to_set(lst)
+        self.result = {}
 
-                value = tuple(
-                    v[0]
-                        if isinstance(v[0], (list, tuple)) else v
-                    for v in value
-                )
+        if source == 'inchikey':
 
-            elif d == '*' or isinstance(d, tuple):
+            self.inchikey2anything(target, lst)
+            return None
 
-                if d == '*':
+        if source == 'smiles':
 
-                    d = tuple(sorted(value[0][0].keys()))
+            self.smiles2chembl(lst)
+            return None
 
-                if len(value[0][0]) > 1:
+        source = (
+            str(source)
+                if type(source) is int else
+            self.name_dict[source]
+        )
+        target = (
+            str(target)
+                if type(target) is int else
+            self.name_dict[target]
+        )
 
-                    _log('List of dicts content encountered.')
+        prg = progress.Progress(
+            total=len(lst),
+            name='Translating compound identifiers',
+            interval=1,
+        )
 
-                value = value[0][0]
-                value = tuple((value.get(k),) for k in d)
-                name = tuple(f'{n}__{k}' for n in name for k in d)
+        for comp in lst:
 
-            elif isinstance(d, str):
+            url = '/'.join([self.url_stem, comp, source, target])
+            c = curl.Curl(url, large = False)
+            result = c.result
+            self.result[comp] = []
 
-                value = tuple(tuple(v.get(d) for v in vv) for vv in value)
+            if result is not None:
 
-        return name, value
+                data = json.loads(result)
 
+                for d in data:
 
-    def __str__(self):
+                    self.result[comp].append(d['src_compound_id'])
 
-        return self.name
+            prg.step()
 
+        prg.terminate()
 
-def hmdb_table(
-        *fields: str | tuple,
-        head: int | None = None,
-        **named_fields: str | tuple,
-    ) -> pd.DataFrame:
-    """
-    Parse various simple and nested array fields from HMDB into data frame.
 
-    Args:
-        fields:
-            Fields to include in the data frame. These must be keys in the
-            schema, and will be also used as column names. Alternatively,
-            tuples of sequetial processing steps can be provided: strings
-            will be used as keys in nested dicts, tuples will be used as
-            multiple keys in dicts, each yielding a separate column, the
-            special symbol "*" means all keys in the sub-dict, while "@"
-            means expand arrays into multiple rows. Be careful with this
-            latter option because it is applied in a combinatorial way, i.e.
-            in case of expanding an array to 5 rowns, and another one to 7
-            rows results already 35 rows from a single record. This might
-            result excessive memory use and processing time.
-        named_fields:
-            Same as `fields`, but the column name can be different from the
-            top level key: argument names will be used as column names,
-            values will be used as processing steps.
-        head:
-            Process the first N records only. Useful for peeking into
-            the data.
-
-    Examples:
-
-        ..code-block:: python
-
-           from pypath.inputs import hmdb
-           df = hmdb.hmdb_table('accession', 'smiles', 'state', head = 10)
-           df = hmdb.hmdb_table('accession', ('synonyms', '@'), head = 10)
-           df = hmdb.hmdb_table(
-               'accession',
-               ('taxonomy', ('class', 'substituents')),
-               head = 10,
-           )
+    def inchikey2anything(self, target, lst):
+        """
+        Translate InChi keys to another identifier type using the ChEMBL
+        web service.
 
-    """
+        Args
+            target (str,int): The target ID type, either as a string label
+                or as a number, as used in UniChem.
+            lst (str,set): One or more InChi keys.
 
-    fields = [Field(d[0], *d) for d in (common.to_tuple(f) for f in fields)]
-    fields.extend(Field(n, *f) for n, f in named_fields.items())
-    keys = [f.d[0] for f in fields]
-    schema = {k: SCHEMA[k] for k in keys}
+        Returns
+            Returns None, the results are stored in the `result` attribute
+            of this object.
+        """
 
-    columns = []
-    data = []
-    result = pd.DataFrame()
+        lst = common.to_set(lst)
 
-    for i, met in enumerate(hmdb_metabolites_raw(schema, head = head)):
+        self.result = {}
+        target = (
+            str(target)
+                if type(target) is int else
+            self.name_dict[target]
+        )
+        prg = progress.Progress(
+            total=len(lst),
+            name='Translating InChi-Keys',
+            interval=1,
+        )
 
-        cols, rows = zip(*(f.process(met) for f in fields))
-        columns = columns or list(itertools.chain(*cols))
-        data.extend(itertools.product(*itertools.chain(*rows)))
+        for inchik in lst:
 
-        if (i + 1) % 100 == 0:
+            url = self.inchi_stem % inchik
+            c = curl.Curl(url, large = False)
+            result = c.result
 
-            df = pd.DataFrame.from_records(data, columns = columns)
-            result = pd.concat((result, df))
-            data = []
+            if result is not None:
 
-    df = pd.DataFrame.from_records(data, columns = columns)
-    result = pd.concat((result, df))
+                data = json.loads(result)
+                self.result[inchik] = [
+                    d['src_compound_id']
+                    for d in data
+                    if d['src_id'] == target
+                ]
+            prg.step()
 
-    return result
+        prg.terminate()
 
 
-def hmdb_mapping(
-        id_type_a: str,
-        id_type_b: str,
-        return_df: bool = False,
-        head: int | None = None,
-    ) -> dict[str, set[str]] | pd.DataFrame:
-    """
-    ID translation input from HMDB.
+    def smiles2chembl(self, smiles):
+        """
+        Translate SMILES to ChEMBL ID using the ChEMBL web service.
 
-    Note: you can use this function for purposes other than ID translation
-    tables, e.g. you can collect the molecular weights, pathways, etc. Though
-    not all these options are guaranteed to work or result a meaningful
-    output.
-
-    Args:
-        id_type_a:
-            An identifier type, see the `ID_FIELDS` set in this module,
-            and keys in the `SIMPLE_FIELDS` dict.
-        id_type_b:
-            Another identifier type, same options as for `id_type_a`.
-        return_df:
-            Return a data frame instead of dict of sets.
-        head:
-            Process the first N records only. Useful for peeking into
-            the data.
+        Args
+            smiles (str,list): One or more SMILES.
 
-    Return:
-        Translation data between two types of identifiers.
-    """
+        Returns
+            Returns None, the results are stored in the `result` attribute
+            of this object.
+        """
 
-    fields = {
-        'id_a': (_id_type(id_type_a), '@'),
-        'id_b': (_id_type(id_type_b), '@'),
-    }
+        smiles = common.to_set(smiles)
 
-    df = hmdb_table(**fields, head = head)
+        self.result = {}
+        prg = progress.Progress(
+            total=len(smiles),
+            name='Translating SMILEs',
+            interval=1
+        )
 
-    if return_df:
+        for sml in smiles:
 
-        return df
+            url = self.chembl_url.format(sml)
+            c = curl.Curl(url, large = False)
+            result = c.result
+            self.result[sml] = []
 
-    else:
+            if result is not None:
 
-        return df.groupby('id_a')['id_b'].apply(set).to_dict()
+                try:
 
+                    data = json.loads(result)
 
-def _id_type(id_type: str) -> str:
-    """
-    Field name from ID type.
-    """
+                    for d in data['compounds']:
+
+                        this_smile = d['smiles']
+                        this_chembl = d['chemblId']
+                        # if this_smile == sml:
+                        self.result[sml].append(this_chembl)
+
+                except ValueError:
+
+                    soup = bs4.BeautifulSoup(result)
+                    compounds = soup.find_all('compound')
+
+                    if compounds is not None:
+
+                        for compound in compounds:
+
+                            this_smile = compound.find('smiles').text
+                            this_chembl = compound.find('chemblid').text
+                            # if this_smile == sml:
+                            self.result[sml].append(this_chembl)
+            prg.step()
+
+        prg.terminate()
+
+
+    def connectivity_search(
+            self,
+            id_list: str | set,
+            id_type: str | int,
+            parameters: list[int] = [1, 0, 0, 0, 0, 1, 0]
+        ):
+        """
+        Search for structurally and chemically similar compounds based on
+        cheminformatics similarity metrics. Read more at
+        https://www.ebi.ac.uk/unichem/info/widesearchInfo.
+
+        Args
+            id_list:
+                One or more identifiers to query.
+            id_type:
+                Type of the identifiers, either as a string
+                label or a number as used by UniChem. SMILES is not
+                available in this type of query.
+            parameters:
+                A list of parameters A-H as described in
+                https://www.ebi.ac.uk/unichem/info/widesearchInfo.
+
+        Returns
+            Returns None, the results are stored in the `result` attribute
+            of this object.
+        """
+
+        id_list = common.to_set(id_list)
+
+        parameters.append(1)  # H parameter must be 1 to process the result
+        parameters = [str(i) for i in parameters]
+        self.result = {}
+
+        if id_type == 'inchikey':
+
+            id_type = ''
+            method = 'key_search'
+
+        elif id_type == 'smiles':
+
+            return None
+
+        else:
+
+            id_type = (
+                str(id_type)
+                    if type(id_type) is int else
+                self.name_dict[id_type]
+            )
+            id_type = '%s/' % id_type
+            method = 'cpd_search'
+
+        prg = progress.Progress(
+            total=len(id_list),
+            name='Connectivity search',
+            interval=1
+        )
+
+        for i in id_list:
+
+            prg.step()
+            url = self.cpd_search.format(
+                method,
+                i,
+                id_type,
+                '/'.join(parameters)
+            )
+            c = curl.Curl(url, large = False)
+            result = c.result
+            self.result[i] = []
+
+            if result is not None:
+
+                data = json.loads(result)
+
+                for k, v in iteritems(data):
+
+                    for j in xrange(1, len(v)):
 
-    for key in (id_type, f'{id_type}_id'):
+                        self.result[i].append(v[j][0])
 
-        if key in SCHEMA:
+            self.result[i] = list(set(self.result[i]))
 
-            return key
+        prg.terminate()
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/homologene.py` & `pypath_omnipath-0.15.4/pypath/inputs/homologene.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/hpmr.py` & `pypath_omnipath-0.15.4/pypath/inputs/hpmr.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/hpo.py` & `pypath_omnipath-0.15.4/pypath/inputs/hpo.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/hprd.py` & `pypath_omnipath-0.15.4/pypath/inputs/hprd.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/htri.py` & `pypath_omnipath-0.15.4/pypath/inputs/htri.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/humancellmap.py` & `pypath_omnipath-0.15.4/pypath/inputs/humancellmap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/humap.py` & `pypath_omnipath-0.15.4/pypath/inputs/humap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/huri.py` & `pypath_omnipath-0.15.4/pypath/inputs/huri.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/i3d.py` & `pypath_omnipath-0.15.4/pypath/inputs/i3d.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/icellnet.py` & `pypath_omnipath-0.15.4/pypath/inputs/icellnet.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ielm.py` & `pypath_omnipath-0.15.4/pypath/inputs/ielm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/imweb.py` & `pypath_omnipath-0.15.4/pypath/inputs/imweb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/innatedb.py` & `pypath_omnipath-0.15.4/pypath/inputs/innatedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/instruct.py` & `pypath_omnipath-0.15.4/pypath/inputs/instruct.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/intact.py` & `pypath_omnipath-0.15.4/pypath/inputs/intact.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/integrins.py` & `pypath_omnipath-0.15.4/pypath/inputs/integrins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/interpro.py` & `pypath_omnipath-0.15.4/pypath/inputs/interpro.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/intogen.py` & `pypath_omnipath-0.15.4/pypath/inputs/intogen.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ipi.py` & `pypath_omnipath-0.15.4/pypath/inputs/ipi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/italk.py` & `pypath_omnipath-0.15.4/pypath/inputs/italk.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/kea.py` & `pypath_omnipath-0.15.4/pypath/inputs/kea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/kegg.py` & `pypath_omnipath-0.15.4/pypath/inputs/kegg.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/kegg_api.py` & `pypath_omnipath-0.15.4/pypath/inputs/kegg_api.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/kinasedotcom.py` & `pypath_omnipath-0.15.4/pypath/inputs/kinasedotcom.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/kirouac2010.py` & `pypath_omnipath-0.15.4/pypath/inputs/kirouac2010.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/lambert2018.py` & `pypath_omnipath-0.15.4/pypath/inputs/lambert2018.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/laudanna.py` & `pypath_omnipath-0.15.4/pypath/inputs/laudanna.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/li2012.py` & `pypath_omnipath-0.15.4/pypath/inputs/li2012.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/lincs.py` & `pypath_omnipath-0.15.4/pypath/inputs/lincs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/lmpid.py` & `pypath_omnipath-0.15.4/pypath/inputs/lmpid.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     """
 
     result = []
 
     url = urls.urls['lmpid']['url']
     c = curl.Curl(url, silent = False, large = False)
 
-    soup = bs4.BeautifulSoup(c.result, 'html.parser')
+    soup = bs4.BeautifulSoup(c.result, features = 'xml')
     uniprots = uniprot_input.get_db(organism = organism, swissprot = None)
     prg = progress.Progress(
         len(soup.find_all('record')),
         'Processing data from LMPID',
         21
     )
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/lncdisease.py` & `pypath_omnipath-0.15.4/pypath/inputs/lncdisease.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/lncrnadb.py` & `pypath_omnipath-0.15.4/pypath/inputs/lncrnadb.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     c = curl.Curl(
         url,
         silent = False,
         large = True,
         encoding = 'utf-8',
     )
 
-    b = bs4.BeautifulSoup(c.fileobj, 'lxml')
+    b = bs4.BeautifulSoup(c.fileobj, features = 'xml')
 
     result = []
 
     for res in b.findAll('results'):
 
         lncrna = res.find('nomenclature').find('name').text
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/locate.py` & `pypath_omnipath-0.15.4/pypath/inputs/locate.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/lrdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/lrdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/macrophage.py` & `pypath_omnipath-0.15.4/pypath/inputs/macrophage.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/main.py` & `pypath_omnipath-0.15.4/pypath/inputs/main.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/matrisome.py` & `pypath_omnipath-0.15.4/pypath/inputs/matrisome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/matrixdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/matrixdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mcam.py` & `pypath_omnipath-0.15.4/pypath/inputs/mcam.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/membranome.py` & `pypath_omnipath-0.15.4/pypath/inputs/membranome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mimp.py` & `pypath_omnipath-0.15.4/pypath/inputs/mimp.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mir2disease.py` & `pypath_omnipath-0.15.4/pypath/inputs/mir2disease.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mirbase.py` & `pypath_omnipath-0.15.4/pypath/inputs/mirbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mirdeathdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/mirdeathdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mirecords.py` & `pypath_omnipath-0.15.4/pypath/inputs/mirecords.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mirtarbase.py` & `pypath_omnipath-0.15.4/pypath/inputs/mirtarbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mitab.py` & `pypath_omnipath-0.15.4/pypath/inputs/mitab.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/mppi.py` & `pypath_omnipath-0.15.4/pypath/inputs/mppi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/msigdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/msigdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ncrdeathdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/ncrdeathdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/negatome.py` & `pypath_omnipath-0.15.4/pypath/inputs/negatome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/netbiol.py` & `pypath_omnipath-0.15.4/pypath/inputs/netbiol.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/netpath.py` & `pypath_omnipath-0.15.4/pypath/inputs/netpath.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/oma.py` & `pypath_omnipath-0.15.4/pypath/inputs/oma.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ontology.py` & `pypath_omnipath-0.15.4/pypath/inputs/ontology.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/opm.py` & `pypath_omnipath-0.15.4/pypath/inputs/opm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/oreganno.py` & `pypath_omnipath-0.15.4/pypath/inputs/oreganno.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/panglaodb.py` & `pypath_omnipath-0.15.4/pypath/inputs/panglaodb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pathophenodb.py` & `pypath_omnipath-0.15.4/pypath/inputs/pathophenodb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pathwaycommons.py` & `pypath_omnipath-0.15.4/pypath/inputs/pathwaycommons.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pazar.py` & `pypath_omnipath-0.15.4/pypath/inputs/pazar.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/pdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pdzbase.py` & `pypath_omnipath-0.15.4/pypath/inputs/pdzbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pepcyber.py` & `pypath_omnipath-0.15.4/pypath/inputs/pepcyber.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pfam.py` & `pypath_omnipath-0.15.4/pypath/inputs/pfam.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pharos.py` & `pypath_omnipath-0.15.4/pypath/inputs/pharos.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/phobius.py` & `pypath_omnipath-0.15.4/pypath/inputs/phobius.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/phosphatome.py` & `pypath_omnipath-0.15.4/pypath/inputs/phosphatome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/phosphoelm.py` & `pypath_omnipath-0.15.4/pypath/inputs/phosphoelm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/phosphonetworks.py` & `pypath_omnipath-0.15.4/pypath/inputs/phosphonetworks.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/phosphopoint.py` & `pypath_omnipath-0.15.4/pypath/inputs/phosphopoint.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/phosphosite.py` & `pypath_omnipath-0.15.4/pypath/inputs/phosphosite.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pisa.py` & `pypath_omnipath-0.15.4/pypath/inputs/pisa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pro.py` & `pypath_omnipath-0.15.4/pypath/inputs/pro.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/progeny.py` & `pypath_omnipath-0.15.4/pypath/inputs/progeny.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/proteinatlas.py` & `pypath_omnipath-0.15.4/pypath/inputs/proteinatlas.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/proteins.py` & `pypath_omnipath-0.15.4/pypath/inputs/proteins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/protmapper.py` & `pypath_omnipath-0.15.4/pypath/inputs/protmapper.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pubchem.py` & `pypath_omnipath-0.15.4/pypath/inputs/pubchem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/pubmed.py` & `pypath_omnipath-0.15.4/pypath/inputs/pubmed.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ramilowski2015.py` & `pypath_omnipath-0.15.4/pypath/inputs/ramilowski2015.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/ramp.py` & `pypath_omnipath-0.15.4/pypath/inputs/ramp.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/rdata.py` & `pypath_omnipath-0.15.4/pypath/inputs/rdata.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/reaction.py` & `pypath_omnipath-0.15.4/pypath/inputs/reaction.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/scconnect.py` & `pypath_omnipath-0.15.4/pypath/inputs/scconnect.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import pypath.utils.mapping as mapping
 import pypath.utils.taxonomy as taxonomy
 import pypath.internals.intera as intera
 import pypath.share.curl as curl
 import pypath.resources.urls as urls
 import pypath.share.common as common
 import pypath.share.session as session
+import pypath.share.constants as constants
 import pypath.core.entity as entity
 
 _logger = session.Logger(name = 'scconnect_input')
 _log = _logger._log
 
 
 def scconnect_annotations(organism = 9606):
@@ -170,14 +171,16 @@
     """
 
 
     def process_partner(rec, partner):
 
         organisms = [
             taxonomy.ensure_ncbi_tax_id(org)
+                if org not in {'', 'None', 'Unknown'} else
+            constants.NOT_ORGANISM_SPECIFIC
             for org in rec['%s_species' % partner].split('|')
         ]
         id_field = (
             'target_uniprot'
                 if partner == 'target' else
             'ligand_gene_symbol'
         )
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/science.py` & `pypath_omnipath-0.15.4/pypath/inputs/science.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/signalink.py` & `pypath_omnipath-0.15.4/pypath/inputs/signalink.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/signor.py` & `pypath_omnipath-0.15.4/pypath/inputs/signor.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/spike.py` & `pypath_omnipath-0.15.4/pypath/inputs/spike.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/stitch.py` & `pypath_omnipath-0.15.4/pypath/inputs/stitch.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/string.py` & `pypath_omnipath-0.15.4/pypath/inputs/string.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/surfaceome.py` & `pypath_omnipath-0.15.4/pypath/inputs/surfaceome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/switches_elm.py` & `pypath_omnipath-0.15.4/pypath/inputs/switches_elm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/talklr.py` & `pypath_omnipath-0.15.4/pypath/inputs/talklr.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/tcdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/tcdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/tfcensus.py` & `pypath_omnipath-0.15.4/pypath/inputs/tfcensus.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/threedcomplex.py` & `pypath_omnipath-0.15.4/pypath/inputs/threedcomplex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/threedid.py` & `pypath_omnipath-0.15.4/pypath/inputs/threedid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/topdb.py` & `pypath_omnipath-0.15.4/pypath/inputs/topdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/transmir.py` & `pypath_omnipath-0.15.4/pypath/inputs/transmir.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/trip.py` & `pypath_omnipath-0.15.4/pypath/inputs/trip.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/unichem.py` & `pypath_omnipath-0.15.4/pypath/inputs/unichem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/uniprot.py` & `pypath_omnipath-0.15.4/pypath/inputs/uniprot.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,19 +66,22 @@
 
 def _all_uniprots(organism = 9606, swissprot = None):
 
     swissprot = _swissprot_param(swissprot)
     rev = '' if swissprot is None else ' AND reviewed: %s' % swissprot
     url = urls.urls['uniprot_basic']['url']
     get = {
-        'query': 'organism:%s%s' % (str(organism), rev),
-        'format': 'tab',
-        'columns': 'id',
+        'query': 'organism_id:%s%s' % (str(organism), rev),
+        'format': 'tsv',
+        'fields': 'accession',
     }
 
+    if organism == '*':
+        get['query'] = rev.strip(' AND ')
+
     c = curl.Curl(url, get = get, silent = False, slow = True)
     data = c.result
 
     return {
         l.strip() for l in data.split('\n')[1:] if l.strip()
     }
 
@@ -96,53 +99,53 @@
 def all_trembls(organism = 9606):
 
     return get_db(organism = organism, swissprot = False)
 
 
 def init_db(organism = 9606, swissprot = None):
 
-    swissprot = _swissprot_param(swissprot)
+    _swissprot = _swissprot_param(swissprot)
     _logger._log(
         'Loading list of all UniProt IDs for '
         'organism `%u` (only SwissProt: %s).' % (
             organism,
             str(swissprot),
         )
     )
 
-    key = (organism, swissprot)
+    key = (organism, _swissprot)
 
     globals()['db'][key] = _all_uniprots(
         organism = organism,
         swissprot = swissprot,
     )
     globals()['_last_used'][key] = time.time()
 
 
 def get_db(organism = 9606, swissprot = None):
 
-    swissprot = _swissprot_param(swissprot)
-    key = (organism, swissprot)
+    _swissprot = _swissprot_param(swissprot)
+    key = (organism, _swissprot)
 
     if key not in globals()['db']:
 
         init_db(organism = organism, swissprot = swissprot)
 
     globals()['_last_used'][key] = time.time()
 
     return globals()['db'][key]
 
 
 def _swissprot_param(swissprot):
 
     return (
-        'yes'
-            if swissprot in {'yes', 'YES', True} else
-        'no'
-            if swissprot in {'no', 'NO', False} else
+        'true'
+            if swissprot in {'true', 'True', 'yes', 'YES', True} else
+        'false'
+            if swissprot in {'false', 'False', 'no', 'NO', False} else
         None
     )
 
 
 def valid_uniprot(name):
     """
     Checks if ``name`` fits the format requirements for UniProt accession
@@ -483,83 +486,86 @@
             )
         ):
 
         yield line
 
 
 _uniprot_fields = {
-    'function': 'comment(FUNCTION)',
-    'activity_regulation': 'comment(ACTIVITY REGULATION)',
-    'tissue_specificity': 'comment(TISSUE SPECIFICITY)',
-    'developmental_stage': 'comment(DEVELOPMENTAL STAGE)',
-    'induction': 'comment(INDUCTION)',
-    'intramembrane': 'feature(INTRAMEMBRANE)',
-    'signal_peptide': 'feature(SIGNAL)',
-    'subcellular_location': 'comment(SUBCELLULAR LOCATION)',
-    'transmembrane': 'feature(TRANSMEMBRANE)',
-    'comment': 'comment(MISCELLANEOUS)',
-    'topological_domain': 'feature(TOPOLOGICAL DOMAIN)',
-    'family': 'families',
-    'interactor': 'interactor',
-    'keywords': 'keywords',
+    'function': 'cc_function',
+    'activity_regulation': 'cc_activity_regulation',
+    'tissue_specificity': 'cc_tissue_specificity',
+    'developmental_stage': 'cc_developmental_stage',
+    'induction': 'cc_induction',
+    'intramembrane': 'ft_intramem',
+    'signal_peptide': 'ft_signal',
+    'subcellular_location': 'cc_subcellular_location',
+    'transmembrane': 'ft_transmem',
+    'comment': 'cc_miscellaneous',
+    'topological_domain': 'ft_topo_dom',
+    'family': 'protein_families',
+    'interactor': 'cc_interaction',
+    'keywords': 'keyword',
 }
 
 
 def uniprot_data(
         field: str | Iterable[str],
         organism: str | int = 9606,
         reviewed: bool = True,
     ) -> dict[str, str] | dict[str, dict[str, str]]:
     """
-    Basic client for the legacy, plain UniProt API.
+    Basic client for the main UniProt API.
 
     Retrieves a field from UniProt for all proteins of one organism, by
     default only the reviewed (SwissProt) proteins.
     For the available fields refer to the ``_uniprot_fields`` attribute of
     this module or the UniProt website:
-    https://legacy.uniprot.org/help/uniprotkb_column_names
+    https://www.uniprot.org/help/return_fields
 
     Args
         field:
             One or more UniProt field name. See details.
         organism:
             Organism name or identifier, e.g. "human", or "Homo sapiens",
             or 9606.
         reviewed:
             Restrict the query to SwissProt (True), to TrEMBL (False), or
             cover both (None).
 
     Return
-        A dictionary for each ke
+        A dictionary for each key
     """
 
     rev = (
-        ' AND reviewed: yes'
+        ' AND reviewed: true'
             if reviewed == True or reviewed == 'yes' else
-        ' AND reviewed: no'
+        ' AND reviewed: false'
         if reviewed == False or reviewed == 'no' else
         ''
     )
 
 
     if organism != '*':
 
         organism = taxonomy.ensure_ncbi_tax_id(organism)
 
     field = common.to_list(field)
-    field_qs = ','.join(['id'] + [_uniprot_fields.get(f, f) for f in field])
+    field_qs = ','.join(['accession'] + [_uniprot_fields.get(f, f) for f in field])
 
     url = urls.urls['uniprot_basic']['url']
     get = {
-        'query': 'organism:%s%s' % (str(organism), rev),
-        'format': 'tab',
-        'columns': field_qs,
-        'compress': 'yes',
+        'query': 'organism_id:%s%s' % (str(organism), rev),
+        'format': 'tsv',
+        'fields': field_qs,
+        'compressed': 'true',
     }
 
+    if organism == '*':
+        get['query'] = rev.strip(' AND ')
+
     c = curl.Curl(url, get = get, silent = False, large = True, compr = 'gz')
     _ = next(c.result)
 
 
     _id, *variables = zip(*(
         line.strip('\n\r').split('\t')
         for line in c.result if line.strip('\n\r')
@@ -1265,22 +1271,22 @@
 
     result = {}
 
     for line in c.result:
 
         line = line.split('\t')
 
-        if line[0].isdigit() and len(line) > 3:
+        if line[0].isdigit() and len(line) > 2:
 
             taxid = int(line[0])
 
             result[taxid] = Taxon(
                 ncbi_id = taxid,
                 latin = line[2],
-                english = line[3],
+                english = line[1] or None,
             )
 
     return result
 
 
 def uniprot_ncbi_taxids_2():
```

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/wang.py` & `pypath_omnipath-0.15.4/pypath/inputs/wang.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/wojtowicz2020.py` & `pypath_omnipath-0.15.4/pypath/inputs/wojtowicz2020.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/inputs/zhong2015.py` & `pypath_omnipath-0.15.4/pypath/inputs/zhong2015.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/internals/annot_formats.py` & `pypath_omnipath-0.15.4/pypath/internals/annot_formats.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/internals/input_formats.py` & `pypath_omnipath-0.15.4/pypath/internals/input_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,44 +40,46 @@
     'ProMapping',
     'ArrayMapping',
     'BiomartMapping',
 ]
 
 
 AC_QUERY = {
-    'genesymbol': ('genes', 'PREFERRED'),
-    'genesymbol-syn': ('genes', 'ALTERNATIVE'),
-    'hgnc': ('database', 'HGNC'),
-    'embl': ('database', 'embl'),
-    'entrez': ('database', 'geneid'),
-    'refseqp': ('database', 'refseq'),
-    'enst': ('database', 'ensembl'),
-    'uniprot-entry': ('entry name', None),
-    'protein-name': ('protein names', None),
-    'ec': ('ec', None),
+    'genesymbol': 'gene_primary',
+    'genesymbol-syn': 'gene_synonym',
+    'hgnc': 'xref_hgnc',
+    'embl': 'xref_embl',
+    'entrez': 'xref_geneid',
+    'geneid': 'xref_geneid',
+    'refseqp': 'xref_refseq',
+    'enst': 'xref_ensembl',
+    'uniprot-entry': 'id',
+    'protein-name': 'protein_name',
+    'ec': 'ec',
 }
 
 AC_MAPPING = {
-    'uniprot': 'ACC',
-    'uniprot_id': 'ID',
-    'embl': 'EMBL',
-    'embl_id': 'EMBL_ID',
+    'uniprot': 'UniProtKB',
+    'uniprot-entry': 'UniProtKB',
+    'embl': 'EMBL-GeneBank-DDBJ',
+    'embl_id': 'EMBL-GeneBank-DDBJ_CDS',
     'pir': 'PIR',
-    'entrez': 'P_ENTREZGENEID',
-    'gi': 'P_GI',
-    'refseqp': 'P_REFSEQ_AC',
-    'refseqn': 'REFSEQ_NT_ID',
-    'ensembl': 'ENSEMBL_ID',
-    'ensp': 'ENSEMBL_PRO_ID',
-    'enst': 'ENSEMBL_TRS_ID',
-    'ensg': 'ENSEMBLGENOME_ID',
-    'ensgp': 'ENSEMBLGENOME_PRO_ID',
-    'ensgt': 'ENSEMBLGENOME_TRS_ID',
-    'hgnc': 'HGNC_ID',
-    'ensp_string': 'STRING_ID',
+    'entrez': 'GeneID',
+    'gi': 'GI_number',
+    'refseqp': 'RefSeq_Protein',
+    'refseqn': 'RefSeq_Nucleotide',
+    'ensembl': 'Ensembl',
+    'ensp': 'Ensembl_Protein',
+    'enst': 'Ensembl_Transcript',
+    'ensg': 'Ensembl',
+    'ensgp': 'Ensembl_Genomes_Protein',
+    'ensgt': 'Ensembl_Genomes_Transcript',
+    'hgnc': 'HGNC',
+    'ensp_string': 'STRING',
+    'genesymbol': 'Gene_Name',
 }
 
 BIOMART_MAPPING = {
     'hgnc_symbol': 'hgnc_symbol',
     'rnacentral': 'rnacentral',
     'hgnc_trans_name': 'hgnc_trans_name',
     'wikigene_name': 'wikigene_name',
@@ -174,22 +176,24 @@
             self,
             type_,
             id_type_a,
             id_type_b,
             ncbi_tax_id = None,
             resource_id_type_a = None,
             resource_id_type_b = None,
+            input_method = None,
         ):
 
         self.type = type_
         self.id_type_a = id_type_a
         self.id_type_b = id_type_b
         self.resource_id_type_a = resource_id_type_a
         self.resource_id_type_b = resource_id_type_b
         self.ncbi_tax_id = ncbi_tax_id or settings.get('default_organism')
+        self.input_method = input_method
 
 
     def _resource_id_type(self, side):
 
         return self.resource_id_type(
             getattr(self, 'id_type_%s' % side),
             override = getattr(self, 'resource_id_type_%s' % side),
@@ -220,14 +224,24 @@
             self.id_type_a == other or
             self.id_type_b == other or
             self._resource_id_type_a == other or
             self._resource_id_type_b == other
         )
 
 
+    def swap_sides(self):
+
+        self.id_type_a, self.id_type_b = self.id_type_b, self.id_type_a
+        self.resource_id_type_a, self.resource_id_type_b = (
+            self.resource_id_type_b,
+            self.resource_id_type_a,
+        )
+
+
+
 class FileMapping(MappingInput):
 
     def __init__(
             self,
             id_type_a,
             id_type_b,
             input_,
@@ -266,22 +280,22 @@
             other_organism.input_args['organism'] = ncbi_tax_id
 
         return other_organism
 
 
 class UniprotMapping(MappingInput):
 
-    _resource_id_type_b = 'id'
+    _resource_id_type_b = 'accession'
 
     def __init__(
             self,
             id_type_a,
             id_type_b = 'uniprot',
             ncbi_tax_id = 9606,
-            swissprot = 'yes',
+            swissprot = 'true',
         ):
         """
         Defines an ID conversion table to retrieve from UniProt.
 
         id_type : str
             Type of accession numbers you would like to translate.
         target_id_type : str
@@ -342,16 +356,15 @@
         list None is returned.
 
         Returns
             (str): The ID type label used by UniProt; None if the input
                 label is not known.
         """
 
-        id_type = AC_QUERY.get(id_type, (None, None))
-        id_type = '%s(%s)' % id_type if id_type[1] else id_type[0]
+        id_type = AC_QUERY.get(id_type, id_type)
 
         return id_type
 
 
 class UniprotListMapping(MappingInput):
     """
     Provides parameters for downloading mapping table from UniProt
@@ -368,14 +381,24 @@
     :arg str uniprot_id_type_b:
         Same as above just for the other ID type.
     :arg bool swissprot:
         DOwnload data only for SwissProt IDs.
     """
 
     _resource_id_types = AC_MAPPING
+    _from_uniprot = {
+        'uniprot': 'UniProtKB_AC-ID',
+        'swissprot': 'UniProtKB_AC-ID',
+        'trembl': 'UniProtKB_AC-ID',
+    }
+    _to_uniprot = {
+        'uniprot': 'UniProtKB',
+        'swissprot': 'UniProtKB-Swiss-Prot',
+        'trembl': 'UniProtKB',
+    }
 
     def __init__(
             self,
             id_type_a,
             id_type_b,
             uniprot_id_type_a = None,
             uniprot_id_type_b = None,
@@ -389,30 +412,74 @@
             id_type_a = id_type_a,
             id_type_b = id_type_b,
             ncbi_tax_id = ncbi_tax_id,
             resource_id_type_a = uniprot_id_type_a,
             resource_id_type_b = uniprot_id_type_b,
         )
 
-        self.swissprot = swissprot
+        self._set_swissprot(swissprot)
         self.ac_mapping = AC_MAPPING
-
-        self.uniprot_id_type_a = self._resource_id_type_a
-        self.uniprot_id_type_b = self._resource_id_type_b
-
+        self._update_uniprot_types()
         self.entity_type = 'protein'
 
 
     def set_organism(self, ncbi_tax_id):
 
         other_organism = copy.deepcopy(self)
         other_organism.ncbi_tax_id = ncbi_tax_id
         return other_organism
 
 
+    def swap_sides(self):
+
+        MappingInput.swap_sides(self)
+        self._update_uniprot_types()
+
+
+    def _update_uniprot_types(self):
+
+        self.uniprot_id_type_a = self._resource_id_type_a
+        self.uniprot_id_type_b = self._resource_id_type_b
+
+
+    def _resource_id_type(self, side: str) -> str:
+
+        uniprot_id_types = {
+            'a': self._from_uniprot,
+            'b': self._to_uniprot,
+        }.get(side)
+
+        id_type = getattr(self, f'id_type_{side}')
+
+        return uniprot_id_types.get(
+            id_type,
+            self._resource_id_types.get(id_type, id_type)
+        )
+
+
+    def _set_swissprot(self, swissprot: bool | None) -> None:
+
+        values = {'swissprot': True, 'trembl': False, 'uniprot': True}
+
+        if swissprot is None:
+
+            swissprot = values.get(
+                self.id_type_a,
+                values.get(self.id_type_b, swissprot)
+            )
+
+        self.swissprot = swissprot
+
+
+    @classmethod
+    def _uniprotkb_id_type(cls, id_type: str) -> bool:
+
+        return id_type in cls._from_uniprot
+
+
 class ProMapping(MappingInput):
     """
     Provides parameters for mapping table from the Protein Ontology
     Consortium.
 
     :arg str id_type_a:
         Custom name for one of the ID types.
@@ -575,14 +642,15 @@
 
         MappingInput.__init__(
             self,
             type_ = 'hmdb',
             id_type_a = id_type_a,
             id_type_b = id_type_b,
             ncbi_tax_id = constants.NOT_ORGANISM_SPECIFIC,
+            input_method = 'hmdb.metabolites_mapping',
         )
 
 
 class ArrayMapping(MappingInput):
     """
     Provides parameters for microarray probe mapping tables.
 
@@ -714,14 +782,15 @@
             huge = False,
             resource = None,
             unique_fields = None,
             expand_complexes = None,
             data_model = None,
             allow_loops = None,
             only_default_organism = False,
+            dataset = None,
         ):
         """
         :param str mark_source:
             Creates a boolean vertex attribute and sets it True for the
             source vertex of directed interactions from this particular
             resource.
         :param str mark_target:
@@ -758,14 +827,15 @@
         self.mark_source = mark_source
         self.mark_target = mark_target
         self.unique_fields = unique_fields or set()
         self.expand_complexes = expand_complexes
         self.data_model = data_model
         self.allow_loops = allow_loops
         self.only_default_organism = only_default_organism
+        self.dataset = dataset
 
 
     def _field(self, value, cls):
 
         return value if isinstance(value, cls) else cls(compact = value)
```

### Comparing `pypath_omnipath-0.14.48/pypath/internals/intera.py` & `pypath_omnipath-0.15.4/pypath/internals/intera.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/internals/license.py` & `pypath_omnipath-0.15.4/pypath/internals/license.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/internals/maps.py` & `pypath_omnipath-0.15.4/pypath/internals/maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 
 uniprot = {
     ('embl', 'uniprot'):
         input_formats.UniprotMapping(
             id_type_a = 'embl',
         ),
-    ('genesymbol', 'uniprot'): 
+    ('genesymbol', 'uniprot'):
         input_formats.UniprotMapping(
             id_type_a = 'genesymbol',
         ),
     ('genesymbol-syn', 'uniprot'):
         input_formats.UniprotMapping(
             id_type_a = 'genesymbol-syn'
         ),
@@ -236,15 +236,15 @@
             header = 0,
             ncbi_tax_id = 0,
         ),
     ('genesymbol', 'trembl'):
         input_formats.UniprotMapping(
             id_type_a = 'genesymbol',
             id_type_b = 'trembl',
-            swissprot = 'no',
+            swissprot = 'false',
         ),
     ('genesymbol', 'swissprot'):
         input_formats.UniprotMapping(
             id_type_a = 'genesymbol',
             id_type_b = 'swissprot',
         ),
     ('genesymbol-syn', 'swissprot'):
```

### Comparing `pypath_omnipath-0.14.48/pypath/internals/refs.py` & `pypath_omnipath-0.15.4/pypath/internals/refs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/internals/resource.py` & `pypath_omnipath-0.15.4/pypath/internals/resource.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,22 +26,23 @@
 
 """
 Generic objects for representing resources.
 """
 
 from future.utils import iteritems
 
-from typing import TYPE_CHECKING
+from typing import Iterable, Mapping, TYPE_CHECKING
 
 if TYPE_CHECKING:
 
     import pypath.internals.license as License
 
 import os
 import collections
+import copy
 
 try:
     import cPickle as pickle
 except:
     import pickle
 
 
@@ -191,25 +192,28 @@
 
 
     def __init__(
             self,
             name,
             data_type,
             evidence_types = None,
+            dataset = None,
             **kwargs
         ):
 
         self.name = name
         self.data_type = data_type
         self.evidence_types = evidence_types or set()
 
         for attr, value in iteritems(kwargs):
 
             setattr(self, attr, value)
 
+        self.dataset = dataset
+
 
     def __eq__(self, other):
 
         return (
             self.name == other.name and self.data_type == other.data_type
                 if isinstance(other, self.__class__) else
             self.name == other
@@ -217,14 +221,34 @@
 
 
     def __str__(self):
 
         return self.name
 
 
+    @property
+    def dataset(self):
+
+        return self._dataset
+
+
+    @dataset.setter
+    def dataset(self, dataset):
+
+        self._dataset = dataset
+
+        networkinput = getattr(self, 'networkinput', None)
+
+        if hasattr(self, 'networkinput'):
+
+            netinput_new = copy.deepcopy(self.networkinput)
+            netinput_new.dataset = dataset
+            self.networkinput = netinput_new
+
+
 class NetworkResourceKey(
         collections.namedtuple(
             'NetworkResourceKeyBase',
             [
                 'name',
                 'data_type',
                 'interaction_type',
@@ -272,25 +296,31 @@
     def __init__(
             self,
             name,
             interaction_type = 'PPI',
             data_model = None,
             evidence_types = None,
             via = None,
+            dataset = None,
             **kwargs
         ):
 
+        if not dataset and 'networkinput' in kwargs:
+
+            dataset = kwargs['networkinput'].dataset
+
         ResourceAttributes.__init__(
             self,
             name = name,
             data_type = 'network',
             interaction_type = interaction_type,
             evidence_types = evidence_types,
             data_model = data_model,
             via = via,
+            dataset = dataset,
             **kwargs
         )
 
 
     def __hash__(self):
 
         return hash(self.key)
@@ -342,14 +372,178 @@
 
     @property
     def license(self) -> license.License | None:
 
         return getattr(self, 'resource_attrs', None).get('license')
 
 
+class NetworkDataset(collections.abc.MutableMapping):
+
+
+    def __init__(
+            self,
+            name: str,
+            resources: dict | list | None = None,
+        ):
+        """
+        A set of network resources.
+
+        Formerly the network datasets were represented by dicts. This is
+        only a thin wrapper around that solution to better organise metadata
+        of the datasets and resources within.
+        """
+
+        self._name = name
+        self._resources = {}
+        self.add(resources)
+
+
+    def __repr__(self):
+
+        it = ', '.join(self.interaction_types)
+
+        return f'<NetworkDataset: {self.name} ({len(self)} resources; {it})>'
+
+
+    def __iter__(self):
+
+        return (r for r in self._resources.values())
+
+
+    def __len__(self):
+
+        return len(self._resources)
+
+
+    @property
+    def interaction_types(self):
+
+        return sorted({r.interaction_type for r in self})
+
+
+    def __setitem__(self, key, value):
+
+        self.add(value, key)
+
+
+    def __getitem__(self, key):
+
+        return self._resources[key]
+
+
+    def __delitem__(self, key):
+
+        del self._resources[key]
+
+
+    def __contains__(self, key):
+
+        return (
+            key in self._resources or
+            any(r.name == key for r in self._resources.values())
+        )
+
+
+    def __eq__(self, other):
+
+        return (
+            self._name == other or
+            self._name == getattr(other, '_name', None)
+        )
+
+
+    def items(self):
+
+        return self._resources.items()
+
+
+    def values(self):
+
+        return self._resources.values()
+
+
+    def keys(self):
+
+        return self._resources.keys()
+
+
+    def add(self, value, key = None):
+
+        if isinstance(value, Mapping):
+
+            for label, resource in value.items():
+
+                self.add(resource, label)
+
+        elif isinstance(value, Iterable):
+
+            for resource in value:
+
+                self.add(resource)
+
+        elif isinstance(value, NetworkResource):
+
+            resource = copy.deepcopy(value)
+            resource.dataset = self.name
+            self._resources[key or resource.name] = resource
+
+
+    update = add
+
+
+    @property
+    def name(self):
+
+        return self._name
+
+
+    @name.setter
+    def name(self, name):
+
+        for resource in self.values():
+
+            resource.networkinput.dataset = name
+
+        self._name = name
+
+
+    def __copy__(self):
+
+        return self.__class__(
+            name = self.name,
+            resources = self._resources,
+        )
+
+
+    def rename(self, name: str):
+
+        new = self.__class__(name = name)
+        new.add(self)
+
+        return new
+
+
+    def remove(self, remove: str | set | None):
+
+        remove = common.to_set(remove)
+
+        self._resources = {
+            k: v for k, v in self.items()
+            if k not in remove and v.name not in remove
+        }
+
+
+    def without(self, exclude: str | set | None):
+
+        new = copy.copy(self)
+        new.remove(exclude)
+
+        return new
+
+
 EnzymeSubstrateResourceKey = collections.namedtuple(
     'EnzymeSubstrateResourceKey',
     [
         'name',
         'data_type',
         'via',
     ]
```

### Comparing `pypath_omnipath-0.14.48/pypath/legacy/db_categories.py` & `pypath_omnipath-0.15.4/pypath/legacy/db_categories.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/legacy/main.py` & `pypath_omnipath-0.15.4/pypath/legacy/main.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/__init__.py` & `pypath_omnipath-0.15.4/pypath/omnipath/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/app.py` & `pypath_omnipath-0.15.4/pypath/omnipath/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,32 +430,32 @@
 
 
     def get_args_mirna_mrna(self):
         """
         Returns the arguments for building the miRNA-mRNA network dataset.
         """
 
-        return {'resources': netres.mirna_target}
+        return {'resources': netres.mirnatarget}
 
 
     def get_args_lncrna_mrna(self):
         """
         Returns the arguments for building the lncRNA-mRNA network dataset.
         """
 
-        return {'resources': netres.lncrna_target}
+        return {'resources': netres.lncrna_mrna}
 
 
     def get_args_small_molecule(self):
         """
         Returns the arguments for building the small molecule-protein
         network dataset.
         """
 
-        return {'resources': netres.small_molecule_protein}
+        return {'resources': netres.small_molecule}
 
 
     def compile_tables(self):
         """
         Compiles the `summaries` table for all datasets. These tables contain
         various quantitative descriptions of the data contents.
         """
```

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/bel.py` & `pypath_omnipath-0.15.4/pypath/omnipath/bel.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/cellphonedb.py` & `pypath_omnipath-0.15.4/pypath/omnipath/cellphonedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/databases/__init__.py` & `pypath_omnipath-0.15.4/pypath/omnipath/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/databases/build.py` & `pypath_omnipath-0.15.4/pypath/omnipath/databases/build.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/databases/builtins.json` & `pypath_omnipath-0.15.4/pypath/omnipath/databases/builtins.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/databases/classes.json` & `pypath_omnipath-0.15.4/pypath/omnipath/databases/classes.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/databases/define.py` & `pypath_omnipath-0.15.4/pypath/omnipath/databases/define.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/export.py` & `pypath_omnipath-0.15.4/pypath/omnipath/export.py`

 * *Files 22% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         'consensus_direction': 'int8',
         'consensus_stimulation': 'int8',
         'consensus_inhibition': 'int8',
         'sources': 'category',
         'references': 'category',
         'curation_effort': 'int16',
         'extra_attrs': 'category',
+        'evidences': 'category',
         'entity_type_source': 'category',
         'entity_type_target': 'category',
     }
 
     def __init__(
             self,
             network = None,
@@ -788,154 +789,80 @@
         )
 
         self.df.to_csv(outfile, sep = '\t', index = False)
 
 
     def webservice_interactions_df(self):
 
-        sources_omnipath = set(netres.omnipath.values())
-        sources_extra_directions = set(netres.extra_directions.values())
-        sources_kinase_extra = set(netres.ptm_misc.values())
-        sources_ligrec_extra = set(netres.ligand_receptor.values())
-        sources_pathway_extra = set(netres.pathway_noref.values())
-        sources_mirna = set(netres.mirna_target.values())
-        sources_tf_target = set(netres.transcription_onebyone.values())
-        sources_dorothea = {'DoRothEA'}
-        sources_collectri = {'CollecTRI'}
+        datasets = (
+            'omnipath',
+            'kinaseextra',
+            'ligrecextra',
+            'pathwayextra',
+            'mirnatarget',
+            'dorothea',
+            'collectri',
+            'tf_target',
+            'lncrna_mrna',
+            'tf_mirna',
+            'small_molecule',
+        )
+
+        def get_dataset_callback(dataset: str) -> callable:
+
+            def has_dataset(e, d) -> bool:
+
+                return e.has_dataset(dataset, direction = d)
+
+            return has_dataset
+
+
+        dataset_args = {
+            dataset: get_dataset_callback(dataset)
+            for dataset in datasets
+        }
 
         self.make_df(
             unique_pairs = False,
             extra_node_attrs = {
                 'ncbi_tax_id': 'taxon',
                 'entity_type': 'entity_type',
             },
             extra_edge_attrs = {
-                'omnipath': lambda e, d: (
-                    (
-                        bool(
-                            e.get_resources(direction = d) &
-                            sources_omnipath
-                        ) or
-                        (
-                            bool(
-                                e.get_resources(direction = 'undirected') &
-                                sources_omnipath
-                            ) and
-                            bool(
-                                e.get_resources(direction = d) &
-                                sources_extra_directions
-                            )
+                **dataset_args,
+                **{
+                    'dorothea_curated': lambda e, d: (
+                        e._get_attr('DoRothEA', 'curated', d)
+                    ),
+                    'dorothea_chipseq': lambda e, d: (
+                        e._get_attr('DoRothEA', 'chipseq', d)
+                    ),
+                    'dorothea_tfbs': lambda e, d: (
+                        e._get_attr('DoRothEA', 'tfbs', d)
+                    ),
+                    'dorothea_coexp': lambda e, d: (
+                        e._get_attr('DoRothEA', 'coexp', d)
+                    ),
+                    'dorothea_level': lambda e, d: (
+                        ';'.join(e.dorothea_levels(d))
+                    ),
+                    'type': lambda e, d: (
+                        list(e.get_interaction_types(direction = d))[0]
+                    ),
+                    'curation_effort': lambda e, d: (
+                        e.count_curation_effort(direction = d) + (
+                            e.count_curation_effort(direction = 'undirected')
+                                if isinstance(d, tuple) else
+                            0
                         )
-                    ) and (
-                        'post_translational' in
-                        e.get_interaction_types(direction = d)
-                    )
-                ),
-                'kinaseextra': lambda e, d: (
-                    bool(
-                        e.get_resources(direction = d) &
-                        sources_kinase_extra
-                    ) and (
-                        'post_translational' in
-                        e.get_interaction_types(direction = d)
-                    )
-                ),
-                'ligrecextra': lambda e, d: (
-                    bool(
-                        e.get_resources(direction = d) &
-                        sources_ligrec_extra
-                    ) and (
-                        'post_translational' in
-                        e.get_interaction_types(direction = d)
-                    )
-                ),
-                'pathwayextra': lambda e, d: (
-                    bool(
-                        e.get_resources(direction = d) &
-                        sources_pathway_extra
-                    ) and (
-                        'post_translational' in
-                        e.get_interaction_types(direction = d)
-                    )
-                ),
-                'mirnatarget': lambda e, d: (
-                    bool(
-                        e.get_resources(direction = d) &
-                        sources_mirna
-                    ) and (
-                        'post_transcriptional' in
-                        e.get_interaction_types(direction = d)
-                    )
-                ),
-                'dorothea': lambda e, d: (
-                    bool(
-                        e.get_resource_names(
-                            direction = d,
-                            interaction_type = 'transcriptional'
-                        ) &
-                        sources_dorothea
-                    )
-                ),
-                'collectri': lambda e, d: (
-                    bool(
-                        e.get_resource_names(
-                            direction = d,
-                            interaction_type = 'transcriptional'
-                        ) &
-                        sources_collectri
-                    )
-                ),
-                'tf_target': lambda e, d: (
-                    bool(
-                        e.get_resources(
-                            direction = d,
-                            interaction_type = 'transcriptional'
-                        ) &
-                        sources_tf_target
-                    )
-                ),
-                'lncrna_mrna': lambda e, d: (
-                    'lncrna_post_transcriptional' in
-                    e.get_interaction_types(direction = d)
-                ),
-                'tf_mirna': lambda e, d: (
-                    'mirna_transcriptional' in
-                    e.get_interaction_types(direction = d)
-                ),
-                'small_molecule': lambda e, d: (
-                    'small_molecule_protein' in
-                    e.get_interaction_types(direction = d)
-                ),
-                'dorothea_curated': lambda e, d: (
-                    e._get_attr('DoRothEA', 'curated', d)
-                ),
-                'dorothea_chipseq': lambda e, d: (
-                    e._get_attr('DoRothEA', 'chipseq', d)
-                ),
-                'dorothea_tfbs': lambda e, d: (
-                    e._get_attr('DoRothEA', 'tfbs', d)
-                ),
-                'dorothea_coexp': lambda e, d: (
-                    e._get_attr('DoRothEA', 'coexp', d)
-                ),
-                'dorothea_level': lambda e, d: (
-                    ';'.join(e.dorothea_levels(d))
-                ),
-                'type': lambda e, d: (
-                    list(e.get_interaction_types(direction = d))[0]
-                ),
-                'curation_effort': lambda e, d: (
-                    e.count_curation_effort(direction = d) + (
-                        e.count_curation_effort(direction = 'undirected')
-                            if isinstance(d, tuple) else
-                        0
-                    )
-                ),
-                'extra_attrs': lambda e, d: e.serialize_attrs(d),
-            }
+                    ),
+                    'extra_attrs': lambda e, d: e.serialize_attrs(d),
+                    'evidences': lambda e, d: e.serialize_evidences(d),
+                },
+            },
         )
 
 
     def webservice_interactions_df_legacy(self):
 
         sources_omnipath = set(
             f.name for f in data_formats.omnipath.values()
```

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/legacy.py` & `pypath_omnipath-0.15.4/pypath/omnipath/legacy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/param.py` & `pypath_omnipath-0.15.4/pypath/omnipath/param.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/server/_html.py` & `pypath_omnipath-0.15.4/pypath/omnipath/server/_html.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/server/build.py` & `pypath_omnipath-0.15.4/pypath/omnipath/server/build.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/server/generate_about_page.py` & `pypath_omnipath-0.15.4/pypath/omnipath/server/generate_about_page.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/server/legacy.py` & `pypath_omnipath-0.15.4/pypath/omnipath/server/legacy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/omnipath/server/run.py` & `pypath_omnipath-0.15.4/pypath/omnipath/server/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,14 +697,16 @@
             },
             'sources':  None,
             'resources': None,
             'databases': None,
             'targets':  None,
             'partners': None,
             'genesymbols': constants.BOOLEAN_VALUES,
+            'evidences': None,
+            'extra_attrs': None,
             'fields': {
                 'entity_type',
                 'references',
                 'sources',
                 'tfregulons_level',
                 'tfregulons_curated',
                 'tfregulons_chipseq',
@@ -719,14 +721,15 @@
                 'ncbi_tax_id',
                 'databases',
                 'resources',
                 'organism',
                 'curation_effort',
                 'datasets',
                 'extra_attrs',
+                'evidences',
             },
             'tfregulons_levels':  {'A', 'B', 'C', 'D', 'E'},
             'tfregulons_methods': {
                 'curated',
                 'chipseq',
                 'coexp',
                 'tfbs',
@@ -1094,15 +1097,15 @@
         'references', 'sources', 'dorothea_level',
         'dorothea_curated', 'dorothea_chipseq',
         'dorothea_tfbs', 'dorothea_coexp',
         'tfregulons_level', 'tfregulons_curated',
         'tfregulons_chipseq', 'tfregulons_tfbs', 'tfregulons_coexp',
         'type', 'ncbi_tax_id', 'databases', 'organism',
         'curation_effort', 'resources', 'entity_type',
-        'datasets', 'extra_attrs',
+        'datasets', 'extra_attrs', 'evidences',
     }
     enzsub_fields = {
         'references', 'sources', 'databases',
         'isoforms', 'organism', 'ncbi_tax_id',
         'curation_effort', 'resources',
     }
     default_input_files = {
@@ -1135,14 +1138,15 @@
             'type': 'category',
             'ncbi_tax_id_source': 'int16',
             'ncbi_tax_id_target': 'int16',
             'entity_type_source': 'category',
             'entity_type_target': 'category',
             'curation_effort': 'int16',
             'extra_attrs': 'category',
+            'evidences': 'category',
         },
         annotations = {
             'uniprot': 'category',
             'genesymbol': 'category',
             'entity_type': 'category',
             'source': 'category',
             'label': 'category',
@@ -2066,49 +2070,55 @@
 
             # pandas is a disaster:
             tbl = tbl.loc[
                 tbl.source.astype('string') !=
                 tbl.target.astype('string')
             ]
 
-        if req.args[b'fields']:
+        req.args[b'fields'] = req.args[b'fields'] or [b'']
 
-            _fields = [
-                f for f in
-                req.args[b'fields'][0].decode('utf-8').split(',')
-                if f in self.interaction_fields
-            ]
+        _fields = [
+            f for f in
+            req.args[b'fields'][0].decode('utf-8').split(',')
+            if f in self.interaction_fields
+        ]
 
-            for f in _fields:
+        for f in (b'evidences', b'extra_attrs'):
 
-                if f == 'ncbi_tax_id' or f == 'organism':
+            if f in req.uri and f not in req.args[b'fields'][0]:
 
-                    hdr.append('ncbi_tax_id_source')
-                    hdr.append('ncbi_tax_id_target')
+                _fields.append(f.decode('utf-8'))
 
-                elif f == 'entity_type':
+        for f in _fields:
 
-                    hdr.append('entity_type_source')
-                    hdr.append('entity_type_target')
+            if f == 'ncbi_tax_id' or f == 'organism':
 
-                elif f in {'databases', 'resources'}:
+                hdr.append('ncbi_tax_id_source')
+                hdr.append('ncbi_tax_id_target')
 
-                    hdr.append('sources')
+            elif f == 'entity_type':
 
-                elif f == 'datasets':
+                hdr.append('entity_type_source')
+                hdr.append('entity_type_target')
 
-                    hdr.extend(
-                        set(tbl.columns) &
-                        self.args_reference['interactions']['datasets'] &
-                        args['datasets']
-                    )
+            elif f in {'databases', 'resources'}:
+
+                hdr.append('sources')
 
-                else:
+            elif f == 'datasets':
+
+                hdr.extend(
+                    set(tbl.columns) &
+                    self.args_reference['interactions']['datasets'] &
+                    args['datasets']
+                )
+
+            else:
 
-                    hdr.append(f)
+                hdr.append(f)
 
         license = self._get_license(req)
 
         tbl = self._filter_by_license_interactions(tbl, license)
 
         tbl = tbl.loc[:,hdr]
```

### Comparing `pypath_omnipath-0.14.48/pypath/reader/field.py` & `pypath_omnipath-0.15.4/pypath/reader/field.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/reader/network.py` & `pypath_omnipath-0.15.4/pypath/reader/network.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/resources/__init__.py` & `pypath_omnipath-0.15.4/pypath/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/resources/controller.py` & `pypath_omnipath-0.15.4/pypath/resources/controller.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/resources/data/resources.json` & `pypath_omnipath-0.15.4/pypath/resources/data/resources.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/resources/data_formats.py` & `pypath_omnipath-0.15.4/pypath/resources/data_formats.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'sif_rule': (2, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = False,
+        data_model = 'process_description',
     ),
 }
 
 pathwaycommons_all = input_formats.NetworkInput(
     name = 'PathwayCommons',
     separator = None,
     id_col_a = 0,
@@ -175,14 +176,15 @@
             'interacts-with',
             'controls-state-change-of',
             'in-complex-with',
             'controls-transport-of',
             'controls-phosphorylation-of',
         },
     },
+    data_model = 'activity_flow',
 )
 
 
 pathwaycommons_transcription_all = input_formats.NetworkInput(
     name = 'PathwayCommons',
     separator = None,
     id_col_a = 0,
@@ -208,14 +210,15 @@
     extra_node_attrs_b = {},
     must_have_references = False,
     input_args = {
         'types': {
             'controls-expression-of',
         },
     },
+    data_model = 'activity_flow',
 )
 
 
 def _pathwaycommons_single_resource(resource, transcription = False):
 
     dmodel_interaction = {'CORUM', 'IntAct', 'DIP', 'BioGRID', 'BIND', 'INOH'}
 
@@ -292,14 +295,15 @@
         ncbi_tax_id = 9606,
         input = 'reaction.pid_interactions',
         references = (3, ';'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'process_description',
     ),
     'acsn': input_formats.NetworkInput(
         name = 'ACSN',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -311,14 +315,15 @@
         ncbi_tax_id = 9606,
         input = 'acsn.acsn_interactions',
         references = (3, ';'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'process_description',
     ),
     'reactome': input_formats.NetworkInput(
         name = 'Reactome',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -332,14 +337,15 @@
         input = 'reaction.reactome_interactions',
         input_args = {'ask': False},
         references = (3, ';'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'process_description',
     ),
 }
 
 reaction_pc = {
     'acsn': input_formats.NetworkInput(
         name = 'ACSN',
         separator = None,
@@ -409,14 +415,15 @@
         input = 'acsn.acsn_interactions',
         header = False,
         extra_edge_attrs = {
             'effect': (2, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'process_description',
     ),
 }
 
 
 """
 Pathway databases included in OmniPath.
 These are manually curated, directed, and in most
@@ -439,14 +446,15 @@
         references = (2, ';'),
         header = False,
         extra_edge_attrs = {
             'method': (3, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'spike': input_formats.NetworkInput(
         name = 'SPIKE',
         separator = '\t',
         id_col_a = 1,
         id_col_b = 3,
         id_type_a = 'genesymbol',
@@ -460,14 +468,15 @@
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'effect': 7,
             'mechanism': 11,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'signalink3': input_formats.NetworkInput(
         name = 'SignaLink3',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -480,14 +489,15 @@
         references = 9,
         resource = 10,
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         positive_filters = [(2, True)], # only direct interactions
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'guide2pharma': input_formats.NetworkInput(
         name = 'Guide2Pharma',
         separator = None,
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'genesymbol',
@@ -498,14 +508,15 @@
         sign = (7, 1, -1),
         input = 'guide2pharma.guide2pharma_interactions',
         references = 11,
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {'g2p_ligand_location': 8},
         extra_node_attrs_b = {'g2p_target_type': 9},
+        data_model = 'ligand_receptor',
     ),
     'ca1': input_formats.NetworkInput(
         name = 'CA1',
         id_col_a = 1,
         id_col_b = 6,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -525,14 +536,15 @@
             'ca1_location': 4,
             'ca1_function': 3,
         },
         extra_node_attrs_b = {
             'ca1_location': 9,
             'ca1_function': 8,
         },
+        data_model = 'activity_flow',
     ),
     'arn': input_formats.NetworkInput(
         name = 'ARN',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -547,14 +559,15 @@
         extra_edge_attrs = {
             'effect': 4,
             'is_direct': 2,
             'is_directed': 3
         },
         extra_node_attrs_a = {'atg': 5},
         extra_node_attrs_b = {'atg': 6},
+        data_model = 'activity_flow',
     ),
     'nrf2': input_formats.NetworkInput(
         name = 'NRF2ome',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -569,14 +582,15 @@
         extra_edge_attrs = {
             'effect': 4,
             'is_direct': 2,
             'is_directed': 3
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'macrophage': input_formats.NetworkInput(
         name = 'Macrophage',
         separator = ';',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -590,14 +604,15 @@
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'type': (2, ','),
             'location': (4, ',')
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'death': input_formats.NetworkInput(
         name = 'DeathDomain',
         separator = '\t',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -610,14 +625,15 @@
         references = (3, ';'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'method': (2, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'pdz': input_formats.NetworkInput(
         name = 'PDZBase',
         separator = None,
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'uniprot',
@@ -632,14 +648,15 @@
         },
         input = 'pdzbase.pdzbase_interactions',
         references = 8,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'signor': input_formats.NetworkInput(
         name = 'SIGNOR',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -695,14 +712,15 @@
         references = (9, ';'),
         header = False,
         extra_edge_attrs = {
             'mechanism': (7, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'adhesome': input_formats.NetworkInput(
         name = 'Adhesome',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -714,14 +732,15 @@
         sign = (2, '+', '_'),
         input = 'adhesome.adhesome_interactions',
         references = 4,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'icellnet': input_formats.NetworkInput(
         name = 'ICELLNET',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -734,14 +753,15 @@
         input = 'icellnet.icellnet_interactions',
         references = 6,
         resource = 5,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'ligand_receptor',
     ),
     'celltalkdb': input_formats.NetworkInput(
         name = 'CellTalkDB',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -753,14 +773,15 @@
         sign = None,
         input = 'celltalkdb.celltalkdb_interactions',
         references = 2,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'ligand_receptor',
     ),
     'cellchatdb': input_formats.NetworkInput(
         name = 'CellChatDB',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -775,14 +796,15 @@
         references = 6,
         header = False,
         extra_edge_attrs = {
             'category': 7,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'ligand_receptor',
     ),
     'connectomedb': input_formats.NetworkInput(
         name = 'connectomeDB2020',
         separator = None,
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'genesymbol',
@@ -790,14 +812,15 @@
         entity_type_a = 'protein',
         entity_type_b = 'protein',
         ncbi_tax_id = 9606,
         is_directed = True,
         input = 'connectomedb.connectomedb_interactions',
         references = 3,
         header = False,
+        data_model = 'ligand_receptor',
     ),
     'talklr': input_formats.NetworkInput(
         name = 'talklr',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -809,14 +832,15 @@
         input = 'talklr.talklr_interactions',
         references = 2,
         resource = 3,
         header = False,
         extra_edge_attrs = {
             'putative': 4,
         },
+        data_model = 'ligand_receptor',
     ),
     'cellinker': input_formats.NetworkInput(
         name = 'Cellinker',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -828,14 +852,15 @@
         input = 'cellinker.cellinker_lr_interactions',
         references = (5, ';'),
         resource = (4, ';'),
         header = False,
         extra_edge_attrs = {
             'type': 6,
         },
+        data_model = 'ligand_receptor',
     ),
     'scconnect': input_formats.NetworkInput(
         name = 'scConnect',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -880,14 +905,15 @@
                 'Pore blocker',
                 'Voltage-dependent inhibition',
             ],
         ),
         input = 'scconnect.scconnect_interactions',
         references = (7, '|'),
         header = False,
+        data_model = 'ligand_receptor',
     ),
 }
 
 # synonym
 activity_flow = pathway
 
 """
@@ -915,14 +941,15 @@
         ],
         negative_filters = [
             (6, True), # transcriptional
         ],
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'wang': input_formats.NetworkInput(
         name = 'Wang',
         separator = None,
         id_col_a = 2,
         id_col_b = 3,
         id_type_a = 'entrez',
@@ -935,14 +962,15 @@
         input = 'wang.wang_interactions',
         references = False,
         must_have_references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'cui': input_formats.NetworkInput(
         name = 'Cui2007',
         separator = None,
         id_col_a = 2,
         id_col_b = 3,
         id_type_a = 'entrez',
@@ -955,14 +983,15 @@
         input = 'wang.cui_interactions',
         references = False,
         must_have_references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'kegg-medicus': input_formats.NetworkInput(
         name = 'KEGG-MEDICUS',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -981,14 +1010,15 @@
         ],
         negative_filters = [
             (5, ['missing', 'enzyme_enzyme']),
         ],
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'spike_lc': input_formats.NetworkInput(
         name = 'SPIKE_LC',
         separator = '\t',
         id_col_a = 1,
         id_col_b = 3,
         id_type_a = 'genesymbol',
@@ -1004,18 +1034,22 @@
             'effect': 7,
             'mechanism': 11,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = False,
         input_args = {'min_confidence': 99},
+        data_model = 'activity_flow',
     ),
 }
 
 
+# synonym
+pathwayextra = pathway_noref
+
 pathway_all = dict(copy.deepcopy(pathway), **copy.deepcopy(pathway_noref))
 
 
 pathway_bad = {
     'laudanna_effects': input_formats.NetworkInput(
         name = 'Laudanna-effects',
         separator = None,
@@ -1031,14 +1065,15 @@
         input = 'laudanna.laudanna_effects',
         references = False,
         must_have_references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'laudanna_directions': input_formats.NetworkInput(
         name = 'Laudanna-directions',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -1050,14 +1085,15 @@
         input = 'laudanna.laudanna_directions',
         references = False,
         must_have_references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
 }
 
 """
 Interaction databases included in OmniPath.
 These are subsets of the named databases, having
 only low throughput, manually curated, undirected
@@ -1078,14 +1114,15 @@
         ncbi_tax_id = 9606,
         input = 'biogrid.biogrid_interactions',
         references = (2, '|'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'ccmap': input_formats.NetworkInput(
         name = 'CancerCellMap',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -1095,14 +1132,15 @@
         sign = False,
         ncbi_tax_id = 9606,
         input = 'cancercellmap.ccmap_interactions',
         references = (3, ';'),
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'mppi': input_formats.NetworkInput(
         name = 'MPPI',
         separator = '|',
         id_col_a = 2,
         id_col_b = 6,
         id_type_a = 'uniprot',
@@ -1115,14 +1153,15 @@
         references = (0, ';'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'evidence': (1, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'dip': input_formats.NetworkInput(
         name = 'DIP',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -1136,14 +1175,15 @@
         extra_edge_attrs = {
             'method': (4, ';'),
             'type': (3, ';'),
             'id': 5,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'netpath': input_formats.NetworkInput(
         name = 'NetPath',
         separator = None,
         id_col_a = 1,
         id_col_b = 3,
         id_type_a = 'entrez',
@@ -1158,14 +1198,15 @@
         extra_edge_attrs = {
             'method': (5, ';'),
             'type': (6, ';'),
             'pathway': (7, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'innatedb': input_formats.NetworkInput(
         name = 'InnateDB',
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -1175,14 +1216,15 @@
         sign = False,
         input = 'innatedb.innatedb_interactions',
         references = (4, ':'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'intact': input_formats.NetworkInput(
         name = 'IntAct',
         separator = ',',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1195,14 +1237,15 @@
         references = 4,
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'method': 5,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'lit17': input_formats.NetworkInput(
         name = 'Lit-BM-17',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1216,14 +1259,15 @@
         input = 'huri.lit_bm_17_interactions',
         header = False,
         extra_edge_attrs = {
             'mentha_score': 3,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'alz': input_formats.NetworkInput(
         name = 'AlzPathway',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1234,14 +1278,15 @@
         sign = False,
         input = urls.urls['alzpathway']['url'],
         references = (8, ';'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'matrixdb': input_formats.NetworkInput(
         name = 'MatrixDB',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -1253,14 +1298,15 @@
         references = (2, '|'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'method': (3, '|'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
 }
 """
 PTM databases included in OmniPath.
 These supply large sets of directed interactions.
 """
 ptm = {
@@ -1279,14 +1325,15 @@
         references = (5, ';'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'evidence': (4, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'depod': input_formats.NetworkInput(
         name = 'DEPOD',
         separator = ';',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1297,14 +1344,15 @@
         sign = False,
         input = 'depod.depod_interactions',
         references = (2, '|'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'lmpid': input_formats.NetworkInput(
         name = 'LMPID',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1316,14 +1364,15 @@
         ncbi_tax_id = 9606,
         input = 'lmpid.lmpid_interactions',
         references = (2, ';'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'phelm': input_formats.NetworkInput(
         name = 'phosphoELM',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1340,14 +1389,15 @@
         },
         input = 'phosphoelm.phosphoelm_interactions',
         references = (2, ';'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'elm': input_formats.NetworkInput(
         name = 'ELM',
         separator = None,
         id_col_a = 2,
         id_col_b = 3,
         id_type_a = 'uniprot',
@@ -1362,14 +1412,15 @@
         },
         input = 'elm.elm_interactions',
         references = 12,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'domino': input_formats.NetworkInput(
         name = 'DOMINO',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1396,14 +1447,15 @@
         references = (5, ';'),
         header = False,
         extra_edge_attrs = {
             'method': (4, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'dbptm': input_formats.NetworkInput(
         name = 'dbPTM',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = ['genesymbol', 'uniprot'],
@@ -1416,14 +1468,15 @@
         input = 'dbptm.dbptm_interactions',
         references = (2, ';'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = True,
+        data_model = 'enzyme_substrate',
     ),
     'hprd_p': input_formats.NetworkInput(
         name = 'HPRD-phos',
         separator = None,
         id_col_a = 6,
         id_col_b = 3,
         id_type_a = 'genesymbol',
@@ -1437,14 +1490,15 @@
         references = (10, ','),
         header = False,
         extra_edge_attrs = {
             'mechanism': 8,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'kea': input_formats.NetworkInput(
         name = 'KEA',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1458,14 +1512,15 @@
         references = 4,
         resource = 5,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = True,
+        data_model = 'enzyme_substrate',
     ),
     'iptmnet': input_formats.NetworkInput(
         name = 'iPTMnet',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1478,14 +1533,15 @@
         input = 'iptmnet.iptmnet_interactions',
         references = 8,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = True,
+        data_model = 'enzyme_substrate',
     ),
 }
 
 # synonym
 enzyme_substrate = ptm
 
 """
@@ -1508,14 +1564,15 @@
         input = 'phosphosite.phosphosite_interactions_noref',
         references = False,
         extra_edge_attrs = {
             'evidence': (4, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'ppoint': input_formats.NetworkInput(
         name = 'PhosphoPoint',
         separator = ';',
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'genesymbol',
@@ -1529,14 +1586,15 @@
         references = False,
         sign = False,
         extra_edge_attrs = {
             'category': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'pnetworks': input_formats.NetworkInput(
         name = 'PhosphoNetworks',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -1548,14 +1606,15 @@
         ncbi_tax_id = 9606,
         input = 'phosphonetworks.phosphonetworks_interactions',
         references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'mimp': input_formats.NetworkInput(
         name = 'MIMP',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -1568,14 +1627,15 @@
         input = 'mimp.mimp_interactions',
         references = False,
         resource = 2,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'li2012': input_formats.NetworkInput(
         name = 'Li2012',
         separator = False,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -1589,14 +1649,15 @@
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'mechanism': 3,
             'route': 2,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'enzyme_substrate',
     ),
     'protmapper': input_formats.NetworkInput(
         name = 'ProtMapper',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1610,19 +1671,21 @@
         references = 3,
         resource = 2,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = False,
+        data_model = 'enzyme_substrate',
     ),
 }
 
 # synonym
 ptm_noref = ptm_misc
+kinaseextra = ptm_misc
 
 ptm_all = copy.deepcopy(ptm_misc)
 ptm_all.update(ptm)
 
 extra_directions = copy.deepcopy(ptm_misc)
 extra_directions.update(copy.deepcopy(pathway_noref))
 extra_directions['acsn'] = copy.deepcopy(reaction_pc['acsn'])
@@ -1647,14 +1710,15 @@
         sign = False,
         input = 'hippie.hippie_interactions',
         references = 4,
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'biogrid': input_formats.NetworkInput(
         name = 'BioGRID',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -1666,14 +1730,15 @@
         ncbi_tax_id = 9606,
         input = 'biogrid.biogrid_interactions',
         references = (2, '|'),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'hi2': input_formats.NetworkInput(
         name = 'HI-II',
         separator = None,
         id_col_a = 2,
         id_col_b = 3,
         id_type_a = 'genesymbol',
@@ -1687,14 +1752,15 @@
         references = False,
         header = False,
         extra_edge_attrs = {
             'numof_screens': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'lit13': input_formats.NetworkInput(
         name = 'Lit-BM-13',
         separator = None,
         id_col_a = 2,
         id_col_b = 3,
         id_type_a = 'genesymbol',
@@ -1706,14 +1772,15 @@
         ncbi_tax_id = 9606,
         input = 'huri.lit_bm_13_interactions',
         references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'huri': input_formats.NetworkInput(
         name = 'HuRI',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1727,14 +1794,15 @@
         references = False,
         header = True,
         extra_edge_attrs = {
             'score': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'hi_union': input_formats.NetworkInput(
         name = 'HI-union',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1748,14 +1816,15 @@
         references = False,
         header = True,
         extra_edge_attrs = {
             'score': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'yu2011': input_formats.NetworkInput(
         name = 'Yu2011',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1769,14 +1838,15 @@
         references = False,
         header = True,
         extra_edge_attrs = {
             'score': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'yang2016': input_formats.NetworkInput(
         name = 'Yang2016',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1790,14 +1860,15 @@
         references = False,
         header = True,
         extra_edge_attrs = {
             'score': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'cpdb': input_formats.NetworkInput(
         name = 'CPDB',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot-entry',
@@ -1809,14 +1880,15 @@
         ncbi_tax_id = 9606,
         input = 'cpdb.cpdb_interactions',
         references = (3, ','),
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
 }
 
 interaction_misc['acsn'] = copy.deepcopy(reaction_pc['acsn'])
 
 
 interaction_deprecated = {
@@ -1835,15 +1907,16 @@
         # note: obtain the file yourself, and replace
         # this location
         input = '/home/denes/Documents/pw/data/hi3-2.3.tsv',
         references = False,
         header = True,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
-        extra_node_attrs_b = {}
+        extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'hi3_local_2': input_formats.NetworkInput(
         name = 'Vidal HI-III',
         separator = None,
         id_col_a = 1,
         id_col_b = 3,
         id_type_a = 'genesymbol',
@@ -1858,14 +1931,15 @@
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = False,
         # note: obtain the file yourself, and replace
         # this location
         input_args = {'fname': '/home/denes/Documents/pw/data/hi3-2.3.tsv'},
+        data_model = 'interaction',
     ),
     'hi3': input_formats.NetworkInput(
         name = 'HI-III',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -1879,14 +1953,15 @@
         references = False,
         header = True,
         extra_edge_attrs = {
             'score': 5,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'hsn': input_formats.NetworkInput(
         name = 'HumanSignalingNetwork',
         separator = None,
         id_col_a = 2,
         id_col_b = 3,
         id_type_a = 'entrez',
@@ -1897,14 +1972,15 @@
         sign = (4, '+', '-'),
         input = 'wang.hsn_interactions',
         references = False,
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
 }
 
 
 interaction_htp = {
     'hprd': input_formats.NetworkInput(
         name = 'HPRD',
@@ -1922,14 +1998,15 @@
         references = (7, ','),
         header = False,
         extra_edge_attrs = {
             'method': (6, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'intact': input_formats.NetworkInput(
         name = 'IntAct',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -1940,14 +2017,15 @@
         input = 'intact.intact_interactions',
         references = 4,
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         input_args = {'miscore': 0.0},
+        data_model = 'interaction',
     ),
     'biogrid': input_formats.NetworkInput(
         name = 'BioGRID',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -1963,14 +2041,15 @@
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         input_args = {
             'htp_limit': None,
             'ltp': False,
         },
+        data_model = 'interaction',
     ),
     'dip': input_formats.NetworkInput(
         name = 'DIP',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -1988,14 +2067,15 @@
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         input_args = {
             'core_only': False,
             'small_scale_only': False,
         },
+        data_model = 'interaction',
     ),
     'ccmap': input_formats.NetworkInput(
         name = 'CancerCellMap',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -2005,14 +2085,15 @@
         sign = False,
         ncbi_tax_id = 9606,
         input = 'cancercellmap.ccmap_interactions',
         references = (3, ';'),
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'innatedb': input_formats.NetworkInput(
         name = 'InnateDB',
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -2022,14 +2103,15 @@
         sign = False,
         input = 'innatedb.innatedb_interactions',
         references = (4, ':'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'matrixdb': input_formats.NetworkInput(
         name = 'MatrixDB',
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
         id_type_b = 'uniprot',
@@ -2041,14 +2123,15 @@
         references = (2, '|'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'method': (3, '|'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
     'mppi': input_formats.NetworkInput(
         name = 'MPPI',
         separator = '|',
         id_col_a = 2,
         id_col_b = 6,
         id_type_a = 'uniprot',
@@ -2061,14 +2144,15 @@
         references = (0, ';'),
         ncbi_tax_id = 9606,
         extra_edge_attrs = {
             'evidences': (1, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'interaction',
     ),
 }
 
 """
 Transcriptional regulatory interactions.
 """
 transcription_onebyone = {
@@ -2087,14 +2171,15 @@
         input = 'abs.abs_interactions',
         interaction_type = 'transcriptional',
         references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'encode_dist': input_formats.NetworkInput(
         name = 'ENCODE-distal',
         separator = None,
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'genesymbol',
@@ -2107,14 +2192,15 @@
         input = 'http://encodenets.gersteinlab.org/enets3.Distal.txt',
         interaction_type = 'transcriptional',
         references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'encode_prox': input_formats.NetworkInput(
         name = 'ENCODE-proximal',
         separator = None,
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'genesymbol',
@@ -2127,14 +2213,15 @@
         input = 'http://encodenets.gersteinlab.org/enets2.Proximal_filtered.txt',
         interaction_type = 'transcriptional',
         references = False,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'pazar': input_formats.NetworkInput(
         name = 'PAZAR',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'enst',
@@ -2147,14 +2234,15 @@
         input = 'pazar.pazar_interactions',
         interaction_type = 'transcriptional',
         references = 2,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'htri': input_formats.NetworkInput(
         name = 'HTRIdb',
         separator = None,
         id_col_a = 1,
         id_col_b = 3,
         id_type_a = 'genesymbol',
@@ -2167,14 +2255,15 @@
         input = 'htri.htri_interactions',
         interaction_type = 'transcriptional',
         references = 4,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'oreganno': input_formats.NetworkInput(
         name = 'ORegAnno',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -2187,14 +2276,15 @@
         input = 'oreganno.oreganno_interactions',
         interaction_type = 'transcriptional',
         references = 2,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'signor': input_formats.NetworkInput(
         name = 'SIGNOR',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -2236,14 +2326,15 @@
         header = True,
         extra_edge_attrs = {
             'mechanism': (7, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         interaction_type = 'transcriptional',
+        data_model = 'activity_flow',
     ),
     'kegg': input_formats.NetworkInput(
         name = 'KEGG',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -2261,14 +2352,15 @@
             (5, True), # is_direct
             (6, True), # transcriptional
         ],
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         interaction_type = 'transcriptional',
+        data_model = 'activity_flow',
     ),
     'kegg-medicus': input_formats.NetworkInput(
         name = 'KEGG-MEDICUS',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -2288,14 +2380,15 @@
         negative_filters = [
             (5, ['missing', 'enzyme_enzyme']),
         ],
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         interaction_type = 'transcriptional',
+        data_model = 'activity_flow',
     ),
 }
 
 """
 New default transcription dataset is only TFregulons
 as it is already an integrated resource and
 has sufficient coverage.
@@ -2341,14 +2434,15 @@
             'coexp':   7,
             'level':   3,
             'kegg_pathways': (14, '|'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = False,
+        data_model = 'activity_flow',
     ),
 }
 
 
 transcription_dorothea = {
     'dorothea': input_formats.NetworkInput(
         name = 'DoRothEA',
@@ -2376,14 +2470,15 @@
         },
         input_args = {
             'levels': {'A', 'B', 'C', 'D'},
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         must_have_references = False,
+        data_model = 'activity_flow',
     ),
 }
 
 # synonyms
 dorothea = transcription_dorothea
 tfregulons = transcription_dorothea
 
@@ -2401,21 +2496,25 @@
         sign = (2, 1, -1),
         ncbi_tax_id = 9606,
         input = 'collectri.collectri_interactions',
         interaction_type = 'transcriptional',
         resource = (4, ';'),
         references = (5, ';'),
         header = False,
-        extra_edge_attrs = {},
+        extra_edge_attrs = {
+            'tf_category': 3,
+            'sign_decision': 6
+        },
         extra_node_attrs_a = {
             'tf_category': 3
         },
         extra_node_attrs_b = {},
         must_have_references = False,
         allow_loops = True,
+        data_model = 'activity_flow',
     ),
 }
 
 # synonyms
 collectri = transcription_collectri
 
 # all transcriptional regulation resources
@@ -2470,14 +2569,15 @@
         input = 'mir2disease.mir2disease_interactions',
         interaction_type = 'post_transcriptional',
         references = None,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'mirdeath': input_formats.NetworkInput(
         name = 'miRDeathDB',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'mirbase',
@@ -2495,14 +2595,15 @@
         references = 3,
         header = False,
         extra_edge_attrs = {
             'function': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'ncrdeath': input_formats.NetworkInput(
         name = 'ncRDeathDB',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'mirbase',
@@ -2527,14 +2628,15 @@
         ],
         extra_edge_attrs = {
             'pathway': 3,
             'effect': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'mirecords': input_formats.NetworkInput(
         name = 'miRecords',
         separator = None,
         id_col_a = 0,
         id_col_b = 2,
         id_type_a = 'mir-mat-name',
@@ -2557,14 +2659,15 @@
         input = 'mirecords.mirecords_interactions',
         interaction_type = 'post_transcriptional',
         references = 5,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'mirtarbase': input_formats.NetworkInput(
         name = 'miRTarBase',
         separator = None,
         id_col_a = 1,
         id_col_b = 3,
         id_type_a = 'mir-mat-name',
@@ -2591,14 +2694,15 @@
         references = 9,
         header = False,
         extra_edge_attrs = {
             'method': (7, '//'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'signor': input_formats.NetworkInput(
         name = 'SIGNOR',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'mir-pre',
@@ -2636,17 +2740,22 @@
         header = True,
         extra_edge_attrs = {
             'mechanism': (7, ';'),
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
         interaction_type = 'post_transcriptional',
+        data_model = 'activity_flow',
     ),
 }
 
+# synonym
+mirnatarget = mirna_target
+
+
 tf_mirna = {
     'transmir': input_formats.NetworkInput(
         name = 'TransmiR',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -2659,14 +2768,15 @@
         input = 'transmir.transmir_interactions',
         interaction_type = 'mirna_transcriptional',
         references = 3,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'encode': input_formats.NetworkInput(
         name = 'ENCODE_tf-mirna',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -2679,14 +2789,15 @@
         input = 'encode.encode_tf_mirna_interactions',
         interaction_type = 'mirna_transcriptional',
         references = None,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
      'collectri': input_formats.NetworkInput(
         name = 'CollecTRI',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'uniprot',
@@ -2697,25 +2808,29 @@
         sign = (2, 1, -1),
         ncbi_tax_id = 9606,
         input = 'collectri.collectri_interactions',
         interaction_type = 'transcriptional',
         resource = (4, ';'),
         references = (5, ';'),
         header = False,
-        extra_edge_attrs = {},
+        extra_edge_attrs = {
+            'tf_category': 3,
+            'sign_decision': 6
+        },
         extra_node_attrs_a = {
             'tf_category': 3
         },
         extra_node_attrs_b = {},
         must_have_references = False,
         allow_loops = True,
         input_args = {
             'protein_coding': False,
             'mirna': True,
-        }
+        },
+        data_model = 'activity_flow',
     ),
 }
 
 lncrna_target = {
     'lncdisease': input_formats.NetworkInput(
         name = 'LncRNADisease',
         separator = None,
@@ -2738,14 +2853,15 @@
         references = 6,
         header = False,
         extra_edge_attrs = {
             'mechanism': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'lncrnadb': input_formats.NetworkInput(
         name = 'lncrnadb',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'lncrna-genesymbol',
@@ -2762,15 +2878,16 @@
         positive_filters = [(2, 'protein')],
         input = 'lncrnadb.lncrnadb_interactions',
         interaction_type = 'lncrna_post_transcriptional',
         references = 4,
         header = False,
         extra_edge_attrs = {},
         extra_node_attrs_a = {},
-        extra_node_attrs_b = {}
+        extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
     'ncrdeath': input_formats.NetworkInput(
         name = 'ncRDeathDB',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'lncrna-genesymbol',
@@ -2795,17 +2912,21 @@
         ],
         extra_edge_attrs = {
             'pathway': 3,
             'effect': 4,
         },
         extra_node_attrs_a = {},
         extra_node_attrs_b = {},
+        data_model = 'activity_flow',
     ),
 }
 
+# synonym
+lncrna_mrna = lncrna_target
+
 ligand_receptor = {
     'ramilowski2015': input_formats.NetworkInput(
         name = 'Ramilowski2015',
         separator = None,
         id_col_a = 0,
         id_col_b = 1,
         id_type_a = 'genesymbol',
@@ -3044,14 +3165,19 @@
         },
         must_have_references = False,
         header = False,
         data_model = 'ligand_receptor',
     ),
 }
 
+
+# synonym
+ligrecextra = ligand_receptor
+
+
 small_molecule_protein = {
     'signor': input_formats.NetworkInput(
         name = 'SIGNOR',
         separator = None,
         id_col_a = (0, lambda x: common.remove_prefix(x, ':')),
         id_col_b = (1, lambda x: common.remove_prefix(x, ':')),
         id_type_a = lambda line: (
@@ -3160,54 +3286,45 @@
         resource = (4, ';'),
         header = False,
         data_model = 'ligand_receptor',
         interaction_type = 'small_molecule_protein',
     ),
 }
 
+# synonym
+small_molecule = small_molecule_protein
+
+
 ligand_receptor['guide2pharma'] = copy.deepcopy(pathway['guide2pharma'])
-ligand_receptor['guide2pharma'].data_model = 'ligand_receptor'
 ligand_receptor['guide2pharma'].must_have_references = False
 ligand_receptor['icellnet'] = copy.deepcopy(pathway['icellnet'])
 ligand_receptor['icellnet'].must_have_references = False
-ligand_receptor['icellnet'].data_model = 'ligand_receptor'
 ligand_receptor['celltalkdb'] = copy.deepcopy(pathway['celltalkdb'])
 ligand_receptor['celltalkdb'].must_have_references = False
-ligand_receptor['celltalkdb'].data_model = 'ligand_receptor'
 ligand_receptor['cellchatdb'] = copy.deepcopy(pathway['cellchatdb'])
 ligand_receptor['cellchatdb'].must_have_references = False
-ligand_receptor['cellchatdb'].data_model = 'ligand_receptor'
 ligand_receptor['connectomedb'] = copy.deepcopy(pathway['connectomedb'])
 ligand_receptor['connectomedb'].must_have_references = False
-ligand_receptor['connectomedb'].data_model = 'ligand_receptor'
 ligand_receptor['talklr'] = copy.deepcopy(pathway['talklr'])
 ligand_receptor['talklr'].must_have_references = False
-ligand_receptor['talklr'].data_model = 'ligand_receptor'
 ligand_receptor['cellinker'] = copy.deepcopy(pathway['cellinker'])
 ligand_receptor['cellinker'].must_have_references = False
-ligand_receptor['cellinker'].data_model = 'ligand_receptor'
 ligand_receptor['scconnect'] = copy.deepcopy(pathway['scconnect'])
 ligand_receptor['scconnect'].must_have_references = False
-ligand_receptor['scconnect'].data_model = 'ligand_receptor'
 
 pathway['hpmr'] = copy.deepcopy(ligand_receptor['hpmr'])
-pathway['hpmr'].data_model = 'activity_flow'
 pathway['hpmr'].must_have_references = True
 pathway['hpmr'].positive_filters = []
 pathway['cellphonedb'] = copy.deepcopy(ligand_receptor['cellphonedb'])
 pathway['cellphonedb'].must_have_references = True
-pathway['cellphonedb'].data_model = 'activity_flow'
 pathway['ramilowski2015'] = copy.deepcopy(ligand_receptor['ramilowski2015'])
 pathway['ramilowski2015'].must_have_references = True
-pathway['ramilowski2015'].data_model = 'activity_flow'
 pathway['lrdb'] = copy.deepcopy(ligand_receptor['lrdb'])
-pathway['lrdb'].data_model = 'activity_flow'
 pathway['lrdb'].must_have_references = True
 pathway['baccin2019'] = copy.deepcopy(ligand_receptor['baccin2019'])
-pathway['baccin2019'].data_model = 'activity_flow'
 pathway['baccin2019'].must_have_references = True
 
 """
 The default set of resources in OmniPath.
 """
 omnipath = {}
 omnipath.update(pathway)
```

### Comparing `pypath_omnipath-0.14.48/pypath/resources/descriptions.py` & `pypath_omnipath-0.15.4/pypath/resources/descriptions.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/resources/licenses.py` & `pypath_omnipath-0.15.4/pypath/resources/licenses.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/resources/urls.py` & `pypath_omnipath-0.15.4/pypath/resources/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,31 +31,39 @@
     'uniprot_pdb': {
         'label': 'Getting PDB IDs of 3D structures for UniProtIDs',
         'url': 'https://ftp.uniprot.org/pub/databases/uniprot/'
             'current_release/knowledgebase/complete/docs/pdbtosp.txt'
     },
     'uniprot_basic': {
         'label': 'URL for UniProt queries',
-        'url': 'https://legacy.uniprot.org/uniprot/',
+        'url': 'https://rest.uniprot.org/uniprotkb/stream',
         'lists': 'https://legacy.uniprot.org/uploadlists/',
-        'datasheet': 'https://legacy.uniprot.org/uniprot/%s.txt',
-        'history': 'https://legacy.uniprot.org/uniprot/%s.tab?version=*',
-        'deleted_sp': 'ftp://ftp.expasy.org/databases/uniprot/'
+        'datasheet': 'https://rest.uniprot.org/uniprotkb/%s.txt',
+        'history': 'https://rest.uniprot.org/uniprot/%s?format=tsv&version=*',
+        'deleted_sp': 'https://ftp.expasy.org/databases/uniprot/'
             'current_release/knowledgebase/complete/docs/delac_sp.txt',
-        'deleted_tr': 'ftp://ftp.expasy.org/databases/uniprot/'
+        'deleted_tr': 'https://ftp.expasy.org/databases/uniprot/'
             'current_release/knowledgebase/complete/docs/delac_tr.txt.gz',
         'speindex_old': 'ftp://ftp.uniprot.org/pub/databases/uniprot/'
             'knowledgebase/docs/speindex.txt',
-        'speindex': 'ftp://ftp.expasy.org/databases/uniprot/current_release/'
+        'speindex': 'https://ftp.expasy.org/databases/uniprot/current_release/'
             'knowledgebase/complete/docs/speindex.txt',
-        'taxids': 'https://www.uniprot.org/taxonomy/?query='
+        'taxids_old': 'https://www.uniprot.org/taxonomy/?query='
             '*&format=tab&force=true&columns=id&compress=yes',
+        'taxids': 'https://rest.uniprot.org/taxonomy/stream?compressed=true'
+            '&fields=id%2Ccommon_name%2Cscientific_name'
+            '&format=tsv&query=%28%2A%29',
         'speclist': 'https://ftp.uniprot.org/pub/databases/uniprot/'
             'current_release/knowledgebase/complete/docs/speclist.txt',
     },
+    'uniprot_idmapping': {
+        'run': 'https://rest.uniprot.org/idmapping/run',
+        'poll': 'https://rest.uniprot.org/idmapping/status/%s',
+        'details': 'https://rest.uniprot.org/idmapping/details/%s',
+    },
     'corum': {
         'label':
         'CORUM is a database of protein complexes, downloadable in csv format',
         'url_old':
         'http://mips.helmholtz-muenchen.de/genre/proj/corum/allComplexes.csv',
         'url': 'http://mips.helmholtz-muenchen.de/corum/download/'
             'allComplexes.txt.zip',
@@ -1629,14 +1637,22 @@
         'url': 'https://figshare.com/ndownloader/files/38534654',
         'api': 'https://rampdb.nih.gov/api/%s',
     },
     'hmdb': {
         'label': 'Human Metabolome Database',
         'metabolites': 'https://hmdb.ca/system/downloads/'
             'current/hmdb_metabolites.zip',
+        'proteins': 'https://hmdb.ca/system/downloads/'
+            'current/hmdb_proteins.zip',
+        'svg': 'https://hmdb.ca/structures/%s/image.svg',
+        'sdf': 'https://hmdb.ca/system/downloads/current/structures.zip',
+    },
+    'lipidmaps': {
+        'label': 'A database of lipid structures',
+        'sdf': 'https://lipidmaps.org/files/?file=LMSD&ext=sdf.zip',
     },
 }
 
 
 files = {
     'phosphosite': {
         'curated': os.path.join(
```

### Comparing `pypath_omnipath-0.14.48/pypath/share/cache.py` & `pypath_omnipath-0.15.4/pypath/share/cache.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/share/common.py` & `pypath_omnipath-0.15.4/pypath/share/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -2684,7 +2684,34 @@
         filter.__eq__
     )
 
     filter = nest(extract, filter)
     obj = obj.items() if _type == dict else obj
 
     return _type(insert(it) for it in obj if filter(it))
+
+
+def ignore_unhashable(func):
+    """
+    Decorator to ignore unhashable values.
+
+    This is useful when using `lru_cache` on functions with optionally
+    unhashable arguments.
+
+    Based on https://stackoverflow.com/a/64111268/854988.
+    """
+
+    uncached = func.__wrapped__
+    attributes = functools.WRAPPER_ASSIGNMENTS + ('cache_info', 'cache_clear')
+    @functools.wraps(func, assigned=attributes)
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except TypeError as error:
+            if 'unhashable type' in str(error):
+                return uncached(*args, **kwargs)
+            raise
+
+    wrapper.__uncached__ = uncached
+
+    return wrapper
+
```

### Comparing `pypath_omnipath-0.14.48/pypath/share/constants.py` & `pypath_omnipath-0.15.4/pypath/share/constants.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/share/curl.py` & `pypath_omnipath-0.15.4/pypath/share/curl.py`

 * *Files 1% similar despite different names*

```diff
@@ -931,14 +931,15 @@
         if CACHEPRINT:
 
             self.show_cache()
 
         if CACHEDEL:
 
             self.delete_cache_file()
+            self.init_cache()
 
         if not self.use_cache and not DRYRUN:
 
             self.title = None
             self.set_title()
             if self.sftp_host is not None:
                 self.sftp_url()
@@ -1643,14 +1644,29 @@
                 self.cache_dir,
                 self.replace_forbidden('%s-%s' % (self.urlmd5, self.filename))
             )
         )
 
 
     @classmethod
+    def cache_path(self, **kwargs) -> str:
+        """
+        Returns the cache path without performing download or creating file.
+
+        Args:
+            kwargs:
+                Arguments to `Curl`.
+        """
+
+        kwargs.update({'setup': False, 'call': False, 'process': False})
+
+        return Curl(**kwargs).cache_file_name
+
+
+    @classmethod
     def replace_forbidden(cls, name: str, repl: str = '_') -> str:
         """
         Replaces the characters that are forbidden in certain file systems.
 
         The slash is forbidden in Unix, while many other characters in Windows
         environments.
         """
```

### Comparing `pypath_omnipath-0.14.48/pypath/share/log.py` & `pypath_omnipath-0.15.4/pypath/share/log.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/share/lookup/_manytomany.py` & `pypath_omnipath-0.15.4/pypath/share/lookup/_manytomany.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany.py` & `pypath_omnipath-0.15.4/pypath/share/lookup/_onetomany.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany2.py` & `pypath_omnipath-0.15.4/pypath/share/lookup/_onetomany2.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/share/progress.py` & `pypath_omnipath-0.15.4/pypath/share/progress.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/share/session.py` & `pypath_omnipath-0.15.4/pypath/share/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         """
         Writes a message to the console and also to the logfile.
         """
 
         self._logger.console(msg = msg, label = self._log_name)
 
 
-    def _log_traceback(self):
+    def _log_traceback(self, console: bool = False):
         """
         Includes a traceback into the log.
         """
 
         exc_type, exc_value, exc_traceback = sys.exc_info()
 
         if exc_type is not None:
@@ -148,19 +148,21 @@
 
             if line.strip().endswith('<module>'):
 
                 stack_top = i
 
         trc_list = trc_list[stack_top:]
 
-        self._log(trc.strip())
+        write = self._console if console else self._log
+
+        write(trc.strip())
 
         for traceline in trc_list:
 
-            self._log(traceline)
+            write(traceline)
 
 
 def get_session():
     """
     Creates new session or returns the one already created.
     """
```

### Comparing `pypath_omnipath-0.14.48/pypath/share/settings.py` & `pypath_omnipath-0.15.4/pypath/share/settings.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/go.py` & `pypath_omnipath-0.15.4/pypath/utils/go.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/homology.py` & `pypath_omnipath-0.15.4/pypath/utils/homology.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from future.utils import iteritems
 from past.builtins import xrange, range
 from typing import Literal
 
 import os
 import sys
 import itertools
+import functools
 import collections
 import importlib as imp
 import re
 import time
 import datetime
 import json
 import pickle
@@ -228,14 +229,16 @@
             homologene = self.homologene,
             ensembl = self.ensembl,
             ensembl_hc = self.ensembl_hc,
             ensembl_types = self.ensembl_types,
         )
 
 
+    @common.ignore_unhashable
+    @functools.lru_cache(maxsize = int(1e5))
     def translate(
             self,
             source_id,
             target,
             source = 9606,
             only_swissprot = True,
             homologene = None,
```

### Comparing `pypath_omnipath-0.14.48/pypath/utils/mapping.py` & `pypath_omnipath-0.15.4/pypath/utils/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 import os
 import sys
 import math
 import re
 import importlib as imp
 import collections
+import functools
 import datetime
 import time
 
 import urllib
 
 if not hasattr(urllib, 'urlencode'):
 
@@ -156,15 +157,15 @@
     'swissprot',
     'uniprot-pri',
     'uniprot-sec',
 }
 
 """
 Classes for reading and use serving ID mapping data from custom file,
-function, UniProt, UniProt uploadlists, Ensembl BioMart,
+function, UniProt, UniProt ID Mapping, Ensembl BioMart,
 PRO (Protein Ontology), miRBase or pickle file.
 """
 
 MappingTableKey = collections.namedtuple(
     'MappingTableKey',
     [
         'id_type',
@@ -403,18 +404,22 @@
 
         if self._to_be_loaded(*args):
 
             cachefile = self._attr('cachefile', *args)
 
             if os.path.exists(cachefile):
 
+                with open(cachefile, 'rb') as fp:
+
+                    from_cache = pickle.load(fp)
+
                 setattr(
                     self,
                     '%s_to_%s' % args,
-                    pickle.load(open(cachefile, 'rb')),
+                    from_cache,
                 )
                 self._log(
                     'Loading `%s` to `%s` mapping table '
                     'from pickle file `%s`.' % (
                         self.param.id_type_a,
                         self.param.id_type_b,
                         cachefile,
@@ -591,39 +596,60 @@
 
             infile.close()
 
         self.a_to_b = a_to_b if self.load_a_to_b else None
         self.b_to_a = b_to_a if self.load_b_to_a else None
 
 
+    @staticmethod
+    def _uniprotkb_id_type(id_type: str) -> bool:
+
+        return input_formats.UniprotListMapping._uniprotkb_id_type(
+            id_type,
+        )
+
+
     def read_mapping_uniprot_list(self):
         """
         Builds a mapping table by downloading data from UniProt's
         upload lists service.
         """
 
         a_to_b = collections.defaultdict(set)
         b_to_a = collections.defaultdict(set)
+        swap = False
 
         if not self.uniprots:
 
             self.set_uniprot_space()
 
         # We need a list to query this service, and we have method only for
         # getting a proteome wide list of UniProt IDs. If the translated
         # ID type is not UniProt, then first we need to translate the
         # proteome wide reference list from UniProt to the target ID type.
-        if self.param.id_type_a != 'uniprot':
+        if not self._uniprotkb_id_type(self.param.id_type_a):
 
-            u_target = self._read_mapping_uniprot_list(
-                uniprot_id_type_a = 'ACC',
-                uniprot_id_type_b = self.param.uniprot_id_type_a,
-            )
+            if self._uniprotkb_id_type(self.param.id_type_b):
+
+                swap = True
+                self.param.swap_sides()
+                self.load_a_to_b, self.load_b_to_a = (
+                    self.load_b_to_a,
+                    self.load_a_to_b,
+                )
+                upload_ac_list = self.uniprots
+
+            else:
+
+                u_target = self._read_mapping_uniprot_list(
+                    uniprot_id_type_a = 'UniProtKB_AC-ID',
+                    uniprot_id_type_b = self.param.uniprot_id_type_a,
+                )
 
-            upload_ac_list = [l.split('\t')[1].strip() for l in u_target]
+                upload_ac_list = [l.split('\t')[1].strip() for l in u_target]
 
         else:
 
             upload_ac_list = self.uniprots
 
         uniprot_data = self._read_mapping_uniprot_list(
             upload_ac_list = upload_ac_list,
@@ -641,14 +667,23 @@
 
                 a_to_b[l[0]].add(l[1])
 
             if self.load_b_to_a:
 
                 b_to_a[l[1]].add(l[0])
 
+        if swap:
+
+            a_to_b, b_to_a = b_to_a, a_to_b
+            self.load_a_to_b, self.load_b_to_a = (
+                self.load_b_to_a,
+                self.load_a_to_b,
+            )
+            self.param.swap_sides()
+
         self.a_to_b = a_to_b if self.load_a_to_b else None
         self.b_to_a = b_to_a if self.load_b_to_a else None
 
 
     def set_uniprot_space(self, swissprot = None):
         """
         Sets up a search space of UniProt IDs.
@@ -677,92 +712,147 @@
         """
         Reads a mapping table from UniProt "upload lists" service.
 
         Args
             uniprot_id_type_a (str): Source ID type label as used in UniProt.
             uniprot_id_type_b (str): Target ID type label as used in UniProt.
             upload_ac_list (list): The identifiers to use in the query to
-                the uploadlists service. By default the list of all UniProt
+                the ID Mapping service. By default the list of all UniProt
                 IDs for the organism is used.
             chunk_size (int): Number of IDs in one query. Too large queries
-                might fail, by default we include 10,000 IDs in one query.
+                might fail, by default we include 100,000 IDs in one query.
         """
 
         chunk_size = (
             chunk_size or
             settings.get('uniprot_uploadlists_chunk_size')
         )
         uniprot_id_type_a = uniprot_id_type_a or self.param.uniprot_id_type_a
         uniprot_id_type_b = uniprot_id_type_b or self.param.uniprot_id_type_b
 
         upload_ac_list = upload_ac_list or self.uniprots
         upload_ac_list = sorted(upload_ac_list)
 
         self._log(
-            'Querying the UniProt uploadlists service for ID translation '
+            'Querying the UniProt ID Mapping service for ID translation '
             'data. Querying a list of %u IDs.' % len(upload_ac_list)
         )
 
-        url = urls.urls['uniprot_basic']['lists']
-
+        run_url = urls.urls['uniprot_idmapping']['run']
+        poll_result = {}
         result = []
 
         # loading data in chunks of 10,000 by default
         for i in range(math.ceil(len(upload_ac_list) / chunk_size)):
 
             this_chunk = upload_ac_list[i * chunk_size:(i + 1) * chunk_size]
 
             self._log(
-                'Request to UniProt uploadlists, chunk #%u with %u IDs.' % (
+                'Request to UniProt ID Mapping, chunk #%u with %u IDs.' % (
                     i,
                     len(this_chunk),
                 )
             )
 
             post = {
                 'from': uniprot_id_type_a,
-                'format': 'tab',
                 'to': uniprot_id_type_b,
-                'uploadQuery': ' '.join(sorted(this_chunk)),
+                'ids': ' '.join(sorted(this_chunk)),
             }
+            accept_json = {'req_headers': ['Accept: application/json']}
 
-            c = curl.Curl(url, post = post, large = True, silent = False)
+            run_args = {'url': run_url, 'post': post}
+            nocache = {'cache': False, 'large': False}
 
-            # 3 extra attempts
-            if c.result is None:
+            cache_path = curl.Curl.cache_path(**run_args)
 
-                for i in xrange(3):
+            if not os.path.exists(cache_path):
 
-                    c = curl.Curl(
-                        url,
-                        post = post,
-                        large = True,
-                        silent = False,
-                        cache = False,
-                        slow = True,
+                run_c = curl.Curl( **run_args, **nocache, **accept_json)
+
+                if run_c.status != 200:
+
+                    raise RuntimeError(
+                        'Failed to submit job to UniProt ID Mapping. '
+                        'See details in the log.'
                     )
 
-                    if c.result is not None:
+                jobid = json.loads(run_c.result)['jobId']
+
+                self._log(
+                    f'Submitted job to UniProt ID Mapping, job ID: `{jobid}`.'
+                )
+
+                timeout = settings.get('uniprot_idmapping_timeout')
+                interval = settings.get('uniprot_idmapping_poll_interval')
+                max_polls = math.ceil(timeout / interval)
+                poll_url = urls.urls['uniprot_idmapping']['poll'] % jobid
+                poll_args = {'url': poll_url} | nocache | accept_json
+
+                for i in range(max_polls):
+
+                    self._log(
+                        f'Polling job UniProt ID Mapping job `{jobid}`, '
+                        f'poll {i + 1} of {max_polls}.'
+                    )
+
+                    poll_c = curl.Curl(**poll_args)
+
+                    if poll_c.status != 200:
+
+                        self._log(f'Poll failed with HTTP {poll_c.status}.')
+                        continue
+
+                    poll_result = json.loads(poll_c.result)
+
+                    if 'status' in poll_result or 'failedIds' in poll_result:
 
                         break
 
-            if c.result is None or c.fileobj.read(5) == '<!DOC':
+                    elif 'messages' in poll_result:
+
+                        msg = (
+                            'UniProt ID Mapping job failed: ' +
+                            ' '.join(common.to_list(poll_result['messages']))
+                        )
+
+                        self._log(msg)
 
-                self._console(
-                    'Error at downloading ID mapping data from UniProt.'
+                        raise RuntimeError(msg)
+
+                    time.sleep(interval)
+
+                det_url = urls.urls['uniprot_idmapping']['details'] % jobid
+                det_c = curl.Curl(url = det_url, **nocache, **accept_json)
+                result_url = (
+                    json.loads(det_c.result)['redirectURL'].
+                    replace('/idmapping/results/', '/idmapping/stream/').
+                    replace('/results/', '/results/stream/').
+                    __add__('?format=tsv')
                 )
 
-                c.result = ''
+                self._log(
+                    'Retrieving UniProt ID Mapping results '
+                    f'from `{result_url}`'
+                )
+
+                with curl.cache_delete_on():
 
-            c.fileobj.seek(0)
+                    res_c = curl.Curl(
+                        url = result_url,
+                        cache = cache_path,
+                        large = True,
+                        silent = False,
+                    )
+
+            else:
 
-            # removing the header row
-            _ = next(c.result)
+                res_c = curl.Curl(**run_args)
 
-            result.extend(list(c.fileobj)[1:])
+            result.extend(list(res_c.fileobj)[1:])
 
         return result
 
 
     def read_mapping_uniprot(self):
         """
         Downloads ID mappings directly from UniProt.
@@ -778,21 +868,21 @@
 
 
         rev = (
             ''
                 if not self.param.swissprot else
             ' AND reviewed:%s' % self.param.swissprot
         )
-        query = 'organism:%u%s' % (int(self.ncbi_tax_id), rev)
+        query = 'organism_id:%u%s' % (int(self.ncbi_tax_id), rev)
 
         url = urls.urls['uniprot_basic']['url']
         post = {
             'query': query,
-            'format': 'tab',
-            'columns': 'id,%s' % self.param._resource_id_type_a,
+            'format': 'tsv',
+            'fields': 'accession,%s' % self.param._resource_id_type_a,
         }
 
         url = '%s?%s' % (url, urllib.urlencode(post))
         c = curl.Curl(url, silent = False)
         # fallback to empty string: Curl returns None in case of
         # empty file but in case of UniProt, especially for under-researched
         # taxons it can happen there is no result for certain queries
@@ -980,16 +1070,23 @@
 
 
     def _read_mapping_smallmolecule(self):
         """
         Loads a small molecule ID translation table.
         """
 
-        mod = globals()[f'{self.source_type}_input']
-        method = getattr(mod, f'{self.source_type}_mapping')
+        if self.param.input_method:
+
+            method = inputs.get_method(self.param.input_method)
+
+        else:
+
+            mod = globals()[f'{self.source_type}_input']
+            method = getattr(mod, f'{self.source_type}_mapping')
+
         data = method(
             id_type_a = self.resource_id_type_a,
             id_type_b = self.resource_id_type_b,
         )
 
         if self.load_a_to_b:
 
@@ -1572,15 +1669,15 @@
 
                         if service_id_type in {'hmdb', 'ramp', 'unichem'}:
 
                             ncbi_tax_id = constants.NOT_ORGANISM_SPECIFIC
                             tbl_key = tbl_key_noorganism
                             tbl_key_rev = tbl_key_rev_noorganism
 
-                        # for uniprot/uploadlists or PRO or array
+                        # for uniprot/idmapping or PRO or array
                         # we create here the mapping params
                         this_param = input_cls(
                             id_type_a = _id_type,
                             id_type_b = _target_id_type,
                             ncbi_tax_id = ncbi_tax_id,
                         )
 
@@ -1718,14 +1815,16 @@
             expand_complexes = expand_complexes,
             uniprot_cleanup = uniprot_cleanup,
         )
 
         return list(names)[0] if names else None
 
 
+    @common.ignore_unhashable
+    @functools.lru_cache(maxsize = int(1e5))
     def map_name(
             self,
             name,
             id_type = None,
             target_id_type = None,
             ncbi_tax_id = None,
             strict = False,
@@ -2331,15 +2430,15 @@
         """
         Special ID translation from ENSP (Ensembl peptide IDs).
         """
 
         mapped_names = set()
         ncbi_tax_id = ncbi_tax_id or self.ncbi_tax_id
 
-        # try first UniProt uploadlists
+        # try first UniProt ID Mapping
         # then Ensembl BioMart
         for id_type in ('ensp', 'ensp_biomart'):
 
             if not mapped_names:
 
                 mapped_names = self._map_name(
                     name = ensp,
@@ -2348,15 +2447,15 @@
                     ncbi_tax_id = ncbi_tax_id,
                 )
 
         if not mapped_names:
 
             tax_ensp = '%u.%s' % (ncbi_tax_id, ensp)
 
-            # this uses UniProt uploadlists with STRING_ID
+            # this uses UniProt ID Mapping with STRING ID type
             mapped_names = self._map_name(
                 name = tax_ensp,
                 id_type = 'ensp_string',
                 target_id_type = target_id_type,
                 ncbi_tax_id = ncbi_tax_id,
             )
 
@@ -2372,30 +2471,30 @@
         """
         Special ID translation to ENSP (Ensembl peptide IDs).
         """
 
         mapped_names = set()
         ncbi_tax_id = ncbi_tax_id or self.ncbi_tax_id
 
-        # try first UniProt uploadlists
+        # try first UniProt ID Mapping
         # then Ensembl BioMart
         for target_id_type in ('ensp', 'ensp_biomart'):
 
             if not mapped_names:
 
                 mapped_names = self._map_name(
                     name = name,
                     id_type = id_type,
                     target_id_type = target_id_type,
                     ncbi_tax_id = ncbi_tax_id,
                 )
 
         if not mapped_names:
 
-            # this uses UniProt uploadlists with STRING_ID
+            # this uses UniProt ID Mapping with STRING type
             mapped_names = self._map_name(
                 name = name,
                 id_type = id_type,
                 target_id_type = 'ensp_string',
                 ncbi_tax_id = ncbi_tax_id,
             )
 
@@ -3238,15 +3337,17 @@
             )
 
             cachefile = os.path.join(cachedir, mapping_id)
             cache_files[key] = cachefile
 
             if os.path.exists(cachefile):
 
-                data[key] = pickle.load(open(cachefile, 'rb'))
+                with open(cachefile, 'rb') as fp:
+
+                    data[key] = pickle.load(fp)
 
             else:
 
                 to_load.add(key)
 
         # loading the remaining from the big UniProt mapping file:
         if to_load:
```

### Comparing `pypath_omnipath-0.14.48/pypath/utils/pdb.py` & `pypath_omnipath-0.15.4/pypath/utils/pdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/proteomicsdb.py` & `pypath_omnipath-0.15.4/pypath/utils/proteomicsdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/pyreact.py` & `pypath_omnipath-0.15.4/pypath/utils/pyreact.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/reflists.py` & `pypath_omnipath-0.15.4/pypath/utils/reflists.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/residues.py` & `pypath_omnipath-0.15.4/pypath/utils/residues.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/seq.py` & `pypath_omnipath-0.15.4/pypath/utils/seq.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/taxonomy.py` & `pypath_omnipath-0.15.4/pypath/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/utils/uniprot.py` & `pypath_omnipath-0.15.4/pypath/utils/uniprot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/visual/drawing.py` & `pypath_omnipath-0.15.4/pypath/visual/drawing.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/__init__.py` & `pypath_omnipath-0.15.4/pypath/visual/igraph_drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/edge.py` & `pypath_omnipath-0.15.4/pypath/visual/igraph_drawing/edge.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/vertex.py` & `pypath_omnipath-0.15.4/pypath/visual/igraph_drawing/vertex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pypath/visual/plot.py` & `pypath_omnipath-0.15.4/pypath/visual/plot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.48/pyproject.toml` & `pypath_omnipath-0.15.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pypath-omnipath"
-version = "0.14.48"
+version = "0.15.4"
 description = "Molecular signaling prior knowledge processing"
 license = "GPL-3.0-only"
 authors = [
     "Denes Turei <turei.denes@gmail.com>",
     "Nicolàs Palacio",
     "Sebastian Lobentanzer",
     "Olga Ivanova",
@@ -69,33 +69,42 @@
 scipy = "*"
 sqlparse = "*"
 tabulate = "*"
 timeloop = "*"
 toml = "*"
 tqdm = "*"
 xlrd = "*"
-pybel = { version = "*", optional = true }
-bio2bel = { version = "*", optional = true }
-click = { version = "*", optional = true }
+# pybel = { version = "*", optional = true, extras = [] }
+# bio2bel = { version = "*", optional = true, extras = [] }
+# click = { version = "*", optional = true }
 python-igraph = { version = "*", optional = true }
+sparqlwrapper = { version = "*", optional = true }
+openbabel = { version = "*", optional = true }
+rdkit = { version = "*", optional = true }
+"epam.indigo" = { version = "*", optional = true }
 pysftp = "^0.2.9"
 typing_extensions = "*"
 
 [tool.poetry.extras]
-bel = [
-    "pybel",
-    "bio2bel",
-    "click",
-]
+# bel = [
+#     "pybel",
+#     "bio2bel",
+#     "click",
+# ]
 graph = [
     "python-igraph",
 ]
 pathophenodb = [
     "sparqlwrapper",
 ]
+metabo = [
+    "epam.indigo",
+    "openbabel",
+    "rdkit",
+]
 
 [tool.poetry.dev-dependencies]
 bump2version = "*"
 sphinx = ">=5.0.0"
 insipid-sphinx-theme = ">=0.3.6"
 sphinx-last-updated-by-git = ">=0.3"
 sphinx-autodoc-typehints = ">=1.18.0"
```

### Comparing `pypath_omnipath-0.14.48/PKG-INFO` & `pypath_omnipath-0.15.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypath-omnipath
-Version: 0.14.48
+Version: 0.15.4
 Summary: Molecular signaling prior knowledge processing
 Home-page: https://omnipathdb.org/
 License: GPL-3.0-only
 Keywords: systems biology,molecular biology,omics,network,signaling
 Author: Denes Turei
 Author-email: turei.denes@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -19,38 +19,39 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: bel
 Provides-Extra: graph
+Provides-Extra: metabo
 Provides-Extra: pathophenodb
 Requires-Dist: PyYAML
 Requires-Dist: beautifulsoup4
-Requires-Dist: bio2bel; extra == "bel"
-Requires-Dist: click; extra == "bel"
 Requires-Dist: dill
+Requires-Dist: epam.indigo ; extra == "metabo"
 Requires-Dist: future
 Requires-Dist: glom
 Requires-Dist: lxml
 Requires-Dist: matplotlib
 Requires-Dist: numpy
+Requires-Dist: openbabel ; extra == "metabo"
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: psutil
-Requires-Dist: pybel; extra == "bel"
 Requires-Dist: pycurl
 Requires-Dist: pyreadr
 Requires-Dist: pysftp (>=0.2.9,<0.3.0)
-Requires-Dist: python-igraph; extra == "graph"
+Requires-Dist: python-igraph ; extra == "graph"
 Requires-Dist: rdata
+Requires-Dist: rdkit ; extra == "metabo"
 Requires-Dist: requests
 Requires-Dist: scipy
+Requires-Dist: sparqlwrapper ; extra == "pathophenodb"
 Requires-Dist: sqlparse
 Requires-Dist: tabulate
 Requires-Dist: timeloop
 Requires-Dist: toml
 Requires-Dist: tqdm
 Requires-Dist: typing_extensions
 Requires-Dist: xlrd
```

