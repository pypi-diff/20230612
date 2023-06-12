# Comparing `tmp/hpo-toolkit-0.1.5.tar.gz` & `tmp/hpo-toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpo-toolkit-0.1.5.tar", last modified: Fri May 12 17:21:42 2023, max compression
+gzip compressed data, was "hpo-toolkit-0.2.0.tar", last modified: Mon Jun 12 17:21:28 2023, max compression
```

## Comparing `hpo-toolkit-0.1.5.tar` & `hpo-toolkit-0.2.0.tar`

### file list

```diff
@@ -1,86 +1,91 @@
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo-toolkit-0.1.5/LICENSE
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    42078 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      834 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/README.md
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      987 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/pyproject.toml
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/setup.cfg
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.857328 hpo-toolkit-0.1.5/src/
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.865328 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    42078 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2092 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       12 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/requires.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2023-05-12 17:21:42.000000 hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.865328 hpo-toolkit-0.1.5/src/hpotk/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      380 2023-05-12 17:16:47.000000 hpo-toolkit-0.1.5/src/hpotk/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.865328 hpo-toolkit-0.1.5/src/hpotk/algorithm/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      183 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2696 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/_augment.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6339 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/_traversal.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      206 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1898 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_ic.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6489 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_model.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2728 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_resnik.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/annotations/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      351 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3309 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     8192 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3409 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/_simple.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/annotations/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/_api.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       43 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     8895 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/_impl.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.869328 hpo-toolkit-0.1.5/src/hpotk/constants/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       18 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.873328 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      139 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      452 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/frequency.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/inheritance.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/onset.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/organ_system.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/constants/hpo/severity.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.877328 hpo-toolkit-0.1.5/src/hpotk/graph/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      239 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2064 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5865 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/_csr_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     9243 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/_factory.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.877328 hpo-toolkit-0.1.5/src/hpotk/graph/csr/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       90 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/csr/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7766 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/csr/_csr.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/graph/csr/test__csr.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4768 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/test__csr_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5299 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/graph/test__factory.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.877328 hpo-toolkit-0.1.5/src/hpotk/model/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      380 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/model/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1908 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/model/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    10107 2023-05-10 21:31:14.000000 hpo-toolkit-0.1.5/src/hpotk/model/_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2821 2023-05-09 16:09:29.000000 hpo-toolkit-0.1.5/src/hpotk/model/_term_id.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/ontology/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      126 2022-12-22 14:58:29.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2003 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      238 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/_attrs.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4567 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/_default.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/ontology/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      110 2023-02-27 15:20:14.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5930 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_factory.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6917 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_load.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     9853 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_model.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/test_load.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7105 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/src/hpotk/util.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.881328 hpo-toolkit-0.1.5/src/hpotk/validate/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.5/src/hpotk/validate/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4770 2023-05-12 17:05:54.000000 hpo-toolkit-0.1.5/src/hpotk/validate/_hpo.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2356 2023-05-12 17:05:54.000000 hpo-toolkit-0.1.5/src/hpotk/validate/_model.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-05-12 17:21:42.885328 hpo-toolkit-0.1.5/tests/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2400 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.5/tests/test_disease.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2922 2023-05-12 16:45:32.000000 hpo-toolkit-0.1.5/tests/test_obographs.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4681 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.5/tests/test_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2070 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.5/tests/test_term_id.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4962 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.5/tests/test_validate.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.618790 hpo-toolkit-0.2.0/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo-toolkit-0.2.0/LICENSE
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    42078 2023-06-12 17:21:28.618790 hpo-toolkit-0.2.0/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      834 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/README.md
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      987 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/pyproject.toml
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2023-06-12 17:21:28.618790 hpo-toolkit-0.2.0/setup.cfg
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.606790 hpo-toolkit-0.2.0/src/
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.610790 hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    42078 2023-06-12 17:21:28.000000 hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2280 2023-06-12 17:21:28.000000 hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-06-12 17:21:28.000000 hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       12 2023-06-12 17:21:28.000000 hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2023-06-12 17:21:28.000000 hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.610790 hpo-toolkit-0.2.0/src/hpotk/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      380 2023-06-12 17:04:16.000000 hpo-toolkit-0.2.0/src/hpotk/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.610790 hpo-toolkit-0.2.0/src/hpotk/algorithm/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      230 2023-05-26 17:21:08.000000 hpo-toolkit-0.2.0/src/hpotk/algorithm/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2696 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/algorithm/_augment.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7146 2023-05-26 17:21:08.000000 hpo-toolkit-0.2.0/src/hpotk/algorithm/_traversal.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.610790 hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      206 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3772 2023-05-26 17:21:08.000000 hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/_ic.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6489 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2728 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/_resnik.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.610790 hpo-toolkit-0.2.0/src/hpotk/annotations/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      313 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2935 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5354 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3983 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/_simple.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.610790 hpo-toolkit-0.2.0/src/hpotk/annotations/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/load/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/load/_api.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/annotations/load/hpoa/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       43 2023-03-08 21:00:13.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/load/hpoa/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    11192 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/load/hpoa/_impl.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1519 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/load/hpoa/test__impl.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      449 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/test__base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      670 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/annotations/test__simple.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/constants/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       18 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/src/hpotk/constants/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      139 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      452 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/frequency.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/inheritance.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/onset.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/organ_system.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/src/hpotk/constants/hpo/severity.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/graph/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      239 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/graph/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6922 2023-06-12 17:08:57.000000 hpo-toolkit-0.2.0/src/hpotk/graph/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7503 2023-06-08 17:48:26.000000 hpo-toolkit-0.2.0/src/hpotk/graph/_csr_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     9243 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/graph/_factory.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/graph/csr/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       90 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/graph/csr/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7766 2023-05-26 17:21:12.000000 hpo-toolkit-0.2.0/src/hpotk/graph/csr/_csr.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2023-05-26 17:21:12.000000 hpo-toolkit-0.2.0/src/hpotk/graph/csr/test__csr.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7323 2023-06-08 17:48:26.000000 hpo-toolkit-0.2.0/src/hpotk/graph/test__api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6821 2023-06-08 17:48:26.000000 hpo-toolkit-0.2.0/src/hpotk/graph/test__csr_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5299 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/src/hpotk/graph/test__factory.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/model/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      422 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/model/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5475 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/model/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    10107 2023-05-10 21:31:14.000000 hpo-toolkit-0.2.0/src/hpotk/model/_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3976 2023-06-12 16:58:54.000000 hpo-toolkit-0.2.0/src/hpotk/model/_term_id.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1478 2023-06-12 16:58:54.000000 hpo-toolkit-0.2.0/src/hpotk/model/test__term_id.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/ontology/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      126 2022-12-22 14:58:29.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2003 2023-03-08 21:00:13.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      238 2023-03-08 21:00:13.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/_attrs.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4559 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/_default.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/ontology/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/load/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.614790 hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      110 2023-02-27 15:20:14.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5930 2023-04-14 14:23:26.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/_factory.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6963 2023-06-12 16:58:54.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/_load.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     9853 2023-04-14 14:23:26.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-02-28 16:13:00.000000 hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/test_load.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7180 2023-06-12 16:58:54.000000 hpo-toolkit-0.2.0/src/hpotk/util.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.618790 hpo-toolkit-0.2.0/src/hpotk/validate/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-02-28 16:13:00.000000 hpo-toolkit-0.2.0/src/hpotk/validate/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6847 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/validate/_hpo.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2302 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/validate/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1909 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/src/hpotk/validate/_util.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-06-12 17:21:28.618790 hpo-toolkit-0.2.0/tests/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2922 2023-05-12 16:45:32.000000 hpo-toolkit-0.2.0/tests/test_obographs.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4681 2023-04-14 14:23:26.000000 hpo-toolkit-0.2.0/tests/test_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2070 2022-12-28 21:43:07.000000 hpo-toolkit-0.2.0/tests/test_term_id.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6216 2023-06-01 18:02:25.000000 hpo-toolkit-0.2.0/tests/test_validate.py
```

### Comparing `hpo-toolkit-0.1.5/LICENSE` & `hpo-toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/PKG-INFO` & `hpo-toolkit-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.1.5
+Version: 0.2.0
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpo-toolkit-0.1.5/README.md` & `hpo-toolkit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/pyproject.toml` & `hpo-toolkit-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/PKG-INFO` & `hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.1.5
+Version: 0.2.0
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpo-toolkit-0.1.5/src/hpo_toolkit.egg-info/SOURCES.txt` & `hpo-toolkit-0.2.0/src/hpo_toolkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,50 +16,55 @@
 src/hpotk/algorithm/similarity/_ic.py
 src/hpotk/algorithm/similarity/_model.py
 src/hpotk/algorithm/similarity/_resnik.py
 src/hpotk/annotations/__init__.py
 src/hpotk/annotations/_api.py
 src/hpotk/annotations/_base.py
 src/hpotk/annotations/_simple.py
