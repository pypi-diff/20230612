# Comparing `tmp/scratchsocket-0.1.1.tar.gz` & `tmp/scratchsocket-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchsocket-0.1.1.tar", last modified: Tue Jan  3 18:16:15 2023, max compression
+gzip compressed data, was "scratchsocket-0.1.2.tar", last modified: Mon Jun 12 19:34:29 2023, max compression
```

## Comparing `scratchsocket-0.1.1.tar` & `scratchsocket-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 18:16:15.475002 scratchsocket-0.1.1/
--rw-rw-rw-   0        0        0      637 2023-01-03 18:16:15.475002 scratchsocket-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5809 2023-01-03 18:11:17.000000 scratchsocket-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-03 18:16:15.475002 scratchsocket-0.1.1/scratchsocket.egg-info/
--rw-rw-rw-   0        0        0      637 2023-01-03 18:16:15.000000 scratchsocket-0.1.1/scratchsocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-01-03 18:16:15.000000 scratchsocket-0.1.1/scratchsocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 18:16:15.000000 scratchsocket-0.1.1/scratchsocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-01-03 18:16:15.000000 scratchsocket-0.1.1/scratchsocket.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 18:16:15.000000 scratchsocket-0.1.1/scratchsocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-03 18:16:15.475002 scratchsocket-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-01-03 18:09:46.000000 scratchsocket-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 19:34:29.497238 scratchsocket-0.1.2/
+-rw-rw-rw-   0        0        0      637 2023-06-12 19:34:29.497238 scratchsocket-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5809 2023-01-03 18:11:17.000000 scratchsocket-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 19:34:29.497238 scratchsocket-0.1.2/scratchsocket.egg-info/
+-rw-rw-rw-   0        0        0      637 2023-06-12 19:34:29.000000 scratchsocket-0.1.2/scratchsocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-12 19:34:29.000000 scratchsocket-0.1.2/scratchsocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 19:34:29.000000 scratchsocket-0.1.2/scratchsocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-12 19:34:29.000000 scratchsocket-0.1.2/scratchsocket.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 19:34:29.000000 scratchsocket-0.1.2/scratchsocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 19:34:29.512243 scratchsocket-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-06-12 19:18:27.000000 scratchsocket-0.1.2/setup.py
```

### Comparing `scratchsocket-0.1.1/PKG-INFO` & `scratchsocket-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchsocket
-Version: 0.1.1
+Version: 0.1.2
 Summary: Establish simple cloud connections with scratch.mit.edu!
 Home-page: https://github.com/abhiramtx/scratchsocket
 Author: Abhiram V
 Author-email: abhiram.tx@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `scratchsocket-0.1.1/README.md` & `scratchsocket-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scratchsocket-0.1.1/scratchsocket.egg-info/PKG-INFO` & `scratchsocket-0.1.2/scratchsocket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchsocket
-Version: 0.1.1
+Version: 0.1.2
 Summary: Establish simple cloud connections with scratch.mit.edu!
 Home-page: https://github.com/abhiramtx/scratchsocket
 Author: Abhiram V
 Author-email: abhiram.tx@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `scratchsocket-0.1.1/setup.py` & `scratchsocket-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="scratchsocket",
     url="https://github.com/abhiramtx/scratchsocket",
-    version="0.1.1",
+    version="0.1.2",
     author="Abhiram V",
     author_email="abhiram.tx@gmail.com",
     license="MIT",
     description="Establish simple cloud connections with scratch.mit.edu!",
     long_description="Establish simple cloud connections with scratch.mit.edu! Complete documentation: https://github.com/abhiramtx/scratchsocket",
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

