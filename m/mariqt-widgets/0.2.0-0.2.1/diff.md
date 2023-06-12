# Comparing `tmp/mariqt_widgets-0.2.0-py2.py3-none-any.whl.zip` & `tmp/mariqt_widgets-0.2.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,15 @@
-Zip file size: 12781 bytes, number of entries: 8
--rw-r--r--  2.0 unx      128 b- defN 23-May-10 11:35 mariqt_widgets/__init__.py
--rw-r--r--  2.0 unx    49232 b- defN 23-May-10 11:35 mariqt_widgets/notebook_widgets.py
--rw-rw-rw-  2.0 unx      118 b- defN 23-May-10 11:35 mariqt_widgets-0.2.0.dist-info/AUTHORS.md
--rw-rw-rw-  2.0 unx     1506 b- defN 23-May-10 11:35 mariqt_widgets-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1443 b- defN 23-May-10 11:35 mariqt_widgets-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-10 11:35 mariqt_widgets-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-10 11:35 mariqt_widgets-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      693 b- defN 23-May-10 11:35 mariqt_widgets-0.2.0.dist-info/RECORD
-8 files, 53245 bytes uncompressed, 11561 bytes compressed:  78.3%
+Zip file size: 21460 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      128 b- defN 23-Jun-12 13:17 mariqt_widgets/__init__.py
+-rw-r--r--  2.0 unx    49232 b- defN 23-Jun-12 13:17 mariqt_widgets/notebook_widgets.py
+-rw-rw-rw-  2.0 unx     1520 b- defN 23-Jun-12 13:17 mariqt_widgets/icons/checkbox-circle-line_gray.png
+-rw-rw-rw-  2.0 unx     1525 b- defN 23-Jun-12 13:17 mariqt_widgets/icons/checkbox-circle-line_green.png
+-rw-rw-rw-  2.0 unx     1502 b- defN 23-Jun-12 13:17 mariqt_widgets/icons/error-warning-line_gray.png
+-rw-rw-rw-  2.0 unx     1513 b- defN 23-Jun-12 13:17 mariqt_widgets/icons/error-warning-line_orange.png
+-rw-rw-rw-  2.0 unx     1470 b- defN 23-Jun-12 13:17 mariqt_widgets/icons/error-warning-line_red.png
+-rw-rw-rw-  2.0 unx      118 b- defN 23-Jun-12 13:17 mariqt_widgets-0.2.1.dist-info/AUTHORS.md
+-rw-rw-rw-  2.0 unx     1506 b- defN 23-Jun-12 13:17 mariqt_widgets-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1443 b- defN 23-Jun-12 13:17 mariqt_widgets-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-12 13:17 mariqt_widgets-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-12 13:17 mariqt_widgets-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1224 b- defN 23-Jun-12 13:17 mariqt_widgets-0.2.1.dist-info/RECORD
+13 files, 61306 bytes uncompressed, 19368 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,25 +1,40 @@
 Filename: mariqt_widgets/__init__.py
 Comment: 
 
 Filename: mariqt_widgets/notebook_widgets.py
 Comment: 
 
-Filename: mariqt_widgets-0.2.0.dist-info/AUTHORS.md
+Filename: mariqt_widgets/icons/checkbox-circle-line_gray.png
 Comment: 
 
-Filename: mariqt_widgets-0.2.0.dist-info/LICENSE
+Filename: mariqt_widgets/icons/checkbox-circle-line_green.png
 Comment: 
 
-Filename: mariqt_widgets-0.2.0.dist-info/METADATA
+Filename: mariqt_widgets/icons/error-warning-line_gray.png
 Comment: 
 
-Filename: mariqt_widgets-0.2.0.dist-info/WHEEL
+Filename: mariqt_widgets/icons/error-warning-line_orange.png
 Comment: 
 
-Filename: mariqt_widgets-0.2.0.dist-info/top_level.txt
+Filename: mariqt_widgets/icons/error-warning-line_red.png
 Comment: 
 
-Filename: mariqt_widgets-0.2.0.dist-info/RECORD
+Filename: mariqt_widgets-0.2.1.dist-info/AUTHORS.md
+Comment: 
+
+Filename: mariqt_widgets-0.2.1.dist-info/LICENSE
+Comment: 
+
+Filename: mariqt_widgets-0.2.1.dist-info/METADATA
+Comment: 
+
+Filename: mariqt_widgets-0.2.1.dist-info/WHEEL
+Comment: 
+
+Filename: mariqt_widgets-0.2.1.dist-info/top_level.txt
+Comment: 
+
+Filename: mariqt_widgets-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mariqt_widgets/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Top-level package for mariqt_widgets."""
 
 __author__ = """Karl Heger"""
 __email__ = 'kheger@geomar.de'
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

## Comparing `mariqt_widgets-0.2.0.dist-info/LICENSE` & `mariqt_widgets-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mariqt_widgets-0.2.0.dist-info/METADATA` & `mariqt_widgets-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mariqt-widgets
-Version: 0.2.0
+Version: 0.2.1
 Summary: Contains widgets commonly used by MarIQT Notebooks.
 Home-page: https://codebase.helmholtz.cloud/datahub/marehub/ag-videosimages/mariqt-notebook-widgets
 Author: Karl Heger
 Author-email: kheger@geomar.de
 License: GNU General Public License v3
 Keywords: mariqt_widgets
 Classifier: Development Status :: 2 - Pre-Alpha
```

