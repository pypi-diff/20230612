# Comparing `tmp/prometheus-summary-0.1.0.tar.gz` & `tmp/prometheus-summary-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-summary-0.1.0.tar", last modified: Mon Jun 12 08:50:31 2023, max compression
+gzip compressed data, was "prometheus-summary-0.1.1.tar", last modified: Mon Jun 12 14:01:54 2023, max compression
```

## Comparing `prometheus-summary-0.1.0.tar` & `prometheus-summary-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/prometheus_summary/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/prometheus_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/prometheus_summary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/prometheus_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 08:50:31.000000 prometheus-summary-0.1.0/prometheus_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 08:50:31.388771 prometheus-summary-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-12 08:50:18.000000 prometheus-summary-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/prometheus_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/prometheus_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/prometheus_summary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/prometheus_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/setup.py
```

### Comparing `prometheus-summary-0.1.0/LICENSE` & `prometheus-summary-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-summary-0.1.0/PKG-INFO` & `prometheus-summary-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-summary
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prometheus summary with quantiles over configurable sliding time window
 Home-page: https://github.com/RefaceAI/prometheus-summary
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 
 # prometheus-summary
 Prometheus summary with quantiles over configurable sliding time window
 
 ## Installation
 
 ```
-pip install prometheus-summary==0.1.0
+pip install prometheus-summary==0.1.1
 ```
 This package can be found on [PyPI](https://pypi.org/project/prometheus-summary/).
 
 ## Collecting
 
 ### Basic usage
```

### Comparing `prometheus-summary-0.1.0/README.md` & `prometheus-summary-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # prometheus-summary
 Prometheus summary with quantiles over configurable sliding time window
 
 ## Installation
 
 ```
-pip install prometheus-summary==0.1.0
+pip install prometheus-summary==0.1.1
 ```
 This package can be found on [PyPI](https://pypi.org/project/prometheus-summary/).
 
 ## Collecting
 
 ### Basic usage
```

### Comparing `prometheus-summary-0.1.0/prometheus_summary/__init__.py` & `prometheus-summary-0.1.1/prometheus_summary/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,18 @@
         self._estimator = TimeWindowEstimator(
             *self._invariants,
             max_age_seconds=self._max_age_seconds,
             age_buckets=self._age_buckets,
         )
 
     def observe(self, amount):
+        if not isinstance(amount, (float, int)):
+            raise TypeError("Summary only works with int or float")
+
+        amount = float(amount)
         super().observe(amount)
         self._estimator.observe(amount)
 
     def _child_samples(self):
         default_samples = super()._child_samples()
         quantile_samples = tuple(
             Sample("", {"quantile": str(quantile)}, self._estimator.query(quantile), None, None)
```

### Comparing `prometheus-summary-0.1.0/prometheus_summary.egg-info/PKG-INFO` & `prometheus-summary-0.1.1/prometheus_summary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-summary
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prometheus summary with quantiles over configurable sliding time window
 Home-page: https://github.com/RefaceAI/prometheus-summary
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 
 # prometheus-summary
 Prometheus summary with quantiles over configurable sliding time window
 
 ## Installation
 
 ```
-pip install prometheus-summary==0.1.0
+pip install prometheus-summary==0.1.1
 ```
 This package can be found on [PyPI](https://pypi.org/project/prometheus-summary/).
 
 ## Collecting
 
 ### Basic usage
```

### Comparing `prometheus-summary-0.1.0/setup.py` & `prometheus-summary-0.1.1/setup.py`

 * *Files identical despite different names*

