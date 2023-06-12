# Comparing `tmp/b21scripts-1.0.7.tar.gz` & `tmp/b21scripts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nathan/Documents/PYTHON/b21scripts/dist/.tmp-dxf4346h/b21scripts-1.0.7.tar", last modified: Fri Jun  2 09:56:11 2023, max compression
+gzip compressed data, was "/Users/nathan/Documents/PYTHON/b21scripts/dist/.tmp-2sxd7dxg/b21scripts-1.1.0.tar", last modified: Mon Jun 12 10:18:26 2023, max compression
```

## Comparing `b21scripts-1.0.7.tar` & `b21scripts-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:56:11.000000 b21scripts-1.0.7/
--rw-r--r--   0 nathan     (503) staff       (20)     1084 2022-09-09 14:05:16.000000 b21scripts-1.0.7/LICENCE
--rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-02 09:56:11.000000 b21scripts-1.0.7/PKG-INFO
--rw-r--r--   0 nathan     (503) staff       (20)     1903 2022-09-19 18:19:39.000000 b21scripts-1.0.7/README.md
--rw-r--r--   0 nathan     (503) staff       (20)       84 2022-09-09 14:05:16.000000 b21scripts-1.0.7/pyproject.toml
--rw-r--r--   0 nathan     (503) staff       (20)      747 2023-06-02 09:56:11.000000 b21scripts-1.0.7/setup.cfg
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts/
--rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.0.7/src/b21scripts/__init__.py
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts/readwrite/
--rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.0.7/src/b21scripts/readwrite/__init__.py
--rw-r--r--   0 nathan     (503) staff       (20)     7530 2023-06-02 09:52:45.000000 b21scripts-1.0.7/src/b21scripts/readwrite/dat.py
--rw-r--r--   0 nathan     (503) staff       (20)      395 2022-09-09 14:05:16.000000 b21scripts-1.0.7/src/b21scripts/readwrite/interface.py
--rw-r--r--   0 nathan     (503) staff       (20)    13786 2022-09-09 14:05:16.000000 b21scripts-1.0.7/src/b21scripts/readwrite/pdb.py
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts/saxs/
--rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-19 18:10:28.000000 b21scripts-1.0.7/src/b21scripts/saxs/__init__.py
--rwxr-xr-x   0 nathan     (503) staff       (20)    11290 2022-09-19 16:24:23.000000 b21scripts-1.0.7/src/b21scripts/saxs/saxs_calc.py
-drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts.egg-info/
--rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts.egg-info/PKG-INFO
--rw-r--r--   0 nathan     (503) staff       (20)      462 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts.egg-info/SOURCES.txt
--rw-r--r--   0 nathan     (503) staff       (20)        1 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts.egg-info/dependency_links.txt
--rw-r--r--   0 nathan     (503) staff       (20)       17 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts.egg-info/requires.txt
--rw-r--r--   0 nathan     (503) staff       (20)       11 2023-06-02 09:56:11.000000 b21scripts-1.0.7/src/b21scripts.egg-info/top_level.txt
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/
+-rw-r--r--   0 nathan     (503) staff       (20)     1084 2022-09-09 14:05:16.000000 b21scripts-1.1.0/LICENCE
+-rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-12 10:18:26.000000 b21scripts-1.1.0/PKG-INFO
+-rw-r--r--   0 nathan     (503) staff       (20)     1903 2022-09-19 18:19:39.000000 b21scripts-1.1.0/README.md
+-rw-r--r--   0 nathan     (503) staff       (20)       84 2022-09-09 14:05:16.000000 b21scripts-1.1.0/pyproject.toml
+-rw-r--r--   0 nathan     (503) staff       (20)      747 2023-06-12 10:18:26.000000 b21scripts-1.1.0/setup.cfg
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/__init__.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts/readwrite/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/readwrite/__init__.py
+-rw-r--r--   0 nathan     (503) staff       (20)    12770 2023-06-12 10:07:41.000000 b21scripts-1.1.0/src/b21scripts/readwrite/dat.py
+-rw-r--r--   0 nathan     (503) staff       (20)      395 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/readwrite/interface.py
+-rw-r--r--   0 nathan     (503) staff       (20)    13786 2022-09-09 14:05:16.000000 b21scripts-1.1.0/src/b21scripts/readwrite/pdb.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts/saxs/
+-rw-r--r--   0 nathan     (503) staff       (20)        0 2022-09-19 18:10:28.000000 b21scripts-1.1.0/src/b21scripts/saxs/__init__.py
+-rwxr-xr-x   0 nathan     (503) staff       (20)    11290 2022-09-19 16:24:23.000000 b21scripts-1.1.0/src/b21scripts/saxs/saxs_calc.py
+drwxr-xr-x   0 nathan     (503) staff       (20)        0 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/
+-rw-r--r--   0 nathan     (503) staff       (20)     2445 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/PKG-INFO
+-rw-r--r--   0 nathan     (503) staff       (20)      462 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan     (503) staff       (20)        1 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan     (503) staff       (20)       17 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/requires.txt
+-rw-r--r--   0 nathan     (503) staff       (20)       11 2023-06-12 10:18:26.000000 b21scripts-1.1.0/src/b21scripts.egg-info/top_level.txt
```

### Comparing `b21scripts-1.0.7/LICENCE` & `b21scripts-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.7/PKG-INFO` & `b21scripts-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b21scripts
-Version: 1.0.7
+Version: 1.1.0
 Summary: Libraries for SAXS data manipulation and analysis
 Home-page: https://github.com/nathancowieson/b21scripts.git
 Author: Nathan Cowieson
 Author-email: nathan.cowieson@diamond.ac.uk
 Project-URL: Bug Tracker, https://github.com/pypa/b21scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `b21scripts-1.0.7/README.md` & `b21scripts-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.7/setup.cfg` & `b21scripts-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = b21scripts
-version = 1.0.7
+version = 1.1.0
 author = Nathan Cowieson
 author_email = nathan.cowieson@diamond.ac.uk
 description = Libraries for SAXS data manipulation and analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nathancowieson/b21scripts.git
 project_urls =
```

### Comparing `b21scripts-1.0.7/src/b21scripts/readwrite/pdb.py` & `b21scripts-1.1.0/src/b21scripts/readwrite/pdb.py`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.7/src/b21scripts/saxs/saxs_calc.py` & `b21scripts-1.1.0/src/b21scripts/saxs/saxs_calc.py`

 * *Files identical despite different names*

### Comparing `b21scripts-1.0.7/src/b21scripts.egg-info/PKG-INFO` & `b21scripts-1.1.0/src/b21scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b21scripts
-Version: 1.0.7
+Version: 1.1.0
 Summary: Libraries for SAXS data manipulation and analysis
 Home-page: https://github.com/nathancowieson/b21scripts.git
 Author: Nathan Cowieson
 Author-email: nathan.cowieson@diamond.ac.uk
 Project-URL: Bug Tracker, https://github.com/pypa/b21scripts/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

