# Comparing `tmp/m-abac-test-1.0.5.tar.gz` & `tmp/m-abac-test-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-test-1.0.5.tar", last modified: Sat Jun  3 02:38:06 2023, max compression
+gzip compressed data, was "m-abac-test-1.0.6.tar", last modified: Mon Jun 12 07:43:36 2023, max compression
```

## Comparing `m-abac-test-1.0.5.tar` & `m-abac-test-1.0.6.tar`

### file list

```diff
@@ -1,97 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.057211 m-abac-test-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-03 02:38:06.056211 m-abac-test-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.006209 m-abac-test-1.0.5/m_abac_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3725 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/m_abac_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:05.996209 m-abac-test-1.0.5/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:05.997209 m-abac-test-1.0.5/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.010209 m-abac-test-1.0.5/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.011209 m-abac-test-1.0.5/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7883 2023-06-03 02:36:04.000000 m-abac-test-1.0.5/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.5/mobio/libs/abac/config.py
--rw-r--r--   0 root         (0) root         (0)    13656 2023-06-03 02:36:04.000000 m-abac-test-1.0.5/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.015210 m-abac-test-1.0.5/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.016209 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.018210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.026210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.031210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.037210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.040210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.045210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.048210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 02:38:06.055210 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6037 2023-05-19 09:33:30.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     4976 2023-06-03 02:36:04.000000 m-abac-test-1.0.5/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 02:38:06.057211 m-abac-test-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9779 2023-06-03 02:38:05.000000 m-abac-test-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.550856 m-abac-test-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-12 07:43:36.549856 m-abac-test-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.496855 m-abac-test-1.0.6/m_abac_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-12 07:43:36.000000 m-abac-test-1.0.6/m_abac_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-12 07:43:36.000000 m-abac-test-1.0.6/m_abac_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 07:43:36.000000 m-abac-test-1.0.6/m_abac_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-12 07:43:36.000000 m-abac-test-1.0.6/m_abac_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-12 07:43:36.000000 m-abac-test-1.0.6/m_abac_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.486854 m-abac-test-1.0.6/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.487854 m-abac-test-1.0.6/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.500855 m-abac-test-1.0.6/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.502855 m-abac-test-1.0.6/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2023-06-03 02:36:04.000000 m-abac-test-1.0.6/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.6/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    15663 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.505855 m-abac-test-1.0.6/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.507855 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.509855 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.518855 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/any_contains.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.523855 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.529855 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.532856 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.537856 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.540856 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:43:36.548856 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-19 09:33:30.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     5139 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5143 2023-06-12 07:41:39.000000 m-abac-test-1.0.6/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 07:43:36.550856 m-abac-test-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9779 2023-06-12 07:43:35.000000 m-abac-test-1.0.6/setup.py
```

### Comparing `m-abac-test-1.0.5/PKG-INFO` & `m-abac-test-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.5
+Version: 1.0.6
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.5/README.md` & `m-abac-test-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/m_abac_test.egg-info/PKG-INFO` & `m-abac-test-1.0.6/m_abac_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.5
+Version: 1.0.6
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.5/m_abac_test.egg-info/SOURCES.txt` & `m-abac-test-1.0.6/m_abac_test.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 mobio/libs/abac/policy/conditions/schema.py
 mobio/libs/abac/policy/conditions/boolean/__init__.py
 mobio/libs/abac/policy/conditions/boolean/base.py
 mobio/libs/abac/policy/conditions/boolean/check_bool.py
 mobio/libs/abac/policy/conditions/collection/__init__.py
 mobio/libs/abac/policy/conditions/collection/all_in.py
 mobio/libs/abac/policy/conditions/collection/all_not_in.py
+mobio/libs/abac/policy/conditions/collection/any_contains.py
 mobio/libs/abac/policy/conditions/collection/any_in.py
+mobio/libs/abac/policy/conditions/collection/any_not_contains.py
 mobio/libs/abac/policy/conditions/collection/any_not_in.py
 mobio/libs/abac/policy/conditions/collection/base.py
 mobio/libs/abac/policy/conditions/collection/is_empty.py
 mobio/libs/abac/policy/conditions/collection/is_in.py
 mobio/libs/abac/policy/conditions/collection/is_not_empty.py
 mobio/libs/abac/policy/conditions/collection/is_not_in.py
 mobio/libs/abac/policy/conditions/date_time/__init__.py