+src/hpotk/annotations/test__base.py
+src/hpotk/annotations/test__simple.py
 src/hpotk/annotations/load/__init__.py
 src/hpotk/annotations/load/_api.py
 src/hpotk/annotations/load/hpoa/__init__.py
 src/hpotk/annotations/load/hpoa/_impl.py
+src/hpotk/annotations/load/hpoa/test__impl.py
 src/hpotk/constants/__init__.py
 src/hpotk/constants/hpo/__init__.py
 src/hpotk/constants/hpo/base.py
 src/hpotk/constants/hpo/frequency.py
 src/hpotk/constants/hpo/inheritance.py
 src/hpotk/constants/hpo/onset.py
 src/hpotk/constants/hpo/organ_system.py
 src/hpotk/constants/hpo/severity.py
 src/hpotk/graph/__init__.py
 src/hpotk/graph/_api.py
 src/hpotk/graph/_csr_graph.py
 src/hpotk/graph/_factory.py
+src/hpotk/graph/test__api.py
 src/hpotk/graph/test__csr_graph.py
 src/hpotk/graph/test__factory.py
 src/hpotk/graph/csr/__init__.py
 src/hpotk/graph/csr/_csr.py
 src/hpotk/graph/csr/test__csr.py
 src/hpotk/model/__init__.py
 src/hpotk/model/_base.py
 src/hpotk/model/_term.py
 src/hpotk/model/_term_id.py
+src/hpotk/model/test__term_id.py
 src/hpotk/ontology/__init__.py
 src/hpotk/ontology/_api.py
 src/hpotk/ontology/_attrs.py
 src/hpotk/ontology/_default.py
 src/hpotk/ontology/load/__init__.py
 src/hpotk/ontology/load/obographs/__init__.py
 src/hpotk/ontology/load/obographs/_factory.py
 src/hpotk/ontology/load/obographs/_load.py
 src/hpotk/ontology/load/obographs/_model.py
 src/hpotk/ontology/load/obographs/test_load.py
 src/hpotk/validate/__init__.py
 src/hpotk/validate/_hpo.py
 src/hpotk/validate/_model.py
-tests/test_disease.py
+src/hpotk/validate/_util.py
 tests/test_obographs.py
 tests/test_term.py
 tests/test_term_id.py
 tests/test_validate.py
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/algorithm/_augment.py` & `hpo-toolkit-0.2.0/src/hpotk/algorithm/_augment.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/algorithm/_traversal.py` & `hpo-toolkit-0.2.0/src/hpotk/algorithm/_traversal.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     The method raises a :class:`ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
     :param source: `:class:`TermId` or a term ID curie as a `str (e.g. `HP:1234567`)
     :param include_source: whether to include the `source` term in the resulting set
     :return: a `frozenset` with ancestor :class:`TermId`\\ (s).
     """
+    # TODO[v1.0.0] - remove the deprecated method
+    warn('The method is deprecated and will be removed in v1.0.0. Use `get_ancestors` of the graph instead',
+         DeprecationWarning, stacklevel=2)
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
     # Init
     builder: set[TermId] = set()
     if include_source:
@@ -41,14 +44,17 @@
     The method raises a :class:`ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
     :param source: :class:`TermId` or a term ID curie as a :class:`str (e.g. `HP:1234567`)
     :param include_source:  whether to include the `source` term ID(s) in the results
     :return: a :class:`frozenset` with parent `TermId`s
     """
+    # TODO[v1.0.0] - remove the deprecated method
+    warn('The method is deprecated and will be removed in v1.0.0. Use `get_parents` of the graph instead',
+         DeprecationWarning, stacklevel=2)
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
     # Init
     builder: typing.Set[TermId] = set()
     if include_source:
@@ -68,14 +74,17 @@
     The method raises a `ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
     :param source: `TermId` or a term ID curie as a `str (e.g. `HP:1234567`)
     :param include_source:  whether to include the `source` term ID(s) in the results
     :return: a :class:`frozenset` with descendants `TermId`s
     """
+    # TODO[v1.0.0] - remove the deprecated method
+    warn('The method is deprecated and will be removed in v1.0.0. Use `get_descendants` of the graph instead',
+         DeprecationWarning, stacklevel=2)
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
     # Init
     builder: set[TermId] = set()
     if include_source:
@@ -114,14 +123,17 @@
     The method raises a `ValueError` if inputs do not meet the requirement described below.
 
     :param g: the ontology graph or a graph-aware entity
     :param source: `TermId` or a CURIE `str` (e.g. `HP:1234567`)
     :param include_source: whether to include the `source` term in the results
     :return: an iterable with child `TermId`s
     """
+    # TODO[v1.0.0] - remove the deprecated method
+    warn('The method is deprecated and will be removed in v1.0.0. Use `get_children` of the graph instead',
+         DeprecationWarning, stacklevel=2)
     # Check
     g = _check_ontology_graph_is_available(g)
     source = _check_curie_or_term_id(source)
 
     builder: set[TermId] = set()
     if include_source:
         builder.add(source)
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_ic.py` & `hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/_ic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,75 @@
 import math
 import typing
 from collections import Counter
 
+from hpotk.model import TermId
 from hpotk.annotations import AnnotatedItemContainer
 from hpotk.ontology import MinimalOntology
 from hpotk.util import validate_instance
 from ._model import SimpleAnnotationIcContainer, AnnotationIcContainer
-from .._augment import augment_with_ancestors
 
 
 def calculate_ic_for_annotated_items(items: AnnotatedItemContainer,
                                      ontology: MinimalOntology,
-                                     base: typing.Optional[float] = None) -> AnnotationIcContainer:
+                                     base: typing.Optional[float] = None,
+                                     module_root: typing.Optional[TermId] = None,
+                                     use_pseudocount: bool = False) -> AnnotationIcContainer:
     """
     Calculate information content (IC) for each :class:`TermId` based on a collection of annotated `items`.
 
+    The calculation can be done for an ontology module - only the descendants of the provided `module_root`
+    will be included in the analysis. If `assume_annotated` is `True`, then the count of all ontology/module terms
+    is set to at least 1, even for those terms that do not annotate the `items`.
+
     :param items: a collection of :class:`hpotk.annotations.AnnotatedItem`\ s
     :param ontology: ontology with concepts used to annotate the `items`
     :param base: information content base or `None` for *e*
                  (produces IC in `nats <https://en.wikipedia.org/wiki/Nat_(unit)>`_)
