# Comparing `tmp/bquest-0.0.1.tar.gz` & `tmp/bquest-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bquest-0.0.1.tar", max compression
+gzip compressed data, was "bquest-0.1.0.tar", max compression
```

## Comparing `bquest-0.0.1.tar` & `bquest-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       56 2023-06-09 07:21:51.207056 bquest-0.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0    11356 2023-06-09 07:21:51.207056 bquest-0.0.1/LICENSE
--rw-r--r--   0        0        0     1597 2023-06-09 07:21:51.207056 bquest-0.0.1/README.rst
--rw-r--r--   0        0        0        0 2023-06-09 07:21:51.207056 bquest-0.0.1/bquest/__init__.py
--rw-r--r--   0        0        0     1948 2023-06-09 07:21:51.207056 bquest-0.0.1/bquest/dataframe.py
--rw-r--r--   0        0        0     8966 2023-06-09 07:21:51.207056 bquest-0.0.1/bquest/runner.py
--rw-r--r--   0        0        0     7272 2023-06-09 07:21:51.207056 bquest-0.0.1/bquest/tables.py
--rw-r--r--   0        0        0      328 2023-06-09 07:21:51.207056 bquest-0.0.1/bquest/util.py
--rw-r--r--   0        0        0     2972 2023-06-09 07:21:51.211056 bquest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3370 1970-01-01 00:00:00.000000 bquest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      132 2023-06-12 14:11:50.571350 bquest-0.1.0/CHANGELOG.rst
+-rw-r--r--   0        0        0    11356 2023-06-12 14:11:50.571350 bquest-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3621 2023-06-12 14:11:50.571350 bquest-0.1.0/README.rst
+-rw-r--r--   0        0        0        0 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/__init__.py
+-rw-r--r--   0        0        0     2085 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/dataframe.py
+-rw-r--r--   0        0        0     9080 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/runner.py
+-rw-r--r--   0        0        0     7272 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/tables.py
+-rw-r--r--   0        0        0      328 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/util.py
+-rw-r--r--   0        0        0     2972 2023-06-12 14:11:50.571350 bquest-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 bquest-0.1.0/PKG-INFO
```

### Comparing `bquest-0.0.1/LICENSE` & `bquest-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bquest-0.0.1/bquest/dataframe.py` & `bquest-0.1.0/bquest/dataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """ Helpers for dealing with pandas.DataFrames """
 from typing import Any
 
 import numpy as np
 import pandas
+import pandas as pd
 from pandas import testing as pd_test
 
+POSSIBLE_INTEGER_DTYPES = (int, pd.Int8Dtype, pd.Int16Dtype, pd.Int32Dtype, pd.Int64Dtype)
+
 
 def standardize_frame_numerics(df: pandas.DataFrame, float_precision: int = 2) -> pandas.DataFrame:
     """Standardizes numerics inside a dataframe to facilitate comparison between
      dataframes with respect to meaningful differences.
 
     Args:
         df: Pandas dataframe to be standardized
         float_precision: level of precision for rounding floats
 
     Returns:
         Standardized dataframe
     """
     df = df.round(float_precision)
-    for col in df.columns:
-        if df[col].dtype != int:
-            continue
+
+    integer_columns = df.select_dtypes(POSSIBLE_INTEGER_DTYPES).columns
+
+    for col in integer_columns:
         df[col] = df[col].astype(float)
 
     return df.fillna(value=np.nan).reset_index(drop=True)
 
 
 def _fix_integer_dtypes(df: pandas.DataFrame) -> None:
     """Since some version, pandas can not infer in assert_frame_equals Int64 as int64
```

### Comparing `bquest-0.0.1/bquest/runner.py` & `bquest-0.1.0/bquest/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         return config
 
 
 class BaseRunner:
     """Base class for runners"""
 
     def __init__(self, bq_client: bq.Client, project: str, dataset: str = "bquest"):
+        # TODO: project is obsolete and can be taken from bq_client
         self._bq_client = bq_client
         self._bq_table_def_builder = BQTableDefinitionBuilder(project, dataset)
 
     def _create_source_tables(self, table_definitions: List[BQTableDefinition]) -> List[BQTable]:
         result = []
         for table_def in table_definitions:
             test_table = table_def.load_to_bq(self._bq_client)
@@ -168,15 +169,15 @@
 
 class SQLRunner(BaseRunner):
     """Runs SQL queries on custom data for testing"""
 
     def __init__(
         self,
         bq_client: bq.Client,
-        project: str,
+        project: str,  # TODO: project is obsolete and can be taken from bq_client
         dataset: str = "bquest",
         clean_up: bool = True,
     ):
         super(SQLRunner, self).__init__(bq_client, project, dataset)
         self._bq_client = bq_client
         self._clean_up = clean_up
 
@@ -204,15 +205,15 @@
         )
 
         sql_with_substitutions = sql.format(**substitutions)
         for key, value in string_replacements.items():
             sql_with_substitutions = sql_with_substitutions.replace(key, value)
 
         job_config = bq.QueryJobConfig()
-        query_job = self._bq_client.query(sql_with_substitutions, location="EU", job_config=job_config)
+        query_job = self._bq_client.query(sql_with_substitutions, job_config=job_config)
         query_job.result()
 
         return query_job.result().to_dataframe()
 
 
 class SQLFileRunner:
     """Class for running SQLFiles."""
```

### Comparing `bquest-0.0.1/bquest/tables.py` & `bquest-0.1.0/bquest/tables.py`

 * *Files identical despite different names*

### Comparing `bquest-0.0.1/pyproject.toml` & `bquest-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bquest"
-version = "0.0.1"
+version = "0.1.0"
 description = "Effortlessly validate and test your Google BigQuery queries with the power of pandas DataFrames in Python."
 authors = ["Otto Group data.works GmbH"]
 license = "Apache Software License"
 readme = "README.rst"
 include = [
     "LICENSE",
     "CHANGELOG.rst"
@@ -46,15 +46,15 @@
 "Issues" = "https://github.com/ottogroup/bquest/issues"
 "Releases" = "https://github.com/ottogroup/bquest/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 google-cloud-bigquery = { version = "^3.8", extras = ["bqstorage", "pandas"] }
-pandas = "^2.0.2"
+pandas = "^1.5.0"
 pandas-gbq = "^0.18"
 sqlvalidator = "^0.0.20"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

