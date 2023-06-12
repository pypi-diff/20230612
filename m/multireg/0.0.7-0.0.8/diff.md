# Comparing `tmp/multireg-0.0.7.tar.gz` & `tmp/multireg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multireg-0.0.7.tar", last modified: Fri Jun  9 09:22:52 2023, max compression
+gzip compressed data, was "multireg-0.0.8.tar", last modified: Mon Jun 12 08:04:20 2023, max compression
```

## Comparing `multireg-0.0.7.tar` & `multireg-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:22:52.000389 multireg-0.0.7/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.7/LICENSE
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.7/MANIFEST.in
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:22:52.000389 multireg-0.0.7/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     3566 2023-06-09 08:56:32.000000 multireg-0.0.7/README.md
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.7/pyproject.toml
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1512 2023-06-09 09:22:52.000389 multireg-0.0.7/setup.cfg
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.7/setup.py
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:22:51.996389 multireg-0.0.7/src/
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:22:51.996389 multireg-0.0.7/src/multireg/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    24872 2023-06-09 09:12:46.000000 multireg-0.0.7/src/multireg/MultiReg.py
--rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-07 14:30:43.000000 multireg-0.0.7/src/multireg/Utils.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-07 14:24:19.000000 multireg-0.0.7/src/multireg/__init__.py
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-07 14:36:50.000000 multireg-0.0.7/src/multireg/napari.yaml
-drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-09 09:22:52.000389 multireg-0.0.7/src/multireg.egg-info/
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     4797 2023-06-09 09:22:51.000000 multireg-0.0.7/src/multireg.egg-info/PKG-INFO
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-09 09:22:51.000000 multireg-0.0.7/src/multireg.egg-info/SOURCES.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-09 09:22:51.000000 multireg-0.0.7/src/multireg.egg-info/dependency_links.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-09 09:22:51.000000 multireg-0.0.7/src/multireg.egg-info/entry_points.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-09 09:22:51.000000 multireg-0.0.7/src/multireg.egg-info/requires.txt
--rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-09 09:22:51.000000 multireg-0.0.7/src/multireg.egg-info/top_level.txt
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.378888 multireg-0.0.8/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1523 2023-06-07 14:15:52.000000 multireg-0.0.8/LICENSE
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-07 14:19:41.000000 multireg-0.0.8/MANIFEST.in
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9457 2023-06-12 08:04:20.378888 multireg-0.0.8/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     8303 2023-06-12 08:02:49.000000 multireg-0.0.8/README.md
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1177 2023-06-07 14:19:41.000000 multireg-0.0.8/pyproject.toml
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     1446 2023-06-12 08:04:20.378888 multireg-0.0.8/setup.cfg
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       37 2023-06-07 14:33:30.000000 multireg-0.0.8/setup.py
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.374888 multireg-0.0.8/src/
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.374888 multireg-0.0.8/src/multireg/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)    24872 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/MultiReg.py
+-rwxrwxr-x   0 gaelle    (1001) gaelle    (1001)     8152 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/Utils.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/__init__.py
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      310 2023-06-12 08:01:54.000000 multireg-0.0.8/src/multireg/napari.yaml
+drwxrwxr-x   0 gaelle    (1001) gaelle    (1001)        0 2023-06-12 08:04:20.378888 multireg-0.0.8/src/multireg.egg-info/
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)     9457 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/PKG-INFO
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)      378 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        1 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       50 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/entry_points.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)       96 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/requires.txt
+-rw-rw-r--   0 gaelle    (1001) gaelle    (1001)        9 2023-06-12 08:04:20.000000 multireg-0.0.8/src/multireg.egg-info/top_level.txt
```

### Comparing `multireg-0.0.7/LICENSE` & `multireg-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `multireg-0.0.7/pyproject.toml` & `multireg-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multireg-0.0.7/setup.cfg` & `multireg-0.0.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [metadata]
 name = multireg
-version = 0.0.7
+version = 0.0.8
 description = Registration of 3D multiplex images with one common chanel
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Gaëlle Letort
 author_email = gaelle.letort@pasteur.fr
 url = https://gitlab.pasteur.fr/gletort/multireg
 project_urls = 
 	Bug Tracker = https://gitlab.pasteur.fr/gletort/multireg/issues
 	Documentation = https://gitlab.pasteur.fr/gletort/mutlireg#README.md
 	Source Code = https://gitlab.pasteur.fr/gletort/multireg
-	User Support = https://gitlab.pasteur.fr/gletort/multireg/issues
 license = BSD-3-Clause
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Framework :: napari
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
```

### Comparing `multireg-0.0.7/src/multireg/MultiReg.py` & `multireg-0.0.8/src/multireg/MultiReg.py`

 * *Files identical despite different names*

### Comparing `multireg-0.0.7/src/multireg/Utils.py` & `multireg-0.0.8/src/multireg/Utils.py`

 * *Files identical despite different names*

