# Comparing `tmp/sharry-jira-tool-0.2.5.tar.gz` & `tmp/sharry-jira-tool-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharry-jira-tool-0.2.5.tar", last modified: Tue Apr 11 06:33:53 2023, max compression
+gzip compressed data, was "sharry-jira-tool-0.2.6.tar", last modified: Mon Jun 12 07:52:21 2023, max compression
```

## Comparing `sharry-jira-tool-0.2.5.tar` & `sharry-jira-tool-0.2.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.814945 sharry-jira-tool-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.814945 sharry-jira-tool-0.2.5/src/jira_tool/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.814945 sharry-jira-tool-0.2.5/src/jira_tool/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/assets/excel_definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/assets/sprint_schedule.json
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/src/jira_tool/story.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 06:33:53.000000 sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:33:53.818946 sharry-jira-tool-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_console_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_excel_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_excel_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_jira_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_sprint_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-11 06:33:44.000000 sharry-jira-tool-0.2.5/tests/test_story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:52:21.510012 sharry-jira-tool-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-12 07:52:21.510012 sharry-jira-tool-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 07:52:21.510012 sharry-jira-tool-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:52:21.502012 sharry-jira-tool-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:52:21.506013 sharry-jira-tool-0.2.6/src/jira_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:52:21.506013 sharry-jira-tool-0.2.6/src/jira_tool/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    12224 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/assets/excel_definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/assets/sprint_schedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21946 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/src/jira_tool/story.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:52:21.510012 sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-12 07:52:21.000000 sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-12 07:52:21.000000 sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:52:21.000000 sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 07:52:21.000000 sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-12 07:52:21.000000 sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 07:52:21.000000 sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:52:21.510012 sharry-jira-tool-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_console_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_excel_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_excel_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_jira_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_sprint_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-06-12 07:51:57.000000 sharry-jira-tool-0.2.6/tests/test_story.py
```

### Comparing `sharry-jira-tool-0.2.5/LICENSE` & `sharry-jira-tool-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/PKG-INFO` & `sharry-jira-tool-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharry-jira-tool
-Version: 0.2.5
+Version: 0.2.6
 Summary: Sort Jira stories in Excel
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,19 +31,19 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
-Important!!!
-============
-We will no longer add new features or fix bugs for this project. 
-All new features/requirements/bug fixes will be move to package: jira-assistant <https://pypi.org/project/jira-assistant>.
-Welcome to provide your good advices as always!
+########################
+⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
+########################
+
+⚠️⚠️⚠️ The :code:`sharry-jira-tool` PyPI package is deprecated use :code:`jira-assistant` instead ⚠️⚠️⚠️
 
 Jira Tool - userful tool to sort jira stories
 =============================================
 
 |pypi| |python 3.11| |python 3.11 (Mac OS)| |CodeQL| |Documentation|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/sharry-jira-tool.svg?style=flat-square
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sharry-jira-tool-0.2.5/README.rst` & `sharry-jira-tool-0.2.6/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Important!!!
-============
-We will no longer add new features or fix bugs for this project. 
-All new features/requirements/bug fixes will be move to package: jira-assistant <https://pypi.org/project/jira-assistant>.
-Welcome to provide your good advices as always!
+########################
+⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
+########################
+
+⚠️⚠️⚠️ The :code:`sharry-jira-tool` PyPI package is deprecated use :code:`jira-assistant` instead ⚠️⚠️⚠️
 
 Jira Tool - userful tool to sort jira stories
 =============================================
 
 |pypi| |python 3.11| |python 3.11 (Mac OS)| |CodeQL| |Documentation|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/sharry-jira-tool.svg?style=flat-square
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sharry-jira-tool-0.2.5/pyproject.toml` & `sharry-jira-tool-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sharry-jira-tool"
-version = "0.2.5"
+version = "0.2.6"
 description = "Sort Jira stories in Excel"
 readme = "README.rst"
 authors = [{ name = "Sharry Xu", email = "sharry.xu@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -17,14 +17,15 @@
 keywords = ["jira", "excel", "jira-cloud"]
 dependencies = [
     "openpyxl >= 3.0.10",
     "python-dateutil >= 2.8.2",
     "python-dotenv >= 0.21.1",
     "requests >= 2.28.2",
     'tomli; python_version < "3.11"',
+    "jira-assistant",
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
 
 [project.urls]
```

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/__init__.py` & `sharry-jira-tool-0.2.6/src/jira_tool/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # -*- coding: utf-8 -*-
 from importlib import metadata
 from importlib.metadata import version
+import warnings
+
+warnings.warn("This package has been deprecated. Please install the `jira-assistant` package instead")
 
 from .console_script import generate_template, sort_excel_file, update_jira_info
 from .excel_definition import ExcelDefinition, ExcelDefinitionColumn
 from .excel_operation import (
     output_to_csv_file,
     output_to_excel_file,
     process_excel_file,
```

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/assets/excel_definition.json` & `sharry-jira-tool-0.2.6/src/jira_tool/assets/excel_definition.json`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/assets/sprint_schedule.json` & `sharry-jira-tool-0.2.6/src/jira_tool/assets/sprint_schedule.json`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/console_script.py` & `sharry-jira-tool-0.2.6/src/jira_tool/console_script.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/excel_definition.py` & `sharry-jira-tool-0.2.6/src/jira_tool/excel_definition.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/excel_operation.py` & `sharry-jira-tool-0.2.6/src/jira_tool/excel_operation.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/jira_client.py` & `sharry-jira-tool-0.2.6/src/jira_tool/jira_client.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/milestone.py` & `sharry-jira-tool-0.2.6/src/jira_tool/milestone.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/priority.py` & `sharry-jira-tool-0.2.6/src/jira_tool/priority.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/sprint_schedule.py` & `sharry-jira-tool-0.2.6/src/jira_tool/sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/jira_tool/story.py` & `sharry-jira-tool-0.2.6/src/jira_tool/story.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/PKG-INFO` & `sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharry-jira-tool
-Version: 0.2.5
+Version: 0.2.6
 Summary: Sort Jira stories in Excel
 Author-email: Sharry Xu <sharry.xu@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Sharry Xu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,19 +31,19 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
-Important!!!
-============
-We will no longer add new features or fix bugs for this project. 
-All new features/requirements/bug fixes will be move to package: jira-assistant <https://pypi.org/project/jira-assistant>.
-Welcome to provide your good advices as always!
+########################
+⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
+########################
+
+⚠️⚠️⚠️ The :code:`sharry-jira-tool` PyPI package is deprecated use :code:`jira-assistant` instead ⚠️⚠️⚠️
 
 Jira Tool - userful tool to sort jira stories
 =============================================
 
 |pypi| |python 3.11| |python 3.11 (Mac OS)| |CodeQL| |Documentation|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/sharry-jira-tool.svg?style=flat-square
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sharry-jira-tool-0.2.5/src/sharry_jira_tool.egg-info/SOURCES.txt` & `sharry-jira-tool-0.2.6/src/sharry_jira_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_console_script.py` & `sharry-jira-tool-0.2.6/tests/test_console_script.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_excel_definition.py` & `sharry-jira-tool-0.2.6/tests/test_excel_definition.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_excel_operation.py` & `sharry-jira-tool-0.2.6/tests/test_excel_operation.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_jira_client.py` & `sharry-jira-tool-0.2.6/tests/test_jira_client.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_milestone.py` & `sharry-jira-tool-0.2.6/tests/test_milestone.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_priority.py` & `sharry-jira-tool-0.2.6/tests/test_priority.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_sprint_schedule.py` & `sharry-jira-tool-0.2.6/tests/test_sprint_schedule.py`

 * *Files identical despite different names*

### Comparing `sharry-jira-tool-0.2.5/tests/test_story.py` & `sharry-jira-tool-0.2.6/tests/test_story.py`

 * *Files identical despite different names*