+    :param module_root: the root of the ontology module to calculate the IC for.
+    :param use_pseudocount: assume that each ontology term annotates at least one of the `items`.
+
     :return: a container with mappings from :class:`TermId` to information content in nats, bits, or else,
              depending on the `base` value
     """
     ontology = validate_instance(ontology, MinimalOntology, 'ontology')
 
     graph = ontology.graph
-    root = graph.root
-
-    hit_count = Counter()
+    term_id_count: Counter[TermId] = Counter()
+    module_term_ids: typing.Optional[typing.Set[TermId]] = None \
+        if module_root is None \
+        else set(graph.get_descendants(module_root, include_source=True))
 
     for item in items:
         for annotation in item.annotations:
             if annotation.is_present:
-                for ancestor in augment_with_ancestors(graph, annotation.identifier, include_source=True):
-                    hit_count[ancestor] += 1
+                if module_root is not None and annotation.identifier not in module_term_ids:
+                    # annotation is not from the target module.
+                    continue
+
+                for ancestor in graph.get_ancestors(annotation.identifier, include_source=True):
+                    if module_term_ids is None:
+                        # Not doing module
+                        term_id_count[ancestor] += 1
+                    elif ancestor in module_term_ids:
+                        # Doing module and the ancestor is from the module
+                        term_id_count[ancestor] += 1
+
+    if use_pseudocount:
+        # Set the count of all primary term IDs to at least one but DO NOT increment the count of the ancestor
+        # that already count>=1 .
+        # Note, in the HPO case, this will set count of non-phenotypic abnormalities (e.g. Clinical modifier)
+        # to 1 as well.
+        corpus = map(lambda t: t.identifier, ontology.terms) \
+            if module_root is None \
+            else module_term_ids
+        for term_id in corpus:
+            if term_id not in term_id_count:
+                term_id_count[term_id] = 1
 
     log_func = math.log if base is None else lambda c: math.log(c, base)
 
-    population_count = hit_count[root]
+    population_count = term_id_count[graph.root] if module_root is None else term_id_count[module_root]
 
-    data = {term_id: -log_func(count / population_count) for term_id, count in hit_count.items()}
+    data = {term_id: -log_func(count / population_count) for term_id, count in term_id_count.items()}
     metadata = {'annotated_items_version': items.version, 'ontology_version': ontology.version}
     return SimpleAnnotationIcContainer(data, metadata=metadata)
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_model.py` & `hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/_model.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/algorithm/similarity/_resnik.py` & `hpo-toolkit-0.2.0/src/hpotk/algorithm/similarity/_resnik.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/annotations/_api.py` & `hpo-toolkit-0.2.0/src/hpotk/annotations/_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,29 @@
 import abc
 import typing
 import warnings
 
-from hpotk.model import TermId, Identified, Versioned
+from hpotk.model import Identified, FrequencyAwareFeature, Versioned
+from hpotk.model import TermId
 
 
 # #####################################################################################################################
 # The file describes generic schema for annotations, annotated items, and annotated item containers.
 # An example application includes phenotypic features (annotations), diseases or samples (annotated items),
 # and OMIM corpus (annotated item containers).
 # #####################################################################################################################
 
 
-class ObservableAnnotation(Identified, metaclass=abc.ABCMeta):
-    """
-    An identified item with present or absent state.
-    """
-
-    @property
-    @abc.abstractmethod
-    def is_present(self) -> bool:
-        """
-        :return: `True` if the annotation has been *observed* in the annotated object.
-        """
-        pass
-
-    @property
-    def is_absent(self) -> bool:
-        """
-        :return: `True` if the annotation has been *excluded* in the annotated object.
-        """
-        return not self.is_present
+class AnnotationBase(Identified, FrequencyAwareFeature, metaclass=abc.ABCMeta):
+    pass
 
 
-ANNOTATION = typing.TypeVar('ANNOTATION', bound=ObservableAnnotation)
+ANNOTATION = typing.TypeVar('ANNOTATION', bound=AnnotationBase)
 """
