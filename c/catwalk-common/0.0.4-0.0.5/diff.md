# Comparing `tmp/catwalk_common-0.0.4.tar.gz` & `tmp/catwalk_common-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catwalk_common-0.0.4.tar", last modified: Mon May  8 14:18:18 2023, max compression
+gzip compressed data, was "catwalk_common-0.0.5.tar", last modified: Mon Jun 12 14:15:52 2023, max compression
```

## Comparing `catwalk_common-0.0.4.tar` & `catwalk_common-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/
--rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)       49 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/README.md
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/catwalk_common/
--rw-rw-r--   0 marek     (1000) marek     (1000)       86 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/catwalk_common/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     1616 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/catwalk_common/_common_case_format.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2225 2023-03-08 14:21:41.000000 catwalk_common-0.0.4/catwalk_common/plugins.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/catwalk_common.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      304 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       16 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-05-08 14:18:18.000000 catwalk_common-0.0.4/catwalk_common.egg-info/top_level.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)      603 2023-05-08 13:58:38.000000 catwalk_common-0.0.4/pyproject.toml
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-05-08 14:18:18.983118 catwalk_common-0.0.4/setup.cfg
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)       49 2023-06-12 07:47:42.000000 catwalk_common-0.0.5/README.md
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/catwalk_common/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      127 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     1698 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/_ccf_dataframe.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2942 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/_common_case_format.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2236 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/plugins.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/catwalk_common.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      337 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       30 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/top_level.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)      622 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/pyproject.toml
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/setup.cfg
```

### Comparing `catwalk_common-0.0.4/PKG-INFO` & `catwalk_common-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk_common
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Marek Połom <marek.polom@deepsense.ai>
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `catwalk_common-0.0.4/catwalk_common/plugins.py` & `catwalk_common-0.0.5/catwalk_common/plugins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import List, Any, Type
+from typing import Type, Optional, List
 
-from pydantic import BaseModel, create_model
+from pydantic import BaseModel
 
 
 class CatwalkDataType(BaseModel):
     key: str
     description: str
     example: dict
-    json_schema: dict = None
+    json_schema: Optional[dict] = None
     src: str
     main: str
 
 
 class CatwalkEvaluation(BaseModel):
     key: str
     description: str
     example: dict
-    json_schema: dict = None
+    json_schema: Optional[dict] = None
     src: str
     main: str
 
 
 class BaseDateType(BaseModel):
     name: str
```

### Comparing `catwalk_common-0.0.4/catwalk_common.egg-info/PKG-INFO` & `catwalk_common-0.0.5/catwalk_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk-common
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Marek Połom <marek.polom@deepsense.ai>
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

