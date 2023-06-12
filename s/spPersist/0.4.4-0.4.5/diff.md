# Comparing `tmp/spPersist-0.4.4.tar.gz` & `tmp/spPersist-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.4.4.tar", last modified: Mon Jun 12 02:02:08 2023, max compression
+gzip compressed data, was "spPersist-0.4.5.tar", last modified: Mon Jun 12 02:23:12 2023, max compression
```

## Comparing `spPersist-0.4.4.tar` & `spPersist-0.4.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:02:08.125261 spPersist-0.4.4/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:02:08.125261 spPersist-0.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 02:02:08.125261 spPersist-0.4.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 01:58:25.000000 spPersist-0.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:02:08.121261 spPersist-0.4.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:02:08.123261 spPersist-0.4.4/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.4/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.4/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.4/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.4/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.4/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.4/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-06-12 01:59:47.000000 spPersist-0.4.4/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:02:08.125261 spPersist-0.4.4/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:02:08.000000 spPersist-0.4.4/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 02:02:08.000000 spPersist-0.4.4/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:02:08.000000 spPersist-0.4.4/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 02:02:08.000000 spPersist-0.4.4/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 02:02:08.000000 spPersist-0.4.4/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.689464 spPersist-0.4.5/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:23:12.689464 spPersist-0.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 02:23:12.689464 spPersist-0.4.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 02:22:25.000000 spPersist-0.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.685464 spPersist-0.4.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.687464 spPersist-0.4.5/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.5/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-06-12 02:22:59.000000 spPersist-0.4.5/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:23:12.688464 spPersist-0.4.5/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 02:23:12.000000 spPersist-0.4.5/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.4.4/LICENSE` & `spPersist-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.4/PKG-INFO` & `spPersist-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.4
+Version: 0.4.5
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-0.4.4/README.md` & `spPersist-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.4/setup.py` & `spPersist-0.4.5/setup.py`

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
-    version="0.4.4",  # Required
+    version="0.4.5",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.4.4/src/spPersist/DTM_filtrations.py` & `spPersist-0.4.5/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.4/src/spPersist/dp.py` & `spPersist-0.4.5/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.4/src/spPersist/hc.py` & `spPersist-0.4.5/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.4/src/spPersist/persistence_statistics.py` & `spPersist-0.4.5/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.4/src/spPersist/ph.py` & `spPersist-0.4.5/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.4/src/spPersist/pp.py` & `spPersist-0.4.5/src/spPersist/pp.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,18 +29,22 @@
       int(p)
     except:
       p = None
     else:
       p = int(p)
     ps.append(p)
 
-  sc.pp.filter_cells(adata, min_counts=ps[0])
-  sc.pp.filter_cells(adata, min_genes=ps[1])
-  sc.pp.filter_cells(adata, max_counts=ps[2])
-  sc.pp.filter_cells(adata, max_genes=ps[3])
+  if ps[0] is not None:
+    sc.pp.filter_cells(adata, min_counts=ps[0])
+  if ps[1] is not None:
+   sc.pp.filter_cells(adata, min_genes=ps[1])
+  if ps[2] is not None:
+    sc.pp.filter_cells(adata, max_counts=ps[2])
+  if ps[3] is not None:
+    sc.pp.filter_cells(adata, max_genes=ps[3])
 
   print('Filtering genes...\nPress Enter to skip the parameter.')
   params = ['min_counts', 'min_cells', 'max_counts','max_cells']
   ps = []
   for s in params:
     p = input('Enter '+ s + ':')
     print(s + ': ' + p)
@@ -48,18 +52,21 @@
       int(p)
     except:
       p = None
     else:
       p = int(p)
     ps.append(p)
 
-  sc.pp.filter_genes(adata, min_counts=ps[0])
-  sc.pp.filter_genes(adata, min_cells=ps[1])
-  sc.pp.filter_genes(adata, max_counts=ps[2])
-  sc.pp.filter_genes(adata, max_cells=ps[3])
+  if ps[0] is not None:
+    sc.pp.filter_genes(adata, min_counts=ps[0])
+  if ps[1] is not None:
+    sc.pp.filter_genes(adata, min_cells=ps[1])
+  if ps[2] is not None:
+    sc.pp.filter_genes(adata, max_counts=ps[2])
+  if sc.pp.filter_genes(adata, max_cells=ps[3])
 
 
 def deconvolute(ad, ref):
   '''
   deconvolute takes an annotated data object ad produced
   in the data processing module and a single-cell reference 
   data ref as a pandas dataframe, and performs deconvolution
```

### Comparing `spPersist-0.4.4/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.4.5/src/spPersist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.4
+Version: 0.4.5
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

