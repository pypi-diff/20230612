# Comparing `tmp/ubkg_api-1.3.0.tar.gz` & `tmp/ubkg_api-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubkg_api-1.3.0.tar", last modified: Wed May 24 15:11:05 2023, max compression
+gzip compressed data, was "ubkg_api-1.3.1.tar", last modified: Mon Jun 12 14:37:31 2023, max compression
```

## Comparing `ubkg_api-1.3.0.tar` & `ubkg_api-1.3.1.tar`

### file list

```diff
@@ -1,73 +1,76 @@
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.650232 ubkg_api-1.3.0/
--rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2023-04-26 01:44:08.000000 ubkg_api-1.3.0/LICENSE
--rw-r--r--   0 ZHY19      (503) staff       (20)     1423 2023-05-24 15:11:05.649984 ubkg_api-1.3.0/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)      850 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/README.md
--rw-r--r--   0 ZHY19      (503) staff       (20)      761 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/pyproject.toml
--rw-r--r--   0 ZHY19      (503) staff       (20)       38 2023-05-24 15:11:05.650282 ubkg_api-1.3.0/setup.cfg
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.547011 ubkg_api-1.3.0/src/
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.569704 ubkg_api-1.3.0/src/ubkg_api/
--rw-r--r--   0 ZHY19      (503) staff       (20)        1 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3649 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/app.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.624138 ubkg_api-1.3.0/src/ubkg_api/models/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     6262 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/assay_type_property_info.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/base_model_.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/codes_codes_obj.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_detail.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2069 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel_depth.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/concept_term.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     8368 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/dataset_property_info.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/qqst.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2404 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_code_term.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      472 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_code_term_rui_code.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_definition.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_prefterm.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_term.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/semantic_stn.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2314 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/sty_tui_stn.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/termtype_code.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      809 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/typing_utils.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/models/util.py
--rw-r--r--   0 ZHY19      (503) staff       (20)    55155 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/neo4j_manager.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.626485 ubkg_api-1.3.0/src/ubkg_api/routes/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/__init__.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.629116 ubkg_api-1.3.0/src/ubkg_api/routes/assaytype/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/assaytype/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1338 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/assaytype/assaytype_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.631552 ubkg_api-1.3.0/src/ubkg_api/routes/codes/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/codes/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1179 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/codes/codes_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.634148 ubkg_api-1.3.0/src/ubkg_api/routes/concepts/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/concepts/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     4450 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/concepts/concepts_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.636693 ubkg_api-1.3.0/src/ubkg_api/routes/datasets/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/datasets/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     2684 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/datasets/datasets_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.639140 ubkg_api-1.3.0/src/ubkg_api/routes/organs/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/organs/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      750 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/organs/organs_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.641076 ubkg_api-1.3.0/src/ubkg_api/routes/semantics/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/semantics/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      633 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/semantics/semantics_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.643147 ubkg_api-1.3.0/src/ubkg_api/routes/terms/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/terms/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1471 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/terms/terms_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.645100 ubkg_api-1.3.0/src/ubkg_api/routes/tui/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/tui/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      559 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/tui/tui_controller.py
--rw-r--r--   0 ZHY19      (503) staff       (20)      364 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/validate.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.647409 ubkg_api-1.3.0/src/ubkg_api/routes/valueset/
--rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/valueset/__init__.py
--rw-r--r--   0 ZHY19      (503) staff       (20)     1396 2023-05-24 14:49:26.000000 ubkg_api-1.3.0/src/ubkg_api/routes/valueset/valueset_controller.py
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.572192 ubkg_api-1.3.0/src/ubkg_api.egg-info/
--rw-r--r--   0 ZHY19      (503) staff       (20)     1423 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/PKG-INFO
--rw-r--r--   0 ZHY19      (503) staff       (20)     2124 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/SOURCES.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)        1 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/dependency_links.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)       68 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/requires.txt
--rw-r--r--   0 ZHY19      (503) staff       (20)        9 2023-05-24 15:11:05.000000 ubkg_api-1.3.0/src/ubkg_api.egg-info/top_level.txt
-drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-05-24 15:11:05.649579 ubkg_api-1.3.0/tests/
--rw-r--r--   0 ZHY19      (503) staff       (20)     3136 2023-05-24 14:49:10.000000 ubkg_api-1.3.0/tests/test_controllers.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.918694 ubkg_api-1.3.1/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2023-04-26 01:44:08.000000 ubkg_api-1.3.1/LICENSE
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1516 2023-06-12 14:37:31.918476 ubkg_api-1.3.1/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)      943 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/README.md
+-rw-r--r--   0 ZHY19      (503) staff       (20)      761 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/pyproject.toml
+-rw-r--r--   0 ZHY19      (503) staff       (20)       38 2023-06-12 14:37:31.918750 ubkg_api-1.3.1/setup.cfg
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.784251 ubkg_api-1.3.1/src/
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.817148 ubkg_api-1.3.1/src/ubkg_api/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        1 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3767 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/src/ubkg_api/app.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.882948 ubkg_api-1.3.1/src/ubkg_api/models/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6262 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/assay_type_property_info.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/base_model_.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/codes_codes_obj.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/concept_detail.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2069 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/concept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/concept_sab_rel_depth.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/concept_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     8368 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/dataset_property_info.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/qqst.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2404 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/sab_code_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      581 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/src/ubkg_api/models/sab_code_term_rui_code.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/sab_definition.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/sab_relationship_concept_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/semantic_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2314 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/sty_tui_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/termtype_code.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      809 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/typing_utils.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/models/util.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    55294 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/src/ubkg_api/neo4j_manager.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.885622 ubkg_api-1.3.1/src/ubkg_api/routes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.889120 ubkg_api-1.3.1/src/ubkg_api/routes/assayname/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/src/ubkg_api/routes/assayname/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1857 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/src/ubkg_api/routes/assayname/assayname_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.892202 ubkg_api-1.3.1/src/ubkg_api/routes/assaytype/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/assaytype/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1529 2023-06-12 14:35:15.000000 ubkg_api-1.3.1/src/ubkg_api/routes/assaytype/assaytype_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.895916 ubkg_api-1.3.1/src/ubkg_api/routes/codes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/codes/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1179 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/codes/codes_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.898852 ubkg_api-1.3.1/src/ubkg_api/routes/concepts/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/concepts/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     4450 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/concepts/concepts_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.903304 ubkg_api-1.3.1/src/ubkg_api/routes/datasets/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/datasets/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2684 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/datasets/datasets_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.905460 ubkg_api-1.3.1/src/ubkg_api/routes/organs/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/organs/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      750 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/organs/organs_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.908330 ubkg_api-1.3.1/src/ubkg_api/routes/semantics/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/semantics/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      633 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/semantics/semantics_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.911410 ubkg_api-1.3.1/src/ubkg_api/routes/terms/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/terms/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1471 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/terms/terms_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.913439 ubkg_api-1.3.1/src/ubkg_api/routes/tui/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/tui/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      559 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/tui/tui_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      364 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/validate.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.916122 ubkg_api-1.3.1/src/ubkg_api/routes/valueset/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/valueset/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1396 2023-05-24 14:49:26.000000 ubkg_api-1.3.1/src/ubkg_api/routes/valueset/valueset_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.820015 ubkg_api-1.3.1/src/ubkg_api.egg-info/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1516 2023-06-12 14:37:31.000000 ubkg_api-1.3.1/src/ubkg_api.egg-info/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2220 2023-06-12 14:37:31.000000 ubkg_api-1.3.1/src/ubkg_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)        1 2023-06-12 14:37:31.000000 ubkg_api-1.3.1/src/ubkg_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       68 2023-06-12 14:37:31.000000 ubkg_api-1.3.1/src/ubkg_api.egg-info/requires.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)        9 2023-06-12 14:37:31.000000 ubkg_api-1.3.1/src/ubkg_api.egg-info/top_level.txt
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2023-06-12 14:37:31.918110 ubkg_api-1.3.1/tests/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3136 2023-06-12 14:34:40.000000 ubkg_api-1.3.1/tests/test_controllers.py
```

### Comparing `ubkg_api-1.3.0/LICENSE` & `ubkg_api-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/PKG-INFO` & `ubkg_api-1.3.1/src/ubkg_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ubkg_api
-Version: 1.3.0
+Name: ubkg-api
+Version: 1.3.1
 Summary: A REST API in front of the Unified Biomedical Knowlegde Graph
 Author-email: HuBMAP Consortium <api-developers@hubmapconsortium.org>
 Project-URL: Homepage, https://github.com/x-atlas-consortia/ubkg-api
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/ubkg-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Unified Biomedical Knowledge Graph
 
 ## UBKG-API
 
