# Comparing `tmp/pyalltools-1.0.0.tar.gz` & `tmp/pyalltools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalltools-1.0.0.tar", last modified: Sat May 20 09:31:57 2023, max compression
+gzip compressed data, was "pyalltools-1.1.0.tar", last modified: Mon Jun 12 10:01:48 2023, max compression
```

## Comparing `pyalltools-1.0.0.tar` & `pyalltools-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 09:31:57.040333 pyalltools-1.0.0/
--rw-rw-rw-   0        0        0      751 2023-05-20 09:31:57.038341 pyalltools-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      127 2023-05-20 09:31:02.000000 pyalltools-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 09:31:57.035883 pyalltools-1.0.0/pyalltools.egg-info/
--rw-rw-rw-   0        0        0      751 2023-05-20 09:31:56.000000 pyalltools-1.0.0/pyalltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-05-20 09:31:56.000000 pyalltools-1.0.0/pyalltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 09:31:56.000000 pyalltools-1.0.0/pyalltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 09:31:56.000000 pyalltools-1.0.0/pyalltools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5114 2023-05-20 09:23:07.000000 pyalltools-1.0.0/pyalltools.py
--rw-rw-rw-   0        0        0       42 2023-05-20 09:31:57.040333 pyalltools-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-05-20 09:30:30.000000 pyalltools-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 10:01:48.680020 pyalltools-1.1.0/
+-rw-rw-rw-   0        0        0      751 2023-06-12 10:01:48.679019 pyalltools-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      127 2023-05-20 09:31:02.000000 pyalltools-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 10:01:48.677058 pyalltools-1.1.0/pyalltools.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-12 10:01:48.000000 pyalltools-1.1.0/pyalltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-06-12 10:01:48.000000 pyalltools-1.1.0/pyalltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 10:01:48.000000 pyalltools-1.1.0/pyalltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 10:01:48.000000 pyalltools-1.1.0/pyalltools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8091 2023-06-12 10:00:34.000000 pyalltools-1.1.0/pyalltools.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 10:01:48.680020 pyalltools-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-06-12 10:01:35.000000 pyalltools-1.1.0/setup.py
```

### Comparing `pyalltools-1.0.0/PKG-INFO` & `pyalltools-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalltools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library containing various tools that are required by programmers frequently
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `pyalltools-1.0.0/pyalltools.egg-info/PKG-INFO` & `pyalltools-1.1.0/pyalltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalltools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library containing various tools that are required by programmers frequently
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `pyalltools-1.0.0/setup.py` & `pyalltools-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyalltools",
-    version="1.0.0",
+    version="1.1.0",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library containing various tools that are required by programmers frequently",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
```

