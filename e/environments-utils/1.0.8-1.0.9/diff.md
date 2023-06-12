# Comparing `tmp/environments_utils-1.0.8.tar.gz` & `tmp/environments_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/environments_utils-1.0.8.tar", last modified: Fri Aug 26 17:42:18 2022, max compression
+gzip compressed data, was "dist/environments_utils-1.0.9.tar", last modified: Fri Sep 30 11:31:51 2022, max compression
```

## Comparing `environments_utils-1.0.8.tar` & `environments_utils-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-08-26 17:42:18.000000 environments_utils-1.0.8/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1073 2022-08-15 18:21:12.000000 environments_utils-1.0.8/LICENSE
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2022-08-15 18:21:12.000000 environments_utils-1.0.8/MANIFEST.in
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4642 2022-08-26 17:42:18.000000 environments_utils-1.0.8/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3172 2022-08-26 17:40:02.000000 environments_utils-1.0.8/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-08-26 17:42:18.000000 environments_utils-1.0.8/environments_utils/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      859 2022-08-26 17:17:29.000000 environments_utils-1.0.8/environments_utils/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       74 2022-08-26 17:41:16.000000 environments_utils-1.0.8/environments_utils/__version__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      524 2022-08-15 18:21:12.000000 environments_utils-1.0.8/environments_utils/is_architecture.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1183 2022-08-15 18:29:16.000000 environments_utils-1.0.8/environments_utils/is_cluster.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      359 2022-08-15 18:21:12.000000 environments_utils-1.0.8/environments_utils/is_notebook.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      334 2022-08-26 17:16:32.000000 environments_utils-1.0.8/environments_utils/is_online.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      575 2022-08-15 18:21:12.000000 environments_utils-1.0.8/environments_utils/is_os.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      251 2022-08-15 18:21:12.000000 environments_utils-1.0.8/environments_utils/is_stdout_enabled.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      238 2022-08-15 18:21:12.000000 environments_utils-1.0.8/environments_utils/is_tmux.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-08-26 17:42:18.000000 environments_utils-1.0.8/environments_utils.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4642 2022-08-26 17:42:18.000000 environments_utils-1.0.8/environments_utils.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      548 2022-08-26 17:42:18.000000 environments_utils-1.0.8/environments_utils.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2022-08-26 17:42:18.000000 environments_utils-1.0.8/environments_utils.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       92 2022-08-26 17:42:18.000000 environments_utils-1.0.8/environments_utils.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       19 2022-08-26 17:42:18.000000 environments_utils-1.0.8/environments_utils.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2022-08-26 17:42:18.000000 environments_utils-1.0.8/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1746 2022-08-26 17:41:08.000000 environments_utils-1.0.8/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-09-30 11:31:51.000000 environments_utils-1.0.9/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1073 2022-08-15 18:21:12.000000 environments_utils-1.0.9/LICENSE
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2022-08-15 18:21:12.000000 environments_utils-1.0.9/MANIFEST.in
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4642 2022-09-30 11:31:51.000000 environments_utils-1.0.9/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3172 2022-08-26 17:40:02.000000 environments_utils-1.0.9/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-09-30 11:31:51.000000 environments_utils-1.0.9/environments_utils/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      859 2022-08-26 17:17:29.000000 environments_utils-1.0.9/environments_utils/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       74 2022-09-30 11:31:43.000000 environments_utils-1.0.9/environments_utils/__version__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      535 2022-09-30 11:30:08.000000 environments_utils-1.0.9/environments_utils/is_architecture.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1183 2022-08-15 18:29:16.000000 environments_utils-1.0.9/environments_utils/is_cluster.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      359 2022-08-15 18:21:12.000000 environments_utils-1.0.9/environments_utils/is_notebook.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      334 2022-08-26 17:16:32.000000 environments_utils-1.0.9/environments_utils/is_online.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      575 2022-08-15 18:21:12.000000 environments_utils-1.0.9/environments_utils/is_os.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      251 2022-08-15 18:21:12.000000 environments_utils-1.0.9/environments_utils/is_stdout_enabled.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      238 2022-08-15 18:21:12.000000 environments_utils-1.0.9/environments_utils/is_tmux.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2022-09-30 11:31:51.000000 environments_utils-1.0.9/environments_utils.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4642 2022-09-30 11:31:51.000000 environments_utils-1.0.9/environments_utils.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      548 2022-09-30 11:31:51.000000 environments_utils-1.0.9/environments_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2022-09-30 11:31:51.000000 environments_utils-1.0.9/environments_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       92 2022-09-30 11:31:51.000000 environments_utils-1.0.9/environments_utils.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       19 2022-09-30 11:31:51.000000 environments_utils-1.0.9/environments_utils.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2022-09-30 11:31:51.000000 environments_utils-1.0.9/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1746 2022-08-26 17:41:08.000000 environments_utils-1.0.9/setup.py
```

### Comparing `environments_utils-1.0.8/LICENSE` & `environments_utils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `environments_utils-1.0.8/PKG-INFO` & `environments_utils-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environments_utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities to identify which environments is your python script running within.
 Home-page: https://github.com/LucaCappelletti94/environments_utils
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: Environment utils
         =========================================================================================
```

### Comparing `environments_utils-1.0.8/README.rst` & `environments_utils-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `environments_utils-1.0.8/environments_utils/__init__.py` & `environments_utils-1.0.9/environments_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `environments_utils-1.0.8/environments_utils/is_architecture.py` & `environments_utils-1.0.9/environments_utils/is_architecture.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 def is_x86() -> bool:
     """Return whether the current computer has x86 (32 bit) architecture."""
     return platform.machine() == "x86"
 
 
 def is_x86_64() -> bool:
     """Return whether the current computer has x86_64 (64 bit) architecture."""
-    return platform.machine() == "x86_64"
+    return platform.machine() in ["x86_64", "AMD64"]
```

### Comparing `environments_utils-1.0.8/environments_utils/is_cluster.py` & `environments_utils-1.0.9/environments_utils/is_cluster.py`

 * *Files identical despite different names*

### Comparing `environments_utils-1.0.8/environments_utils/is_os.py` & `environments_utils-1.0.9/environments_utils/is_os.py`

 * *Files identical despite different names*

### Comparing `environments_utils-1.0.8/environments_utils.egg-info/PKG-INFO` & `environments_utils-1.0.9/environments_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environments-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities to identify which environments is your python script running within.
 Home-page: https://github.com/LucaCappelletti94/environments_utils
 Author: Luca Cappelletti
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: Environment utils
         =========================================================================================
```

### Comparing `environments_utils-1.0.8/environments_utils.egg-info/SOURCES.txt` & `environments_utils-1.0.9/environments_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `environments_utils-1.0.8/setup.py` & `environments_utils-1.0.9/setup.py`

 * *Files identical despite different names*

