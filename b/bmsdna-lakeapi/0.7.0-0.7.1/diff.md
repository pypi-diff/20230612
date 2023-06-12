# Comparing `tmp/bmsdna_lakeapi-0.7.0.tar.gz` & `tmp/bmsdna_lakeapi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.7.0.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.7.1.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.7.0.tar` & `bmsdna_lakeapi-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-09 19:14:25.049285 bmsdna_lakeapi-0.7.0/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-09 19:14:25.049285 bmsdna_lakeapi-0.7.0/README.md
--rw-r--r--   0        0        0      337 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      566 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6595 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     9385 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6030 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11077 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12618 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15585 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6887 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6467 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4291 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3763 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3109 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-09 19:14:25.053285 bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1999 2023-06-09 19:14:25.057285 bmsdna_lakeapi-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-12 11:13:36.309071 bmsdna_lakeapi-0.7.1/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-12 11:13:36.309071 bmsdna_lakeapi-0.7.1/README.md
+-rw-r--r--   0        0        0      337 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      566 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6876 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9792 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6091 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11077 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12618 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15585 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6887 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6467 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4291 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3763 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3109 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-12 11:13:36.313072 bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1999 2023-06-12 11:13:36.317072 bmsdna_lakeapi-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.7.1/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.7.0/LICENSE` & `bmsdna_lakeapi-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/README.md` & `bmsdna_lakeapi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/df_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,37 +115,38 @@
 
     def get_pyarrow_dataset(
         self,
         uri: str,
         file_type: FileTypes,
         partitions: Optional[List[Tuple[str, str, Any]]],
     ) -> Optional[pa.dataset.Dataset | pa.Table]:
-        if file_type in ["parquet", "ipc", "arrow", "feather", "csv", "orc"]:
-            ds = pa.dataset.dataset(uri, format=file_type)
-        elif file_type in ["ndjson", "json"]:
-            import pandas
-
-            pd = pandas.read_json(uri, orient="records", lines=file_type == "ndjson")
-
-            return pyarrow.Table.from_pandas(pd)
-        elif file_type == "avro":
-            import polars as pl
-
-            pd = pl.read_avro(uri).to_arrow()
-            return pd
-        elif file_type == "delta":
-            dt = DeltaTable(
-                uri,
-            )
-
-            ds = dt.to_pyarrow_dataset(partitions=partitions)
-
-        else:
-            raise Exception(f"Not supported file type {file_type}")
-        return ds
+        match file_type:
+            case "parquet":
+                import pyarrow.dataset as ds
+                return pa.dataset.dataset(uri, format=ds.ParquetFileFormat(read_options={"coerce_int96_timestamp_unit": "us"}))
+            case "ipc" | "arrow" | "feather" | "csv" | "orc":
+                return pa.dataset.dataset(uri, format=file_type)
+            case "ndjson" | "json":
+                import pandas
+
+                pd = pandas.read_json(uri, orient="records", lines=file_type == "ndjson")
+
+                return pyarrow.Table.from_pandas(pd)
+            case "avro":
+                import polars as pl
+
+                pd = pl.read_avro(uri).to_arrow()
+                return pd
+            case "delta":
+                dt = DeltaTable(
+                    uri,
+                )
+                return dt.to_pyarrow_dataset(partitions=partitions, parquet_read_options={"coerce_int96_timestamp_unit": "us"})
+            case _:
+                raise Exception(f"Not supported file type {file_type}")
 
     @abstractmethod
     def register_arrow(self, name: str, ds: Union[pyarrow.dataset.Dataset, pyarrow.Table]):
         ...
 
     @abstractmethod
     def close(self):
```

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 
 ENABLE_COPY_TO = os.environ.get("ENABLE_COPY_TO", "0") == "1"
 
-
 class DuckDBResultData(ResultData):
     def __init__(
         self,
         original_sql: Union[pypika.queries.QueryBuilder, str],
         con: duckdb.DuckDBPyConnection,
     ) -> None:
         super().__init__()
@@ -177,15 +176,15 @@
         persistance_file_name = os.path.join(persitance_path, persistence_name + ".duckdb")
 
         if (
             not os.path.exists(persistance_file_name)
             or datetime.fromtimestamp(os.path.getmtime(persistance_file_name), tz=timezone.utc)
             < modified_date.astimezone(timezone.utc)
             or datetime.fromtimestamp(os.path.getmtime(persistance_file_name), tz=timezone.utc)
-            < datetime.fromisoformat("2023-05-19T00:00Z")  # before duckdb upgrade
+            < datetime.fromisoformat("2023-05-19").astimezone(timezone.utc)  # before duckdb upgrade
         ):
             persistance_file_name_temp = persistance_file_name + "_temp"
             if os.path.exists(persistance_file_name_temp):
                 os.remove(persistance_file_name_temp)
             search_con = duckdb.connect(persistance_file_name_temp, read_only=False)
             search_con.commit()  # create empty duck file
             search_con.close()
@@ -200,20 +199,27 @@
                 os.remove(persistance_file_name)
             os.rename(persistance_file_name_temp, persistance_file_name)
         self.persistance_file_name = persistance_file_name
 
     def register_dataframe(
         self, name: str, uri: str, file_type: FileTypes, partitions: List[Tuple[str, str, Any]] | None
     ):
+        self.modified_dates[name] = self.get_modified_date(uri, file_type)
         if file_type == "json":
             self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_json_auto('{uri}', format='array')")
             return
         if file_type == "ndjson":
             self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_json_auto('{uri}', format='newline_delimited')")
             return
+        if file_type == "parquet":
+            self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_parquet('{uri}')")
+            return
+        if file_type == "csv":
+            self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_csv_auto('{uri}', delim=',', header=True)")
+            return
         return super().register_dataframe(name, uri, file_type, partitions)
 
     def list_tables(self) -> ResultData:
         return self.execute_sql(
             "SELECT table_name as name, table_type from information_schema.tables where table_schema='main'"
         )
```

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/context/df_polars.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         self.modified_dates[name] = self.get_modified_date(uri, file_type)
         match file_type:
             case "delta":
                 from bmsdna.lakeapi.polars_extensions.delta import scan_delta2
 
                 df = pl.scan_delta2(  # type: ignore
                     uri,
-                    pyarrow_options={"partitions": partitions},
+                    pyarrow_options={"partitions": partitions, "parquet_read_options":{"coerce_int96_timestamp_unit": "us"}}
                 )
             case "parquet":
                 df = pl.scan_parquet(uri)
             case "arrow":
                 df = pl.scan_ipc(uri)
             case "avro":
                 df = cast(pl.LazyFrame, pl.read_avro(uri))
```

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.7.1/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.7.0/pyproject.toml` & `bmsdna_lakeapi-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.7.0/PKG-INFO` & `bmsdna_lakeapi-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

