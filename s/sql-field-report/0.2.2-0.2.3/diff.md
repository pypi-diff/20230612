# Comparing `tmp/sql_field_report-0.2.2.tar.gz` & `tmp/sql_field_report-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-0.2.2.tar", max compression
+gzip compressed data, was "sql_field_report-0.2.3.tar", max compression
```

## Comparing `sql_field_report-0.2.2.tar` & `sql_field_report-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      701 2023-06-10 12:09:46.620393 sql_field_report-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.2.2/README.md
--rw-r--r--   0        0        0       82 2023-06-10 11:17:52.279652 sql_field_report-0.2.2/sql_field_report/__init__.py
--rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.2.2/sql_field_report/__main__.py
--rw-r--r--   0        0        0     2866 2023-06-10 12:18:37.485263 sql_field_report-0.2.2/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.2.2/sql_field_report/utils/__init__.py
--rw-r--r--   0        0        0     6898 2023-06-10 12:18:03.137006 sql_field_report-0.2.2/sql_field_report/utils/analysis.py
--rw-r--r--   0        0        0     1579 2023-06-10 12:18:23.532065 sql_field_report-0.2.2/sql_field_report/utils/databases.py
--rw-r--r--   0        0        0     3152 2023-06-10 11:47:50.435359 sql_field_report-0.2.2/sql_field_report/utils/excel.py
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 sql_field_report-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      737 2023-06-12 10:03:03.243946 sql_field_report-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-0.2.3/README.md
+-rw-r--r--   0        0        0      116 2023-06-12 09:54:08.238167 sql_field_report-0.2.3/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-0.2.3/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     4069 2023-06-12 10:03:44.017730 sql_field_report-0.2.3/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-0.2.3/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0     6919 2023-06-12 09:54:08.250421 sql_field_report-0.2.3/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-0.2.3/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-0.2.3/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 sql_field_report-0.2.3/PKG-INFO
```

### Comparing `sql_field_report-0.2.2/pyproject.toml` & `sql_field_report-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -12,14 +12,15 @@
 openpyxl = "^3.1.2"
 sqlalchemy = "^2.0.11"
 python-dotenv = "^1.0.0"
 regex = "^2023.3.23"
 pyodbc = "^4.0.39"
 typer = {extras = ["all"], version = "^0.7.0"}
 coloredlogs = "^15.0.1"
+mysql-connector-python = "^8.0.33"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 
 [tool.poetry.scripts]
```

### Comparing `sql_field_report-0.2.2/README.md` & `sql_field_report-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-0.2.2/sql_field_report/utils/analysis.py` & `sql_field_report-0.2.3/sql_field_report/utils/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import logging
 from typing import Callable
 
-import logging
 import pandas as pd
 import regex as re
 from sqlalchemy import text
+from sqlalchemy.engine import Connection
 
 logger = logging.getLogger(__name__)
 
+
 def most_common(lst):
     """
     Return the most common element in a list
     """
     return max(set(lst), key=lst.count)
 
 
@@ -121,26 +123,26 @@
 
     else:
         analysis = (file, column, 0, 0, 0, "EMPTY")
 
     return analysis
 
 
-def analyze_sql_table(table: str, schema: str, conn):
+def analyze_sql_table(table: str, conn: Connection):
     """
     Take in a file path and return an overview of the shape of that file
 
     Params:
     str: table - the database table to query
 
     Returns:
     Tuple: file_shape - a tuple of tuples containing the file name, field name, row count for each field
     """
     try:
-        data = pd.read_sql(text(f"SELECT * FROM [{schema}].[{table}]"), conn)
+        data = pd.read_sql(text(f"SELECT * FROM {table}"), conn)
 
         file_shape = tuple((review_column(table, data, h) for h in data.columns))
     except:
         data = pd.DataFrame.from_records(
             data=[["ERROR", "ERROR"]], columns=["ERROR", "ERROR2"]
         )
         file_shape = tuple((review_column(table, data, h) for h in data.columns))
@@ -167,27 +169,27 @@
             data=[["ERROR", "ERROR"]], columns=["ERROR", "ERROR2"]
         )
         file_shape = tuple((review_column(table, data, h) for h in data.columns))
 
     return file_shape
 
 
-def analyze_sql_tables(objects: list, schema: str, conn) -> pd.DataFrame:
+def analyze_sql_tables(objects: list, conn: Connection) -> pd.DataFrame:
     """
     Analyze SQL Tables
 
     Params:
     list db_tables - list of database tables
     conn - sql server connection
 
     Returns:
     pd.DataFrame: analysis - a summary of all files, fields and their row counts
     """
 
-    data_shapes = tuple(analyze_sql_table(l, schema, conn) for l in objects)
+    data_shapes = tuple(analyze_sql_table(l, conn) for l in objects)
 
     # flatten tuple
     data_shapes = tuple((element for t in data_shapes for element in t))
 
     analysis = pd.DataFrame(
         data=data_shapes,
         columns=[
```

### Comparing `sql_field_report-0.2.2/sql_field_report/utils/excel.py` & `sql_field_report-0.2.3/sql_field_report/utils/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import logging
+
 import pandas as pd
 from openpyxl.styles import Alignment, PatternFill
 from openpyxl.utils import get_column_letter
 from openpyxl.worksheet.table import Table, TableStyleInfo
 
 logger = logging.getLogger(__name__)
 
+
 def generate_excel_report(analysis: pd.DataFrame, file_path: str) -> str:
     """Generate an excel data report
 
     Args:
         analysis (pd.DataFrame): the analysis dataframe
         filepath (str): the filepath to the produced excel
 
     Returns:
         str: the filepath of the produced excel
     """
-    
+
     logger.info("Generating Excel Report...")
 
     try:
         oddFill = PatternFill(
             start_color="DCE6F1", end_color="DCE6F1", fill_type="solid"
         )
         evenFill = PatternFill(
```

### Comparing `sql_field_report-0.2.2/PKG-INFO` & `sql_field_report-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
+Requires-Dist: mysql-connector-python (>=8.0.33,<9.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyodbc (>=4.0.39,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: regex (>=2023.3.23,<2024.0.0)
 Requires-Dist: sqlalchemy (>=2.0.11,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
```

