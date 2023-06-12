# Comparing `tmp/pysparkler-0.7.dev1686161652.tar.gz` & `tmp/pysparkler-0.7.dev1686592407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.7.dev1686161652.tar", max compression
+gzip compressed data, was "pysparkler-0.7.dev1686592407.tar", max compression
```

## Comparing `pysparkler-0.7.dev1686161652.tar` & `pysparkler-0.7.dev1686592407.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    12173 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/README.md
--rw-r--r--   0        0        0     1203 2023-06-07 18:14:12.646876 pysparkler-0.7.dev1686161652/pyproject.toml
--rw-r--r--   0        0        0      807 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/__init__.py
--rw-r--r--   0        0        0     5294 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/api.py
--rw-r--r--   0        0        0     7372 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/base.py
--rw-r--r--   0        0        0     6398 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2206 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10561 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4550 2023-06-07 18:14:04.374793 pysparkler-0.7.dev1686161652/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0    13052 1970-01-01 00:00:00.000000 pysparkler-0.7.dev1686161652/PKG-INFO
+-rw-r--r--   0        0        0    12173 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/README.md
+-rw-r--r--   0        0        0     1203 2023-06-12 17:53:28.181575 pysparkler-0.7.dev1686592407/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/__init__.py
+-rw-r--r--   0        0        0     5294 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/api.py
+-rw-r--r--   0        0        0     7372 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/base.py
+-rw-r--r--   0        0        0     6398 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2206 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10561 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     3895 2023-06-12 17:53:17.697330 pysparkler-0.7.dev1686592407/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0    13052 1970-01-01 00:00:00.000000 pysparkler-0.7.dev1686592407/PKG-INFO
```

### Comparing `pysparkler-0.7.dev1686161652/README.md` & `pysparkler-0.7.dev1686592407/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pyproject.toml` & `pysparkler-0.7.dev1686592407/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.7.dev1686161652"
+version = "0.7.dev1686592407"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
     "Holden Karau <holden@pigscanfly.ca>",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-libcst = "^0.4.9"
+libcst = "^1.0.1"
 click = "^8.1.3"
 rich = "^13.3.3"
 nbformat = "^5.8.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
```

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/__init__.py` & `pysparkler-0.7.dev1686592407/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/api.py` & `pysparkler-0.7.dev1686592407/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/base.py` & `pysparkler-0.7.dev1686592407/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/cli.py` & `pysparkler-0.7.dev1686592407/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.7.dev1686592407/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.7.dev1686592407/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.7.dev1686592407/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.7.dev1686592407/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.7.dev1686161652/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.7.dev1686592407/pysparkler/pyspark_32_to_33.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,51 +31,35 @@
 
     def __init__(
         self,
         pyspark_version: str = "3.3",
     ):
         super().__init__(
             transformer_id="PY32-33-001",
-            comment=f"Explicitly setting axis to 1 to drop by column, since as of PySpark {pyspark_version} the drop \
-method of pandas API on Spark DataFrame sets drop by index as default, instead of drop by column.",
+            comment=f"As of PySpark {pyspark_version} the drop method of pandas API on Spark DataFrame sets drop by \
+index as default, instead of drop by column. Please explicitly set axis argument to 1 to drop by column.",
         )
-        self.inside_drop_call = False
 
-    def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
-        """Specify the axis argument to 1 if it is not specified to maintain the behavior of dropping columns"""
+    def visit_Call(self, node: cst.Call) -> None:
+        """Check if drop method does not specify the axis argument and drops by labels"""
         if m.matches(
-            original_node,
+            node,
             m.Call(
                 func=m.Attribute(
                     attr=m.Name("drop"),
                 ),
                 args=[
                     m.OneOf(
                         m.Arg(keyword=m.Name("labels")),
                         m.Arg(keyword=None),
                     )
                 ],
             ),
         ):
             self.match_found = True
-            return updated_node.with_changes(
-                args=[
-                    *updated_node.args,
-                    cst.Arg(
-                        keyword=cst.Name("axis"),
-                        value=cst.Integer("1"),
-                        equal=cst.AssignEqual(
-                            whitespace_before=cst.SimpleWhitespace(""),
-                            whitespace_after=cst.SimpleWhitespace(""),
-                        ),
-                    ),
-                ]
-            )
-        else:
-            return updated_node
 
 
 class RequiredPandasVersionCommentWriter(RequiredDependencyVersionCommentWriter):
     """In Spark 3.3, PySpark upgrades Pandas version, the new minimum required version changes from 0.23.2 to 1.0.5."""
 
     def __init__(
         self,
```

### Comparing `pysparkler-0.7.dev1686161652/PKG-INFO` & `pysparkler-0.7.dev1686592407/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.7.dev1686161652
+Version: 0.7.dev1686592407
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: libcst (>=0.4.9,<0.5.0)
+Requires-Dist: libcst (>=1.0.1,<2.0.0)
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Project-URL: Repository, https://github.com/holdenk/spark-upgrade
 Description-Content-Type: text/markdown
 
 # PySparkler
```

