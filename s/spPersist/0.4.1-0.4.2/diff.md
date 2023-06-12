# Comparing `tmp/spPersist-0.4.1.tar.gz` & `tmp/spPersist-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.4.1.tar", last modified: Mon Jun 12 01:26:45 2023, max compression
+gzip compressed data, was "spPersist-0.4.2.tar", last modified: Mon Jun 12 01:41:38 2023, max compression
```

## Comparing `spPersist-0.4.1.tar` & `spPersist-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:26:45.276196 spPersist-0.4.1/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:26:45.276196 spPersist-0.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 01:26:45.276196 spPersist-0.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 01:26:13.000000 spPersist-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:26:45.271196 spPersist-0.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:26:45.274196 spPersist-0.4.1/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.1/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.1/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.1/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.1/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.1/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.1/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-06-12 01:23:43.000000 spPersist-0.4.1/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:26:45.275196 spPersist-0.4.1/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:26:45.000000 spPersist-0.4.1/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 01:26:45.000000 spPersist-0.4.1/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 01:26:45.000000 spPersist-0.4.1/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 01:26:45.000000 spPersist-0.4.1/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 01:26:45.000000 spPersist-0.4.1/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.781515 spPersist-0.4.2/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:41:38.780515 spPersist-0.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 01:41:38.781515 spPersist-0.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 01:40:44.000000 spPersist-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.777515 spPersist-0.4.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.779515 spPersist-0.4.2/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-06-12 01:23:43.000000 spPersist-0.4.2/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.780515 spPersist-0.4.2/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.4.1/LICENSE` & `spPersist-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/PKG-INFO` & `spPersist-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.1
+Version: 0.4.2
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-0.4.1/README.md` & `spPersist-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/setup.py` & `spPersist-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="spPersist",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.1",  # Required
+    version="0.4.2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.4.1/src/spPersist/DTM_filtrations.py` & `spPersist-0.4.2/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/src/spPersist/dp.py` & `spPersist-0.4.2/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/src/spPersist/hc.py` & `spPersist-0.4.2/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/src/spPersist/persistence_statistics.py` & `spPersist-0.4.2/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/src/spPersist/ph.py` & `spPersist-0.4.2/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/src/spPersist/pp.py` & `spPersist-0.4.2/src/spPersist/pp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.1/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.4.2/src/spPersist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.1
+Version: 0.4.2
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

