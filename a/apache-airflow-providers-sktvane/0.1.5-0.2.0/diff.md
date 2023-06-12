# Comparing `tmp/apache-airflow-providers-sktvane-0.1.5.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.1.5.tar", last modified: Tue May 23 04:40:37 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.2.0.tar", last modified: Mon Jun 12 04:46:43 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.1.5.tar` & `apache-airflow-providers-sktvane-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 04:40:37.150298 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 04:40:37.000000 apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 04:40:37.154298 apache-airflow-providers-sktvane-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-23 04:40:32.000000 apache-airflow-providers-sktvane-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.789150 apache-airflow-providers-sktvane-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-12 04:46:43.789150 apache-airflow-providers-sktvane-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.781150 apache-airflow-providers-sktvane-0.2.0/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.781150 apache-airflow-providers-sktvane-0.2.0/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.785150 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.789150 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.789150 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.789150 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.789150 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/tests/operator_nes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:46:43.789150 apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-12 04:46:43.000000 apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-12 04:46:43.000000 apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:46:43.000000 apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 04:46:43.000000 apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 04:46:43.000000 apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 04:46:43.793150 apache-airflow-providers-sktvane-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-12 04:46:36.000000 apache-airflow-providers-sktvane-0.2.0/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.1.5/PKG-INFO` & `apache-airflow-providers-sktvane-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.1.5
+Version: 0.2.0
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.1.5/README.md` & `apache-airflow-providers-sktvane-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/gcp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from google.cloud import bigquery
+from google.cloud import bigquery, storage
 from google.oauth2 import service_account
 
 from ..macros.vault import get_secrets
 
 
 def _get_credentials():
     key = get_secrets("gcp/skt-datahub/dataflow")["config"]
@@ -19,7 +19,14 @@
 
 def bigquery_client():
     return bigquery.Client(
         credentials=_get_credentials(),
         project="skt-datahub",
         location="asia-northeast3",
     )
+
+
+def gcs_client():
+    return storage.Client(
+        credentials=_get_credentials(),
+        project="skt-datahub",
+    )
```

### Comparing `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/macros/slack_notifier.py` & `apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/macros/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.5/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.2.0/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.1.5
+Version: 0.2.0
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
```

### Comparing `apache-airflow-providers-sktvane-0.1.5/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.2.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 airflow/providers/sktvane/macros/slack_notifier.py
 airflow/providers/sktvane/macros/vault.py
 airflow/providers/sktvane/operators/__init__.py
 airflow/providers/sktvane/operators/nes.py
 airflow/providers/sktvane/sensors/__init__.py
 airflow/providers/sktvane/sensors/gcp.py
 airflow/providers/sktvane/tests/__init__.py
+airflow/providers/sktvane/tests/operator_nes_test.py
 airflow/providers/sktvane/tests/test.py
 apache_airflow_providers_sktvane.egg-info/PKG-INFO
 apache_airflow_providers_sktvane.egg-info/SOURCES.txt
 apache_airflow_providers_sktvane.egg-info/dependency_links.txt
 apache_airflow_providers_sktvane.egg-info/requires.txt
 apache_airflow_providers_sktvane.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-sktvane-0.1.5/setup.py` & `apache-airflow-providers-sktvane-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="0.1.5",
+    version="0.2.0",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

