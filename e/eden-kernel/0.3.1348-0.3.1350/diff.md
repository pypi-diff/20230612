# Comparing `tmp/eden-kernel-0.3.1348.tar.gz` & `tmp/eden-kernel-0.3.1350.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eden-kernel-0.3.1348.tar", last modified: Tue Jun 28 11:15:48 2022, max compression
+gzip compressed data, was "eden-kernel-0.3.1350.tar", last modified: Mon Jun 12 10:07:16 2023, max compression
```

## Comparing `eden-kernel-0.3.1348.tar` & `eden-kernel-0.3.1350.tar`

### file list

```diff
@@ -1,59 +1,35 @@
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.276756 eden-kernel-0.3.1348/
--rw-r--r--   0 ikea      (1000) ikea      (1000)      926 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/.gitignore
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1527 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/.travis.yml
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1081 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/LICENSE
--rw-r--r--   0 ikea      (1000) ikea      (1000)      270 2022-06-28 11:15:48.273423 eden-kernel-0.3.1348/PKG-INFO
--rw-r--r--   0 ikea      (1000) ikea      (1000)     4604 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/README.md
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.270089 eden-kernel-0.3.1348/conda/
--rw-r--r--   0 ikea      (1000) ikea      (1000)       38 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/conda/build.sh
--rw-r--r--   0 ikea      (1000) ikea      (1000)      408 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/conda/conda_upload.sh
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1293 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/conda/meta.yaml
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.270089 eden-kernel-0.3.1348/eden/
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2410 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/__init__.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      182 2022-06-28 11:15:48.000000 eden-kernel-0.3.1348/eden/_version.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.270089 eden-kernel-0.3.1348/eden/align/
--rw-r--r--   0 ikea      (1000) ikea      (1000)    14027 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/align/__init__.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.270089 eden-kernel-0.3.1348/eden/display/
--rw-r--r--   0 ikea      (1000) ikea      (1000)    27291 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/display/__init__.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     6356 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/display/graph_layout.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)    42815 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/graph.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.273423 eden-kernel-0.3.1348/eden/io/
--rw-r--r--   0 ikea      (1000) ikea      (1000)      295 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/eden/io/__init__.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3512 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/io/gspan.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1436 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/io/node_link_data.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      837 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/io/sequence.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1113 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/io/word_sequence.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     5138 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/iterated_maximum_subarray.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.273423 eden-kernel-0.3.1348/eden/ml/
--rw-r--r--   0 ikea      (1000) ikea      (1000)        0 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/eden/ml/__init__.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     9130 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/ml/estimator.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     7330 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/ml/estimator_utils.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3261 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/ml/link_prediction.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     3390 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/ml/link_prediction_utils.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)    17175 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/ml/ml.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)    22172 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/sequence.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     9140 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/eden/util.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.273423 eden-kernel-0.3.1348/eden_kernel.egg-info/
--rw-r--r--   0 ikea      (1000) ikea      (1000)      270 2022-06-28 11:15:48.000000 eden-kernel-0.3.1348/eden_kernel.egg-info/PKG-INFO
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1232 2022-06-28 11:15:48.000000 eden-kernel-0.3.1348/eden_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)        1 2022-06-28 11:15:48.000000 eden-kernel-0.3.1348/eden_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)      108 2022-06-28 11:15:48.000000 eden-kernel-0.3.1348/eden_kernel.egg-info/requires.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)        5 2022-06-28 11:15:48.000000 eden-kernel-0.3.1348/eden_kernel.egg-info/top_level.txt
--rw-r--r--   0 ikea      (1000) ikea      (1000)      138 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/requirements.txt
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.273423 eden-kernel-0.3.1348/resources/
--rw-r--r--   0 ikea      (1000) ikea      (1000)    86500 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/resources/EDeN_logo.png
--rw-r--r--   0 ikea      (1000) ikea      (1000)   209400 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/resources/EDeN_logo.svg
--rw-r--r--   0 ikea      (1000) ikea      (1000)    29595 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/resources/EDeN_logo_small.png
--rw-r--r--   0 ikea      (1000) ikea      (1000)      979 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/resources/example_restart_python.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)       38 2022-06-28 11:15:48.276756 eden-kernel-0.3.1348/setup.cfg
--rwxr-xr-x   0 ikea      (1000) ikea      (1000)     3484 2022-06-28 11:15:36.000000 eden-kernel-0.3.1348/setup.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.273423 eden-kernel-0.3.1348/test/
--rw-r--r--   0 ikea      (1000) ikea      (1000)        0 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/test/__init__.py
-drwxr-xr-x   0 ikea      (1000) ikea      (1000)        0 2022-06-28 11:15:48.273423 eden-kernel-0.3.1348/test/disabled_tests/
--rw-r--r--   0 ikea      (1000) ikea      (1000)      699 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/test/disabled_tests/test_annotate_cycle.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      844 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/test/disabled_tests/test_annotate_rna_secondary_structure.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)     1796 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/test/disabled_tests/test_eden_modifier_graph_vertex_attributes.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      106 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/test/disabled_tests/test_fasta_to_sequence.fa
--rw-r--r--   0 ikea      (1000) ikea      (1000)     2229 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/test/disabled_tests/test_fasta_to_sequence.py
--rw-r--r--   0 ikea      (1000) ikea      (1000)      116 2021-03-08 19:55:31.000000 eden-kernel-0.3.1348/test/disabled_tests/test_fasta_to_sequence_with_center_annotation.fa
--rw-r--r--   0 ikea      (1000) ikea      (1000)      471 2021-03-08 19:55:55.000000 eden-kernel-0.3.1348/test/disabled_tests/test_notebooks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-12 10:07:16.688000 eden-kernel-0.3.1350/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1081 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      276 2023-06-12 10:07:16.688000 eden-kernel-0.3.1350/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-12 10:07:16.684000 eden-kernel-0.3.1350/eden/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2410 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      182 2023-06-12 10:07:16.000000 eden-kernel-0.3.1350/eden/_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-12 10:07:16.684000 eden-kernel-0.3.1350/eden/display/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27291 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/display/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6356 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/display/graph_layout.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42817 2023-06-12 10:03:55.000000 eden-kernel-0.3.1350/eden/graph.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-12 10:07:16.684000 eden-kernel-0.3.1350/eden/io/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/io/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3512 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/io/gspan.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1436 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/io/node_link_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/io/sequence.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/io/word_sequence.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5138 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/iterated_maximum_subarray.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-12 10:07:16.688000 eden-kernel-0.3.1350/eden/ml/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/ml/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9130 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/ml/estimator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7330 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/ml/estimator_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3261 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/ml/link_prediction.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3390 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/ml/link_prediction_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17175 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/ml/ml.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22172 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/sequence.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9140 2021-05-03 20:51:04.000000 eden-kernel-0.3.1350/eden/util.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-12 10:07:16.688000 eden-kernel-0.3.1350/eden_kernel.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      276 2023-06-12 10:07:16.000000 eden-kernel-0.3.1350/eden_kernel.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      616 2023-06-12 10:07:16.000000 eden-kernel-0.3.1350/eden_kernel.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-12 10:07:16.000000 eden-kernel-0.3.1350/eden_kernel.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2023-06-12 10:07:16.000000 eden-kernel-0.3.1350/eden_kernel.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-12 10:07:16.000000 eden-kernel-0.3.1350/eden_kernel.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-12 10:07:16.688000 eden-kernel-0.3.1350/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-06-12 09:14:40.000000 eden-kernel-0.3.1350/setup.py
```

### Comparing `eden-kernel-0.3.1348/LICENSE` & `eden-kernel-0.3.1350/LICENSE`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/README.md` & `eden-kernel-0.3.1350/README.md`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/__init__.py` & `eden-kernel-0.3.1350/eden/__init__.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/display/__init__.py` & `eden-kernel-0.3.1350/eden/display/__init__.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/display/graph_layout.py` & `eden-kernel-0.3.1350/eden/display/graph_layout.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/graph.py` & `eden-kernel-0.3.1350/eden/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from eden import fast_hash, fast_hash_vec
 from eden import fast_hash_2, fast_hash_3, fast_hash_4
 from eden import AbstractVectorizer
 from eden.util import serialize_dict
 from itertools import tee
 import logging
 logger = logging.getLogger(__name__)
