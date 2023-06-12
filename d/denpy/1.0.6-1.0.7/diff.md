# Comparing `tmp/denpy-1.0.6.tar.gz` & `tmp/denpy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-1.0.6.tar", last modified: Mon Jun 12 14:48:14 2023, max compression
+gzip compressed data, was "denpy-1.0.7.tar", last modified: Mon Jun 12 14:50:31 2023, max compression
```

## Comparing `denpy-1.0.6.tar` & `denpy-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:48:14.780609 denpy-1.0.6/
--rw-rw-rw-   0        0        0      112 2023-06-12 14:48:14.779611 denpy-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 14:48:14.774624 denpy-1.0.6/denpy/
--rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.6/denpy/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.6/denpy/color.py
--rw-rw-rw-   0        0        0     1784 2023-06-12 14:47:58.000000 denpy-1.0.6/denpy/database.py
--rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.6/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:48:14.778614 denpy-1.0.6/denpy.egg-info/
--rw-rw-rw-   0        0        0      112 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 14:48:14.780609 denpy-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      205 2023-06-12 14:48:10.000000 denpy-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:50:31.832041 denpy-1.0.7/
+-rw-rw-rw-   0        0        0      112 2023-06-12 14:50:31.831045 denpy-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 14:50:31.814096 denpy-1.0.7/denpy/
+-rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.7/denpy/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.7/denpy/color.py
+-rw-rw-rw-   0        0        0     1784 2023-06-12 14:47:58.000000 denpy-1.0.7/denpy/database.py
+-rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.7/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:50:31.829049 denpy-1.0.7/denpy.egg-info/
+-rw-rw-rw-   0        0        0      112 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 14:50:31.000000 denpy-1.0.7/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:50:31.832041 denpy-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      205 2023-06-12 14:50:10.000000 denpy-1.0.7/setup.py
```

### Comparing `denpy-1.0.6/denpy/database.py` & `denpy-1.0.7/denpy/database.py`

 * *Files identical despite different names*

### Comparing `denpy-1.0.6/denpy/utils.py` & `denpy-1.0.7/denpy/utils.py`

 * *Files identical despite different names*

