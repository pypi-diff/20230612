# Comparing `tmp/Operetta_tool-1.4.3.tar.gz` & `tmp/Operetta_tool-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.4.3.tar", last modified: Mon Jun 12 15:52:21 2023, max compression
+gzip compressed data, was "Operetta_tool-1.4.4.tar", last modified: Mon Jun 12 15:53:12 2023, max compression
```

## Comparing `Operetta_tool-1.4.3.tar` & `Operetta_tool-1.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 15:52:21.775661 Operetta_tool-1.4.3/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.4.3/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.4.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-12 15:52:21.770063 Operetta_tool-1.4.3/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-06-12 15:52:21.000000 Operetta_tool-1.4.3/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-12 15:52:21.000000 Operetta_tool-1.4.3/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 15:52:21.000000 Operetta_tool-1.4.3/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-06-12 15:52:21.000000 Operetta_tool-1.4.3/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 15:52:21.000000 Operetta_tool-1.4.3/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-06-12 15:52:21.773113 Operetta_tool-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 15:52:21.773113 Operetta_tool-1.4.3/operetta/
--rw-rw-rw-   0        0        0      153 2023-06-12 15:52:12.000000 Operetta_tool-1.4.3/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.4.3/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    59095 2023-06-12 15:51:54.000000 Operetta_tool-1.4.3/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-06-12 15:52:21.775661 Operetta_tool-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-06-12 15:52:16.000000 Operetta_tool-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:53:12.388142 Operetta_tool-1.4.4/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.4.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-12 15:53:12.379589 Operetta_tool-1.4.4/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-06-12 15:53:11.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-12 15:53:12.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:53:11.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-06-12 15:53:12.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 15:53:12.000000 Operetta_tool-1.4.4/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-06-12 15:53:12.387019 Operetta_tool-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 15:53:12.381605 Operetta_tool-1.4.4/operetta/
+-rw-rw-rw-   0        0        0      153 2023-06-12 15:53:06.000000 Operetta_tool-1.4.4/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.4.4/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    59095 2023-06-12 15:51:54.000000 Operetta_tool-1.4.4/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 15:53:12.388142 Operetta_tool-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-06-12 15:53:01.000000 Operetta_tool-1.4.4/setup.py
```

### Comparing `Operetta_tool-1.4.3/LICENSE` & `Operetta_tool-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.3/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.4.4/Operetta_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.4.3
+Version: 1.4.4
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.4.3/PKG-INFO` & `Operetta_tool-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.4.3
+Version: 1.4.4
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.4.3/README.md` & `Operetta_tool-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.3/operetta/jbsicon.ico` & `Operetta_tool-1.4.4/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.3/operetta/operetta_annotation.py` & `Operetta_tool-1.4.4/operetta/operetta_annotation.py`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.4.3/setup.py` & `Operetta_tool-1.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.3' 
+VERSION = '1.4.4' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

