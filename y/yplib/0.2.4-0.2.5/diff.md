# Comparing `tmp/yplib-0.2.4.tar.gz` & `tmp/yplib-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.2.4.tar", last modified: Mon Jun 12 07:50:36 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.5.tar", last modified: Mon Jun 12 09:00:51 2023, max compression
```

## Comparing `yplib-0.2.4.tar` & `yplib-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:50:36.944774 yplib-0.2.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-12 07:50:36.944774 yplib-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 07:50:36.944774 yplib-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-12 07:50:15.000000 yplib-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:50:36.941955 yplib-0.2.4/yplib/
--rw-rw-rw-   0        0        0    15370 2023-06-12 07:49:32.000000 yplib-0.2.4/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.4/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:50:36.944774 yplib-0.2.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 09:00:51.408081 yplib-0.2.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-12 09:00:51.407904 yplib-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:00:51.408689 yplib-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-12 09:00:39.000000 yplib-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:00:51.404835 yplib-0.2.5/yplib/
+-rw-rw-rw-   0        0        0    15370 2023-06-12 07:49:32.000000 yplib-0.2.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.5/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:00:51.407140 yplib-0.2.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.2.4/LICENSE` & `yplib-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.2.4/PKG-INFO` & `yplib-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.4
+Version: 0.2.5
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.2.4/setup.py` & `yplib-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.2.4",
+  version="0.2.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.2.4/yplib/__init__.py` & `yplib-0.2.5/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.4/yplib/line_stack_temp.py` & `yplib-0.2.5/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.4/yplib.egg-info/PKG-INFO` & `yplib-0.2.5/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.4
+Version: 0.2.5
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

