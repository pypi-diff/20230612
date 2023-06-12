# Comparing `tmp/blessable-1.0.1.tar.gz` & `tmp/blessable-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blessable-1.0.1.tar", last modified: Mon Jun 12 02:44:40 2023, max compression
+gzip compressed data, was "blessable-1.0.2.tar", last modified: Mon Jun 12 02:47:34 2023, max compression
```

## Comparing `blessable-1.0.1.tar` & `blessable-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:44:40.362607 blessable-1.0.1/
--rw-r--r--   0 benjaminlee   (501) staff       (20)      140 2023-06-12 02:44:40.362479 blessable-1.0.1/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1429 2023-06-12 01:37:31.000000 blessable-1.0.1/README.md
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:44:40.361650 blessable-1.0.1/blessable/
--rw-r--r--   0 benjaminlee   (501) staff       (20)       33 2023-06-12 01:36:24.000000 blessable-1.0.1/blessable/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)      624 2023-06-12 01:36:31.000000 blessable-1.0.1/blessable/blessable.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    15184 2023-06-12 00:48:54.000000 blessable-1.0.1/blessable/colormap.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:44:40.362307 blessable-1.0.1/blessable.egg-info/
--rw-r--r--   0 benjaminlee   (501) staff       (20)      140 2023-06-12 02:44:40.000000 blessable-1.0.1/blessable.egg-info/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      249 2023-06-12 02:44:40.000000 blessable-1.0.1/blessable.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2023-06-12 02:44:40.000000 blessable-1.0.1/blessable.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        8 2023-06-12 02:44:40.000000 blessable-1.0.1/blessable.egg-info/requires.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       10 2023-06-12 02:44:40.000000 blessable-1.0.1/blessable.egg-info/top_level.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2023-06-12 02:44:40.362653 blessable-1.0.1/setup.cfg
--rw-r--r--   0 benjaminlee   (501) staff       (20)      305 2023-06-12 02:43:34.000000 blessable-1.0.1/setup.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:47:34.869949 blessable-1.0.2/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1611 2023-06-12 02:47:34.869815 blessable-1.0.2/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1429 2023-06-12 01:37:31.000000 blessable-1.0.2/README.md
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:47:34.868973 blessable-1.0.2/blessable/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       33 2023-06-12 01:36:24.000000 blessable-1.0.2/blessable/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      624 2023-06-12 01:36:31.000000 blessable-1.0.2/blessable/blessable.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)    15184 2023-06-12 00:48:54.000000 blessable-1.0.2/blessable/colormap.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:47:34.869624 blessable-1.0.2/blessable.egg-info/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1611 2023-06-12 02:47:34.000000 blessable-1.0.2/blessable.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      249 2023-06-12 02:47:34.000000 blessable-1.0.2/blessable.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2023-06-12 02:47:34.000000 blessable-1.0.2/blessable.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        8 2023-06-12 02:47:34.000000 blessable-1.0.2/blessable.egg-info/requires.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       10 2023-06-12 02:47:34.000000 blessable-1.0.2/blessable.egg-info/top_level.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2023-06-12 02:47:34.869995 blessable-1.0.2/setup.cfg
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      444 2023-06-12 02:47:31.000000 blessable-1.0.2/setup.py
```

### Comparing `blessable-1.0.1/README.md` & `blessable-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `blessable-1.0.1/blessable/blessable.py` & `blessable-1.0.2/blessable/blessable.py`

 * *Files identical despite different names*

### Comparing `blessable-1.0.1/blessable/colormap.py` & `blessable-1.0.2/blessable/colormap.py`

 * *Files identical despite different names*