-A world item annotation with present or absent state.
+A world item annotation with an identifier and present or excluded state.
 """
 
 
 class AnnotatedItem(typing.Generic[ANNOTATION], metaclass=abc.ABCMeta):
     """
     A world item with annotations. For instance, a disease annotated by phenotypic features.
     """
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/annotations/_base.py` & `hpo-toolkit-0.2.0/src/hpotk/annotations/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,100 +1,14 @@
 import abc
 import enum
 import typing
 
-from hpotk.model import Identified, Named, Versioned, TermId
+from hpotk.model import Identified, Named, TermId
 from hpotk.model import CURIE_OR_TERM_ID
-from ._api import ObservableAnnotation, AnnotatedItem, AnnotatedItemContainer
-
-
-class Ratio(metaclass=abc.ABCMeta):
-
-    @staticmethod
-    def create(numerator: int, denominator: int):
-        return SimpleRatio(numerator, denominator)
-
-    @property
-    @abc.abstractmethod
-    def numerator(self) -> int:
-        pass
-
-    @property
-    @abc.abstractmethod
-    def denominator(self) -> int:
-        pass
-
-    @property
-    def frequency(self) -> float:
-        return self.numerator / self.denominator
-
-    def is_positive(self) -> bool:
-        return self.numerator > 0
-
-    def is_zero(self) -> bool:
-        return self.numerator == 0
-
-    @staticmethod
-    def fold(left, right):
-        """
-        Fold two :class:`Ratio`s together into a new :class:`Ratio` that represents `n` over `m` of both inputs.
-
-        Note that this is *NOT* the addition of two :class:`Ratio`s!
-
-        For instance, if :math:`n_1` of :math:`m_1` and :math:`n_2` of :math:`m_2` population members like lasagna,
-        then :math:`n_1 + n_2` of :math:`m_1 + m_2` people like lasagna in total.
-
-        :param left: left :class:`Ratio`.
-        :param right: right :class:`Ratio`.
-        :return: the result as a :class:`SimpleRatio`.
-        """
-        if isinstance(left, Ratio) and isinstance(right, Ratio):
-            return SimpleRatio(left.numerator + right.numerator, left.denominator + right.denominator)
-        else:
-            msg = 'left arg must be an instance of `Ratio`' \
-                if isinstance(right, Ratio) \
-                else 'right arg must be an instance of `Ratio`'
-            raise ValueError(msg)
-
-    def __eq__(self, other):
-        return isinstance(other, Ratio) \
-            and self.numerator * other.denominator == other.numerator * self.denominator
-
-    def __str__(self):
-        return f"{self.numerator}/{self.denominator}"
-
-
-class SimpleRatio(Ratio):
-
-    def __init__(self, numerator: int, denominator: int):
-        if not isinstance(numerator, int) or numerator < 0:
-            raise ValueError(f'Numerator {numerator} must be a non-negative `int`')
-        if not isinstance(denominator, int) or denominator <= 0:
-            raise ValueError(f'Denominator {denominator} must be a positive `int`')
-        self._numerator = numerator
-        self._denominator = denominator
-
-    @property
-    def numerator(self) -> int:
-        return self._numerator
-
-    @property
-    def denominator(self) -> int:
-        return self._denominator
-
-    def __eq__(self, other):
-        if isinstance(other, SimpleRatio):
-            return self._numerator * other._denominator == self._denominator * other._numerator
-        else:
-            return super().__eq__(other)
-
-    def __repr__(self):
-        return f"SimpleRatio(" \
-               f"numerator={self._numerator}, " \
-               f"denominator={self._denominator})"
+from ._api import FrequencyAwareFeature, AnnotatedItem, AnnotatedItemContainer
 
 
 class EvidenceCode(enum.Enum):
     """Inferred from electronic evidence."""
     IEA = enum.auto()
     """Traceable author statement."""
     TAS = enum.auto()
@@ -178,28 +92,15 @@
 
     def __repr__(self):
         return f"AnnotationReference(" \
                f"identifier={repr(self._identifier)}, " \
                f"evidence_code={repr(self._evidence_code)})"
 
 
-class HpoDiseaseAnnotation(ObservableAnnotation, metaclass=abc.ABCMeta):
-
-    @property
-    @abc.abstractmethod
-    def ratio(self) -> Ratio:
-        """
-        :return: ratio representing a total number of the cohort members who displayed presence
-                 of the phenotypic feature represented by :class:`HpoDiseaseAnnotation` at some point in their life.
-        """
-        pass
-
-    @property
-    def is_present(self) -> bool:
-        return not self.ratio.is_zero()
+class HpoDiseaseAnnotation(Identified, FrequencyAwareFeature, metaclass=abc.ABCMeta):
 
     @property
     @abc.abstractmethod
     def references(self) -> typing.List[AnnotationReference]:
         """
         :return: a list of `AnnotationReference`s that support presence/absence of the disease annotation
         """
@@ -211,16 +112,24 @@
         """
         :return: a list of disease annotation modifiers
         """
         pass
 
     def __str__(self):
         return f"HpoDiseaseAnnotation(" \
+               f"identifier={self.identifier.value}, " \
+               f"frequency={self.numerator}/{self.denominator}, " \
+               f"references={self.references}, " \
+               f"modifiers={self.modifiers})"
+
+    def __repr__(self):
+        return f"HpoDiseaseAnnotation(" \
                f"identifier={self.identifier}, " \
-               f"ratio={self.ratio}, " \
+               f"numerator={self.numerator}, " \
+               f"denominator={self.denominator}, " \
                f"references={self.references}, " \
                f"modifiers={self.modifiers})"
 
 
 class HpoDisease(AnnotatedItem[HpoDiseaseAnnotation], Identified, Named, metaclass=abc.ABCMeta):
 
     @property
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/annotations/_simple.py` & `hpo-toolkit-0.2.0/src/hpotk/annotations/_simple.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 import typing
 import warnings
 
 from hpotk.model import TermId, CURIE_OR_TERM_ID
 from ._api import ANNOTATED_ITEM
-from ._base import AnnotationReference, Ratio
+from ._base import AnnotationReference
 from ._base import HpoDisease, HpoDiseaseAnnotation, HpoDiseases
 
 
 class SimpleHpoDiseaseAnnotation(HpoDiseaseAnnotation):
 
     def __init__(self, identifier: TermId,
-                 ratio: Ratio,
-                 references: typing.List[AnnotationReference],
-                 modifiers: typing.List[TermId]):
+                 numerator: int,
+                 denominator: int,
+                 references: typing.Sequence[AnnotationReference],
+                 modifiers: typing.Sequence[TermId]):
         self._id = identifier
-        self._ratio = ratio
+        self.check_numerator_and_denominator(numerator, denominator)
+        self._numerator = numerator
+        self._denominator = denominator
         self._refs = references
         self._modifiers = modifiers
 
     @property
     def identifier(self) -> TermId:
         return self._id
 
     @property
-    def ratio(self) -> Ratio:
-        return self._ratio
+    def numerator(self) -> int:
+        return self._numerator
 
     @property
-    def references(self) -> typing.List[AnnotationReference]:
+    def denominator(self) -> int:
+        return self._denominator
+
+    @property
+    def references(self) -> typing.Sequence[AnnotationReference]:
         return self._refs
 
     @property
-    def modifiers(self) -> typing.List[TermId]:
+    def modifiers(self) -> typing.Sequence[TermId]:
         return self._modifiers
 
+    def __repr__(self):
+        return f"SimpleHpoDiseaseAnnotation(" \
+               f"identifier={self.identifier}, " \
+               f"numerator={self.numerator}, " \
+               f"denominator={self.denominator}, " \
+               f"references={self.references}, " \
+               f"modifiers={self.modifiers})"
+
 
 class SimpleHpoDisease(HpoDisease):
 
     def __init__(self, identifier: TermId,
                  name: str,
                  annotations: typing.Collection[HpoDiseaseAnnotation],
                  modes_of_inheritance: typing.Collection[TermId]):
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/annotations/load/hpoa/_impl.py` & `hpo-toolkit-0.2.0/src/hpotk/annotations/load/hpoa/_impl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import enum
 import typing
 from collections import defaultdict, namedtuple
 
-from hpotk.annotations import HpoDiseases, EvidenceCode, AnnotationReference, Sex, Ratio
+from hpotk.annotations import HpoDiseases, EvidenceCode, AnnotationReference, Sex
 from hpotk.annotations import SimpleHpoDiseaseAnnotation, SimpleHpoDisease, SimpleHpoDiseases
 from hpotk.model import TermId
 from hpotk.ontology import MinimalOntology
 from hpotk.util import open_text_io_handle_for_reading
 from hpotk.constants.hpo.frequency import parse_hpo_frequency
 from hpotk.annotations.load._api import HpoDiseaseLoader
 
@@ -21,14 +21,76 @@
 
 HPOA_VERSION_PATTERN = re.compile(r'^#(date|version): (?P<version>[\w-]+)\w?$')
 HPO_PATTERN = re.compile(r'^HP:\d{7}$')
 RATIO_PATTERN = re.compile(r'^(?P<numerator>\d+)/(?P<denominator>\d+)$')
 PERCENTAGE_PATTERN = re.compile(r'^(?P<value>\d+\.?(\d+)?)%$')
 
 
+class Ratio:
+    """
+    A private helper class for parsing frequency data.
+    """
+
+    def __init__(self, numerator: int, denominator: int):
+        self._numerator = numerator
+        self._denominator = denominator
+
+    @property
+    def numerator(self) -> int:
+        return self._numerator
+
+    @property
+    def denominator(self) -> int:
+        return self._denominator
+
+    @property
+    def frequency(self) -> float:
+        return self.numerator / self.denominator
+
+    def is_positive(self) -> bool:
+        return self.numerator > 0
+
+    def is_zero(self) -> bool:
+        return self.numerator == 0
+
+    @staticmethod
+    def fold(left, right):
+        """
+        Fold two :class:`Ratio`s together into a new :class:`Ratio` that represents `n` over `m` of both inputs.
+
+        Note that this is *NOT* the addition of two :class:`Ratio`s!
+
+        For instance, if :math:`n_1` of :math:`m_1` and :math:`n_2` of :math:`m_2` population members like lasagna,
+        then :math:`n_1 + n_2` of :math:`m_1 + m_2` people like lasagna in total.
+
+        :param left: left :class:`Ratio`.
+        :param right: right :class:`Ratio`.
+        :return: the result as a :class:`SimpleRatio`.
+        """
+        if isinstance(left, Ratio) and isinstance(right, Ratio):
+            return Ratio(left.numerator + right.numerator, left.denominator + right.denominator)
+        else:
+            msg = 'left arg must be an instance of `Ratio`' \
+                if isinstance(right, Ratio) \
+                else 'right arg must be an instance of `Ratio`'
+            raise ValueError(msg)
+
+    def __eq__(self, other):
+        return isinstance(other, Ratio) \
+            and self.numerator * other.denominator == other.numerator * self.denominator
+
+    def __str__(self):
+        return f"{self.numerator}/{self.denominator}"
+
+    def __repr__(self):
+        return f"SimpleRatio(" \
+               f"numerator={self._numerator}, " \
+               f"denominator={self._denominator})"
+
+
 class SimpleHpoaDiseaseLoader(HpoDiseaseLoader):
     """
     Loads HPO annotation file into :class:`HpoDiseases`.
     """
 
     def __init__(self, hpo: MinimalOntology,
                  cohort_size: int = 50,
@@ -36,15 +98,15 @@
         if not isinstance(hpo, MinimalOntology):
             raise ValueError(f'hpo must be an instance of `MinimalOntology` but was {type(hpo)}')
         self._hpo = hpo
         self._cohort_size = cohort_size
         self._salvage_negated_frequencies = salvage_negated_frequencies
 
     def load(self, file: typing.Union[typing.IO, str]) -> HpoDiseases:
-        data = defaultdict(list)
+        data: typing.Mapping[str, typing.List[HpoAnnotationLine]] = defaultdict(list)
         version = None
         expecting_to_see_header_line = True
         with open_text_io_handle_for_reading(file) as fh:
             for line in fh:
                 if expecting_to_see_header_line:
                     if line.startswith('#'):
                         # header
@@ -72,72 +134,75 @@
 
         return SimpleHpoDiseases(diseases, version)
 
     @property
     def cohort_size(self) -> int:
         return self._cohort_size
 
-    def _assemble_hpo_disease(self, disease_id, hpoa_lines):
+    def _assemble_hpo_disease(self, disease_curie: str, hpoa_lines: typing.List[HpoAnnotationLine]):
         # If the hpoa_lines is empty, then there is something wrong with the `defaultdict` and the logic above.
+        disease_id = TermId.from_curie(disease_curie)
         disease_name = hpoa_lines[0].disease_name
         annotations, moi = self._parse_hpo_annotations(hpoa_lines)
         return SimpleHpoDisease(disease_id, disease_name, annotations, moi)
 
     def _parse_hpo_annotations(self, hpoa_lines: typing.Iterable[HpoAnnotationLine]) \
             -> typing.Tuple[typing.List[SimpleHpoDiseaseAnnotation], typing.Collection[TermId]]:
 
-        line_by_phenotype = defaultdict(list)
+        line_by_phenotype: typing.Mapping[str, typing.List[HpoAnnotationLine]] = defaultdict(list)
         moi = set()
         for hpoa in hpoa_lines:
             if hpoa.aspect == Aspect.PHENOTYPE:
                 # Several HPOA lines may correspond to a single phenotype feature
                 line_by_phenotype[hpoa.phenotype_term_id].append(hpoa)
             elif hpoa.aspect == Aspect.INHERITANCE:
                 moi.add(hpoa.phenotype_term_id)
             else:
                 # TODO - handle the remaining aspect lines
                 pass
 
         annotations = []
-        for phenotype_term_id, lines in line_by_phenotype.items():
+        for phenotype_curie, lines in line_by_phenotype.items():
+            phenotype_id = TermId.from_curie(phenotype_curie)
             total_ratio = None
             annotation_references = set()
             modifiers = set()
             for line in lines:
                 ratio = self._parse_frequency(line.is_negated, line.frequency)
                 if total_ratio:
                     total_ratio = Ratio.fold(total_ratio, ratio)
                 else:
                     total_ratio = ratio
 
                 annotation_references.update(line.annotation_references)
                 modifiers.update(line.modifiers)
 
-            ann = SimpleHpoDiseaseAnnotation(phenotype_term_id,
-                                             total_ratio,
-                                             list(annotation_references),
-                                             list(modifiers))
+            ann = SimpleHpoDiseaseAnnotation(phenotype_id,
+                                             numerator=total_ratio.numerator,
+                                             denominator=total_ratio.denominator,
+                                             references=tuple(annotation_references),
+                                             modifiers=tuple(modifiers))
             annotations.append(ann)
 
         return annotations, moi
 
     def _parse_frequency(self, is_negated: bool, frequency: str) -> Ratio:
         # An empty string is assumed to represent a case study
         if not frequency:
             numerator = 0 if is_negated else 1
             denominator = 1
-            return Ratio.create(numerator, denominator)
+            return Ratio(numerator, denominator)
 
         # HPO term, e.g. HP:0040280 (Obligate)
         hpo_match = HPO_PATTERN.match(frequency)
         if hpo_match:
             hpo_frequency = parse_hpo_frequency(frequency)
             numerator = 0 if is_negated else round(hpo_frequency.frequency * self._cohort_size)
             denominator = self._cohort_size
-            return Ratio.create(numerator, denominator)
+            return Ratio(numerator, denominator)
 
         # Ratio, e.g. 1/2
         ratio_match = RATIO_PATTERN.match(frequency)
         if ratio_match:
             denominator = int(ratio_match.group('denominator'))
             i = int(ratio_match.group('numerator'))
             if is_negated:
@@ -147,34 +212,34 @@
                 if i == 0 and self._salvage_negated_frequencies:
                     numerator = 0
                 else:
                     numerator = denominator - i
             else:
                 numerator = i
 
-            return Ratio.create(numerator, denominator)
+            return Ratio(numerator, denominator)
 
         # Percentage, e.g. 20%
         percentage_match = PERCENTAGE_PATTERN.match(frequency)
         if percentage_match:
             percentage = float(percentage_match.group('value'))
             numerator = round(percentage * self._cohort_size / 100)
             denominator = self._cohort_size
-            return Ratio.create(numerator, denominator)
+            return Ratio(numerator, denominator)
 
         raise ValueError(f'Unable to parse frequency {frequency}')
 
 
 def _parse_hpoa_line(line: str) -> typing.Optional[HpoAnnotationLine]:
     fields = line.strip().split('\t')
 
-    disease_id = TermId.from_curie(fields[0])
+    disease_id = fields[0]
     disease_name = fields[1]
     is_negated = fields[2].upper() == 'NOT'
-    phenotype_id = TermId.from_curie(fields[3])
+    phenotype_id = fields[3]
     evidence_code = EvidenceCode.parse(fields[5])
     annotation_references = [AnnotationReference(TermId.from_curie(term_id), evidence_code)
                              for term_id
                              in filter(lambda t: t and not t.isspace(), fields[4].split(';'))]
     # TODO - implement parsing of temporal data
     onset = None
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/frequency.py` & `hpo-toolkit-0.2.0/src/hpotk/constants/hpo/frequency.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/inheritance.py` & `hpo-toolkit-0.2.0/src/hpotk/constants/hpo/inheritance.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/onset.py` & `hpo-toolkit-0.2.0/src/hpotk/constants/hpo/onset.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/constants/hpo/organ_system.py` & `hpo-toolkit-0.2.0/src/hpotk/constants/hpo/organ_system.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/graph/_csr_graph.py` & `hpo-toolkit-0.2.0/src/hpotk/graph/_csr_graph.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import bisect
 import typing
 import warnings
 from collections import deque
 
 import numpy as np
 
-from hpotk.model import TermId
+from hpotk.model import TermId, Identified
 from hpotk.util import validate_instance
 from ._api import OntologyGraph, NODE
 from .csr import ImmutableCsrMatrix
 
 
 class BaseCsrOntologyGraph(OntologyGraph, metaclass=abc.ABCMeta):
     CHILD_RELATIONSHIP_CODE = 1
@@ -23,66 +23,97 @@
         self._nodes = validate_instance(nodes, np.ndarray, 'nodes')
         self._adjacency_matrix = validate_instance(adjacency_matrix, ImmutableCsrMatrix, 'adjacency_matrix')
 
     @property
     def root(self) -> NODE:
         return self._root
 
-    def get_children(self, source: NODE) -> typing.Iterable[NODE]:
+    def get_children(self, source: typing.Union[str, NODE, Identified],
+                     include_source: bool = False) -> typing.Iterable[NODE]:
         # In other words, find a row in the CSR corresponding to the `source`
         # and retrieve the columns to which the `source` is the PARENT.
         return map(self._get_node_for_idx,
-                   self._get_node_indices_with_relationship(source, BaseCsrOntologyGraph.PARENT_RELATIONSHIP_CODE))
+                   self._get_node_indices_with_relationship(source,
+                                                            BaseCsrOntologyGraph.PARENT_RELATIONSHIP_CODE,
+                                                            include_source))
 
-    def get_descendants(self, source: NODE) -> typing.Iterable[NODE]:
+    def get_descendants(self, source: typing.Union[str, NODE, Identified],
+                        include_source: bool = False) -> typing.Iterable[NODE]:
         # See `self.get_children()` for explanation of `BaseCsrOntologyGraph.PARENT_RELATIONSHIP_CODE`.
         return map(self._get_node_for_idx,
-                   self._traverse_graph(source, BaseCsrOntologyGraph.PARENT_RELATIONSHIP_CODE))
+                   self._traverse_graph(source,
+                                        BaseCsrOntologyGraph.PARENT_RELATIONSHIP_CODE,
+                                        include_source))
 
-    def get_parents(self, source: NODE) -> typing.Iterable[NODE]:
+    def get_parents(self, source: typing.Union[str, NODE, Identified],
+                    include_source: bool = False) -> typing.Iterable[NODE]:
         # In other words, find a row in the CSR corresponding to the `source`
         # and retrieve the columns to which the `source` is the CHILD.
         return map(self._get_node_for_idx,
-                   self._get_node_indices_with_relationship(source, BaseCsrOntologyGraph.CHILD_RELATIONSHIP_CODE))
+                   self._get_node_indices_with_relationship(source,
+                                                            BaseCsrOntologyGraph.CHILD_RELATIONSHIP_CODE,
+                                                            include_source))
 
-    def get_ancestors(self, source: NODE) -> typing.Iterable[NODE]:
+    def get_ancestors(self, source: typing.Union[str, NODE, Identified],
+                      include_source: bool = False) -> typing.Iterable[NODE]:
         # See `self.get_parents()` for explanation of `BaseCsrOntologyGraph.CHILD_RELATIONSHIP_CODE`.
         return map(self._get_node_for_idx,
-                   self._traverse_graph(source, BaseCsrOntologyGraph.CHILD_RELATIONSHIP_CODE))
+                   self._traverse_graph(source,
+                                        BaseCsrOntologyGraph.CHILD_RELATIONSHIP_CODE,
+                                        include_source))
+
+    def is_leaf(self, node: typing.Union[str, NODE, Identified]) -> bool:
+        for _ in self._get_node_indices_with_relationship(node, BaseCsrOntologyGraph.PARENT_RELATIONSHIP_CODE, False):
+            return False
+        return True
 
     def __contains__(self, item: NODE) -> bool:
         return self._get_idx_for_node(item) is not None
 
     def __iter__(self) -> typing.Iterator[NODE]:
         return iter(self._nodes)
 
-    def _traverse_graph(self, source: NODE, relationship) -> typing.Generator[int, None, None]:
+    def _traverse_graph(self, source: typing.Union[str, NODE, Identified],
+                        relationship,
+                        include_source: bool) -> typing.Generator[int, None, None]:
+        source: TermId = self._map_to_term_id(source)
         seen: set[int] = set()
         buffer: typing.Deque[int] = deque()
 
         # Init
-        for idx in self._get_node_indices_with_relationship(source, relationship):
+        for idx in self._get_node_indices_with_relationship(source, relationship, include_source):
             seen.add(idx)
             buffer.append(idx)
 
         # Loop
         while buffer:
             current = buffer.popleft()
             for idx in self._get_cols_with_relationship(current, relationship):
                 if idx not in seen:
                     seen.add(idx)
                     buffer.append(idx)
 
             yield current
 
-    def _get_node_indices_with_relationship(self, source: NODE, relationship) -> typing.Generator[int, None, None]:
+    def _get_node_indices_with_relationship(self, source: typing.Union[str, NODE, Identified],
+                                            relationship,
+                                            include_source: bool) -> typing.Generator[int, None, None]:
+        source: TermId = self._map_to_term_id(source)
         row_idx = self._get_idx_for_node(source)
-        return self._get_cols_with_relationship(row_idx, relationship)
+        if row_idx is None:
+            raise ValueError(f'Term ID not found in the graph: {source.value}')
 
-    def _get_cols_with_relationship(self, idx: typing.Optional[int], relationship) -> typing.Generator[int, None, None]:
+        if include_source:
+            yield row_idx
+
+        for idx in self._get_cols_with_relationship(row_idx, relationship):
+            yield idx
+
+    def _get_cols_with_relationship(self, idx: typing.Optional[int],
+                                    relationship) -> typing.Generator[int, None, None]:
         if idx is None:
             return
         col_indices = self._adjacency_matrix.col_indices_of_val(idx, relationship)
         for col_idx in col_indices:
             yield int(col_idx)  # Numpy returns np.i64 but we need int
 
     @abc.abstractmethod
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/graph/_factory.py` & `hpo-toolkit-0.2.0/src/hpotk/graph/_factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/graph/csr/_csr.py` & `hpo-toolkit-0.2.0/src/hpotk/graph/csr/_csr.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/graph/csr/test__csr.py` & `hpo-toolkit-0.2.0/src/hpotk/graph/csr/test__csr.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/graph/test__factory.py` & `hpo-toolkit-0.2.0/src/hpotk/graph/test__factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/model/_term.py` & `hpo-toolkit-0.2.0/src/hpotk/model/_term.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/model/_term_id.py` & `hpo-toolkit-0.2.0/src/hpotk/model/_term_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,16 +52,26 @@
     def value(self) -> str:
         """
         Get concept value consisting of `self.prefix` and `self.value`. For instance, `HP:1234567`.
         :return: concept value `str`
         """
         return self.prefix + ':' + self.id
 
+    @staticmethod
+    def _calculate_hash(prefix: str, id: str) -> int:
+        """
+        Calculate hash of a term ID from the members.
+        :param prefix: the prefix part of the term ID (e.g. `HP` for `HP:1234567`) as a `str.
+        :param id: the id part of the term ID (e.g. `1234567` for `HP:1234567`) as a str.
+        :return: a hash as an `int`.
+        """
+        return hash((prefix, id))
+
     def __hash__(self) -> int:
-        return hash((self.prefix, self.id))
+        return self._calculate_hash(self.prefix, self.id)
 
     def __eq__(self, other):
         return isinstance(other, TermId) \
             and self.prefix == other.prefix \
             and self.id == other.id
 
     def __lt__(self, other):
@@ -75,26 +85,53 @@
 
     def __str__(self):
         return self.value
 
 
 class DefaultTermId(TermId):
     """
-    A default implementation of :class:`TermId` that stores the index of the delimiter and the value as a string.
+    A default implementation of :class:`TermId` that stores the index of the delimiter and the value as a string
+    and caches the hash value.
     """
 
     def __init__(self, value: str, idx: int):
         self._value = value
         self._idx = idx
+        self._hash = self._calculate_hash(prefix=value[:idx], id=value[idx + 1:])
 
     @property
     def prefix(self) -> str:
         return self._value[:self._idx]
 
     @property
     def id(self) -> str:
         return self._value[self._idx + 1:]
 
     def __repr__(self):
         return f'DefaultTermId(idx={self._idx}, value={self._value})'
 
+    def __hash__(self) -> int:
+        return self._hash
+
     # TODO - make specific HPO TermId
+
+
+class SimpleTermId(TermId):
+    """
+    The simplest possible implementation of a `TermId` that stores the entire curie and the position
+    of the delimiter that separates the prefix and the id.
+    """
+
+    def __init__(self, value: str, idx: int):
+        self._value = value
+        self._idx = idx
+
+    @property
+    def prefix(self) -> str:
+        return self._value[:self._idx]
+
+    @property
+    def id(self) -> str:
+        return self._value[self._idx + 1:]
+
+    def __repr__(self):
+        return f'SimpleTermId(idx={self._idx}, value={self._value})'
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/ontology/_api.py` & `hpo-toolkit-0.2.0/src/hpotk/ontology/_api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/ontology/_default.py` & `hpo-toolkit-0.2.0/src/hpotk/ontology/_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,8 +134,8 @@
     Validate that `term_id` is a `TermId` or a valid CURIE `str`.
     """
     if isinstance(term_id, TermId):
         return term_id
     elif isinstance(term_id, str):
         return TermId.from_curie(term_id)
     else:
-        raise ValueError(f'Expected a `{type(TermId)}` or a `str` but got {type(term_id)}')
+        raise ValueError(f'Expected a `TermId` or a `str` but got {type(term_id)}')
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_factory.py` & `hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/_factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_load.py` & `hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,24 +37,26 @@
 def _load_impl(file: typing.Union[typing.IO, str],
                term_factory: ObographsTermFactory[MinimalTerm],
                graph_factory: GraphFactory,
                ontology_creator):
     hpo = get_hpo_graph(file)
     logger.debug("Extracting ontology terms")
     id_to_term_id, terms = extract_terms(hpo['nodes'], term_factory)
-    logger.debug(f"Creating the edge list")
+    logger.debug("Creating the edge list")
     edge_list = create_edge_list(hpo['edges'], id_to_term_id)
-    logger.debug(f"Building ontology graph")
+    logger.debug("Building ontology graph")
     graph: OntologyGraph = graph_factory.create_graph(edge_list)
     if graph.root == OWL_THING:
         # TODO - consider adding Owl thing into terms list
         pass
     version = extract_ontology_version(hpo['meta'])
-    logger.debug(f"Assembling the ontology")
-    return ontology_creator(graph, terms, version)
+    logger.debug("Assembling the ontology")
+    ontology = ontology_creator(graph, terms, version)
+    logger.debug("Done")
+    return ontology
 
 
 def get_hpo_graph(file: typing.Union[typing.IO, str]):
     with open_text_io_handle_for_reading(file) as fh:
         document = json.load(fh)
     if not isinstance(document, dict):
         raise ValueError(f'The JSON document should have been a dict but was {type(document)}')
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/_model.py` & `hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/_model.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/ontology/load/obographs/test_load.py` & `hpo-toolkit-0.2.0/src/hpotk/ontology/load/obographs/test_load.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/src/hpotk/util.py` & `hpo-toolkit-0.2.0/src/hpotk/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 DEFAULT_LOG_FMT = '%(asctime)s %(name)-20s %(levelname)-3s : %(message)s'
 
 
 def setup_logging(level: int = logging.INFO,
                   log_fmt: str = DEFAULT_LOG_FMT):
     """
-        Create a basic configuration for the logging library. Set up console and file handler using provided `log_fmt`.
-        :param level: verbosity to use, INFO by default
-        :param log_fmt: format string for logging
-        """
+    Create a basic configuration for the logging library. Set up console and file handler using provided `log_fmt`.
+    :param level: verbosity to use, `20` (INFO) by default. Use `10` for DEBUG, `30` for `WARNING`, `40` for `ERROR`, and `50` for `CRITICAL`.
+    :param log_fmt: format string for logging
+    """
     # create logger
     logger = logging.getLogger()
     logger.setLevel(level)
     # create console handler and set level to debug
     ch = logging.StreamHandler()
     ch.setLevel(level)
     # create formatter
```

