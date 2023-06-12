# Comparing `tmp/clickhouse-toolset-0.8.dev0.tar.gz` & `tmp/clickhouse-toolset-0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clickhouse-toolset-0.8.dev0.tar", last modified: Mon Oct 26 11:44:15 2020, max compression
+gzip compressed data, was "dist/clickhouse-toolset-0.9.dev0.tar", last modified: Tue Oct 27 17:18:26 2020, max compression
```

## Comparing `clickhouse-toolset-0.8.dev0.tar` & `clickhouse-toolset-0.9.dev0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)      318 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/PKG-INFO
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     1858 2020-10-26 11:41:48.000000 clickhouse-toolset-0.8.dev0/README.md
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       38 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/setup.cfg
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     4862 2020-10-26 11:42:46.000000 clickhouse-toolset-0.8.dev0/setup.py
-drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/
-drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/chtoolset/
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       20 2020-08-21 07:16:14.000000 clickhouse-toolset-0.8.dev0/src/chtoolset/__init__.py
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     2164 2020-04-27 16:19:40.000000 clickhouse-toolset-0.8.dev0/src/chtoolset/query.py
-drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/clickhouse_toolset.egg-info/
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)      318 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/clickhouse_toolset.egg-info/PKG-INFO
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)      310 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/clickhouse_toolset.egg-info/SOURCES.txt
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)        1 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/clickhouse_toolset.egg-info/dependency_links.txt
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       50 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/clickhouse_toolset.egg-info/requires.txt
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       10 2020-10-26 11:44:15.000000 clickhouse-toolset-0.8.dev0/src/clickhouse_toolset.egg-info/top_level.txt
--rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     5031 2019-12-11 13:20:20.000000 clickhouse-toolset-0.8.dev0/src/query.cpp
+drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)      318 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/PKG-INFO
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     1858 2020-10-26 12:02:37.000000 clickhouse-toolset-0.9.dev0/README.md
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       38 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/setup.cfg
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     4862 2020-10-27 17:17:10.000000 clickhouse-toolset-0.9.dev0/setup.py
+drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/
+drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/chtoolset/
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       20 2020-08-21 07:16:14.000000 clickhouse-toolset-0.9.dev0/src/chtoolset/__init__.py
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     2311 2020-10-27 15:18:12.000000 clickhouse-toolset-0.9.dev0/src/chtoolset/query.py
+drwxrwxr-x   0 rochoa    (1000) rochoa    (1000)        0 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/clickhouse_toolset.egg-info/
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)      318 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/clickhouse_toolset.egg-info/PKG-INFO
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)      310 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/clickhouse_toolset.egg-info/SOURCES.txt
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)        1 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/clickhouse_toolset.egg-info/dependency_links.txt
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       50 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/clickhouse_toolset.egg-info/requires.txt
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)       10 2020-10-27 17:18:26.000000 clickhouse-toolset-0.9.dev0/src/clickhouse_toolset.egg-info/top_level.txt
+-rw-rw-r--   0 rochoa    (1000) rochoa    (1000)     5031 2019-12-11 13:20:20.000000 clickhouse-toolset-0.9.dev0/src/query.cpp
```

### Comparing `clickhouse-toolset-0.8.dev0/README.md` & `clickhouse-toolset-0.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-toolset-0.8.dev0/setup.py` & `clickhouse-toolset-0.9.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from setuptools import setup, Extension, find_packages
 from setuptools.command.build_ext import build_ext
 
 
 NAME = 'clickhouse-toolset'
 # https://www.python.org/dev/peps/pep-0440/#developmental-releases
-VERSION = '0.8.dev0'
+VERSION = '0.9.dev0'
 
 ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
 CLICKHOUSE_PATH = os.path.join(ROOT_DIR, 'ClickHouse')
 CLICKHOUSE_BUILD_PATH = os.path.join(CLICKHOUSE_PATH, 'build')
 
 class ClickHouseParsersBuildExt(build_ext):
     def run(self):
```

### Comparing `clickhouse-toolset-0.8.dev0/src/chtoolset/query.py` & `clickhouse-toolset-0.9.dev0/src/chtoolset/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,24 @@
             raise e
         return set([replacement])
 
 class ReplacementsDict(dict):
     def __getitem__(self, key):
         v = super().__getitem__(key)
         if isinstance(v, tuple):
-            return (v[0], v[1]() if callable(v[1]) else v[1])
-        return v() if callable(v) else v
+            k, r = v
+            if callable(r):
+                r = r()
+                super().__setitem__(key, (k, r))
+            return (k, r)
+        if callable(v):
+            v = v()
+            super().__setitem__(key, v)
+        return v
+
 
 def replace_tables(sql, replacements, default_database=''):
     if not replacements:
         return format(sql)
 
     _replacements = ReplacementsDict()
     for k, r in replacements.items():
```

### Comparing `clickhouse-toolset-0.8.dev0/src/query.cpp` & `clickhouse-toolset-0.9.dev0/src/query.cpp`

 * *Files identical despite different names*

