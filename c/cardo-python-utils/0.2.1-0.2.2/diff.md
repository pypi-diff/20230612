# Comparing `tmp/cardo-python-utils-0.2.1.tar.gz` & `tmp/cardo-python-utils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardo-python-utils-0.2.1.tar", last modified: Fri Jun  9 17:06:47 2023, max compression
+gzip compressed data, was "cardo-python-utils-0.2.2.tar", last modified: Mon Jun 12 10:11:27 2023, max compression
```

## Comparing `cardo-python-utils-0.2.1.tar` & `cardo-python-utils-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.1/README.rst
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 17:06:47.086227 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-06-09 17:06:47.000000 cardo-python-utils-0.2.1/cardo_python_utils.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/python_utils/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1949 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.1/python_utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/data_structures.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/db.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/django_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    14223 2023-06-09 17:06:36.000000 cardo-python-utils-0.2.1/python_utils/esma_choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/imports.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/math.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/pandas_utils.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/rest.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/text.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/time.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/python_utils/types_hinting.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-06-09 17:06:47.090227 cardo-python-utils-0.2.1/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.1/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.2/README.rst
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-12 10:11:27.448061 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2023-06-12 10:11:27.000000 cardo-python-utils-0.2.2/cardo_python_utils.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/python_utils/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1949 2023-06-09 16:10:08.000000 cardo-python-utils-0.2.2/python_utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/data_structures.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/db.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/django_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    14437 2023-06-12 10:10:18.000000 cardo-python-utils-0.2.2/python_utils/esma_choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/imports.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/math.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/pandas_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/rest.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/text.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/time.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/python_utils/types_hinting.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2023-06-12 10:11:27.452061 cardo-python-utils-0.2.2/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.2/setup.py
```

### Comparing `cardo-python-utils-0.2.1/LICENSE` & `cardo-python-utils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/PKG-INFO` & `cardo-python-utils-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.1/README.rst` & `cardo-python-utils-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/cardo_python_utils.egg-info/PKG-INFO` & `cardo-python-utils-0.2.2/cardo_python_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `cardo-python-utils-0.2.1/cardo_python_utils.egg-info/SOURCES.txt` & `cardo-python-utils-0.2.2/cardo_python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/choices.py` & `cardo-python-utils-0.2.2/python_utils/choices.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/data_structures.py` & `cardo-python-utils-0.2.2/python_utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/django_utils.py` & `cardo-python-utils-0.2.2/python_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/esma_choices.py` & `cardo-python-utils-0.2.2/python_utils/esma_choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,7 +387,17 @@
     CACB = 50, "Collection Account Bank"
     COLA = 51, "Collateral Account Bank"
     SBLP = 52, "Subordinated Loan Provider"
     CLOM = 53, "Collateralised Loan Obligation Manager"
     PRTA = 54, "Portfolio Advisor"
     SUBA = 55, "Substitution Agent"
     OTHR = 100, "Other"
+
+
+class PaymentFrequencyChoices(ChoiceEnum):
+    DAIL = 1, "Daily"
+    WEEK = 2, "Weekly"
+    MNTH = 3, "Monthly"
+    QUTR = 4, "Quarterly"
+    SEMI = 5, "Semi Annual"
+    YEAR = 6, "Annual"
+    OTHR = 10, "Other"
```

### Comparing `cardo-python-utils-0.2.1/python_utils/exceptions.py` & `cardo-python-utils-0.2.2/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/imports.py` & `cardo-python-utils-0.2.2/python_utils/imports.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/math.py` & `cardo-python-utils-0.2.2/python_utils/math.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/pandas_utils.py` & `cardo-python-utils-0.2.2/python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/rest.py` & `cardo-python-utils-0.2.2/python_utils/rest.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/text.py` & `cardo-python-utils-0.2.2/python_utils/text.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/python_utils/time.py` & `cardo-python-utils-0.2.2/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.1/setup.cfg` & `cardo-python-utils-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardo-python-utils
-version = 0.2.1
+version = 0.2.2
 description = Python library enhanced with a wide range of functions for different scenarios.
 long_description = file: README.rst
 url = https://github.com/CardoAI/cardo-python-utils
 author = Kristi Kotini
 author_email = hello@cardoai.com
 license = MIT (X11)
 classifiers =
```

