# Comparing `tmp/pysparkler-0.7.dev1686599090.tar.gz` & `tmp/pysparkler-0.8.dev1686599891.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.7.dev1686599090.tar", max compression
+gzip compressed data, was "pysparkler-0.8.dev1686599891.tar", max compression
```

## Comparing `pysparkler-0.7.dev1686599090.tar` & `pysparkler-0.8.dev1686599891.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    12173 2023-06-12 19:44:42.110184 pysparkler-0.7.dev1686599090/README.md
--rw-r--r--   0        0        0     1203 2023-06-12 19:44:50.990220 pysparkler-0.7.dev1686599090/pyproject.toml
--rw-r--r--   0        0        0      807 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/__init__.py
--rw-r--r--   0        0        0     5294 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/api.py
--rw-r--r--   0        0        0     7372 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/base.py
--rw-r--r--   0        0        0     6398 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     4650 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10561 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     3895 2023-06-12 19:44:42.114184 pysparkler-0.7.dev1686599090/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0    13052 1970-01-01 00:00:00.000000 pysparkler-0.7.dev1686599090/PKG-INFO
+-rw-r--r--   0        0        0    12173 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/README.md
+-rw-r--r--   0        0        0     1203 2023-06-12 19:58:11.968255 pysparkler-0.8.dev1686599891/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/__init__.py
+-rw-r--r--   0        0        0     5294 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/api.py
+-rw-r--r--   0        0        0     7372 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/base.py
+-rw-r--r--   0        0        0     6398 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     4650 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10561 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     3895 2023-06-12 19:58:02.840129 pysparkler-0.8.dev1686599891/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0    13052 1970-01-01 00:00:00.000000 pysparkler-0.8.dev1686599891/PKG-INFO
```

### Comparing `pysparkler-0.7.dev1686599090/README.md` & `pysparkler-0.8.dev1686599891/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pyproject.toml` & `pysparkler-0.8.dev1686599891/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.7.dev1686599090"
+version = "0.8.dev1686599891"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/__init__.py` & `pysparkler-0.8.dev1686599891/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/api.py` & `pysparkler-0.8.dev1686599891/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/base.py` & `pysparkler-0.8.dev1686599891/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/cli.py` & `pysparkler-0.8.dev1686599891/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.8.dev1686599891/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.8.dev1686599891/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.8.dev1686599891/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.8.dev1686599891/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.8.dev1686599891/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686599090/PKG-INFO` & `pysparkler-0.8.dev1686599891/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.7.dev1686599090
+Version: 0.8.dev1686599891
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

