# Comparing `tmp/yetl-framework-1.5.0.dev1.tar.gz` & `tmp/yetl-framework-1.5.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.5.0.dev1.tar", last modified: Sat Jun 10 19:35:50 2023, max compression
+gzip compressed data, was "yetl-framework-1.5.0.dev2.tar", last modified: Sun Jun 11 22:14:56 2023, max compression
```

## Comparing `yetl-framework-1.5.0.dev1.tar` & `yetl-framework-1.5.0.dev2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16007 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3143 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9236 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4094 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.995067 yetl-framework-1.5.0.dev1/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-10 19:34:57.000000 yetl-framework-1.5.0.dev1/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-10 19:35:49.999067 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-10 19:35:49.000000 yetl-framework-1.5.0.dev1/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.177345 yetl-framework-1.5.0.dev2/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-11 22:14:56.177345 yetl-framework-1.5.0.dev2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-11 22:14:56.177345 yetl-framework-1.5.0.dev2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.173345 yetl-framework-1.5.0.dev2/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.173345 yetl-framework-1.5.0.dev2/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.173345 yetl-framework-1.5.0.dev2/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16007 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.173345 yetl-framework-1.5.0.dev2/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3143 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9270 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.173345 yetl-framework-1.5.0.dev2/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4094 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.177345 yetl-framework-1.5.0.dev2/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-11 22:14:00.000000 yetl-framework-1.5.0.dev2/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 22:14:56.177345 yetl-framework-1.5.0.dev2/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-11 22:14:56.000000 yetl-framework-1.5.0.dev2/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-06-11 22:14:56.000000 yetl-framework-1.5.0.dev2/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-11 22:14:56.000000 yetl-framework-1.5.0.dev2/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-11 22:14:56.000000 yetl-framework-1.5.0.dev2/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-11 22:14:56.000000 yetl-framework-1.5.0.dev2/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-11 22:14:56.000000 yetl-framework-1.5.0.dev2/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.5.0.dev1/PKG-INFO` & `yetl-framework-1.5.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.5.0.dev1
+Version: 1.5.0.dev2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.5.0.dev1/README.md` & `yetl-framework-1.5.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/setup.py` & `yetl-framework-1.5.0.dev2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.5.0.dev1",
+    version="1.5.0.dev2",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.5.0.dev1/yetl/__main__.py` & `yetl-framework-1.5.0.dev2/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/cli/_init.py` & `yetl-framework-1.5.0.dev2/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.5.0.dev2/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/__init__.py` & `yetl-framework-1.5.0.dev2/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_config.py` & `yetl-framework-1.5.0.dev2/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_decorators.py` & `yetl-framework-1.5.0.dev2/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_logging_config.py` & `yetl-framework-1.5.0.dev2/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_project.py` & `yetl-framework-1.5.0.dev2/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_spark_context.py` & `yetl-framework-1.5.0.dev2/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_tables.py` & `yetl-framework-1.5.0.dev2/yetl/config/_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
         **kwargs,
     ):
         return self.lookup_table(
             stage=stage,
             database=database,
             table=table,
             first_match=first_match,
+            create_database=True,
             create_table=True,
             **kwargs,
         )
 
     def lookup_table(
         self,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
```

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_timeslice.py` & `yetl-framework-1.5.0.dev2/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/_utils.py` & `yetl-framework-1.5.0.dev2/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/deltalake.py` & `yetl-framework-1.5.0.dev2/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/table/_deltalake.py` & `yetl-framework-1.5.0.dev2/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/table/_factory.py` & `yetl-framework-1.5.0.dev2/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/table/_read.py` & `yetl-framework-1.5.0.dev2/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/config/table/_table.py` & `yetl-framework-1.5.0.dev2/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/workflow/_dlt.py` & `yetl-framework-1.5.0.dev2/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.5.0.dev2/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.5.0.dev1/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.5.0.dev2/yetl_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.5.0.dev1
+Version: 1.5.0.dev2
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.5.0.dev1/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.5.0.dev2/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

