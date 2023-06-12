# Comparing `tmp/aioprometheus-summary-0.0.2.tar.gz` & `tmp/aioprometheus-summary-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioprometheus-summary-0.0.2.tar", last modified: Fri Jun  9 14:22:52 2023, max compression
+gzip compressed data, was "aioprometheus-summary-0.1.0.tar", last modified: Mon Jun 12 08:49:40 2023, max compression
```

## Comparing `aioprometheus-summary-0.0.2.tar` & `aioprometheus-summary-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:22:52.283922 aioprometheus-summary-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 14:22:37.000000 aioprometheus-summary-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 14:22:52.283922 aioprometheus-summary-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 14:22:37.000000 aioprometheus-summary-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:22:52.283922 aioprometheus-summary-0.0.2/aioprometheus_summary/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-09 14:22:37.000000 aioprometheus-summary-0.0.2/aioprometheus_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 14:22:37.000000 aioprometheus-summary-0.0.2/aioprometheus_summary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:22:52.283922 aioprometheus-summary-0.0.2/aioprometheus_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 14:22:52.000000 aioprometheus-summary-0.0.2/aioprometheus_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-09 14:22:52.000000 aioprometheus-summary-0.0.2/aioprometheus_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:22:52.000000 aioprometheus-summary-0.0.2/aioprometheus_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 14:22:52.000000 aioprometheus-summary-0.0.2/aioprometheus_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 14:22:52.000000 aioprometheus-summary-0.0.2/aioprometheus_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:22:52.283922 aioprometheus-summary-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-09 14:22:37.000000 aioprometheus-summary-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:49:40.615719 aioprometheus-summary-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 08:49:29.000000 aioprometheus-summary-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-12 08:49:40.615719 aioprometheus-summary-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-12 08:49:29.000000 aioprometheus-summary-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:49:40.615719 aioprometheus-summary-0.1.0/aioprometheus_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-12 08:49:29.000000 aioprometheus-summary-0.1.0/aioprometheus_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 08:49:29.000000 aioprometheus-summary-0.1.0/aioprometheus_summary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:49:40.615719 aioprometheus-summary-0.1.0/aioprometheus_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-12 08:49:40.000000 aioprometheus-summary-0.1.0/aioprometheus_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-12 08:49:40.000000 aioprometheus-summary-0.1.0/aioprometheus_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:49:40.000000 aioprometheus-summary-0.1.0/aioprometheus_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 08:49:40.000000 aioprometheus-summary-0.1.0/aioprometheus_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 08:49:40.000000 aioprometheus-summary-0.1.0/aioprometheus_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:49:40.615719 aioprometheus-summary-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-12 08:49:29.000000 aioprometheus-summary-0.1.0/setup.py
```

### Comparing `aioprometheus-summary-0.0.2/LICENSE` & `aioprometheus-summary-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioprometheus-summary-0.0.2/aioprometheus_summary/__init__.py` & `aioprometheus-summary-0.1.0/aioprometheus_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `aioprometheus-summary-0.0.2/setup.py` & `aioprometheus-summary-0.1.0/setup.py`

 * *Files identical despite different names*

