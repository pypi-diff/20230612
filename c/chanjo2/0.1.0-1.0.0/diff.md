# Comparing `tmp/chanjo2-0.1.0.tar.gz` & `tmp/chanjo2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanjo2-0.1.0.tar", max compression
+gzip compressed data, was "chanjo2-1.0.0.tar", max compression
```

## Comparing `chanjo2-0.1.0.tar` & `chanjo2-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,26 @@
--rw-r--r--   0        0        0     1073 2022-02-18 13:57:11.317041 chanjo2-0.1.0/LICENSE
--rw-r--r--   0        0        0      414 2022-02-18 12:30:18.898295 chanjo2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       21 2022-02-18 12:30:32.254299 chanjo2-0.1.0/src/chanjo2/__init__.py
--rw-r--r--   0        0        0      321 2022-02-18 12:30:32.254537 chanjo2-0.1.0/src/chanjo2/dependencies.py
--rw-r--r--   0        0        0        0 2021-12-02 14:18:46.715091 chanjo2-0.1.0/src/chanjo2/endpoints/__init__.py
--rw-r--r--   0        0        0     4021 2022-02-18 12:30:32.254884 chanjo2-0.1.0/src/chanjo2/endpoints/individuals.py
--rw-r--r--   0        0        0     1129 2022-02-18 12:30:32.255179 chanjo2-0.1.0/src/chanjo2/endpoints/regions.py
--rw-r--r--   0        0        0     1143 2022-02-18 12:30:32.255599 chanjo2-0.1.0/src/chanjo2/main.py
--rw-r--r--   0        0        0        0 2022-02-18 12:30:32.255699 chanjo2-0.1.0/src/chanjo2/meta/__init__.py
--rw-r--r--   0        0        0      487 2022-02-18 12:30:32.256123 chanjo2-0.1.0/src/chanjo2/meta/handle_bed.py
--rw-r--r--   0        0        0        0 2021-12-02 14:18:46.715366 chanjo2-0.1.0/src/chanjo2/models/__init__.py
--rw-r--r--   0        0        0      185 2022-02-18 12:30:32.256464 chanjo2-0.1.0/src/chanjo2/models/coverage_interval.py
--rw-r--r--   0        0        0      390 2022-02-18 12:30:32.256690 chanjo2-0.1.0/src/chanjo2/models/individuals.py
--rw-r--r--   0        0        0      362 2022-02-18 12:30:32.256858 chanjo2-0.1.0/src/chanjo2/models/regions.py
--rw-r--r--   0        0        0      817 2022-02-18 13:59:18.232771 chanjo2-0.1.0/setup.py
--rw-r--r--   0        0        0      542 2022-02-18 13:59:18.232950 chanjo2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      729 2023-06-12 11:23:58.810682 chanjo2-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/__init__.py
+-rw-r--r--   0        0        0     3099 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/constants.py
+-rw-r--r--   0        0        0     2743 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/crud/cases.py
+-rw-r--r--   0        0        0     5309 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/crud/intervals.py
+-rw-r--r--   0        0        0     3110 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/crud/samples.py
+-rw-r--r--   0        0        0     1067 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/dbutil.py
+-rw-r--r--   0        0        0      346 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/demo/109_green.bed
+-rw-r--r--   0        0        0      292 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/demo/__init__.py
+-rw-r--r--   0        0        0   450444 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/demo/panelapp_109_example.d4
+-rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/__init__.py
+-rw-r--r--   0        0        0     1588 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/cases.py
+-rw-r--r--   0        0        0     6649 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/coverage.py
+-rw-r--r--   0        0        0     5278 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/intervals.py
+-rw-r--r--   0        0        0     2018 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/samples.py
+-rw-r--r--   0        0        0     1690 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/__init__.py
+-rw-r--r--   0        0        0      694 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_bed.py
+-rw-r--r--   0        0        0     6816 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_d4.py
+-rw-r--r--   0        0        0     7707 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_load_intervals.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_query_intervals.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/models/__init__.py
+-rw-r--r--   0        0        0     3913 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/models/pydantic_models.py
+-rw-r--r--   0        0        0     4360 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/models/sql_models.py
+-rw-r--r--   0        0        0     2999 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/populate_demo.py
+-rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 chanjo2-1.0.0/PKG-INFO
```

