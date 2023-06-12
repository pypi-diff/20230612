# Comparing `tmp/spPersist-1.0.1.tar.gz` & `tmp/spPersist-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-1.0.1.tar", last modified: Mon Jun 12 06:52:33 2023, max compression
+gzip compressed data, was "spPersist-1.0.2.tar", last modified: Mon Jun 12 07:25:18 2023, max compression
```

## Comparing `spPersist-1.0.1.tar` & `spPersist-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.843641 spPersist-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 06:52:13.000000 spPersist-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 06:52:33.842641 spPersist-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 06:52:13.000000 spPersist-1.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 06:52:33.843641 spPersist-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 06:52:13.000000 spPersist-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.839641 spPersist-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.841641 spPersist-1.0.1/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 06:49:31.000000 spPersist-1.0.1/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     4791 2023-06-12 06:51:08.000000 spPersist-1.0.1/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 06:52:33.842641 spPersist-1.0.1/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 06:52:33.000000 spPersist-1.0.1/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.345485 spPersist-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-12 06:52:13.000000 spPersist-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 07:25:18.339484 spPersist-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-12 06:52:13.000000 spPersist-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 07:25:18.345485 spPersist-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8134 2023-06-12 07:24:24.000000 spPersist-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.333484 spPersist-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.338484 spPersist-1.0.2/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-12 06:49:31.000000 spPersist-1.0.2/src/spPersist/ph.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-06-12 07:24:05.000000 spPersist-1.0.2/src/spPersist/pp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:25:18.339484 spPersist-1.0.2/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 07:25:18.000000 spPersist-1.0.2/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-1.0.1/LICENSE` & `spPersist-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.1/PKG-INFO` & `spPersist-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.1
+Version: 1.0.2
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spPersist-1.0.1/README.md` & `spPersist-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.1/setup.py` & `spPersist-1.0.2/setup.py`

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
-    version="1.0.1",  # Required
+    version="1.0.2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-1.0.1/src/spPersist/DTM_filtrations.py` & `spPersist-1.0.2/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.1/src/spPersist/dp.py` & `spPersist-1.0.2/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.1/src/spPersist/hc.py` & `spPersist-1.0.2/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.1/src/spPersist/persistence_statistics.py` & `spPersist-1.0.2/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.1/src/spPersist/ph.py` & `spPersist-1.0.2/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.1/src/spPersist/pp.py` & `spPersist-1.0.2/src/spPersist/pp.py`

 * *Files 24% similar despite different names*

```diff
@@ -109,14 +109,53 @@
     p = None
     print('Empty entry or the parameter is invalid.')
   else:
     p = int(p)
     sc.pp.filter_genes(adata, max_cells=p)
 
 
+def extract_reference_data(adata_ref):
+  '''
+  extract_reference_data takes a single-cell reference data adata_ref
+  as annotated data object, and returns the estimated reference expression
+  as a pandas dataframe.
+  '''
+
+  # prepare anndata for the regression model
+  cell2location.models.RegressionModel.setup_anndata(adata=adata_ref, 
+                          # 10X reaction / sample / batch
+                          batch_key='Sample', 
+                          # cell type, covariate used for constructing signatures
+                          labels_key='Subset', 
+                          # multiplicative technical effects (platform, 3' vs 5', donor effect)
+                          categorical_covariate_keys=['Method']
+                        )
+  
+  from cell2location.models import RegressionModel
+  mod = RegressionModel(adata_ref) 
+
+  mod.train(max_epochs=250, use_gpu=True)
+
+  adata_ref = mod.export_posterior(
+      adata_ref, sample_kwargs={'num_samples': 1000, 'batch_size': 2500, 'use_gpu': True}
+  )
+
+  # export estimated expression in each cluster
+  if 'means_per_cluster_mu_fg' in adata_ref.varm.keys():
+      inf_aver = adata_ref.varm['means_per_cluster_mu_fg'][[f'means_per_cluster_mu_fg_{i}' 
+                                      for i in adata_ref.uns['mod']['factor_names']]].copy()
+  else:
+      inf_aver = adata_ref.var[[f'means_per_cluster_mu_fg_{i}' 
+                                      for i in adata_ref.uns['mod']['factor_names']]].copy()
+  inf_aver.columns = adata_ref.uns['mod']['factor_names']
+  inf_aver.iloc[0:5, 0:5]
+
+  return inf_aver
+
+
 def deconvolute(ad, ref):
   '''
   deconvolute takes an annotated data object ad produced
   in the data processing module and a single-cell reference 
   data ref as a pandas dataframe, and performs deconvolution 
   methods as demonstrated in the cell2location tutorial with 
   human lymph node. It returns the spatially resolved
```

### Comparing `spPersist-1.0.1/src/spPersist.egg-info/PKG-INFO` & `spPersist-1.0.2/src/spPersist.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.1
+Version: 1.0.2
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

