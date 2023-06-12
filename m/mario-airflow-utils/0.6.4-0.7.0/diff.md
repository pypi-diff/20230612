# Comparing `tmp/mario_airflow_utils-0.6.4.tar.gz` & `tmp/mario_airflow_utils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tom/code/mario_airflow_utils/dist/.tmp-9ivwoxev/mario_airflow_utils-0.6.4.tar", last modified: Fri Jun  9 04:54:33 2023, max compression
+gzip compressed data, was "/home/tom/code/mario_airflow_utils/dist/.tmp-40ch3bs0/mario_airflow_utils-0.7.0.tar", last modified: Mon Jun 12 01:38:54 2023, max compression
```

## Comparing `mario_airflow_utils-0.6.4.tar` & `mario_airflow_utils-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/
--rw-r--r--   0 tom       (1000) tom       (1000)    35149 2023-06-09 02:31:03.000000 mario_airflow_utils-0.6.4/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      996 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      399 2023-06-09 02:31:03.000000 mario_airflow_utils-0.6.4/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)      103 2023-06-09 02:31:03.000000 mario_airflow_utils-0.6.4/pyproject.toml
--rw-r--r--   0 tom       (1000) tom       (1000)      820 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/setup.cfg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils/
--rw-r--r--   0 tom       (1000) tom       (1000)      192 2023-06-09 04:53:35.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1205 2023-06-09 04:53:15.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils/mario_airflow_utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      996 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       70 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       20 2023-06-09 04:54:33.000000 mario_airflow_utils-0.6.4/src/mario_airflow_utils.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 01:38:54.000000 mario_airflow_utils-0.7.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)    35149 2023-06-09 02:31:03.000000 mario_airflow_utils-0.7.0/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      996 2023-06-12 01:38:54.000000 mario_airflow_utils-0.7.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      399 2023-06-09 02:31:03.000000 mario_airflow_utils-0.7.0/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)      103 2023-06-09 02:31:03.000000 mario_airflow_utils-0.7.0/pyproject.toml
+-rw-r--r--   0 tom       (1000) tom       (1000)      820 2023-06-12 01:38:54.000000 mario_airflow_utils-0.7.0/setup.cfg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 01:38:54.000000 mario_airflow_utils-0.7.0/src/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 01:38:54.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils/
+-rw-r--r--   0 tom       (1000) tom       (1000)      192 2023-06-09 04:53:35.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2449 2023-06-12 01:37:41.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils/mario_airflow_utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 01:38:54.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      996 2023-06-12 01:38:53.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2023-06-12 01:38:53.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-12 01:38:53.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       70 2023-06-12 01:38:53.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       20 2023-06-12 01:38:53.000000 mario_airflow_utils-0.7.0/src/mario_airflow_utils.egg-info/top_level.txt
```

### Comparing `mario_airflow_utils-0.6.4/LICENSE` & `mario_airflow_utils-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mario_airflow_utils-0.6.4/PKG-INFO` & `mario_airflow_utils-0.7.0/src/mario_airflow_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mario_airflow_utils
-Version: 0.6.4
+Name: mario-airflow-utils
+Version: 0.7.0
 Summary: apache airflow utils
 Home-page: https://dMario24.github.io/mario_airflow_utils
 Author: dMario24
 Author-email: data.mario24@gmail.com
 License: GNU General Public License (GPL)
 Project-URL: Bug Tracker, https://github.com/dMario24/mario_airflow_utils/issues
 Platform: macOS
```

### Comparing `mario_airflow_utils-0.6.4/setup.cfg` & `mario_airflow_utils-0.7.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mario_airflow_utils
-version = 0.6.4
+version = 0.7.0
 author = dMario24
 author_email = data.mario24@gmail.com
 description = apache airflow utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://dMario24.github.io/mario_airflow_utils
 project_urls =
```

### Comparing `mario_airflow_utils-0.6.4/src/mario_airflow_utils.egg-info/PKG-INFO` & `mario_airflow_utils-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mario-airflow-utils
-Version: 0.6.4
+Name: mario_airflow_utils
+Version: 0.7.0
 Summary: apache airflow utils
 Home-page: https://dMario24.github.io/mario_airflow_utils
 Author: dMario24
 Author-email: data.mario24@gmail.com
 License: GNU General Public License (GPL)
 Project-URL: Bug Tracker, https://github.com/dMario24/mario_airflow_utils/issues
 Platform: macOS
```

