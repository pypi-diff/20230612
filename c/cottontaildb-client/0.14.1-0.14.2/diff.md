# Comparing `tmp/cottontaildb-client-0.14.1.tar.gz` & `tmp/cottontaildb-client-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cottontaildb-client-0.14.1.tar", last modified: Tue Mar 28 09:22:53 2023, max compression
+gzip compressed data, was "cottontaildb-client-0.14.2.tar", last modified: Mon Jun 12 18:53:01 2023, max compression
```

## Comparing `cottontaildb-client-0.14.1.tar` & `cottontaildb-client-0.14.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:22:53.630559 cottontaildb-client-0.14.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-28 09:22:53.630559 cottontaildb-client-0.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:22:53.630559 cottontaildb-client-0.14.1/cottontaildb_client/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/cottontaildb_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/cottontaildb_client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50592 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/cottontaildb_client/cottontail_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/cottontaildb_client/cottontail_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/cottontaildb_client/cottontaildb_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/cottontaildb_client/cottontaildb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:22:53.630559 cottontaildb-client-0.14.1/cottontaildb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-28 09:22:53.000000 cottontaildb-client-0.14.1/cottontaildb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-28 09:22:53.000000 cottontaildb-client-0.14.1/cottontaildb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 09:22:53.000000 cottontaildb-client-0.14.1/cottontaildb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-28 09:22:53.000000 cottontaildb-client-0.14.1/cottontaildb_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 09:22:53.000000 cottontaildb-client-0.14.1/cottontaildb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-28 09:22:53.000000 cottontaildb-client-0.14.1/cottontaildb_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-28 09:22:53.634559 cottontaildb-client-0.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 09:22:53.630559 cottontaildb-client-0.14.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-03-28 09:22:40.000000 cottontaildb-client-0.14.1/tests/test_cottontaildb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/cottontaildb_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50592 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontail_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45483 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontail_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontaildb_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21761 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/cottontaildb_client/cottontaildb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-12 18:53:01.000000 cottontaildb-client-0.14.2/cottontaildb_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:53:01.691947 cottontaildb-client-0.14.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13046 2023-06-12 18:52:48.000000 cottontaildb-client-0.14.2/tests/test_cottontaildb_client.py
```

### Comparing `cottontaildb-client-0.14.1/LICENSE` & `cottontaildb-client-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cottontaildb-client-0.14.1/PKG-INFO` & `cottontaildb-client-0.14.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cottontaildb-client
-Version: 0.14.1
+Version: 0.14.2
 Summary: A Cottontail DB gRPC client.
 Home-page: https://github.com/Spiess/cottontaildb-python-client
 Author: Florian Spiess
 Author-email: florian.spiess@unibas.ch
 Project-URL: Bug Tracker, https://github.com/Spiess/cottontaildb-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 
 ## Installation
 
 Clone and install locally, or with `pip install cottontaildb-client`.
 
 ## Usage
 
-Running the interactive CLI is as easy as `cottontaildb-client [--port PORT] host`.
+Running the interactive CLI is as easy as `cottontaildb-client [--port PORT] HOST`.
 
 Example usage in scripts:
 
 ```python
 from cottontaildb_client import CottontailDBClient, Type, Literal, column_def
 
 with CottontailDBClient('localhost', 1865) as client:
```

### Comparing `cottontaildb-client-0.14.1/README.md` & `cottontaildb-client-0.14.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Installation
 
 Clone and install locally, or with `pip install cottontaildb-client`.
 
 ## Usage
 
-Running the interactive CLI is as easy as `cottontaildb-client [--port PORT] host`.
+Running the interactive CLI is as easy as `cottontaildb-client [--port PORT] HOST`.
 
 Example usage in scripts:
 
 ```python
 from cottontaildb_client import CottontailDBClient, Type, Literal, column_def
 
 with CottontailDBClient('localhost', 1865) as client:
```

### Comparing `cottontaildb-client-0.14.1/cottontaildb_client/cottontail_pb2.py` & `cottontaildb-client-0.14.2/cottontaildb_client/cottontail_pb2.py`

 * *Files identical despite different names*

