# Comparing `tmp/spacy-transformers-1.2.4.tar.gz` & `tmp/spacy-transformers-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-transformers-1.2.4.tar", last modified: Mon May 22 15:30:04 2023, max compression
+gzip compressed data, was "spacy-transformers-1.2.5.tar", last modified: Fri Jun  9 17:31:50 2023, max compression
```

## Comparing `spacy-transformers-1.2.4.tar` & `spacy-transformers-1.2.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4671 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      129 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3067 2023-05-22 15:30:04.557306 spacy-transformers-1.2.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.549306 spacy-transformers-1.2.4/spacy_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/align.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/align.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/annotation_setters.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/data_classes.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.549306 spacy-transformers-1.2.4/spacy_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/hf_shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/hf_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/listener.py
--rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/split_trf.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6448 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/trfs2arrays.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/py.typed
--rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/span_getters.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/spacy_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/spacy_transformers/tests/regression/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/regression/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue6401.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue7029.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_alignment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_configs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_data_classes.py
--rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_deprecations.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_model_sequence_classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_model_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16846 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9837 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_spanners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1588 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_textcatcnn.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3132 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_tok2vectransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_truncation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/truncate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.549306 spacy-transformers-1.2.4/spacy_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1876 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4671 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      129 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3067 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.688743 spacy-transformers-1.2.5/spacy_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/align.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/align.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/annotation_setters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/data_classes.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.688743 spacy-transformers-1.2.5/spacy_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/hf_shim.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/hf_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/listener.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/split_trf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6448 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/layers/trfs2arrays.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/span_getters.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/spacy_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.692743 spacy-transformers-1.2.5/spacy_transformers/tests/regression/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/regression/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue6401.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue7029.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_alignment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_configs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_data_classes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_deprecations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_model_sequence_classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_model_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16846 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9837 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_spanners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1588 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_textcatcnn.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3132 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_tok2vectransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/test_truncation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/truncate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-06-09 17:31:35.000000 spacy-transformers-1.2.5/spacy_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-09 17:31:50.688743 spacy-transformers-1.2.5/spacy_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1876 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-06-09 17:31:50.000000 spacy-transformers-1.2.5/spacy_transformers.egg-info/top_level.txt
```

### Comparing `spacy-transformers-1.2.4/LICENSE` & `spacy-transformers-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/PKG-INFO` & `spacy-transformers-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.4
+Version: 1.2.5
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.4 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.5 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `spacy-transformers-1.2.4/README.md` & `spacy-transformers-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/setup.cfg` & `spacy-transformers-1.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.4
+version = 1.2.5
 description = spaCy pipelines for pre-trained BERT and other transformers
 url = https://spacy.io
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -29,15 +29,15 @@
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	spacy>=3.5.0,<4.0.0
 	numpy>=1.15.0
-	transformers>=3.4.0,<4.30.0
+	transformers>=3.4.0,<4.31.0
 	torch>=1.8.0
 	srsly>=2.4.0,<3.0.0
 	dataclasses>=0.6,<1.0; python_version < "3.7"
 	spacy-alignments>=0.7.2,<1.0.0
 
 [options.extras_require]
 cuda =
```

### Comparing `spacy-transformers-1.2.4/setup.py` & `spacy-transformers-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/align.pyi` & `spacy-transformers-1.2.5/spacy_transformers/align.pyi`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/align.pyx` & `spacy-transformers-1.2.5/spacy_transformers/align.pyx`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/annotation_setters.py` & `spacy-transformers-1.2.5/spacy_transformers/annotation_setters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/architectures.py` & `spacy-transformers-1.2.5/spacy_transformers/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/data_classes.py` & `spacy-transformers-1.2.5/spacy_transformers/data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/layers/_util.py` & `spacy-transformers-1.2.5/spacy_transformers/layers/_util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/layers/hf_shim.py` & `spacy-transformers-1.2.5/spacy_transformers/layers/hf_shim.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/layers/hf_wrapper.py` & `spacy-transformers-1.2.5/spacy_transformers/layers/hf_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/layers/listener.py` & `spacy-transformers-1.2.5/spacy_transformers/layers/listener.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/layers/transformer_model.py` & `spacy-transformers-1.2.5/spacy_transformers/layers/transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/layers/trfs2arrays.py` & `spacy-transformers-1.2.5/spacy_transformers/layers/trfs2arrays.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/pipeline_component.py` & `spacy-transformers-1.2.5/spacy_transformers/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/span_getters.py` & `spacy-transformers-1.2.5/spacy_transformers/span_getters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue6401.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue6401.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue7029.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/regression/test_spacy_issue7029.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_alignment.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_configs.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_data_classes.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_model_sequence_classification.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_model_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_model_wrapper.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_pipeline_component.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_pipeline_component.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_serialize.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_spanners.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_spanners.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_textcatcnn.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_textcatcnn.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_tok2vectransformer.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_tok2vectransformer.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/test_truncation.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/tests/util.py` & `spacy-transformers-1.2.5/spacy_transformers/tests/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/truncate.py` & `spacy-transformers-1.2.5/spacy_transformers/truncate.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers/util.py` & `spacy-transformers-1.2.5/spacy_transformers/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers.egg-info/PKG-INFO` & `spacy-transformers-1.2.5/spacy_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.4
+Version: 1.2.5
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.4 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.5 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
```

### Comparing `spacy-transformers-1.2.4/spacy_transformers.egg-info/SOURCES.txt` & `spacy-transformers-1.2.5/spacy_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers.egg-info/entry_points.txt` & `spacy-transformers-1.2.5/spacy_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.4/spacy_transformers.egg-info/requires.txt` & `spacy-transformers-1.2.5/spacy_transformers.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spacy<4.0.0,>=3.5.0
 numpy>=1.15.0
-transformers<4.30.0,>=3.4.0
+transformers<4.31.0,>=3.4.0
 torch>=1.8.0
 srsly<3.0.0,>=2.4.0
 spacy-alignments<1.0.0,>=0.7.2
 
 [:python_version < "3.7"]
 dataclasses<1.0,>=0.6
```

