# Comparing `tmp/litesqlite-2.6.0.tar.gz` & `tmp/litesqlite-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.0.tar", last modified: Mon Jun 12 07:12:28 2023, max compression
+gzip compressed data, was "litesqlite-2.6.1.tar", last modified: Mon Jun 12 07:56:39 2023, max compression
```

## Comparing `litesqlite-2.6.0.tar` & `litesqlite-2.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:12:28.181785 litesqlite-2.6.0/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.0/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:12:28.181785 litesqlite-2.6.0/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.0/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:12:28.181785 litesqlite-2.6.0/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.0/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.0/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     7714 2023-06-12 07:11:31.000000 litesqlite-2.6.0/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:12:28.181785 litesqlite-2.6.0/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 07:12:28.181785 litesqlite-2.6.0/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 07:12:14.000000 litesqlite-2.6.0/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:56:39.172356 litesqlite-2.6.1/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.1/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:56:39.172356 litesqlite-2.6.1/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.1/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:56:39.172356 litesqlite-2.6.1/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.1/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.1/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     7715 2023-06-12 07:56:30.000000 litesqlite-2.6.1/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:56:39.172356 litesqlite-2.6.1/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 07:56:39.172356 litesqlite-2.6.1/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 07:56:30.000000 litesqlite-2.6.1/setup.py
```

### Comparing `litesqlite-2.6.0/LICENSE` & `litesqlite-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.0/PKG-INFO` & `litesqlite-2.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.0
+Version: 2.6.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.0/README.md` & `litesqlite-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.0/litesqlite/datatypes.py` & `litesqlite-2.6.1/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.0/litesqlite/lite_sqlite.py` & `litesqlite-2.6.1/litesqlite/lite_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import aiosqlite
 import sqlite3
 from typing import Dict, Union, Tuple, List
-from datatypes import DataTypes
+from .datatypes import DataTypes
 
 
 class Sqlite:
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
```

### Comparing `litesqlite-2.6.0/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.1/litesqlite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.0
+Version: 2.6.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.0/setup.py` & `litesqlite-2.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.0',
+    version='2.6.1',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