### Comparing `cottontaildb-client-0.14.1/cottontaildb_client/cottontail_pb2_grpc.py` & `cottontaildb-client-0.14.2/cottontaildb_client/cottontail_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cottontaildb-client-0.14.1/cottontaildb_client/cottontaildb_client.py` & `cottontaildb-client-0.14.2/cottontaildb_client/cottontaildb_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,32 @@
                     'name': c.data[name_index].stringData,
                     'type': c.data[type_index].stringData
                 } for c in response.tuples if c.data[class_index].stringData == 'INDEX'
             ]
         }
 
         return entity_details
+    
+    def sample_entity(self, schema, entity, limit=10, skip=0):
+        """
+        Retrieves a preview of the specified entity.
+
+        @param schema: the entity's schema
+        @param entity: entity name
+        @param limit: number of rows to return
+        @param skip: number of rows to skip from the beginning
+        @return: query response message
+        """
+        schema_name = SchemaName(name=schema)
+        entity_name = EntityName(schema=schema_name, name=entity)
+        op = Projection.ProjectionOperation.SELECT
+        column = ColumnName(entity=entity_name, name="*")
+        elements = [Projection.ProjectionElement(expression=Expression(column=column))]
+        projection = Projection(op=op, elements=elements)
+        return self.query(schema, entity, projection, None, limit=limit, skip=skip)
 
     # Data management
 
     def insert(self, schema, entity, values):
         """
         Inserts column values into an entity.
```

### Comparing `cottontaildb-client-0.14.1/cottontaildb_client.egg-info/PKG-INFO` & `cottontaildb-client-0.14.2/cottontaildb_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cottontaildb-client
-Version: 0.14.1
+Version: 0.14.2
 Summary: A Cottontail DB gRPC client.
 Home-page: https://github.com/Spiess/cottontaildb-python-client
 Author: Florian Spiess
 Author-email: florian.spiess@unibas.ch
 Project-URL: Bug Tracker, https://github.com/Spiess/cottontaildb-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 
 ## Installation
 
 Clone and install locally, or with `pip install cottontaildb-client`.
 
 ## Usage
 
-Running the interactive CLI is as easy as `cottontaildb-client [--port PORT] host`.
+Running the interactive CLI is as easy as `cottontaildb-client [--port PORT] HOST`.
 
 Example usage in scripts:
 
 ```python
 from cottontaildb_client import CottontailDBClient, Type, Literal, column_def
 
 with CottontailDBClient('localhost', 1865) as client:
```

### Comparing `cottontaildb-client-0.14.1/cottontaildb_client.egg-info/SOURCES.txt` & `cottontaildb-client-0.14.2/cottontaildb_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cottontaildb-client-0.14.1/setup.cfg` & `cottontaildb-client-0.14.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cottontaildb-client
-version = 0.14.1
+version = 0.14.2
 author = Florian Spiess
 author_email = florian.spiess@unibas.ch
 description = A Cottontail DB gRPC client.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Spiess/cottontaildb-python-client
 project_urls =
```

### Comparing `cottontaildb-client-0.14.1/tests/test_cottontaildb_client.py` & `cottontaildb-client-0.14.2/tests/test_cottontaildb_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,22 @@
     def test_query(self):
         self._create_schema()
         self._create_entity()
         self._batch_insert()
         query_key = 'test_1'
         query_result = self._query_value_with_key(query_key)
         self.assertEqual(len(query_result), 1, 'unexpected number of rows returned from query')
+    
+    def test_sample_entity(self):
+        self._create_schema()
+        self._create_entity()
+        self._batch_insert()
+        sample = self.client.sample_entity(TEST_SCHEMA_STR, TEST_ENTITY_STR, limit=2)
+        should = [{'id': 'test_1', 'value': 1}, {'id': 'test_2', 'value': 2}]
+        self.assertEqual(sample, should, 'unexpected preview result')
 
     def test_query_vectors(self):
         self._create_schema()
         self._create_vector_entity()
         self._batch_insert_vectors()
         query = [0.1, 0.2, 0.4]
```

