# Comparing `tmp/poetry_issue_test-0.1.5.tar.gz` & `tmp/poetry_issue_test-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_issue_test-0.1.5.tar", max compression
+gzip compressed data, was "poetry_issue_test-0.1.6.tar", max compression
```

## Comparing `poetry_issue_test-0.1.5.tar` & `poetry_issue_test-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-12 10:38:36.662892 poetry_issue_test-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2023-06-12 10:25:39.552911 poetry_issue_test-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-12 10:25:12.826245 poetry_issue_test-0.1.5/poetry_test/__init__.py
--rw-r--r--   0        0        0      566 2023-06-12 13:06:59.129855 poetry_issue_test-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 poetry_issue_test-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 10:38:36.662892 poetry_issue_test-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-12 10:25:39.552911 poetry_issue_test-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 10:25:12.826245 poetry_issue_test-0.1.6/poetry_test/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-12 13:09:03.376519 poetry_issue_test-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 poetry_issue_test-0.1.6/PKG-INFO
```

### Comparing `poetry_issue_test-0.1.5/LICENSE` & `poetry_issue_test-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_issue_test-0.1.5/pyproject.toml` & `poetry_issue_test-0.1.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "poetry-issue-test"
-version = "v0.1.5"
+version = "v0.1.6"
 description = ""
 authors = []
 readme = "README.md"
 packages = [{include = "poetry_test"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 requests = "^2.31.0"
-ibis-framework = { version = "^5.1.0", extras = [ "duckdb" ] }
-Ibis-framework =    { version = "^5.1.0", extras = [ "postgres" ], optional = true }
+ibis-framework = [
+    { version = "^5.1.0", extras = [ "duckdb" ] },
+    { version = "^5.1.0", extras = [ "postgres" ], optional = true },
+]
 httpx = {version = "^0.24.1", optional = true}
 
-
 [tool.poetry.extras]
-postgres = ["Ibis-framework"]
+postgres = ["ibis-framework"]
 http = ['httpx']
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `poetry_issue_test-0.1.5/PKG-INFO` & `poetry_issue_test-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: poetry-issue-test
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: http
 Provides-Extra: postgres
-Requires-Dist: Ibis-framework[postgres] (>=5.1.0,<6.0.0) ; extra == "postgres"
 Requires-Dist: httpx (>=0.24.1,<0.25.0) ; extra == "http"
 Requires-Dist: ibis-framework[duckdb] (>=5.1.0,<6.0.0) ; extra == "postgres"
+Requires-Dist: ibis-framework[postgres] (>=5.1.0,<6.0.0) ; extra == "postgres"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
```

