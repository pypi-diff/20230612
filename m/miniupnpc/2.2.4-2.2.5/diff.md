# Comparing `tmp/miniupnpc-2.2.4-py3.9-win-amd64.egg` & `tmp/miniupnpc-2.2.5-py3.6-win-amd64.egg`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11606 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    20992 b- defN 22-Oct-21 21:52 miniupnpc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      431 b- defN 22-Oct-21 21:52 miniupnpc.py
--rw-rw-rw-  2.0 fat      251 b- defN 22-Oct-21 21:52 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat     1217 b- defN 22-Oct-21 21:52 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 22-Oct-21 21:52 EGG-INFO/dependency_links.txt
--rw-rw-rw-  2.0 fat       30 b- defN 22-Oct-21 21:52 EGG-INFO/native_libs.txt
--rw-rw-rw-  2.0 fat        2 b- defN 22-Oct-21 21:52 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       10 b- defN 22-Oct-21 21:52 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      555 b- defN 22-Oct-21 21:52 __pycache__/miniupnpc.cpython-39.pyc
-9 files, 23489 bytes uncompressed, 10482 bytes compressed:  55.4%
+Zip file size: 11561 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    21504 b- defN 23-Jun-11 23:26 miniupnpc.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      308 b- defN 23-Jun-11 23:26 miniupnpc.py
+-rw-rw-rw-  2.0 fat      237 b- defN 23-Jun-11 23:26 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat     1217 b- defN 23-Jun-11 23:26 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-11 23:26 EGG-INFO/dependency_links.txt
+-rw-rw-rw-  2.0 fat       30 b- defN 23-Jun-11 23:26 EGG-INFO/native_libs.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-11 23:26 EGG-INFO/not-zip-safe
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-11 23:26 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      431 b- defN 23-Jun-11 23:26 __pycache__/miniupnpc.cpython-36.pyc
+9 files, 23740 bytes uncompressed, 10437 bytes compressed:  56.0%
```

## zipnote «TEMP»/diffoscope_zqml3xho_/tmp2z00iam7_.zip

```diff
@@ -1,8 +1,8 @@
-Filename: miniupnpc.cp39-win_amd64.pyd
+Filename: miniupnpc.cp36-win_amd64.pyd
 Comment: 
 
 Filename: miniupnpc.py
 Comment: 
 
 Filename: EGG-INFO/PKG-INFO
 Comment: 
@@ -18,11 +18,11 @@
 
 Filename: EGG-INFO/not-zip-safe
 Comment: 
 
 Filename: EGG-INFO/top_level.txt
 Comment: 
 
-Filename: __pycache__/miniupnpc.cpython-39.pyc
+Filename: __pycache__/miniupnpc.cpython-36.pyc
 Comment: 
 
 Zip file comment:
```

## miniupnpc.py

```diff
@@ -1,9 +1,7 @@
 def __bootstrap__():
     global __bootstrap__, __loader__, __file__
-    import sys, pkg_resources, importlib.util
-    __file__ = pkg_resources.resource_filename(__name__, 'miniupnpc.cp39-win_amd64.pyd')
+    import sys, pkg_resources, imp
+    __file__ = pkg_resources.resource_filename(__name__, 'miniupnpc.cp36-win_amd64.pyd')
     __loader__ = None; del __bootstrap__, __loader__
-    spec = importlib.util.spec_from_file_location(__name__,__file__)
-    mod = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(mod)
+    imp.load_dynamic(__name__,__file__)
 __bootstrap__()
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,13 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.0
 Name: miniupnpc
-Version: 2.2.4
+Version: 2.2.5
 Summary: miniUPnP client
 Home-page: http://miniupnp.free.fr/
 Author: Thomas BERNARD
 Author-email: miniupnp@free.fr
 License: ../LICENSE
+Description: UNKNOWN
 Platform: UNKNOWN
-License-File: LICENSE
-
-UNKNOWN
-
```

## EGG-INFO/native_libs.txt

```diff
@@ -1 +1 @@
-miniupnpc.cp39-win_amd64.pyd
+miniupnpc.cp36-win_amd64.pyd
```

