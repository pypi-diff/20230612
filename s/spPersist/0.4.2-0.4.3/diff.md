# Comparing `tmp/spPersist-0.4.2.tar.gz` & `tmp/spPersist-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.4.2.tar", last modified: Mon Jun 12 01:41:38 2023, max compression
+gzip compressed data, was "spPersist-0.4.3.tar", last modified: Mon Jun 12 01:51:07 2023, max compression
```

## Comparing `spPersist-0.4.2.tar` & `spPersist-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.781515 spPersist-0.4.2/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:41:38.780515 spPersist-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 01:41:38.781515 spPersist-0.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 01:40:44.000000 spPersist-0.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.777515 spPersist-0.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.779515 spPersist-0.4.2/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.2/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-06-12 01:23:43.000000 spPersist-0.4.2/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:41:38.780515 spPersist-0.4.2/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 01:41:38.000000 spPersist-0.4.2/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:51:07.420174 spPersist-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-0.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:51:07.420174 spPersist-0.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-0.4.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 01:51:07.420174 spPersist-0.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 01:50:15.000000 spPersist-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:51:07.414173 spPersist-0.4.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:51:07.418174 spPersist-0.4.3/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-0.4.3/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-0.4.3/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-0.4.3/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-0.4.3/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-0.4.3/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-0.4.3/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2023-06-12 01:50:33.000000 spPersist-0.4.3/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 01:51:07.419174 spPersist-0.4.3/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 01:51:07.000000 spPersist-0.4.3/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 01:51:07.000000 spPersist-0.4.3/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 01:51:07.000000 spPersist-0.4.3/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 01:51:07.000000 spPersist-0.4.3/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 01:51:07.000000 spPersist-0.4.3/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.4.2/LICENSE` & `spPersist-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.2/PKG-INFO` & `spPersist-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.2
+Version: 0.4.3
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-0.4.2/README.md` & `spPersist-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.2/setup.py` & `spPersist-0.4.3/setup.py`

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
-    version="0.4.2",  # Required
+    version="0.4.3",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.4.2/src/spPersist/DTM_filtrations.py` & `spPersist-0.4.3/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.2/src/spPersist/dp.py` & `spPersist-0.4.3/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.2/src/spPersist/hc.py` & `spPersist-0.4.3/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.2/src/spPersist/persistence_statistics.py` & `spPersist-0.4.3/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.2/src/spPersist/ph.py` & `spPersist-0.4.3/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.4.2/src/spPersist/pp.py` & `spPersist-0.4.3/src/spPersist/pp.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,18 @@
       int(p)
     except:
       p = None
     else:
       p = int(p)
     ps.append(p)
 
-  sc.pp.filter_cells(adata, min_counts=ps[0],min_genes=ps[1],max_counts=ps[2],max_genes=ps[3],inplace=True)
+  sc.pp.filter_cells(adata, min_counts=ps[0], inplace=True)
+  sc.pp.filter_cells(adata, min_genes=ps[1], inplace=True)
+  sc.pp.filter_cells(adata, max_counts=ps[2], inplace=True)
+  sc.pp.filter_cells(adata, max_genes=ps[3], inplace=True)
 
   print('Filtering genes...\nPress Enter to skip the parameter.')
   params = ['min_counts', 'min_cells', 'max_counts','max_cells']
   ps = []
   for s in params:
     p = input('Enter '+ s + ':')
     print(s + ': ' + p)
@@ -45,15 +48,18 @@
       int(p)
     except:
       p = None
     else:
       p = int(p)
     ps.append(p)
 
-  sc.pp.filter_genes(adata, min_counts=ps[0],min_cells=ps[1],max_counts=ps[2],max_cells=ps[3],inplace=True)
+  sc.pp.filter_genes(adata, min_counts=ps[0], inplace=True)
+  sc.pp.filter_genes(adata, min_cells=ps[1], inplace=True)
+  sc.pp.filter_genes(adata, max_counts=ps[2], inplace=True)
+  sc.pp.filter_genes(adata, max_cells=ps[3], inplace=True)
 
 
 def deconvolute(ad, ref):
   '''
   deconvolute takes an annotated data object ad produced
   in the data processing module and a single-cell reference 
   data ref as a pandas dataframe, and performs deconvolution
```

### Comparing `spPersist-0.4.2/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.4.3/src/spPersist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.4.2
+Version: 0.4.3
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

