# Comparing `tmp/macrometa-source-collection-0.0.40.tar.gz` & `tmp/macrometa-source-collection-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.40.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.41.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.40.tar` & `macrometa-source-collection-0.0.41.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9482 2023-06-12 14:42:41.861404 macrometa-source-collection-0.0.40/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9087 2023-06-12 14:42:41.861404 macrometa-source-collection-0.0.40/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-06-12 14:42:42.149423 macrometa-source-collection-0.0.40/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.40/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.40/PKG-INFO
+-rw-r--r--   0        0        0     9563 2023-06-12 16:22:42.553805 macrometa-source-collection-0.0.41/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9087 2023-06-12 16:22:42.553805 macrometa-source-collection-0.0.41/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-12 16:22:42.845821 macrometa-source-collection-0.0.41/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.41/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.41/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.40/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.41/macrometa_source_collection/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,21 +136,23 @@
             raise KeyError(f'Integration property `{e}` not found.')
 
 
 def get_schema_and_data(client: C8Client, collection: str, sample_size: int, workflow_run=False):
     cursor = None
     schema_counts = defaultdict(int)
     records_by_schema = defaultdict(list)
+    LOGGER.warn("Determining schema..")
+    LOGGER.error("Determining schema..")
     LOGGER.info("Determining schema..")
     while cursor is None or cursor.empty():
         cursor = client.execute_query(f"FOR d IN @@collection LIMIT 0, @count RETURN d",
                                       bind_vars={"@collection": collection, "count": sample_size})
         if cursor.empty():
             if workflow_run:
-                LOGGER.info("Cannot determine schema as no records found in collection. Retrying after 30 seconds..")
+                LOGGER.warn("Cannot determine schema as no records found in collection. Retrying after 30 seconds..")
                 time.sleep(30)
             else:
                 raise Exception("Cannot determine schema as no records found in collection.")
 
     while not cursor.empty():
         rec = cursor.next()
         rec.pop('_id', None)
```

### Comparing `macrometa-source-collection-0.0.40/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.41/macrometa_source_collection/client.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.40/pyproject.toml` & `macrometa-source-collection-0.0.41/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.40'
+version='0.0.41'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
     "Macrometa",
     "GDN",
     "Collection",
-    "Tap"
+    "Source"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
 ]
 packages = [
```

### Comparing `macrometa-source-collection-0.0.40/setup.py` & `macrometa-source-collection-0.0.41/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.40',
+    'version': '0.0.41',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.40/PKG-INFO` & `macrometa-source-collection-0.0.41/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.40
+Version: 0.0.41
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
-Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
+Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

