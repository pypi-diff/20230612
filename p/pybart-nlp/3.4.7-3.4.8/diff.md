# Comparing `tmp/pybart-nlp-3.4.7.tar.gz` & `tmp/pybart-nlp-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybart-nlp-3.4.7.tar", last modified: Sun Jun 11 21:03:58 2023, max compression
+gzip compressed data, was "pybart-nlp-3.4.8.tar", last modified: Mon Jun 12 07:26:59 2023, max compression
```

## Comparing `pybart-nlp-3.4.7.tar` & `pybart-nlp-3.4.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:03:58.897195 pybart-nlp-3.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-11 21:03:58.897195 pybart-nlp-3.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:03:58.893195 pybart-nlp-3.4.7/pybart/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/conllu_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:03:58.893195 pybart-nlp-3.4.7/pybart/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/constants/eud_literal_allowed_list_en.json
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/constants/eud_literal_allowed_list_he.json
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    90095 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/graph_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/pybart/spacy_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:03:58.897195 pybart-nlp-3.4.7/pybart_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-11 21:03:58.000000 pybart-nlp-3.4.7/pybart_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-11 21:03:58.000000 pybart-nlp-3.4.7/pybart_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:03:58.000000 pybart-nlp-3.4.7/pybart_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 21:03:58.000000 pybart-nlp-3.4.7/pybart_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 21:03:58.897195 pybart-nlp-3.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-11 21:03:44.000000 pybart-nlp-3.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:26:59.284033 pybart-nlp-3.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-12 07:26:59.284033 pybart-nlp-3.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:26:59.280033 pybart-nlp-3.4.8/pybart/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/conllu_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:26:59.280033 pybart-nlp-3.4.8/pybart/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/constants/eud_literal_allowed_list_en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/constants/eud_literal_allowed_list_he.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90095 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/graph_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/pybart/spacy_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:26:59.284033 pybart-nlp-3.4.8/pybart_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-12 07:26:59.000000 pybart-nlp-3.4.8/pybart_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-12 07:26:59.000000 pybart-nlp-3.4.8/pybart_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:26:59.000000 pybart-nlp-3.4.8/pybart_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 07:26:59.000000 pybart-nlp-3.4.8/pybart_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 07:26:59.284033 pybart-nlp-3.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-12 07:26:45.000000 pybart-nlp-3.4.8/setup.py
```

### Comparing `pybart-nlp-3.4.7/LICENSE` & `pybart-nlp-3.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/PKG-INFO` & `pybart-nlp-3.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybart-nlp
-Version: 3.4.7
+Version: 3.4.8
 Summary: python converter from UD-tree to BART-graph representations
 Home-page: https://github.com/allenai/pybart
 Author: Aryeh Tiktinsky
 Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.7 Summary: python converter
+Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.8 Summary: python converter
 from UD-tree to BART-graph representations Home-page: https://github.com/
 allenai/pybart Author: Aryeh Tiktinsky Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown License-File: LICENSE ![CI](https://github.com/allenai/pybart/actions/
 workflows/ci.yml/badge.svg)
```

### Comparing `pybart-nlp-3.4.7/README.md` & `pybart-nlp-3.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart/api.py` & `pybart-nlp-3.4.8/pybart/api.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart/conllu_wrapper.py` & `pybart-nlp-3.4.8/pybart/conllu_wrapper.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart/constants/eud_literal_allowed_list_en.json` & `pybart-nlp-3.4.8/pybart/constants/eud_literal_allowed_list_en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960159362549801%*

 * *Differences: {'insert': '[(1000, \'and/or\'), (1001, "\'cause"), (1002, \'adjacent\'), (1003, \'wth\')]'}*

```diff
@@ -994,9 +994,13 @@
     "by_et",
     "equivalently_to",
     "independently_to",
     "west_to",
     "in_place",
     "in_common",
     "quantitatively",
-    "definitely"
+    "definitely",
+    "and/or",
+    "'cause",
+    "adjacent",
+    "wth"
 ]
```

### Comparing `pybart-nlp-3.4.7/pybart/constants/eud_literal_allowed_list_he.json` & `pybart-nlp-3.4.8/pybart/constants/eud_literal_allowed_list_he.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984251968503937%*

 * *Differences: {'insert': "[(250, 'ב_מסגרת'), (251, 'על_רקע'), (252, 'לצורך'), (253, 'בשונה')]"}*

```diff
@@ -244,9 +244,13 @@
     "\u05de\u05d9\u05d3",
     "\u05e4\u05d9",
     "\u05dc\u05d7\u05d3\u05e8",
     "\u05db\u05d5\u05dc\u05dc",
     "\u05d1_\u05de\u05d4\u05dc\u05da",
     "\u05db\u05d9\u05d5\u05dd",
     "\u05dc\u05e2\u05d5\u05dc\u05dd",
-    "\u05de\u05e2\u05d8"
+    "\u05de\u05e2\u05d8",
+    "\u05d1_\u05de\u05e1\u05d2\u05e8\u05ea",
+    "\u05e2\u05dc_\u05e8\u05e7\u05e2",
+    "\u05dc\u05e6\u05d5\u05e8\u05da",
+    "\u05d1\u05e9\u05d5\u05e0\u05d4"
 ]
```

### Comparing `pybart-nlp-3.4.7/pybart/constraints.py` & `pybart-nlp-3.4.8/pybart/constraints.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart/converter.py` & `pybart-nlp-3.4.8/pybart/converter.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart/graph_token.py` & `pybart-nlp-3.4.8/pybart/graph_token.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart/matcher.py` & `pybart-nlp-3.4.8/pybart/matcher.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart/spacy_wrapper.py` & `pybart-nlp-3.4.8/pybart/spacy_wrapper.py`

 * *Files identical despite different names*

### Comparing `pybart-nlp-3.4.7/pybart_nlp.egg-info/PKG-INFO` & `pybart-nlp-3.4.8/pybart_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybart-nlp
-Version: 3.4.7
+Version: 3.4.8
 Summary: python converter from UD-tree to BART-graph representations
 Home-page: https://github.com/allenai/pybart
 Author: Aryeh Tiktinsky
 Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.7 Summary: python converter
+Metadata-Version: 2.1 Name: pybart-nlp Version: 3.4.8 Summary: python converter
 from UD-tree to BART-graph representations Home-page: https://github.com/
 allenai/pybart Author: Aryeh Tiktinsky Author-email: aryehgigi@gmail.com
 Classifier: Programming Language :: Python :: 3.7 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown License-File: LICENSE ![CI](https://github.com/allenai/pybart/actions/
 workflows/ci.yml/badge.svg)
```

### Comparing `pybart-nlp-3.4.7/setup.py` & `pybart-nlp-3.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybart-nlp",
-    version="3.4.7",
+    version="3.4.8",
     author="Aryeh Tiktinsky",
     author_email="aryehgigi@gmail.com",
     description="python converter from UD-tree to BART-graph representations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allenai/pybart",
     packages=setuptools.find_packages(),
```

