# Comparing `tmp/pyfii-1.1.0.tar.gz` & `tmp/pyfii-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfii-1.1.0.tar", last modified: Mon Oct 10 13:32:10 2022, max compression
+gzip compressed data, was "pyfii-1.2.0.tar", last modified: Mon Jun 12 15:13:12 2023, max compression
```

## Comparing `pyfii-1.1.0.tar` & `pyfii-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2022-10-10 13:32:10.167113 pyfii-1.1.0/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     4801 2022-10-10 13:32:10.166374 pyfii-1.1.0/PKG-INFO
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3615 2022-09-30 15:01:33.000000 pyfii-1.1.0/README.md
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2022-10-10 13:32:10.153481 pyfii-1.1.0/pyfii/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      132 2022-09-30 15:01:33.000000 pyfii-1.1.0/pyfii/__init__.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16682 2022-09-30 15:01:33.000000 pyfii-1.1.0/pyfii/drone.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3190 2022-09-30 15:01:33.000000 pyfii-1.1.0/pyfii/fii.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16559 2022-09-30 15:01:33.000000 pyfii-1.1.0/pyfii/read.py
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)    21818 2022-09-30 15:01:33.000000 pyfii-1.1.0/pyfii/show.py
-drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2022-10-10 13:32:10.164337 pyfii-1.1.0/pyfii.egg-info/
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)     4801 2022-10-10 13:32:10.000000 pyfii-1.1.0/pyfii.egg-info/PKG-INFO
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      236 2022-10-10 13:32:10.000000 pyfii-1.1.0/pyfii.egg-info/SOURCES.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)        1 2022-10-10 13:32:10.000000 pyfii-1.1.0/pyfii.egg-info/dependency_links.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)       14 2022-10-10 13:32:10.000000 pyfii-1.1.0/pyfii.egg-info/requires.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)        6 2022-10-10 13:32:10.000000 pyfii-1.1.0/pyfii.egg-info/top_level.txt
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)       38 2022-10-10 13:32:10.167559 pyfii-1.1.0/setup.cfg
--rwxrwxrwx   0 aurora    (1000) aurora    (1000)      578 2022-10-10 13:29:38.000000 pyfii-1.1.0/setup.py
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.898677 pyfii-1.2.0/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    35149 2023-06-09 19:42:27.000000 pyfii-1.2.0/LICENSE
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:13:12.897819 pyfii-1.2.0/PKG-INFO
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1578 2023-06-12 14:42:00.000000 pyfii-1.2.0/README.md
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      687 2023-06-12 15:12:52.000000 pyfii-1.2.0/pyproject.toml
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)       38 2023-06-12 15:13:12.898963 pyfii-1.2.0/setup.cfg
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.858571 pyfii-1.2.0/src/
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.875986 pyfii-1.2.0/src/pyfii/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      132 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/__init__.py
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.895746 pyfii-1.2.0/src/pyfii/cv3d/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     5441 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/cv3d/IIID.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3978 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/cv3d/IIID2.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     1426 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/cv3d/transfer.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16682 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/drone.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     3190 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/fii.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    16559 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/read.py
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)    21818 2023-06-09 19:42:27.000000 pyfii-1.2.0/src/pyfii/show.py
+drwxrwxrwx   0 aurora    (1000) aurora    (1000)        0 2023-06-12 15:13:12.885609 pyfii-1.2.0/src/pyfii.egg-info/
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)     2127 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/PKG-INFO
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)      332 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        1 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aurora    (1000) aurora    (1000)        6 2023-06-12 15:13:12.000000 pyfii-1.2.0/src/pyfii.egg-info/top_level.txt
```

### Comparing `pyfii-1.1.0/pyfii/drone.py` & `pyfii-1.2.0/src/pyfii/drone.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.1.0/pyfii/fii.py` & `pyfii-1.2.0/src/pyfii/fii.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.1.0/pyfii/read.py` & `pyfii-1.2.0/src/pyfii/read.py`

 * *Files identical despite different names*

### Comparing `pyfii-1.1.0/pyfii/show.py` & `pyfii-1.2.0/src/pyfii/show.py`

 * *Files identical despite different names*