### Comparing `hpo-toolkit-0.1.5/src/hpotk/validate/_model.py` & `hpo-toolkit-0.2.0/src/hpotk/validate/_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 import abc
 import enum
 
 from collections import namedtuple
 
 from hpotk.model import Identified, TermId
+from ._util import SimpleFeature, map_to_stateful_feature
 
 
 class ValidationLevel(enum.Enum):
     WARNING = 1
     ERROR = 2
 
 
@@ -35,35 +36,30 @@
 
     def __repr__(self) -> str:
         return f"ValidationResults(results={[self._results]})"
 
 
 class RuleValidator(metaclass=abc.ABCMeta):
     """
-    `RuleValidator` checks if a sequence of :class:`Identified` or :class:`TermId` instances meet
-    the validation requirements.
+    `RuleValidator` checks if a sequence of :class:`Identified` or :class:`TermId` items meet
+    the validation requirements. The observation status is included in case the items extend :class:`ObservableFeature`.
 
     The validators can check each item individually or as a collection, for instance,
     to discover violation of the annotation propagation rule, etc.
 
     The issues are returned as :class:`ValidationResults`.
     """
 
     @abc.abstractmethod
     def validate(self, items: typing.Sequence[typing.Union[Identified, TermId]]) -> ValidationResults:
         pass
 
     @staticmethod
