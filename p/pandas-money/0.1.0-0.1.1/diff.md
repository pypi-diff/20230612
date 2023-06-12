# Comparing `tmp/pandas_money-0.1.0.tar.gz` & `tmp/pandas_money-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_money-0.1.0.tar", max compression
+gzip compressed data, was "pandas_money-0.1.1.tar", max compression
```

## Comparing `pandas_money-0.1.0.tar` & `pandas_money-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.1.0/LICENSE
--rw-r--r--   0        0        0      578 2023-06-12 05:05:36.820318 pandas_money-0.1.0/README.md
--rw-r--r--   0        0        0      152 2023-06-12 00:16:34.192150 pandas_money-0.1.0/pandas_money/__init__.py
--rw-r--r--   0        0        0     7411 2023-06-12 03:40:40.766131 pandas_money-0.1.0/pandas_money/money_dtype.py
--rw-r--r--   0        0        0        0 2023-06-12 04:25:47.563979 pandas_money-0.1.0/pandas_money/tests/__init__.py
--rw-r--r--   0        0        0    10506 2023-06-12 03:34:06.593176 pandas_money-0.1.0/pandas_money/tests/test_money_dtype.py
--rw-r--r--   0        0        0     1383 2023-06-12 05:10:38.789971 pandas_money-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 pandas_money-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 03:17:36.171096 pandas_money-0.1.1/LICENSE
+-rw-r--r--   0        0        0      823 2023-06-12 06:06:19.598747 pandas_money-0.1.1/README.md
+-rw-r--r--   0        0        0      152 2023-06-12 00:16:34.192150 pandas_money-0.1.1/pandas_money/__init__.py
+-rw-r--r--   0        0        0     7411 2023-06-12 03:40:40.766131 pandas_money-0.1.1/pandas_money/money_dtype.py
+-rw-r--r--   0        0        0        0 2023-06-12 04:25:47.563979 pandas_money-0.1.1/pandas_money/tests/__init__.py
+-rw-r--r--   0        0        0    10506 2023-06-12 03:34:06.593176 pandas_money-0.1.1/pandas_money/tests/test_money_dtype.py
+-rw-r--r--   0        0        0     1434 2023-06-12 06:13:36.743901 pandas_money-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 pandas_money-0.1.1/PKG-INFO
```

### Comparing `pandas_money-0.1.0/LICENSE` & `pandas_money-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_money-0.1.0/pandas_money/money_dtype.py` & `pandas_money-0.1.1/pandas_money/money_dtype.py`

 * *Files identical despite different names*

### Comparing `pandas_money-0.1.0/pandas_money/tests/test_money_dtype.py` & `pandas_money-0.1.1/pandas_money/tests/test_money_dtype.py`

 * *Files identical despite different names*

### Comparing `pandas_money-0.1.0/pyproject.toml` & `pandas_money-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "pandas-money"
-version = "0.1.0"
-description = "A Pandas/Pyarrow mashup for handling currency with Decimal128 performance"
+version = "0.1.1"
+description = "A Pandas ArrayExtension for handling currency with int64 performance"
 authors = ["Rod Morison <rmorison@users.noreply.github.com>"]
+repository = "https://github.com/rmorison/pandas-money"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandas_money"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pandas = "^2.0.2"
```

