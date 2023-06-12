# Comparing `tmp/spPersist-1.0.0.tar.gz` & `tmp/spPersist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-1.0.0.tar", last modified: Mon Jun 12 03:45:56 2023, max compression
+gzip compressed data, was "spPersist-1.0.1.tar", last modified: Mon Jun 12 06:52:33 2023, max compression
```

## Comparing `spPersist-1.0.0.tar` & `spPersist-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:45:56.320697 spPersist-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 01:26:13.000000 spPersist-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 03:45:56.320697 spPersist-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 01:26:13.000000 spPersist-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 03:45:56.320697 spPersist-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 03:45:01.000000 spPersist-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:45:56.316697 spPersist-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:45:56.319697 spPersist-1.0.0/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 01:23:44.000000 spPersist-1.0.0/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 01:23:44.000000 spPersist-1.0.0/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 01:23:44.000000 spPersist-1.0.0/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 01:23:44.000000 spPersist-1.0.0/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 01:23:44.000000 spPersist-1.0.0/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 01:23:44.000000 spPersist-1.0.0/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     4499 2023-06-12 03:44:40.000000 spPersist-1.0.0/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:45:56.320697 spPersist-1.0.0/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 03:45:56.000000 spPersist-1.0.0/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 03:45:56.000000 spPersist-1.0.0/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:45:56.000000 spPersist-1.0.0/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 03:45:56.000000 spPersist-1.0.0/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 03:45:56.000000 spPersist-1.0.0/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.843641 spPersist-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 06:52:13.000000 spPersist-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 06:52:33.842641 spPersist-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 06:52:13.000000 spPersist-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 06:52:33.843641 spPersist-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 06:52:13.000000 spPersist-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.839641 spPersist-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.841641 spPersist-1.0.1/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2023-06-12 06:51:08.000000 spPersist-1.0.1/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.842641 spPersist-1.0.1/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-1.0.0/LICENSE` & `spPersist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.0/PKG-INFO` & `spPersist-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-Metadata-Version: 2.1
-Name: spPersist
-Version: 1.0.0
-Summary: Spatial transcriptomics with Persistent Homology
-Author: Lirong Yang
-Author-email: lirong.yang@outlook.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Spatial transcriptomics with Persistent Homology
-
-This is a package for classifying Spatial transcriptomics data according to its 
-spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and persistence diagram. The package 
-contains a data processing module, called dp, allowing users to load either the
-standard datasets from Visium and MERFISH, or published datasets into desired
-annotated data format for the analysis performed in this package. The format is
-compatible with the package Squidpy.
-
-The package also includes a pre-processing module, a 
-persistent homology module and a homological classification module, respectively
-named pp, ph and hc.
-
-The pre-processing module contains quality control metrics, deconvolution
-methods and cell type identifications.
-
-The persistent homology module contains functions for computing simplicial 
-complexes of point clouds (See data structures in the gudhi package.) and their
-topological measures. It also includes plotting features of the persistence 
-diagram.
-
-The homological classification module computes the number of holes and connected
-components as a dictionary.
+# Spatial transcriptomics with Persistent Homology
+
+This is a package for classifying Spatial transcriptomics data according to its 
+spatial topology. The specific mathematical foundation for the classification is
+the theory of Persistent Homology and persistence diagram. The package 
+contains a data processing module, called dp, allowing users to load either the
+standard datasets from Visium and MERFISH, or published datasets into desired
+annotated data format for the analysis performed in this package. The format is
+compatible with the package Squidpy.
+
+The package also includes a pre-processing module, a 
+persistent homology module and a homological classification module, respectively
+named pp, ph and hc.
+
+The pre-processing module contains quality control metrics, deconvolution
+methods and cell type identifications.
+
+The persistent homology module contains functions for computing simplicial 
+complexes of point clouds (See data structures in the gudhi package.) and their
+topological measures. It also includes plotting features of the persistence 
+diagram.
+
+The homological classification module computes the number of holes and connected
+components as a dictionary.
```

### Comparing `spPersist-1.0.0/README.md` & `spPersist-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,34 @@
-# Spatial transcriptomics with Persistent Homology
-
-This is a package for classifying Spatial transcriptomics data according to its 
-spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and persistence diagram. The package 
-contains a data processing module, called dp, allowing users to load either the
-standard datasets from Visium and MERFISH, or published datasets into desired
-annotated data format for the analysis performed in this package. The format is
-compatible with the package Squidpy.
-
-The package also includes a pre-processing module, a 
-persistent homology module and a homological classification module, respectively
-named pp, ph and hc.
-
-The pre-processing module contains quality control metrics, deconvolution
-methods and cell type identifications.
-
-The persistent homology module contains functions for computing simplicial 
-complexes of point clouds (See data structures in the gudhi package.) and their
-topological measures. It also includes plotting features of the persistence 
-diagram.
-
-The homological classification module computes the number of holes and connected
-components as a dictionary.
+Metadata-Version: 2.1
+Name: spPersist
+Version: 1.0.1
+Summary: Spatial transcriptomics with Persistent Homology
+Author: Lirong Yang
+Author-email: lirong.yang@outlook.com
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Spatial transcriptomics with Persistent Homology
+
+This is a package for classifying Spatial transcriptomics data according to its 
+spatial topology. The specific mathematical foundation for the classification is
+the theory of Persistent Homology and persistence diagram. The package 
+contains a data processing module, called dp, allowing users to load either the
+standard datasets from Visium and MERFISH, or published datasets into desired
+annotated data format for the analysis performed in this package. The format is
+compatible with the package Squidpy.
+
+The package also includes a pre-processing module, a 
+persistent homology module and a homological classification module, respectively
+named pp, ph and hc.
+
+The pre-processing module contains quality control metrics, deconvolution
+methods and cell type identifications.
+
+The persistent homology module contains functions for computing simplicial 
+complexes of point clouds (See data structures in the gudhi package.) and their
+topological measures. It also includes plotting features of the persistence 
+diagram.
+
+The homological classification module computes the number of holes and connected
+components as a dictionary.
```

### Comparing `spPersist-1.0.0/setup.py` & `spPersist-1.0.1/setup.py`

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
-    version="1.0.0",  # Required
+    version="1.0.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-1.0.0/src/spPersist/DTM_filtrations.py` & `spPersist-1.0.1/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.0/src/spPersist/dp.py` & `spPersist-1.0.1/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.0/src/spPersist/hc.py` & `spPersist-1.0.1/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.0/src/spPersist/persistence_statistics.py` & `spPersist-1.0.1/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.0/src/spPersist/ph.py` & `spPersist-1.0.1/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.0/src/spPersist/pp.py` & `spPersist-1.0.1/src/spPersist/pp.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,14 +147,23 @@
           )
 
   # In this section, we export the estimated cell abundance (summary of the posterior distribution).
   adata = mod.export_posterior(
       adata, sample_kwargs={'num_samples': 1000, 'batch_size': mod.adata.n_obs, 'use_gpu': True}
   )
 
+  # Compute expected expression per cell type
+  expected_dict = mod.module.model.compute_expected_per_cell_type(
+      mod.samples["post_sample_q05"], mod.adata_manager
+  )
+
+  # Add to anndata layers
+  for i, n in enumerate(mod.factor_names_):
+      adata.layers[n] = expected_dict['mu'][i]
+
   return adata
 
 
 def cell_type_identification(adata):
   '''
   cell_type_identification takes an annotated data object adata, and
   identifies cell types in adata via KNN and Leiden clustering, as
```

### Comparing `spPersist-1.0.0/src/spPersist.egg-info/PKG-INFO` & `spPersist-1.0.1/src/spPersist.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

