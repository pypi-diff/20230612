# Comparing `tmp/peitho_data-2.2.2.tar.gz` & `tmp/peitho_data-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peitho_data-2.2.2.tar", last modified: Sun Jun 11 06:15:12 2023, max compression
+gzip compressed data, was "peitho_data-2.3.0.tar", last modified: Mon Jun 12 01:47:38 2023, max compression
```

## Comparing `peitho_data-2.2.2.tar` & `peitho_data-2.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 06:12:38.000000 peitho_data-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-11 06:12:38.000000 peitho_data-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 06:15:12.826266 peitho_data-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-11 06:12:38.000000 peitho_data-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/
--rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/Ubuntu-B.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/datafication/epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/graph/visualization/file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/machine_learning/concept_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data/tests/datafication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/datafication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/datafication/test_epub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/peitho_data/tests/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/test_knowledge_graph_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/peitho_data/tests/graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/graph/visualization/test_file_based_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.826266 peitho_data-2.2.2/peitho_data/tests/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/machine_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/machine_learning/test_concept_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/test_trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/tests/test_word_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/trello_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-11 06:12:38.000000 peitho_data-2.2.2/peitho_data/word_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 06:15:12.822265 peitho_data-2.2.2/peitho_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 06:13:08.000000 peitho_data-2.2.2/peitho_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 06:15:12.000000 peitho_data-2.2.2/peitho_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-11 06:15:12.826266 peitho_data-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-11 06:12:38.000000 peitho_data-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 01:45:13.000000 peitho_data-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 01:45:13.000000 peitho_data-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 01:47:38.883241 peitho_data-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-12 01:45:13.000000 peitho_data-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   333612 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/Ubuntu-B.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/datafication/epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/graph/knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/graph/visualization/file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/machine_learning/concept_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/tests/datafication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/datafication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/datafication/test_epub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/tests/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/graph/test_knowledge_graph_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/tests/graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/graph/visualization/test_file_based_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data/tests/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/machine_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/machine_learning/test_concept_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/test_trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/tests/test_word_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/trello_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-12 01:45:13.000000 peitho_data-2.3.0/peitho_data/word_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:47:38.883241 peitho_data-2.3.0/peitho_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 01:47:38.000000 peitho_data-2.3.0/peitho_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-12 01:47:38.000000 peitho_data-2.3.0/peitho_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:47:38.000000 peitho_data-2.3.0/peitho_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:45:43.000000 peitho_data-2.3.0/peitho_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-12 01:47:38.000000 peitho_data-2.3.0/peitho_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 01:47:38.000000 peitho_data-2.3.0/peitho_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 01:47:38.887241 peitho_data-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 01:45:13.000000 peitho_data-2.3.0/setup.py
```

### Comparing `peitho_data-2.2.2/LICENSE` & `peitho_data-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/README.md` & `peitho_data-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,33 +39,33 @@
 What is Peitho Data <sup>![Python Version Badge is Missing](https://img.shields.io/badge/Python-3.10-brightgreen?style=flat-square&logo=python&logoColor=white)</sup>
 -------------------
 
 <a href="https://www.bilibili.com/video/BV1kb4y1m7e7?p=3">
     <img align="right" width="50%" alt="永恒" src="./theme/永恒.gif">
 </a>
 
-[Peitho Data](https://qubitpi.github.io/peitho-data/) is an opinionated **data analytics** package that team can
+[Peitho Data](https://peitho-data.readthedocs.io/en/latest/) is an opinionated **data analytics** package that team can
 leverage to quickly incorporate capabilities of
 
 * Data Analytics/Visualization
 * Machine Learning
 * AI
 
 
 Documentation
 -------------
 
 <img src="./theme/雷电将军.png" alt="雷电将军.png" width="5%"></img>
-[Start exploring Peitho Data](https://qubitpi.github.io/peitho-data/)
+[Start exploring Peitho Data](https://peitho-data.readthedocs.io/en/latest/)
 
 
 License
 -------
 
-The use and distribution terms for [Peitho Data](https://qubitpi.github.io/peitho-data/) are covered by the
+The use and distribution terms for [Peitho Data](https://peitho-data.readthedocs.io/en/latest/) are covered by the
 [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
 
 <div align="center">
     <a href="https://opensource.org/licenses">
         <img align="center" width="50%" alt="License Illustration" src="https://github.com/QubitPi/QubitPi/blob/master/img/apache-2.png?raw=true">
     </a>
 </div>
```

#### html2text {}

```diff
@@ -43,16 +43,16 @@
 new_code?id=QubitPi_peitho-data) [![Security Rating](https://sonarcloud.io/api/
   project_badges/measure?project=QubitPi_peitho-data&metric=security_rating)]
         (https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
          [![SonarCloud](https://sonarcloud.io/images/project_badges/sonarcloud-
     orange.svg)](https://sonarcloud.io/summary/new_code?id=QubitPi_peitho-data)
 What is Peitho Data ![Python Version Badge is Missing](https://img.shields.io/
 badge/Python-3.10-brightgreen?style=flat-square&logo=python&logoColor=white) --
------------------ [æ°¸æ] [Peitho Data](https://qubitpi.github.io/peitho-data/
-) is an opinionated **data analytics** package that team can leverage to
+----------------- [æ°¸æ] [Peitho Data](https://peitho-data.readthedocs.io/en/
+latest/) is an opinionated **data analytics** package that team can leverage to
 quickly incorporate capabilities of * Data Analytics/Visualization * Machine
 Learning * AI Documentation ------------- [é·çµå°å.png] [Start exploring
-Peitho Data](https://qubitpi.github.io/peitho-data/) License ------- The use
-and distribution terms for [Peitho Data](https://qubitpi.github.io/peitho-data/
-) are covered by the [Apache License, Version 2.0](http://www.apache.org/
-licenses/LICENSE-2.0.html).
+Peitho Data](https://peitho-data.readthedocs.io/en/latest/) License ------- The
+use and distribution terms for [Peitho Data](https://peitho-
+data.readthedocs.io/en/latest/) are covered by the [Apache License, Version
+2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
                             [License_Illustration]
```

### Comparing `peitho_data-2.2.2/peitho_data/Ubuntu-B.ttf` & `peitho_data-2.3.0/peitho_data/Ubuntu-B.ttf`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/datafication/epub.py` & `peitho_data-2.3.0/peitho_data/datafication/epub.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/graph/knowledge_graph_spec.py` & `peitho_data-2.3.0/peitho_data/graph/knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/graph/visualization/file_based_visualization.py` & `peitho_data-2.3.0/peitho_data/graph/visualization/file_based_visualization.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/machine_learning/concept_learning.py` & `peitho_data-2.3.0/peitho_data/machine_learning/concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/tests/graph/test_knowledge_graph_spec.py` & `peitho_data-2.3.0/peitho_data/tests/graph/test_knowledge_graph_spec.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/tests/machine_learning/test_concept_learning.py` & `peitho_data-2.3.0/peitho_data/tests/machine_learning/test_concept_learning.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/tests/test_trello_api.py` & `peitho_data-2.3.0/peitho_data/tests/test_trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/tests/test_word_cloud.py` & `peitho_data-2.3.0/peitho_data/tests/test_word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/trello_api.py` & `peitho_data-2.3.0/peitho_data/trello_api.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data/word_cloud.py` & `peitho_data-2.3.0/peitho_data/word_cloud.py`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/peitho_data.egg-info/SOURCES.txt` & `peitho_data-2.3.0/peitho_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peitho_data-2.2.2/setup.py` & `peitho_data-2.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="peitho_data",
-    version="2.2.2",
+    version="2.3.0",
     description="An opinionated Python package on Big Data Analytics",
     url="https://github.com/QubitPi/peitho-data",
     author="Jiaqi liu",
     author_email="jack20191124@proton.me",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

