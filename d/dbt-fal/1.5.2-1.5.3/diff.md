# Comparing `tmp/dbt_fal-1.5.2.tar.gz` & `tmp/dbt_fal-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_fal-1.5.2.tar", max compression
+gzip compressed data, was "dbt_fal-1.5.3.tar", max compression
```

## Comparing `dbt_fal-1.5.2.tar` & `dbt_fal-1.5.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     3009 2023-06-01 16:04:53.928301 dbt_fal-1.5.2/README.md
--rw-r--r--   0        0        0     1607 2023-06-01 16:05:09.504125 dbt_fal-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      639 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal/__init__.py
--rw-r--r--   0        0        0       18 2023-06-01 16:05:10.184118 dbt_fal-1.5.2/src/dbt/adapters/fal/__version__.py
--rw-r--r--   0        0        0      392 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal/connections.py
--rw-r--r--   0        0        0     3369 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal/impl.py
--rw-r--r--   0        0        0     2768 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal/load_db_profile.py
--rw-r--r--   0        0        0     4091 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal/wrappers.py
--rw-r--r--   0        0        0      344 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/__init__.py
--rw-r--r--   0        0        0       18 2023-06-01 16:05:10.184118 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/__version__.py
--rw-r--r--   0        0        0     4820 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/adapter.py
--rw-r--r--   0        0        0     8381 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/adapter_support.py
--rw-r--r--   0        0        0     1627 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/connections.py
--rw-r--r--   0        0        0     8714 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/impl.py
--rw-r--r--   0        0        0     3192 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/athena.py
--rw-r--r--   0        0        0     2686 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/bigquery.py
--rw-r--r--   0        0        0      980 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/duckdb.py
--rw-r--r--   0        0        0     2977 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/postgres.py
--rw-r--r--   0        0        0     1633 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/redshift.py
--rw-r--r--   0        0        0     2781 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/snowflake.py
--rw-r--r--   0        0        0      821 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/trino.py
--rw-r--r--   0        0        0       25 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/telemetry/__init__.py
--rw-r--r--   0        0        0    10763 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
--rw-r--r--   0        0        0     6572 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport.py
--rw-r--r--   0        0        0     1153 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
--rw-r--r--   0        0        0     4719 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
--rw-r--r--   0        0        0     2972 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
--rw-r--r--   0        0        0     1256 2023-06-01 16:04:53.932301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/utils/__init__.py
--rw-r--r--   0        0        0     9804 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/utils/environments.py
--rw-r--r--   0        0        0     1970 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
--rw-r--r--   0        0        0      208 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/fal/adapters/python/__init__.py
--rw-r--r--   0        0        0    11898 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/fal/adapters/python/connections.py
--rw-r--r--   0        0        0    10015 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/fal/adapters/python/impl.py
--rw-r--r--   0        0        0      181 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/fal/adapters/teleport/__init__.py
--rw-r--r--   0        0        0     3498 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/fal/adapters/teleport/impl.py
--rw-r--r--   0        0        0     2310 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/fal/adapters/teleport/info.py
--rw-r--r--   0        0        0       52 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal/__init__.py
--rw-r--r--   0        0        0       70 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal/dbt_project.yml
--rw-r--r--   0        0        0     1213 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal/macros/materializations/table.sql
--rw-r--r--   0        0        0      265 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal/macros/teleport_duckdb.sql
--rw-r--r--   0        0        0      921 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal/macros/teleport_snowflake.sql
--rw-r--r--   0        0        0       52 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal_experimental/__init__.py
--rw-r--r--   0        0        0       83 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal_experimental/dbt_project.yml
--rw-r--r--   0        0        0      989 2023-06-01 16:04:53.936301 dbt_fal-1.5.2/src/dbt/include/fal_experimental/macros/materializations/table.sql
--rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 dbt_fal-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3009 2023-06-12 18:06:15.192159 dbt_fal-1.5.3/README.md
+-rw-r--r--   0        0        0     1607 2023-06-12 18:06:30.460368 dbt_fal-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      639 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal/__init__.py
+-rw-r--r--   0        0        0       18 2023-06-12 18:06:30.956375 dbt_fal-1.5.3/src/dbt/adapters/fal/__version__.py
+-rw-r--r--   0        0        0      392 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal/connections.py
+-rw-r--r--   0        0        0     3369 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal/impl.py
+-rw-r--r--   0        0        0     2768 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal/load_db_profile.py
+-rw-r--r--   0        0        0     4091 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal/wrappers.py
+-rw-r--r--   0        0        0      344 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       18 2023-06-12 18:06:30.956375 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/__version__.py
+-rw-r--r--   0        0        0     4820 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/adapter.py
+-rw-r--r--   0        0        0     8381 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/adapter_support.py
+-rw-r--r--   0        0        0     1627 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/connections.py
+-rw-r--r--   0        0        0     8714 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/impl.py
+-rw-r--r--   0        0        0     3192 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/athena.py
+-rw-r--r--   0        0        0     2686 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/bigquery.py
+-rw-r--r--   0        0        0      980 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/duckdb.py
+-rw-r--r--   0        0        0     2977 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/postgres.py
+-rw-r--r--   0        0        0     1633 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/redshift.py
+-rw-r--r--   0        0        0     2781 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/snowflake.py
+-rw-r--r--   0        0        0      821 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/trino.py
+-rw-r--r--   0        0        0       25 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/telemetry/__init__.py
+-rw-r--r--   0        0        0    10763 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
+-rw-r--r--   0        0        0     6572 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport.py
+-rw-r--r--   0        0        0     1153 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
+-rw-r--r--   0        0        0     4719 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
+-rw-r--r--   0        0        0     2972 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
+-rw-r--r--   0        0        0     1256 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/utils/__init__.py
+-rw-r--r--   0        0        0     9804 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/utils/environments.py
+-rw-r--r--   0        0        0     1970 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
+-rw-r--r--   0        0        0      208 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/fal/adapters/python/__init__.py
+-rw-r--r--   0        0        0    11898 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/fal/adapters/python/connections.py
+-rw-r--r--   0        0        0    10015 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/fal/adapters/python/impl.py
+-rw-r--r--   0        0        0      181 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/fal/adapters/teleport/__init__.py
+-rw-r--r--   0        0        0     3498 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/fal/adapters/teleport/impl.py
+-rw-r--r--   0        0        0     2310 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/fal/adapters/teleport/info.py
+-rw-r--r--   0        0        0       52 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal/dbt_project.yml
+-rw-r--r--   0        0        0     1213 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal/macros/materializations/table.sql
+-rw-r--r--   0        0        0      265 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal/macros/teleport_duckdb.sql
+-rw-r--r--   0        0        0      921 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal/macros/teleport_snowflake.sql
+-rw-r--r--   0        0        0       52 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal_experimental/dbt_project.yml
+-rw-r--r--   0        0        0      989 2023-06-12 18:06:15.196159 dbt_fal-1.5.3/src/dbt/include/fal_experimental/macros/materializations/table.sql
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 dbt_fal-1.5.3/PKG-INFO
```

### Comparing `dbt_fal-1.5.2/README.md` & `dbt_fal-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/pyproject.toml` & `dbt_fal-1.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-fal"
-version = "1.5.2"
+version = "1.5.3"
 description = "Simplest way to run dbt python models."
 readme = "README.md"
 homepage = "https://github.com/fal-ai/fal/blob/-/projects/adapter"
 repository = "https://github.com/fal-ai/fal"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
     { include = "dbt", from = "src" }