```

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-test-1.0.6/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/call_api.py` & `m-abac-test-1.0.6/mobio/libs/abac/call_api.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/config.py` & `m-abac-test-1.0.6/mobio/libs/abac/config.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/pdp.py` & `m-abac-test-1.0.6/mobio/libs/abac/pdp.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                  user_info: dict = None, data_before: dict = None, data_after: dict = None, environment: dict = None,
                  account_type=AccountType.NORMAL):
         if not resource:
             raise ValueError("resource required")
         if not action:
             raise ValueError("action required")
         pass_policy = False
-        if not merchant_id or not account_id:
+        if account_type == self.AccountType.NORMAL and (not merchant_id or not account_id):
             auth_type, json_token = Utils.get_info_jwt()
             if auth_type == self.AuthorizationType.BEARER:
                 merchant_id = json_token.get("merchant_id")
                 account_id = json_token.get("account_id")
             else:
                 account_type = self.AccountType.SYSTEM
         if account_type == PolicyDecisionPoint.AccountType.NORMAL:
@@ -101,29 +101,17 @@
             :param request: request object
             :return: True if authorized else False
         """
         try:
             if self.pass_policy:
                 self.result_access.set_allow_access(True)
                 return self.result_access
-            action_info = CallAPI.admin_get_json_action(merchant_id=self.merchant_id)
-            if not action_info:
-                raise ValueError("action for merchant_id {} not found".format(self.merchant_id))
-            if not action_info.get(self.action):
-                raise ValueError("action {} not found".format(self.action))
-            self.access_level = action_info.get(self.action, {}).get("access_level", "").lower()
-            if not self.access_level:
-                raise ValueError("access_level {} not valid".format(self.action))
-            self.service = action_info.get(self.action, {}).get("service", "")
-            if not self.service:
-                raise ValueError("service {} not valid".format(self.service))
-
+            self.check_info_action()
             list_statement = self.get_policy_statement_for_target()
             if list_statement:
-
                 if self.access_level == PolicyDecisionPoint.AccessLevel.ADD:
                     self.data_after.update(self.data_before)
                 statement_check_allow, statement_check_deny = self.get_statement_by_type(list_statement)
                 if statement_check_deny:
                     if self.check_list_statement_is_deny(statement_check_deny):
                         self.result_access.set_allow_access(False)
                         return self.result_access
@@ -289,7 +277,59 @@
 
         except Exception as err:
             msg_err = "check_list_statement_is_allow err: {}".format(err)
             print(msg_err)
             self.result_access.add_log_error(msg_err)
             result_allow = False
         return result_allow
+
+    def check_info_action(self):
+        action_info = CallAPI.admin_get_json_action(merchant_id=self.merchant_id)
+        if not action_info:
+            raise ValueError("action for merchant_id {} not found".format(self.merchant_id))
+        if not action_info.get(self.action):
+            raise ValueError("action {} not found".format(self.action))
+        self.access_level = action_info.get(self.action, {}).get("access_level", "").lower()
+        if not self.access_level:
+            raise ValueError("access_level {} not valid".format(self.action))
+        self.service = action_info.get(self.action, {}).get("service", "")
+        if not self.service:
+            raise ValueError("service {} not valid".format(self.service))
+
+    def is_allowed_list(self, data: list):
+        """
+            Check if authorization request is allowed data
+        """
+        try:
+            if self.pass_policy:
+                self.result_access.set_allow_access(True)
+                self.result_access.data_allow = data
+                return self.result_access
+            self.check_info_action()
+            list_statement = self.get_policy_statement_for_target()
+            if list_statement:
+                statement_check_allow, statement_check_deny = self.get_statement_by_type(list_statement)
+                for item_data in data:
+                    self.data_after = item_data.get("data_after", {})
+                    self.data_before = item_data.get("data_before", {})
+                    self.request_access.update({
+                        self.resource: self.data_before if self.data_before else {}
+                    })
+                    if self.access_level == PolicyDecisionPoint.AccessLevel.ADD:
+                        self.data_after.update(self.data_before)
+                    if statement_check_deny:
+                        if self.check_list_statement_is_deny(statement_check_deny):
+                            continue
+                    if statement_check_allow and self.check_list_statement_is_allow(statement_check_allow):
+                        self.result_access.add_data_allow(item_data)
+                if self.result_access.get_data_allow():
+                    self.result_access.set_allow_access(True)
+                else:
+                    self.result_access.set_allow_access(False)
+            else:
+                self.result_access.set_allow_access(False)
+        except Exception as err:
+            msg_err = "is_allowed_list err: {}".format(err)
+            print(msg_err)
+            self.result_access.add_log_error(msg_err)
+            self.result_access.set_allow_access(False)
+        return self.result_access
```

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     Operation base class
 """
 
 from abc import ABCMeta, abstractmethod
 
 # from py_abac.context import EvaluationContext
-
+# what is value of field, values is list value policy
 MapAnyValue = ""
 
 class ConditionBase(metaclass=ABCMeta):
     """
         Base class for conditions
     """
```

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         "ListAllNotIn": AllNotInSchema,
         "ListAnyIn": AnyInSchema,
         "ListAnyNotIn": AnyNotInSchema,
         "ListIsEmpty": IsEmptySchema,
         "ListIsIn": IsInSchema,
         "ListIsNotEmpty": IsNotEmptySchema,
         "ListIsNotIn": IsNotInSchema,
+        "ListAnyContains": AnyContainsSchema,
+        "ListAnyNotContains": AnyNotContainsSchema,
 
         "DayEquals": DayEqSchema,
         "DayNotEquals": DayNeqSchema,
         "DayLessThan": DayLtSchema,
         "DayLessThanEquals": DayLteSchema,
         "DayGreaterThan": DayGtSchema,
         "DayGreaterThanEquals": DayGteSchema,
```

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,27 @@
         Condition for string `self.what` contains `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower() in i.lower():
+                    if i.lower() in self.what.lower():
                         return True
                 else:
-                    if self.what in i:
+                    if i in self.what:
                         return True
             return False
         else:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower() not in i.lower():
+                    if i.lower() not in self.what.lower():
                         return False
                 else:
-                    if self.what not in i:
+                    if i not in self.what:
                         return False
             return True
 
 class ContainsSchema(StringConditionSchema):
     """
         JSON schema for contains string conditions
     """
```

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,27 @@
         Condition for string `self.what` not contains `value`
     """
 
     def _is_satisfied(self) -> bool:
         if self.qualifier == self.Qualifier.ForAnyValue:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower() in i.lower():
