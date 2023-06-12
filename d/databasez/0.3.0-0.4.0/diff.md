# Comparing `tmp/databasez-0.3.0.tar.gz` & `tmp/databasez-0.4.0.tar.gz`

## Comparing `databasez-0.3.0.tar` & `databasez-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/__init__.py
--rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/core.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/importer.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/interfaces.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/py.typed
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/testclient.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/__init__.py
--rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/aiopg.py
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/asyncmy.py
--rw-r--r--   0        0        0    11987 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/mssql.py
--rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/mysql.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/postgres.py
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/common/__init__.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/common/records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/compilers/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/compilers/psycopg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/dialects/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.3.0/databasez/backends/dialects/psycopg.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.3.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.3.0/README.md
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 databasez-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 databasez-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/__init__.py
+-rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/core.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/importer.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/interfaces.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/py.typed
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/testclient.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/__init__.py
+-rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/aiopg.py
+-rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/asyncmy.py
+-rw-r--r--   0        0        0    11987 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/mssql.py
+-rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/mysql.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/postgres.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/common/__init__.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/common/records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/compilers/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/compilers/psycopg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/dialects/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/dialects/psycopg.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.4.0/README.md
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 databasez-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 databasez-0.4.0/PKG-INFO
```

### Comparing `databasez-0.3.0/databasez/core.py` & `databasez-0.4.0/databasez/core.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/importer.py` & `databasez-0.4.0/databasez/importer.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/interfaces.py` & `databasez-0.4.0/databasez/interfaces.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/testclient.py` & `databasez-0.4.0/databasez/testclient.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/backends/aiopg.py` & `databasez-0.4.0/databasez/backends/aiopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/backends/asyncmy.py` & `databasez-0.4.0/databasez/backends/asyncmy.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,23 @@
     def _get_connection_kwargs(self) -> dict:
         url_options = self._database_url.options
 
         kwargs = {}
         min_size = url_options.get("min_size")
         max_size = url_options.get("max_size")
         pool_recycle = url_options.get("pool_recycle")
+        unix_socket = url_options.get("unix_socket")
         ssl = url_options.get("ssl")
 
         if min_size is not None:
             kwargs["minsize"] = int(min_size)
         if max_size is not None:
             kwargs["maxsize"] = int(max_size)
+        if unix_socket is not None:
+            kwargs["unix_socket"] = unix_socket
         if pool_recycle is not None:
             kwargs["pool_recycle"] = int(pool_recycle)
         if ssl is not None:
             kwargs["ssl"] = {"true": True, "false": False}[ssl.lower()]
 
         for key, value in self._options.items():
             # Coerce 'min_size' and 'max_size' for consistency.
```

### Comparing `databasez-0.3.0/databasez/backends/mssql.py` & `databasez-0.4.0/databasez/backends/mssql.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/backends/mysql.py` & `databasez-0.4.0/databasez/backends/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,23 @@
     def _get_connection_kwargs(self) -> dict:
         url_options = self._database_url.options
 
         kwargs = {}
         min_size = url_options.get("min_size")
         max_size = url_options.get("max_size")
         pool_recycle = url_options.get("pool_recycle")
+        unix_socket = url_options.get("unix_socket")
         ssl = url_options.get("ssl")
 
         if min_size is not None:
             kwargs["minsize"] = int(min_size)
         if max_size is not None:
             kwargs["maxsize"] = int(max_size)
+        if unix_socket is not None:
+            kwargs["unix_socket"] = unix_socket
         if pool_recycle is not None:
             kwargs["pool_recycle"] = int(pool_recycle)
         if ssl is not None:
             kwargs["ssl"] = {"true": True, "false": False}[ssl.lower()]
 
         for key, value in self._options.items():
             # Coerce 'min_size' and 'max_size' for consistency.
```

### Comparing `databasez-0.3.0/databasez/backends/postgres.py` & `databasez-0.4.0/databasez/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/backends/sqlite.py` & `databasez-0.4.0/databasez/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/backends/common/records.py` & `databasez-0.4.0/databasez/backends/common/records.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/databasez/backends/dialects/psycopg.py` & `databasez-0.4.0/databasez/backends/dialects/psycopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/LICENSE.md` & `databasez-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/README.md` & `databasez-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `databasez-0.3.0/pyproject.toml` & `databasez-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
-dependencies = ["nest_asyncio>=1.5.6,<2.0.0", "sqlalchemy>=2.0.12,<2.1"]
+dependencies = ["nest_asyncio>=1.5.6,<2.0.0", "sqlalchemy>=2.0.16,<2.1"]
 keywords = [
     "mysql",
     "postgres",
     "sqlalchemy",
     "sqlite",
     "asyncio",
     "esmerald",
```

### Comparing `databasez-0.3.0/PKG-INFO` & `databasez-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databasez
-Version: 0.3.0
+Version: 0.4.0
 Summary: Async database support for Python.
 Project-URL: Homepage, https://github.com/tarsil/databasez
 Project-URL: Documentation, https://databasez.tarsild/
 Project-URL: Changelog, https://databasez.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/databasez
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -33,15 +33,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.6
-Requires-Dist: sqlalchemy<2.1,>=2.0.12
+Requires-Dist: sqlalchemy<2.1,>=2.0.16
 Provides-Extra: aiomysql
 Requires-Dist: aiomysql; extra == 'aiomysql'
 Provides-Extra: aioodbc
 Requires-Dist: aioodbc; extra == 'aioodbc'
 Provides-Extra: aiopg
 Requires-Dist: aiopg; extra == 'aiopg'
 Provides-Extra: aiosqlite
```