@@ -40,15 +40,15 @@
 
 # teleport
 s3fs = { version = ">=2022.8.2", optional = true }
 
 # fal cloud
 dill = ">=0.3.5.1"
 packaging = ">=23"
-fal-serverless = "^0.6.33"
+fal-serverless = "^0.6.34"
 importlib-metadata = "^6.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.extras]
 postgres = []
```

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal/__init__.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal/impl.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal/load_db_profile.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal/load_db_profile.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal/wrappers.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal/wrappers.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/adapter.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/adapter.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/adapter_support.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/adapter_support.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/connections.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/impl.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/athena.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/athena.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/bigquery.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/bigquery.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/duckdb.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/postgres.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/postgres.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/redshift.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/redshift.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/snowflake.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/support/trino.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/support/trino.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/telemetry/telemetry.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport_adapter_support.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport_adapter_support.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/utils/__init__.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/utils/environments.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/utils/environments.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/adapters/fal_experimental/utils/yaml_helper.py` & `dbt_fal-1.5.3/src/dbt/adapters/fal_experimental/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/fal/adapters/python/connections.py` & `dbt_fal-1.5.3/src/dbt/fal/adapters/python/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/fal/adapters/python/impl.py` & `dbt_fal-1.5.3/src/dbt/fal/adapters/python/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/fal/adapters/teleport/impl.py` & `dbt_fal-1.5.3/src/dbt/fal/adapters/teleport/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/fal/adapters/teleport/info.py` & `dbt_fal-1.5.3/src/dbt/fal/adapters/teleport/info.py`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/include/fal/macros/materializations/table.sql` & `dbt_fal-1.5.3/src/dbt/include/fal/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/include/fal/macros/teleport_snowflake.sql` & `dbt_fal-1.5.3/src/dbt/include/fal/macros/teleport_snowflake.sql`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/src/dbt/include/fal_experimental/macros/materializations/table.sql` & `dbt_fal-1.5.3/src/dbt/include/fal_experimental/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_fal-1.5.2/PKG-INFO` & `dbt_fal-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fal
-Version: 1.5.2
+Version: 1.5.3
 Summary: Simplest way to run dbt python models.
 Home-page: https://github.com/fal-ai/fal/blob/-/projects/adapter
 Keywords: dbt,pandas,fal,runtime
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7.2,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -21,15 +21,15 @@
 Provides-Extra: snowflake
 Provides-Extra: teleport
 Provides-Extra: trino
 Requires-Dist: awswrangler[redshift] (>=3.0.0) ; (python_version >= "3.8") and (extra == "redshift")
 Requires-Dist: backports.functools_lru_cache (>=1.6.4,<2.0.0)
 Requires-Dist: dbt-core (>=1.5.0,<1.6)
 Requires-Dist: dill (>=0.3.5.1)
-Requires-Dist: fal-serverless (>=0.6.33,<0.7.0)
+Requires-Dist: fal-serverless (>=0.6.34,<0.7.0)
 Requires-Dist: google-cloud-bigquery[pandas] (>=3.5.0,<3.6.0) ; extra == "bigquery"
 Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
 Requires-Dist: packaging (>=23)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: posthog (>=1.4.5,<2.0.0)
 Requires-Dist: s3fs (>=2022.8.2) ; extra == "teleport"
 Requires-Dist: snowflake-connector-python[pandas] (>=3.0,<4.0) ; extra == "snowflake"
```

