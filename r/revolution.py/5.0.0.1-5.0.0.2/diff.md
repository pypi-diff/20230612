# Comparing `tmp/revolution.py-5.0.0.1.tar.gz` & `tmp/revolution.py-5.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revolution.py-5.0.0.1.tar", last modified: Mon Jun 12 06:03:06 2023, max compression
+gzip compressed data, was "revolution.py-5.0.0.2.tar", last modified: Mon Jun 12 06:14:16 2023, max compression
```

## Comparing `revolution.py-5.0.0.1.tar` & `revolution.py-5.0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:03:06.652243 revolution.py-5.0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.0.1/LICENSE
--rw-rw-rw-   0        0        0      449 2023-06-12 06:03:06.651009 revolution.py-5.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 06:03:06.646891 revolution.py-5.0.0.1/revolution.py.egg-info/
--rw-rw-rw-   0        0        0      449 2023-06-12 06:03:05.000000 revolution.py-5.0.0.1/revolution.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-12 06:03:05.000000 revolution.py-5.0.0.1/revolution.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:03:05.000000 revolution.py-5.0.0.1/revolution.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:03:05.000000 revolution.py-5.0.0.1/revolution.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 06:03:06.653604 revolution.py-5.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      587 2023-06-12 06:02:53.000000 revolution.py-5.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:14:16.182117 revolution.py-5.0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-11 23:52:23.000000 revolution.py-5.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      449 2023-06-12 06:14:16.182117 revolution.py-5.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2023-06-12 05:49:37.000000 revolution.py-5.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 06:14:16.176776 revolution.py-5.0.0.2/revolution.py.egg-info/
+-rw-rw-rw-   0        0        0      449 2023-06-12 06:14:15.000000 revolution.py-5.0.0.2/revolution.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-12 06:14:16.000000 revolution.py-5.0.0.2/revolution.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:14:15.000000 revolution.py-5.0.0.2/revolution.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:14:15.000000 revolution.py-5.0.0.2/revolution.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 06:14:16.182117 revolution.py-5.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      587 2023-06-12 06:14:10.000000 revolution.py-5.0.0.2/setup.py
```

### Comparing `revolution.py-5.0.0.1/LICENSE` & `revolution.py-5.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.1/README.md` & `revolution.py-5.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `revolution.py-5.0.0.1/setup.py` & `revolution.py-5.0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "revolution.py",
-    version = "5.0.0.1",
+    version = "5.0.0.2",
     description = "A simple Py package to integrate Revolution's bot API into python.",
     long_description = "A simple Py package to integrate Revolution's bot API into Python. \nhttps://github.com/JustAnEric/Revolution.py",
     author = "JustAnEric",
     maintainer = "Revolution Corporation",
     requires = ["requests"],
     url = "https://revolution.ericplayzyt.repl.co/",
     packages = find_packages(),
```

