# Comparing `tmp/prometheus-summary-0.0.1.tar.gz` & `tmp/prometheus-summary-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-summary-0.0.1.tar", last modified: Fri Jun  9 14:36:31 2023, max compression
+gzip compressed data, was "prometheus-summary-0.1.0.tar", last modified: Mon Jun 12 08:50:31 2023, max compression
```

## Comparing `prometheus-summary-0.0.1.tar` & `prometheus-summary-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:36:31.052601 prometheus-summary-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 14:36:17.000000 prometheus-summary-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-09 14:36:31.052601 prometheus-summary-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-09 14:36:17.000000 prometheus-summary-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:36:31.052601 prometheus-summary-0.0.1/prometheus_summary/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-09 14:36:17.000000 prometheus-summary-0.0.1/prometheus_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 14:36:17.000000 prometheus-summary-0.0.1/prometheus_summary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:36:31.052601 prometheus-summary-0.0.1/prometheus_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-09 14:36:30.000000 prometheus-summary-0.0.1/prometheus_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 14:36:31.000000 prometheus-summary-0.0.1/prometheus_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:36:30.000000 prometheus-summary-0.0.1/prometheus_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 14:36:30.000000 prometheus-summary-0.0.1/prometheus_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 14:36:30.000000 prometheus-summary-0.0.1/prometheus_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:36:31.056602 prometheus-summary-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-09 14:36:17.000000 prometheus-summary-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/prometheus_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/prometheus_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/prometheus_summary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/prometheus_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/setup.py
```

### Comparing `prometheus-summary-0.0.1/LICENSE` & `prometheus-summary-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-summary-0.0.1/prometheus_summary/__init__.py` & `prometheus-summary-0.1.0/prometheus_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `prometheus-summary-0.0.1/setup.py` & `prometheus-summary-0.1.0/setup.py`

 * *Files identical despite different names*

