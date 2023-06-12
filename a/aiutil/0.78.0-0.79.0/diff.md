# Comparing `tmp/aiutil-0.78.0.tar.gz` & `tmp/aiutil-0.79.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiutil-0.78.0.tar", max compression
+gzip compressed data, was "aiutil-0.79.0.tar", max compression
```

## Comparing `aiutil-0.78.0.tar` & `aiutil-0.79.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-11 22:53:53.604088 aiutil-0.78.0/LICENSE
--rw-r--r--   0        0        0     1825 2023-06-11 22:53:53.604088 aiutil-0.78.0/README.md
--rw-r--r--   0        0        0       96 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/__init__.py
--rw-r--r--   0        0        0     1968 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/collections.py
--rw-r--r--   0        0        0    10716 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/cv.py
--rw-r--r--   0        0        0     3246 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/dataframe.py
--rw-r--r--   0        0        0     3501 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/datetime.py
--rw-r--r--   0        0        0     2092 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/dockerhub.py
--rw-r--r--   0        0        0    22905 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/filesystem.py
--rw-r--r--   0        0        0       81 2023-06-11 22:53:53.604088 aiutil-0.78.0/aiutil/hadoop/__init__.py
--rw-r--r--   0        0        0     9194 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/hdfs.py
--rw-r--r--   0        0        0     5910 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/kerberos.py
--rw-r--r--   0        0        0    18754 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/log.py
--rw-r--r--   0        0        0     7473 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/logf.py
--rw-r--r--   0        0        0    16000 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/pyspark_submit.py
--rw-r--r--   0        0        0     1245 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hadoop/pyspark_submit.yaml
--rw-r--r--   0        0        0     1450 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/hash.py
--rw-r--r--   0        0        0     3950 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/memory.py
--rw-r--r--   0        0        0        0 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/notebook/__init__.py
--rwxr-xr-x   0        0        0     9614 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/notebook/search.py
--rw-r--r--   0        0        0     2337 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/notebook/util.py
--rw-r--r--   0        0        0     1612 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/pdf.py
--rw-r--r--   0        0        0    10562 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/poetry.py
--rw-r--r--   0        0        0     1102 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/pypi.py
--rw-r--r--   0        0        0     2111 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/shebang.py
--rw-r--r--   0        0        0     4504 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/shell.py
--rw-r--r--   0        0        0      660 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/sql.py
--rw-r--r--   0        0        0      651 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/url.py
--rw-r--r--   0        0        0     1159 2023-06-11 22:53:53.608088 aiutil-0.78.0/aiutil/utils.py
--rw-r--r--   0        0        0     2508 2023-06-11 22:53:53.608088 aiutil-0.78.0/pyproject.toml
--rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 aiutil-0.78.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-12 05:21:15.154671 aiutil-0.79.0/LICENSE
+-rw-r--r--   0        0        0     1825 2023-06-12 05:21:15.154671 aiutil-0.79.0/README.md
+-rw-r--r--   0        0        0       96 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/__init__.py
+-rw-r--r--   0        0        0     1968 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/collections.py
+-rw-r--r--   0        0        0    10716 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/cv.py
+-rw-r--r--   0        0        0     3246 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/dataframe.py
+-rw-r--r--   0        0        0     3501 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/datetime.py
+-rw-r--r--   0        0        0     2092 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/dockerhub.py
+-rw-r--r--   0        0        0    22905 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/filesystem.py
+-rw-r--r--   0        0        0       81 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/__init__.py
+-rw-r--r--   0        0        0     9194 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/hdfs.py
+-rw-r--r--   0        0        0     5910 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/kerberos.py
+-rw-r--r--   0        0        0    18754 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/log.py
+-rw-r--r--   0        0        0     7473 2023-06-12 05:21:15.154671 aiutil-0.79.0/aiutil/hadoop/logf.py
+-rw-r--r--   0        0        0    16000 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/hadoop/pyspark_submit.py
+-rw-r--r--   0        0        0     1245 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/hadoop/pyspark_submit.yaml
+-rw-r--r--   0        0        0     1450 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/hash.py
+-rw-r--r--   0        0        0     3950 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/memory.py
+-rw-r--r--   0        0        0        0 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/notebook/__init__.py
+-rwxr-xr-x   0        0        0     9614 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/notebook/search.py
+-rw-r--r--   0        0        0     2337 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/notebook/util.py
+-rw-r--r--   0        0        0     1612 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/pdf.py
+-rw-r--r--   0        0        0    10562 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/poetry.py
+-rw-r--r--   0        0        0     1102 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/pypi.py
+-rw-r--r--   0        0        0     2111 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/shebang.py
+-rw-r--r--   0        0        0     4504 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/shell.py
+-rw-r--r--   0        0        0      660 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/sql.py
+-rw-r--r--   0        0        0      651 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/url.py
+-rw-r--r--   0        0        0     1159 2023-06-12 05:21:15.158671 aiutil-0.79.0/aiutil/utils.py
+-rw-r--r--   0        0        0     2508 2023-06-12 05:21:15.158671 aiutil-0.79.0/pyproject.toml
+-rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 aiutil-0.79.0/PKG-INFO
```

### Comparing `aiutil-0.78.0/LICENSE` & `aiutil-0.79.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/README.md` & `aiutil-0.79.0/README.md`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/collections.py` & `aiutil-0.79.0/aiutil/collections.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/cv.py` & `aiutil-0.79.0/aiutil/cv.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/dataframe.py` & `aiutil-0.79.0/aiutil/dataframe.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/datetime.py` & `aiutil-0.79.0/aiutil/datetime.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/dockerhub.py` & `aiutil-0.79.0/aiutil/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/filesystem.py` & `aiutil-0.79.0/aiutil/filesystem.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/hadoop/hdfs.py` & `aiutil-0.79.0/aiutil/hadoop/hdfs.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/hadoop/kerberos.py` & `aiutil-0.79.0/aiutil/hadoop/kerberos.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/hadoop/log.py` & `aiutil-0.79.0/aiutil/hadoop/log.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/hadoop/logf.py` & `aiutil-0.79.0/aiutil/hadoop/logf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/hadoop/pyspark_submit.py` & `aiutil-0.79.0/aiutil/hadoop/pyspark_submit.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/hadoop/pyspark_submit.yaml` & `aiutil-0.79.0/aiutil/hadoop/pyspark_submit.yaml`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/hash.py` & `aiutil-0.79.0/aiutil/hash.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/memory.py` & `aiutil-0.79.0/aiutil/memory.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/notebook/search.py` & `aiutil-0.79.0/aiutil/notebook/search.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/notebook/util.py` & `aiutil-0.79.0/aiutil/notebook/util.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/pdf.py` & `aiutil-0.79.0/aiutil/pdf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/poetry.py` & `aiutil-0.79.0/aiutil/poetry.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/pypi.py` & `aiutil-0.79.0/aiutil/pypi.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/shebang.py` & `aiutil-0.79.0/aiutil/shebang.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/shell.py` & `aiutil-0.79.0/aiutil/shell.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/sql.py` & `aiutil-0.79.0/aiutil/sql.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/url.py` & `aiutil-0.79.0/aiutil/url.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/aiutil/utils.py` & `aiutil-0.79.0/aiutil/utils.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.78.0/pyproject.toml` & `aiutil-0.79.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiutil"
-version = "0.78.0"
+version = "0.79.0"
 description = "A utils Python package for data scientists."
 authors = ["Benjamin Du <longendu@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/legendu-net/aiutil"
 keywords = ["AI", "Machine Learning", "tools", "utils"]
 
@@ -13,15 +13,15 @@
 repart_hdfs = "aiutil.hadoop:repart_hdfs.main"
 pyspark_submit = "aiutil.hadoop:pyspark_submit.main"
 pykinit = "aiutil.hadoop:kerberos.main"
 match_memory = "aiutil:memory.main"
 snb = "aiutil.notebook:search.main"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.11"
+python = ">=3.10,<3.12"
 sqlparse = ">=0.4.1"
 pathspec = ">=0.8.1"
 dateparser = ">=0.7.1"
 numba = ">=0.53.0rc1.post1"
 pandas = ">=1.2.0"
 ydata-profiling = ">=4.2.0"
 loguru = ">=0.3.2"
```

### Comparing `aiutil-0.78.0/PKG-INFO` & `aiutil-0.79.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aiutil
-Version: 0.78.0
+Version: 0.79.0
 Summary: A utils Python package for data scientists.
 Home-page: https://github.com/legendu-net/aiutil
 License: MIT
 Keywords: AI,Machine Learning,tools,utils
 Author: Benjamin Du
 Author-email: longendu@yahoo.com
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: admin
 Provides-Extra: all
 Provides-Extra: cv
 Provides-Extra: docker
 Provides-Extra: jupyter
 Provides-Extra: pdf
 Requires-Dist: GitPython (>=3.0.0)
```