+                    if i.lower() in self.what.lower():
                         return False
                 else:
-                    if self.what in i:
+                    if i in self.what:
                         return False
             return True
         else:
             for i in self.values:
                 if self.case_insensitive:
-                    if self.what.lower() in i.lower():
+                    if i.lower() in self.what.lower():
                         return False
                 else:
-                    if self.what in i:
+                    if i in self.what:
                         return False
             return True
 
 
 class NotContainsSchema(StringConditionSchema):
     """
         JSON schema for not contains string condition
```

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/exceptions.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/policy.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/policy/utils.py` & `m-abac-test-1.0.6/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.5/mobio/libs/abac/result_access.py` & `m-abac-test-1.0.6/mobio/libs/abac/result_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     def __init__(self):
         self.allow_access = False
         self.display_config = []
         self.filter_config = []
         self.log_statement_deny = []
         self.log_statement_allow = []
         self.log_error = []
+        self.data_allow = []
 
     def get_allow_access(self):
         if self.allow_access:
             print("statement_allow: {}".format(self.log_statement_allow))
         else:
             print("statement_deny: {}".format(self.log_statement_deny))
         print("log_error: {}".format(self.log_error))
@@ -118,7 +119,13 @@
                 })
             index_statement += 1
         for k, v in dict_exists.items():
             if k in dict_field:
                 list_filter_config[dict_field.get(k)[0]].get("condition")[dict_field.get(k)[1]].get("values").extend(
                     v.get("values"))
         return list_filter_config
+
+    def get_data_allow(self):
+        return self.data_allow
+
+    def add_data_allow(self, value):
+        self.data_allow.append(value)
```

### Comparing `m-abac-test-1.0.5/setup.py` & `m-abac-test-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.5'
+version_dev='1.0.6'
 version_prod='1.0.0'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.5',  # Required
+    version='1.0.6',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

