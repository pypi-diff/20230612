# Comparing `tmp/dagster_polars-0.0.0.tar.gz` & `tmp/dagster_polars-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.0.0.tar", max compression
+gzip compressed data, was "dagster_polars-0.0.1.tar", max compression
```

## Comparing `dagster_polars-0.0.0.tar` & `dagster_polars-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11344 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/LICENSE
--rw-r--r--   0        0        0     2031 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/README.md
--rw-r--r--   0        0        0      314 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/dagster_polars/__init__.py
--rw-r--r--   0        0        0       76 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/dagster_polars/_version.py
--rw-r--r--   0        0        0        0 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0     6631 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     1263 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0        0 2023-06-11 19:43:11.413265 dagster_polars-0.0.0/dagster_polars/py.typed
--rw-r--r--   0        0        0     2735 2023-06-11 19:43:11.417265 dagster_polars-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     3194 1970-01-01 00:00:00.000000 dagster_polars-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/LICENSE
+-rw-r--r--   0        0        0     2031 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/README.md
+-rw-r--r--   0        0        0      314 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-12 07:41:16.377835 dagster_polars-0.0.1/dagster_polars/_version.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0     6354 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     1263 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/py.typed
+-rw-r--r--   0        0        0     2736 2023-06-12 07:41:16.377835 dagster_polars-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3194 1970-01-01 00:00:00.000000 dagster_polars-0.0.1/PKG-INFO
```

### Comparing `dagster_polars-0.0.0/LICENSE` & `dagster_polars-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.0/README.md` & `dagster_polars-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.0/dagster_polars/io_managers/base.py` & `dagster_polars-0.0.1/dagster_polars/io_managers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     UPathIOManager,
 )
 from dagster import _check as check
 from pydantic.fields import Field, PrivateAttr
 from upath import UPath
 
 POLARS_DATA_FRAME_ANNOTATIONS = [
+    Any,
     pl.DataFrame,
     Dict[str, pl.DataFrame],
     Mapping[str, pl.DataFrame],
     type(None),
     None,
 ]
 
@@ -162,29 +163,17 @@
         ldf = self.scan_df_from_path(path=path, context=context)
 
         columns = context.metadata.get("columns")
         if columns is not None:
             context.log.debug(f"Loading {columns=}")
             ldf = ldf.select(columns)
 
-        if context.dagster_type.typing_type in (
-            pl.DataFrame,
-            Dict[str, pl.DataFrame],
-            Dict[str, pl.DataFrame],
-            Mapping[str, pl.DataFrame],
-            type(None),
-            None,
-        ):
+        if context.dagster_type.typing_type in POLARS_DATA_FRAME_ANNOTATIONS:
             return ldf.collect(streaming=True)
-        elif context.dagster_type.typing_type in (
-            pl.LazyFrame,
-            Dict[str, pl.LazyFrame],
-            Dict[str, pl.LazyFrame],
-            Mapping[str, pl.LazyFrame],
-        ):
+        elif context.dagster_type.typing_type in POLARS_LAZY_FRAME_ANNOTATIONS:
             return ldf
         else:
             raise NotImplementedError(f"Can't load object for type annotation {context.dagster_type.typing_type}")
 
     def get_metadata(self, context: OutputContext, obj: pl.DataFrame) -> Dict[str, MetadataValue]:
         assert context.metadata is not None
         schema, table = get_metadata_table_and_schema(
```

### Comparing `dagster_polars-0.0.0/dagster_polars/io_managers/parquet.py` & `dagster_polars-0.0.1/dagster_polars/io_managers/parquet.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.0/pyproject.toml` & `dagster_polars-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.0.0"
+version = "0.0.1"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
@@ -46,15 +46,15 @@
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 strict = false
 vcs = "git"
 style = "pep440"
 dirty = true
 
 [tool.poetry-dynamic-versioning.substitution]
 files = [
```

### Comparing `dagster_polars-0.0.0/PKG-INFO` & `dagster_polars-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.0.0
+Version: 0.0.1
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
```