-    def extract_term_id(item: typing.Union[Identified, TermId]) -> TermId:
-        if isinstance(item, Identified):
-            return item.identifier
-        elif isinstance(item, TermId):
-            return item
-        else:
-            raise ValueError(f'Item {item} of type {type(item)} is not a TermId nor extends Identified')
+    def _extract_stateful_feature(item: typing.Union[Identified, TermId]) -> SimpleFeature:
+        return map_to_stateful_feature(item)
 
 
 class ValidationRunner:
     """
     The runner applies a sequence of `RuleValidator`s on items and returns the results as `ValidationResults`.
     """
```

### Comparing `hpo-toolkit-0.1.5/tests/test_obographs.py` & `hpo-toolkit-0.2.0/tests/test_obographs.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/tests/test_term.py` & `hpo-toolkit-0.2.0/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/tests/test_term_id.py` & `hpo-toolkit-0.2.0/tests/test_term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.5/tests/test_validate.py` & `hpo-toolkit-0.2.0/tests/test_validate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 import os
 import unittest
 
 import ddt
 from pkg_resources import resource_filename
 
-from hpotk.model import MinimalTerm, TermId
+from hpotk.model import Identified, ObservableFeature, TermId
 from hpotk.ontology.load.obographs import load_minimal_ontology
 from hpotk.validate import ValidationResult, ValidationLevel
 from hpotk.validate import AnnotationPropagationValidator, PhenotypicAbnormalityValidator, ObsoleteTermIdsValidator
 
 
 TOY_HPO = resource_filename(__name__, os.path.join('data', 'hp.toy.json'))
 
 