+[![PyPI version](https://badge.fury.io/py/ubkg-api.svg)](https://badge.fury.io/py/ubkg-api)
+
 The components of the UBKG include:
 - The **source framework** that extracts ontology information from the UMLS to create a set of CSV files (**UMLS CSVs**)
 - The **generation framework** that appends to the UMLS CSVs assertion data from other ontologies to create a set of **ontology CSVs**.
 - A neo4j **ontology knowledge graph** populated from the ontology CSVS.
 - An **API server** that provides RESTful endpoints to query the ontology knowledge graph.
 
 This repository contains the source for the API.
```

### Comparing `ubkg_api-1.3.0/README.md` & `ubkg_api-1.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Unified Biomedical Knowledge Graph
 
 ## UBKG-API
 
+[![PyPI version](https://badge.fury.io/py/ubkg-api.svg)](https://badge.fury.io/py/ubkg-api)
+
 The components of the UBKG include:
 - The **source framework** that extracts ontology information from the UMLS to create a set of CSV files (**UMLS CSVs**)
 - The **generation framework** that appends to the UMLS CSVs assertion data from other ontologies to create a set of **ontology CSVs**.
 - A neo4j **ontology knowledge graph** populated from the ontology CSVS.
 - An **API server** that provides RESTful endpoints to query the ontology knowledge graph.
 
 This repository contains the source for the API.
```

### Comparing `ubkg_api-1.3.0/pyproject.toml` & `ubkg_api-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ubkg_api"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="HuBMAP Consortium", email="api-developers@hubmapconsortium.org" },
 ]
 description = "A REST API in front of the Unified Biomedical Knowlegde Graph"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ubkg_api-1.3.0/src/ubkg_api/app.py` & `ubkg_api-1.3.1/src/ubkg_api/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import sys
 import logging
 from pathlib import Path
-from flask import Flask, jsonify
+from flask import Flask
 
 # To fix the ModuleNotFoundError when used as a package
 path_root = Path(__file__).parents[0]
 sys.path.append(str(path_root))
 
 # Local modules
 from neo4j_manager import Neo4jManager
 from routes.assaytype.assaytype_controller import assaytype_blueprint
+from routes.assayname.assayname_controller import assayname_blueprint
 from routes.codes.codes_controller import codes_blueprint
 from routes.concepts.concepts_controller import concepts_blueprint
 from routes.datasets.datasets_controller import datasets_blueprint
 from routes.organs.organs_controller import organs_blueprint
 from routes.semantics.semantics_controller import semantics_blueprint
 from routes.terms.terms_controller import terms_blueprint
 from routes.tui.tui_controller import tui_blueprint
@@ -27,14 +28,15 @@
 
 class UbkgAPI:
     def __init__(self, config = None):
 
         self.app = Flask(__name__, instance_path=os.path.join(os.path.abspath(os.path.dirname(__file__)), 'instance'), instance_relative_config=True)
 
         self.app.register_blueprint(assaytype_blueprint)
+        self.app.register_blueprint(assayname_blueprint)
         self.app.register_blueprint(codes_blueprint)
         self.app.register_blueprint(concepts_blueprint)
         self.app.register_blueprint(datasets_blueprint)
         self.app.register_blueprint(semantics_blueprint)
         self.app.register_blueprint(tui_blueprint)
         self.app.register_blueprint(valueset_blueprint)
         self.app.register_blueprint(terms_blueprint)
```

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/assay_type_property_info.py` & `ubkg_api-1.3.1/src/ubkg_api/models/assay_type_property_info.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/base_model_.py` & `ubkg_api-1.3.1/src/ubkg_api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/codes_codes_obj.py` & `ubkg_api-1.3.1/src/ubkg_api/models/codes_codes_obj.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/concept_detail.py` & `ubkg_api-1.3.1/src/ubkg_api/models/concept_detail.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/concept_prefterm.py` & `ubkg_api-1.3.1/src/ubkg_api/models/concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel.py` & `ubkg_api-1.3.1/src/ubkg_api/models/concept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/concept_sab_rel_depth.py` & `ubkg_api-1.3.1/src/ubkg_api/models/concept_sab_rel_depth.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/concept_term.py` & `ubkg_api-1.3.1/src/ubkg_api/models/concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/dataset_property_info.py` & `ubkg_api-1.3.1/src/ubkg_api/models/dataset_property_info.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py` & `ubkg_api-1.3.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/qconcept_tconcept_sab_rel.py` & `ubkg_api-1.3.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/qqst.py` & `ubkg_api-1.3.1/src/ubkg_api/models/qqst.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/sab_code_term.py` & `ubkg_api-1.3.1/src/ubkg_api/models/sab_code_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/sab_definition.py` & `ubkg_api-1.3.1/src/ubkg_api/models/sab_definition.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_prefterm.py` & `ubkg_api-1.3.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/sab_relationship_concept_term.py` & `ubkg_api-1.3.1/src/ubkg_api/models/sab_relationship_concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/semantic_stn.py` & `ubkg_api-1.3.1/src/ubkg_api/models/semantic_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/sty_tui_stn.py` & `ubkg_api-1.3.1/src/ubkg_api/models/sty_tui_stn.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/termtype_code.py` & `ubkg_api-1.3.1/src/ubkg_api/models/termtype_code.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/typing_utils.py` & `ubkg_api-1.3.1/src/ubkg_api/models/typing_utils.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/models/util.py` & `ubkg_api-1.3.1/src/ubkg_api/models/util.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/neo4j_manager.py` & `ubkg_api-1.3.1/src/ubkg_api/neo4j_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -953,15 +953,15 @@
                 elif primary is True and record['primary'] is True:
                     assaytypes.append(make_assaytype_property_info(record).serialize())
                 elif primary is False and record['primary'] is False:
                     assaytypes.append(make_assaytype_property_info(record).serialize())
         result: dict = {"result": assaytypes}
         return result
 
-    def assaytype_name_get(self, name: str, application_context: str = 'HUBMAP') -> AssayTypePropertyInfo:
+    def assaytype_name_get(self, name: str, alt_names: list = None, application_context: str = 'HUBMAP') -> AssayTypePropertyInfo:
         """
         This is intended to be a drop in replacement for the same endpoint in search-src.
 
         The only difference is the optional application_contect to make it consistent with a HUBMAP or SENNET
         environment.
         """
         # datasets: List[DatasetPropertyInfo] = self.dataset_get(application_context, name)
@@ -969,18 +969,18 @@
         # Build the Cypher query that will return the table of data.
         query = self.__query_cypher_dataset_info(application_context)
 
         # Execute Cypher query and return result.
         with self.driver.session() as session:
             recds: neo4j.Result = session.run(query)
             for record in recds:
-                if record.get('data_type') == name:
+                if record.get('data_type') == name and (alt_names is None or record.get('alt_names') == alt_names):
                     # Accessing the record by .get('str') does not appear to work?! :-(
                     return make_assaytype_property_info(record).serialize()
-        return AssayTypePropertyInfo().serialize()
+        return None
 
     # Objectives: Provide crosswalk information between SenNet and RUI for organ types. Replicate the original organ_types.yaml.
     # 1.FindSAB, code, and term for all organs.
     # 2.Find UBERON codes for organs.The code for Skin maps to UBERON 0002097 and UBERON 002097 cross-references
     # UMLS with CUI C1123023; however, the UMLS CUI also maps to UBERON 0000014. It is necessary to specify the
     # UBERON code explicitly.
     # 3.Find two - digit code for organs.
@@ -1017,10 +1017,11 @@
             "RETURN OrganCode,OrganSAB,OrganName,OrganUBERON,OrganTwoCharacterCode ORDER BY OrganName"
 
         with self.driver.session() as session:
             recds: neo4j.Result = session.run(query)
             for record in recds:
                 item = SabCodeTermRuiCode(sab=record.get('OrganSAB'), code=record.get('OrganCode'),
                                           term=record.get('OrganName'),
-                                          rui_code=record.get('OrganTwoCharacterCode')).serialize()
+                                          rui_code=record.get('OrganTwoCharacterCode'),
+                                          organ_uberon=record.get('OrganUBERON')).serialize()
                 result.append(item)
         return result
```

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/assaytype/assaytype_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/assaytype/assaytype_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from flask import Blueprint, jsonify, current_app, request
+from flask import Blueprint, jsonify, current_app, request, make_response
 
 from routes.validate import validate_application_context
 
 assaytype_blueprint = Blueprint('assaytype', __name__, url_prefix='/assaytype')
 
 
 @assaytype_blueprint.route('', methods=['GET'])
@@ -16,20 +16,25 @@
     """
     primary: bool = request.args.get('primary', default=None)
     if primary is not None:
         primary = primary.lower() == 'true'
     application_context = validate_application_context()
     return jsonify(current_app.neo4jManager.assaytype_get(primary, application_context))
 
+
 @assaytype_blueprint.route('/<name>', methods=['GET'])
 def assaytype_name_get(name):
     """Get all of the assaytypes with name.
+    This is a replacement for search-src endpoint of the same name.
 
     :param name: AssayType name
     :type name: str
     :param application_context: Filter to indicate application context
     :type application_context: str
 
     :rtype: Union[AssayTypePropertyInfo, Tuple[AssayTypePropertyInfo, int], Tuple[AssayTypePropertyInfo, int, Dict[str, str]]
     """
     application_context = validate_application_context()
-    return jsonify(current_app.neo4jManager.assaytype_name_get(name, application_context))
+    result = current_app.neo4jManager.assaytype_name_get(name, application_context)
+    if result is None:
+        return make_response(f"No such assay_type {name}", 400)
+    return jsonify(result)
```

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/codes/codes_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/codes/codes_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/concepts/concepts_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/concepts/concepts_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/datasets/datasets_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/datasets/datasets_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/organs/organs_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/organs/organs_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/semantics/semantics_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/semantics/semantics_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/terms/terms_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/terms/terms_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/tui/tui_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/tui/tui_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api/routes/valueset/valueset_controller.py` & `ubkg_api-1.3.1/src/ubkg_api/routes/valueset/valueset_controller.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.3.0/src/ubkg_api.egg-info/PKG-INFO` & `ubkg_api-1.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ubkg-api
-Version: 1.3.0
+Name: ubkg_api
+Version: 1.3.1
 Summary: A REST API in front of the Unified Biomedical Knowlegde Graph
 Author-email: HuBMAP Consortium <api-developers@hubmapconsortium.org>
 Project-URL: Homepage, https://github.com/x-atlas-consortia/ubkg-api
 Project-URL: Bug Tracker, https://github.com/x-atlas-consortia/ubkg-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Unified Biomedical Knowledge Graph
 
 ## UBKG-API
 
+[![PyPI version](https://badge.fury.io/py/ubkg-api.svg)](https://badge.fury.io/py/ubkg-api)
+
 The components of the UBKG include:
 - The **source framework** that extracts ontology information from the UMLS to create a set of CSV files (**UMLS CSVs**)
 - The **generation framework** that appends to the UMLS CSVs assertion data from other ontologies to create a set of **ontology CSVs**.
 - A neo4j **ontology knowledge graph** populated from the ontology CSVS.
 - An **API server** that provides RESTful endpoints to query the ontology knowledge graph.
 
 This repository contains the source for the API.
```

### Comparing `ubkg_api-1.3.0/src/ubkg_api.egg-info/SOURCES.txt` & `ubkg_api-1.3.1/src/ubkg_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 src/ubkg_api/models/semantic_stn.py
 src/ubkg_api/models/sty_tui_stn.py
 src/ubkg_api/models/termtype_code.py
 src/ubkg_api/models/typing_utils.py
 src/ubkg_api/models/util.py
 src/ubkg_api/routes/__init__.py
 src/ubkg_api/routes/validate.py
+src/ubkg_api/routes/assayname/__init__.py
+src/ubkg_api/routes/assayname/assayname_controller.py
 src/ubkg_api/routes/assaytype/__init__.py
 src/ubkg_api/routes/assaytype/assaytype_controller.py
 src/ubkg_api/routes/codes/__init__.py
 src/ubkg_api/routes/codes/codes_controller.py
 src/ubkg_api/routes/concepts/__init__.py
 src/ubkg_api/routes/concepts/concepts_controller.py
 src/ubkg_api/routes/datasets/__init__.py
```

### Comparing `ubkg_api-1.3.0/tests/test_controllers.py` & `ubkg_api-1.3.1/tests/test_controllers.py`

 * *Files identical despite different names*

