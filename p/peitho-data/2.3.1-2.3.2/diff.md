# Comparing `tmp/peitho_data-2.3.1.tar.gz` & `tmp/peitho_data-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.3.1.tar", last modified: Mon Jun 12 04:08:54 2023, max compression
+gzip compressed data, was "peitho_data-2.3.2.tar", last modified: Mon Jun 12 04:20:38 2023, max compression
```

## Comparing `peitho_data-2.3.1.tar` & `peitho_data-2.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.859320 peitho_data-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 04:06:57.000000 peitho_data-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 04:06:57.000000 peitho_data-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 04:08:54.859320 peitho_data-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-12 04:06:57.000000 peitho_data-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.855321 peitho_data-2.3.1/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.855321 peitho_data-2.3.1/peitho_data/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/datafication/epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.855321 peitho_data-2.3.1/peitho_data/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/graph/knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.859320 peitho_data-2.3.1/peitho_data/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/machine_learning/concept_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.859320 peitho_data-2.3.1/peitho_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.859320 peitho_data-2.3.1/peitho_data/tests/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/datafication/test_epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.859320 peitho_data-2.3.1/peitho_data/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/graph/test_knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.859320 peitho_data-2.3.1/peitho_data/tests/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/machine_learning/test_concept_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/test_trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/tests/test_word_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-12 04:06:57.000000 peitho_data-2.3.1/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:08:54.855321 peitho_data-2.3.1/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 04:08:54.000000 peitho_data-2.3.1/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-12 04:08:54.000000 peitho_data-2.3.1/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:08:54.000000 peitho_data-2.3.1/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:07:19.000000 peitho_data-2.3.1/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 04:08:54.000000 peitho_data-2.3.1/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 04:08:54.000000 peitho_data-2.3.1/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 04:08:54.859320 peitho_data-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 04:06:57.000000 peitho_data-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.169567 peitho_data-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 04:18:10.000000 peitho_data-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 04:18:10.000000 peitho_data-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 04:20:38.169567 peitho_data-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-12 04:18:10.000000 peitho_data-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.161567 peitho_data-2.3.2/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.165567 peitho_data-2.3.2/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.165567 peitho_data-2.3.2/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/graph/knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.165567 peitho_data-2.3.2/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.165567 peitho_data-2.3.2/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.165567 peitho_data-2.3.2/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.165567 peitho_data-2.3.2/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/graph/test_knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.169567 peitho_data-2.3.2/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-12 04:18:10.000000 peitho_data-2.3.2/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:20:38.161567 peitho_data-2.3.2/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 04:20:38.000000 peitho_data-2.3.2/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-12 04:20:38.000000 peitho_data-2.3.2/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:20:38.000000 peitho_data-2.3.2/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:18:43.000000 peitho_data-2.3.2/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 04:20:38.000000 peitho_data-2.3.2/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 04:20:38.000000 peitho_data-2.3.2/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 04:20:38.169567 peitho_data-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 04:18:10.000000 peitho_data-2.3.2/setup.py
```

### Comparing `peitho_data-2.3.1/LICENSE` & `peitho_data-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/README.md` & `peitho_data-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.3.2/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/datafication/epub.py` & `peitho_data-2.3.2/peitho_data/datafication/epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/graph/knowledge_graph_spec.py` & `peitho_data-2.3.2/peitho_data/graph/knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/machine_learning/concept_learning.py` & `peitho_data-2.3.2/peitho_data/machine_learning/concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/tests/datafication/test_epub.py` & `peitho_data-2.3.2/peitho_data/tests/datafication/test_epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/tests/graph/test_knowledge_graph_spec.py` & `peitho_data-2.3.2/peitho_data/tests/graph/test_knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/tests/machine_learning/test_concept_learning.py` & `peitho_data-2.3.2/peitho_data/tests/machine_learning/test_concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/tests/test_trello_api.py` & `peitho_data-2.3.2/peitho_data/tests/test_trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/tests/test_word_cloud.py` & `peitho_data-2.3.2/peitho_data/tests/test_word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/trello_api.py` & `peitho_data-2.3.2/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data/word_cloud.py` & `peitho_data-2.3.2/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/peitho_data.egg-info/SOURCES.txt` & `peitho_data-2.3.2/peitho_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peitho_data-2.3.1/setup.py` & `peitho_data-2.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.3.1",
+    version="2.3.2",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