+class SimpleFeature(Identified, ObservableFeature):
+
+    def __init__(self, curie: str, status: bool):
+        self._id = TermId.from_curie(curie)
+        self._status = status
+
+    @property
+    def identifier(self) -> TermId:
+        return self._id
+
+    @property
+    def is_present(self) -> bool:
+        return self._status
+
+
 class TestBaseRuleValidator(unittest.TestCase):
 
     o = None
     example_terms = None
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.o = load_minimal_ontology(TOY_HPO)
         cls.example_terms = [
-            MinimalTerm.create_minimal_term(
-                TermId.from_curie('HP:0001166'),
-                name='Arachnodactyly', alt_term_ids=[], is_obsolete=False),
-            MinimalTerm.create_minimal_term(
-                TermId.from_curie('HP:0002266'),
-                name='Focal clonic seizure', alt_term_ids=[], is_obsolete=False),
-            MinimalTerm.create_minimal_term(
-                TermId.from_curie('HP:0032648'),
-                name='Tubularization of Bowman capsule', alt_term_ids=[], is_obsolete=False)
+            SimpleFeature('HP:0001166', True),  # Arachnodactyly
+            SimpleFeature('HP:0001250', True),  # Seizure
+            SimpleFeature('HP:0032648', True),  # Tubularization of Bowman capsule
+            SimpleFeature('HP:0000805', False)  # excluded Enuresis
         ]
 
 
 @ddt.ddt
 class TestAnnotationPropagationValidator(TestBaseRuleValidator):
 
     def setUp(self) -> None:
