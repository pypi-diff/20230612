# Comparing `tmp/bquest-0.1.0.tar.gz` & `tmp/bquest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bquest-0.1.0.tar", max compression
+gzip compressed data, was "bquest-0.2.0.tar", max compression
```

## Comparing `bquest-0.1.0.tar` & `bquest-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      132 2023-06-12 14:11:50.571350 bquest-0.1.0/CHANGELOG.rst
--rw-r--r--   0        0        0    11356 2023-06-12 14:11:50.571350 bquest-0.1.0/LICENSE
--rw-r--r--   0        0        0     3621 2023-06-12 14:11:50.571350 bquest-0.1.0/README.rst
--rw-r--r--   0        0        0        0 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/__init__.py
--rw-r--r--   0        0        0     2085 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/dataframe.py
--rw-r--r--   0        0        0     9080 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/runner.py
--rw-r--r--   0        0        0     7272 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/tables.py
--rw-r--r--   0        0        0      328 2023-06-12 14:11:50.571350 bquest-0.1.0/bquest/util.py
--rw-r--r--   0        0        0     2972 2023-06-12 14:11:50.571350 bquest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 bquest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      259 2023-06-12 14:34:28.302203 bquest-0.2.0/CHANGELOG.rst
+-rw-r--r--   0        0        0    11356 2023-06-12 14:34:28.302203 bquest-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3621 2023-06-12 14:34:28.302203 bquest-0.2.0/README.rst
+-rw-r--r--   0        0        0        0 2023-06-12 14:34:28.302203 bquest-0.2.0/bquest/__init__.py
+-rw-r--r--   0        0        0     2085 2023-06-12 14:34:28.302203 bquest-0.2.0/bquest/dataframe.py
+-rw-r--r--   0        0        0     8885 2023-06-12 14:34:28.302203 bquest-0.2.0/bquest/runner.py
+-rw-r--r--   0        0        0     7272 2023-06-12 14:34:28.302203 bquest-0.2.0/bquest/tables.py
+-rw-r--r--   0        0        0      328 2023-06-12 14:34:28.302203 bquest-0.2.0/bquest/util.py
+-rw-r--r--   0        0        0     2972 2023-06-12 14:34:28.302203 bquest-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 bquest-0.2.0/PKG-INFO
```

### Comparing `bquest-0.1.0/LICENSE` & `bquest-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bquest-0.1.0/README.rst` & `bquest-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `bquest-0.1.0/bquest/dataframe.py` & `bquest-0.2.0/bquest/dataframe.py`

 * *Files identical despite different names*

### Comparing `bquest-0.1.0/bquest/runner.py` & `bquest-0.2.0/bquest/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,17 @@
         config["source_tables"] = self._map_source_table_ids_to_mock_table_ids(test_tables)
         return config
 
 
 class BaseRunner:
     """Base class for runners"""
 
-    def __init__(self, bq_client: bq.Client, project: str, dataset: str = "bquest"):
-        # TODO: project is obsolete and can be taken from bq_client
+    def __init__(self, bq_client: bq.Client, dataset: str = "bquest"):
         self._bq_client = bq_client
-        self._bq_table_def_builder = BQTableDefinitionBuilder(project, dataset)
+        self._bq_table_def_builder = BQTableDefinitionBuilder(bq_client.project, dataset)
 
     def _create_source_tables(self, table_definitions: List[BQTableDefinition]) -> List[BQTable]:
         result = []
         for table_def in table_definitions:
             test_table = table_def.load_to_bq(self._bq_client)
             result.append(test_table)
         return result
@@ -88,19 +87,18 @@
 class BQConfigRunner(BaseRunner):
     """Runs BQ configurations on custom data for testing"""
 
     def __init__(
         self,
         bq_client: bq.Client,
         bq_executor_func: Callable[[Dict[str, Any], Optional[Dict[str, str]]], None],
-        project: str,
         dataset: str = "bquest",
         clean_up: bool = True,
     ):
-        super(BQConfigRunner, self).__init__(bq_client, project, dataset)
+        super(BQConfigRunner, self).__init__(bq_client, dataset)
         self._bq_executor_func = bq_executor_func
         self._clean_up = clean_up
 
     def run_config(
         self,
         start_date: str,
         end_date: str,
@@ -169,19 +167,18 @@
 
 class SQLRunner(BaseRunner):
     """Runs SQL queries on custom data for testing"""
 
     def __init__(
         self,
         bq_client: bq.Client,
-        project: str,  # TODO: project is obsolete and can be taken from bq_client
         dataset: str = "bquest",
         clean_up: bool = True,
     ):
-        super(SQLRunner, self).__init__(bq_client, project, dataset)
+        super(SQLRunner, self).__init__(bq_client, dataset)
         self._bq_client = bq_client
         self._clean_up = clean_up
 
     def run(
         self,
         sql: str,
         source_table_definitions: List[BQTableDefinition],
```

### Comparing `bquest-0.1.0/bquest/tables.py` & `bquest-0.2.0/bquest/tables.py`

 * *Files identical despite different names*

### Comparing `bquest-0.1.0/pyproject.toml` & `bquest-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bquest"
-version = "0.1.0"
+version = "0.2.0"
 description = "Effortlessly validate and test your Google BigQuery queries with the power of pandas DataFrames in Python."
 authors = ["Otto Group data.works GmbH"]
 license = "Apache Software License"
 readme = "README.rst"
 include = [
     "LICENSE",
     "CHANGELOG.rst"
```

### Comparing `bquest-0.1.0/PKG-INFO` & `bquest-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bquest
-Version: 0.1.0
+Version: 0.2.0
 Summary: Effortlessly validate and test your Google BigQuery queries with the power of pandas DataFrames in Python.
 Home-page: https://github.com/ottogroup/bquest
 License: Apache Software License
 Keywords: open-source,google-big-query,query,sql,testing,pandas
 Author: Otto Group data.works GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

