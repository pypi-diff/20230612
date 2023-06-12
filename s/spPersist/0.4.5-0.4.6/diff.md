# Comparing `tmp/spPersist-0.4.5.tar.gz` & `tmp/spPersist-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.4.5.tar", last modified: Mon Jun 12 02:23:12 2023, max compression
+gzip compressed data, was "spPersist-0.4.6.tar", last modified: Mon Jun 12 02:36:34 2023, max compression
```

## Comparing `spPersist-0.4.5.tar` & `spPersist-0.4.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.689464 spPersist-0.4.5/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:23:12.689464 spPersist-0.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 02:23:12.689464 spPersist-0.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 02:22:25.000000 spPersist-0.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.685464 spPersist-0.4.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.687464 spPersist-0.4.5/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     3081 2023-06-12 02:22:59.000000 spPersist-0.4.5/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.688464 spPersist-0.4.5/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:36:34.558396 spPersist-0.4.6/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:36:34.557396 spPersist-0.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 02:36:34.558396 spPersist-0.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 02:36:08.000000 spPersist-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:36:34.554396 spPersist-0.4.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:36:34.556396 spPersist-0.4.6/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.6/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.6/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.6/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.6/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.6/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.6/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-06-12 02:34:59.000000 spPersist-0.4.6/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:36:34.557396 spPersist-0.4.6/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:36:34.000000 spPersist-0.4.6/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 02:36:34.000000 spPersist-0.4.6/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:36:34.000000 spPersist-0.4.6/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 02:36:34.000000 spPersist-0.4.6/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 02:36:34.000000 spPersist-0.4.6/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.4.5/LICENSE` & `spPersist-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.5/PKG-INFO` & `spPersist-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.5
+Version: 0.4.6
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-0.4.5/README.md` & `spPersist-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.5/setup.py` & `spPersist-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="spPersist",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.5",  # Required
+    version="0.4.6",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.4.5/src/spPersist/DTM_filtrations.py` & `spPersist-0.4.6/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.5/src/spPersist/dp.py` & `spPersist-0.4.6/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.5/src/spPersist/hc.py` & `spPersist-0.4.6/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.5/src/spPersist/persistence_statistics.py` & `spPersist-0.4.6/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.5/src/spPersist/ph.py` & `spPersist-0.4.6/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.5/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.4.6/src/spPersist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.5
+Version: 0.4.6
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