-from multiprocessing import Pool 
+from multiprocessing import Pool
 
 def auto_label(graphs, n_clusters=16, **opts):
     """Label nodes with cluster id.
 
     Cluster nodes using as features the output of vertex_vectorize.
     """
     data_list = Vectorizer(**opts).vertex_transform(graphs)
@@ -458,16 +458,16 @@
                 node_feature_list)
             self._update_feature_list(
                 node_sparse_feature_list,
                 feature_list)
 
     def _add_vector_labes(self, graph, vertex_v, node_feature_list):
         # add the vector with an offset given by the feature, multiplied by val
-        vec = graph.nodes[vertex_v].get(self.key_vec, None)
-        if vec:
+        vec = graph.nodes[vertex_v].get(self.key_vec, [])
+        if any(vec):
             vec_feature_list = defaultdict(lambda: defaultdict(float))
             for radius_dist_key in node_feature_list:
                 for feature in node_feature_list[radius_dist_key]:
                     val = node_feature_list[radius_dist_key][feature]
                     for i, vec_val in enumerate(vec):
                         key = (feature + i) % self.bitmask
                         vec_feature_list[radius_dist_key][key] += val * vec_val
```

### Comparing `eden-kernel-0.3.1348/eden/io/gspan.py` & `eden-kernel-0.3.1350/eden/io/gspan.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/io/node_link_data.py` & `eden-kernel-0.3.1350/eden/io/node_link_data.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/io/sequence.py` & `eden-kernel-0.3.1350/eden/io/sequence.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/io/word_sequence.py` & `eden-kernel-0.3.1350/eden/io/word_sequence.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/iterated_maximum_subarray.py` & `eden-kernel-0.3.1350/eden/iterated_maximum_subarray.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/ml/estimator.py` & `eden-kernel-0.3.1350/eden/ml/estimator.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/ml/estimator_utils.py` & `eden-kernel-0.3.1350/eden/ml/estimator_utils.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/ml/link_prediction.py` & `eden-kernel-0.3.1350/eden/ml/link_prediction.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/ml/link_prediction_utils.py` & `eden-kernel-0.3.1350/eden/ml/link_prediction_utils.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/ml/ml.py` & `eden-kernel-0.3.1350/eden/ml/ml.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/sequence.py` & `eden-kernel-0.3.1350/eden/sequence.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/eden/util.py` & `eden-kernel-0.3.1350/eden/util.py`

 * *Files identical despite different names*

### Comparing `eden-kernel-0.3.1348/setup.py` & `eden-kernel-0.3.1350/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     author='Fabrizio Costa',
     author_email='graph-eden@googlegroups.com',
     packages=['eden',
               'eden.ml',
               'eden.display',
               'eden.io'
               ],
+    python_requires='>=3.8',
     include_package_data=True,
     package_data={},
     url='https://github.com/smautner/',
     license='LICENSE',
     description='Explicit Decomposition with Neighborhoods',
     long_description='',
     install_requires=[
```

