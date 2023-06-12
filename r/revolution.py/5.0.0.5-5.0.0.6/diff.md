# Comparing `tmp/revolution.py-5.0.0.5.tar.gz` & `tmp/revolution.py-5.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolution.py-5.0.0.5.tar", last modified: Mon Jun 12 06:33:09 2023, max compression
+gzip compressed data, was "revolution.py-5.0.0.6.tar", last modified: Mon Jun 12 06:39:51 2023, max compression
```

## Comparing `revolution.py-5.0.0.5.tar` & `revolution.py-5.0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:33:09.811646 revolution.py-5.0.0.5/
--rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.0.5/LICENSE
--rw-rw-rw-   0        0        0      449 2023-06-12 06:33:09.809352 revolution.py-5.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 06:33:09.807159 revolution.py-5.0.0.5/revolution.py.egg-info/
--rw-rw-rw-   0        0        0      449 2023-06-12 06:33:09.000000 revolution.py-5.0.0.5/revolution.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-12 06:33:09.000000 revolution.py-5.0.0.5/revolution.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:33:09.000000 revolution.py-5.0.0.5/revolution.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:33:09.000000 revolution.py-5.0.0.5/revolution.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 06:33:09.811646 revolution.py-5.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      587 2023-06-12 06:32:27.000000 revolution.py-5.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:39:51.831614 revolution.py-5.0.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-06-12 06:39:51.831096 revolution.py-5.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 06:39:51.825946 revolution.py-5.0.0.6/revolution.py.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-06-12 06:39:51.000000 revolution.py-5.0.0.6/revolution.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-12 06:39:51.000000 revolution.py-5.0.0.6/revolution.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:39:51.000000 revolution.py-5.0.0.6/revolution.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:39:51.000000 revolution.py-5.0.0.6/revolution.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 06:39:51.833334 revolution.py-5.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      624 2023-06-12 06:39:35.000000 revolution.py-5.0.0.6/setup.py
```

### Comparing `revolution.py-5.0.0.5/LICENSE` & `revolution.py-5.0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.5/README.md` & `revolution.py-5.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.5/setup.py` & `revolution.py-5.0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "revolution.py",
-    version = "5.0.0.5",
+    version = "5.0.0.6",
     description = "A simple Py package to integrate Revolution's bot API into python.",
     long_description = "A simple Py package to integrate Revolution's bot API into Python. \nhttps://github.com/JustAnEric/Revolution.py",
     author = "JustAnEric",
     maintainer = "Revolution Corporation",
     requires = ["requests"],
     url = "https://revolution.ericplayzyt.repl.co/",
     packages = find_packages(),
-    keywords = ["revolutionpy", "python3", "revolution"]
+    keywords = ["revolutionpy", "python3", "revolution"],
+    include_dirs="./revolution_py"
 )
```