@@ -44,81 +54,97 @@
         results = self.validator.validate([])
         self.assertTrue(results.is_ok())
 
     def test_ok_input_produces_no_errors(self):
         results = self.validator.validate(self.example_terms)
         self.assertTrue(results.is_ok())
 
+    def test_obsolete_ancestor_produces_error(self):
+        example_terms = list(self.example_terms)
+        example_terms.append(TermId.from_curie('HP:0006010'))
+
+        results = self.validator.validate(example_terms)
+
+        self.assertFalse(results.is_ok())
+        self.assertEqual(results.results[0],
+                         ValidationResult(level=ValidationLevel.ERROR, category='annotation_propagation',
+                                          message='Terms should not contain both present Arachnodactyly [HP:0001166] '
+                                                  f'and its present or excluded ancestor Long fingers [HP:0100807]'))
+
     @ddt.data(
-        ("HP:0100807", "HP:0100807", "Long fingers"),
-        ("HP:0006010", 'HP:0100807', "Long fingers"),
+        ("HP:0100807", True, 'HP:0001166', True),   # present Long fingers vs. present Arachnodactyly
+        ("HP:0100807", False, 'HP:0001166', True),  # excluded Long fingers vs. present Arachnodactyly
+
+        # The case is commented out since it is possible to have some abnormality but excluded specific abnormality
+        # ("HP:0000014", True, 'HP:0000805', False),  # present Abnormality of the bladder vs. excluded Enuresis
+
+        ("HP:0000014", False, 'HP:0000805', False),  # excluded Abnormality of the bladder vs. excluded Enuresis
     )
     @ddt.unpack
-    def test_ancestor_presence_produces_error(self, query_id, current_id, name):
+    def test_ancestor_presence_produces_error(self, ancestor_curie, ancestor_status, base_curie, base_status):
         example_terms = list(self.example_terms)
-        example_terms.append(
-            MinimalTerm.create_minimal_term(
-                TermId.from_curie(query_id), name=name, alt_term_ids=[], is_obsolete=False)
-        )
+        example_terms.append(SimpleFeature(ancestor_curie, ancestor_status))
+
         results = self.validator.validate(example_terms)
+
         self.assertFalse(results.is_ok())
-        self.assertEqual(results.results[0],
-                         ValidationResult(level=ValidationLevel.ERROR, category='annotation_propagation',
-                                          message='Terms should not contain both Arachnodactyly [HP:0001166] '
-                                                  f'and its ancestor {name} [{current_id}]'))
+        self.assertEqual(1, len(results.results))
+        first = results.results[0]
+        self.assertEqual(ValidationLevel.ERROR, first.level)
+        self.assertEqual('annotation_propagation', first.category)
+
+        state = 'present' if base_status else 'excluded'
+        self.assertEqual(f'Terms should not contain both {state} '
+                         f'{self.o.get_term(base_curie).name} [{self.o.get_term(base_curie).identifier.value}] '
+                         f'and its present or excluded ancestor '
+                         f'{self.o.get_term(ancestor_curie).name} [{ancestor_curie}]',
+                         first.message)
 
 
 @ddt.ddt
 class TestPhenotypicAbnormalityValidator(TestBaseRuleValidator):
 
     def setUp(self) -> None:
         self.validator = PhenotypicAbnormalityValidator(self.o)
 
     def test_ok_input_produces_no_errors(self):
         results = self.validator.validate(self.example_terms)
         self.assertTrue(results.is_ok())
 
     @ddt.data(
-        ("HP:0012823", "HP:0012823", "Clinical modifier"),
-        ("HP:0003825", 'HP:0003828', "Variable expressivity"),
-        ("HP:0003621", 'HP:0003621', "Juvenile onset"),
+        ("HP:0012823",),  # Clinical modifier
+        ("HP:0003825",),  # Variable expressivity
+        ("HP:0003621",),  # Juvenile onset
     )
     @ddt.unpack
-    def test_clinical_modifier_presence_produces_error(self, query_id, current_id, name):
+    def test_presence_of_clinical_modifier_produces_error(self, curie):
         example_terms = list(self.example_terms)
-        example_terms.append(
-            MinimalTerm.create_minimal_term(
-                TermId.from_curie(query_id), name=name, alt_term_ids=[], is_obsolete=False)
-        )
+        example_terms.append(SimpleFeature(curie, True))
         results = self.validator.validate(example_terms)
         self.assertFalse(results.is_ok())
         self.assertEqual(results.results[0],
                          ValidationResult(level=ValidationLevel.ERROR, category='phenotypic_abnormality_descendant',
-                                          message=f'{name} [{current_id}] is not a descendant of '
+                                          message=f'{self.o.get_term(curie).name} [{self.o.get_term(curie).identifier.value}] is not a descendant of '
                                                   'Phenotypic abnormality [HP:0000118]'))
 
 
 @ddt.ddt
 class TestObsoleteTermIdsValidator(TestBaseRuleValidator):
 
     def setUp(self) -> None:
         self.validator = ObsoleteTermIdsValidator(self.o)
 
     def test_ok_input_produces_no_errors(self):
         results = self.validator.validate(self.example_terms)
         self.assertTrue(results.is_ok())
 
-    @ddt.data(
-        ("HP:0006010", 'HP:0100807', "Long fingers"),
-    )
-    @ddt.unpack
-    def test_clinical_modifier_presence_produces_error(self, query_id, current_id, name):
+    def test_presence_of_an_obsolete_term_produces_error(self):
+        curie = 'HP:0006010'  # obsolete Long fingers
         example_terms = list(self.example_terms)
-        example_terms.append(
-            MinimalTerm.create_minimal_term(
-                TermId.from_curie(query_id), name=name, alt_term_ids=[], is_obsolete=False)
-        )
+        example_terms.append(SimpleFeature(curie, True))
         results = self.validator.validate(example_terms)
         self.assertFalse(results.is_ok())
         self.assertEqual(results.results[0],
                          ValidationResult(level=ValidationLevel.WARNING, category='obsolete_term_id_is_used',
-                                          message=f'Using the obsolete {query_id} instead of {current_id} for {name}'))
+                                          message=f'Using the obsolete {curie} instead of '
+                                                  f'{self.o.get_term(curie).identifier.value} '
+                                                  f'for {self.o.get_term(curie).name}'))
```

