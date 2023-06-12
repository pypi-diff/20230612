# Comparing `tmp/litesqlite-2.6.2.tar.gz` & `tmp/litesqlite-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.2.tar", last modified: Mon Jun 12 11:14:10 2023, max compression
+gzip compressed data, was "litesqlite-2.6.3.tar", last modified: Mon Jun 12 11:23:38 2023, max compression
```

## Comparing `litesqlite-2.6.2.tar` & `litesqlite-2.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:14:10.505861 litesqlite-2.6.2/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.2/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:14:10.505861 litesqlite-2.6.2/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.2/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:14:10.501861 litesqlite-2.6.2/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.2/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.2/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8316 2023-06-12 11:13:52.000000 litesqlite-2.6.2/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:14:10.505861 litesqlite-2.6.2/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 11:14:10.505861 litesqlite-2.6.2/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 11:08:41.000000 litesqlite-2.6.2/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:23:38.612458 litesqlite-2.6.3/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.3/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:23:38.612458 litesqlite-2.6.3/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.3/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:23:38.608458 litesqlite-2.6.3/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.3/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.3/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8324 2023-06-12 11:23:15.000000 litesqlite-2.6.3/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:23:38.612458 litesqlite-2.6.3/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 11:23:38.000000 litesqlite-2.6.3/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 11:23:38.612458 litesqlite-2.6.3/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 11:23:22.000000 litesqlite-2.6.3/setup.py
```

### Comparing `litesqlite-2.6.2/LICENSE` & `litesqlite-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.2/PKG-INFO` & `litesqlite-2.6.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.2
+Version: 2.6.3
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.2/README.md` & `litesqlite-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.2/litesqlite/datatypes.py` & `litesqlite-2.6.3/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.2/litesqlite/lite_sqlite.py` & `litesqlite-2.6.3/litesqlite/lite_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         values = tuple(where.values())
         if not self.__conn:
             self.__enter__()
         self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
         self.__conn.commit()
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        if self.__conn:
+        if not self.__conn:
             self.__conn.close()
 
 
 class AioSqlite:
 
     def __init__(self,
                  db_name: str) -> None:
@@ -199,9 +199,9 @@
         values = tuple(where.values())
         if not self.__conn:
             self.__aenter__()
         await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
         await self.__conn.commit()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        if self.__conn:
+        if not self.__conn:
             await self.__conn.close()
```

### Comparing `litesqlite-2.6.2/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.3/litesqlite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.2
+Version: 2.6.3
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.2/setup.py` & `litesqlite-2.6.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.2',
+    version='2.6.3',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

