# Comparing `tmp/revolution.py-5.0.0.7.tar.gz` & `tmp/revolution.py-5.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolution.py-5.0.0.7.tar", last modified: Mon Jun 12 06:42:49 2023, max compression
+gzip compressed data, was "revolution.py-5.0.0.8.tar", last modified: Mon Jun 12 06:46:27 2023, max compression
```

## Comparing `revolution.py-5.0.0.7.tar` & `revolution.py-5.0.0.8.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:42:49.307518 revolution.py-5.0.0.7/
--rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.0.7/LICENSE
--rw-rw-rw-   0        0        0      449 2023-06-12 06:42:49.306019 revolution.py-5.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 06:42:49.305063 revolution.py-5.0.0.7/revolution.py.egg-info/
--rw-rw-rw-   0        0        0      449 2023-06-12 06:42:49.000000 revolution.py-5.0.0.7/revolution.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-12 06:42:49.000000 revolution.py-5.0.0.7/revolution.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:42:49.000000 revolution.py-5.0.0.7/revolution.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:42:49.000000 revolution.py-5.0.0.7/revolution.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 06:42:49.308524 revolution.py-5.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-06-12 06:42:35.000000 revolution.py-5.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:46:27.351793 revolution.py-5.0.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-06-12 06:46:27.350238 revolution.py-5.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 06:46:27.344621 revolution.py-5.0.0.8/revolution.py.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-06-12 06:46:27.000000 revolution.py-5.0.0.8/revolution.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-12 06:46:27.000000 revolution.py-5.0.0.8/revolution.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:46:27.000000 revolution.py-5.0.0.8/revolution.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-12 06:46:27.000000 revolution.py-5.0.0.8/revolution.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 06:46:27.346593 revolution.py-5.0.0.8/revolution_py/
+-rw-rw-rw-   0        0        0     4979 2023-06-12 06:20:33.000000 revolution.py-5.0.0.8/revolution_py/lib.py
+-rw-rw-rw-   0        0        0     3162 2023-06-12 03:43:38.000000 revolution.py-5.0.0.8/revolution_py/main.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 06:46:27.351793 revolution.py-5.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-06-12 06:46:16.000000 revolution.py-5.0.0.8/setup.py
```

### Comparing `revolution.py-5.0.0.7/LICENSE` & `revolution.py-5.0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.7/README.md` & `revolution.py-5.0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.7/setup.py` & `revolution.py-5.0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "revolution.py",
-    version = "5.0.0.7",
+    version = "5.0.0.8",
     description = "A simple Py package to integrate Revolution's bot API into python.",
     long_description = "A simple Py package to integrate Revolution's bot API into Python. \nhttps://github.com/JustAnEric/Revolution.py",
     author = "JustAnEric",
     maintainer = "Revolution Corporation",
     requires = ["requests"],
     url = "https://revolution.ericplayzyt.repl.co/",
-    packages = find_packages(),
+    packages = ["revolution_py"],
     keywords = ["revolutionpy", "python3", "revolution"],
-    include_dirs=["./revolution_py"]
+    #include_dirs=["./revolution_py"]
 )
```

