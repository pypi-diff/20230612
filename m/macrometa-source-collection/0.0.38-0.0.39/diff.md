# Comparing `tmp/macrometa-source-collection-0.0.38.tar.gz` & `tmp/macrometa-source-collection-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.38.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.39.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.38.tar` & `macrometa-source-collection-0.0.39.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8969 2023-06-06 05:15:44.779250 macrometa-source-collection-0.0.38/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9087 2023-06-06 05:15:44.779250 macrometa-source-collection-0.0.38/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-06-06 05:15:45.023257 macrometa-source-collection-0.0.38/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.38/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.38/PKG-INFO
+-rw-r--r--   0        0        0     9485 2023-06-12 13:42:20.268404 macrometa-source-collection-0.0.39/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9087 2023-06-12 13:42:20.268404 macrometa-source-collection-0.0.39/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-06-12 13:42:20.512405 macrometa-source-collection-0.0.39/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.39/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.39/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.38/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.39/macrometa_source_collection/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """GDN data connector source for GDN Collections."""
 from collections import defaultdict
 from urllib.parse import urlparse
 
 import pkg_resources
 import singer
+import time
 from c8 import C8Client
 from c8connector import C8Connector, Sample, ConfigProperty, ConfigAttributeType, Schema, SchemaAttributeType, \
     SchemaAttribute
 from singer import utils
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema as SingerSchema
 
@@ -131,19 +132,29 @@
                 'fabric': integration['fabric'],
                 'source_collection': integration['source_collection']
             }
         except KeyError as e:
             raise KeyError(f'Integration property `{e}` not found.')
 
 
-def get_schema_and_data(client: C8Client, collection: str, sample_size: int):
-    cursor = client.execute_query(f"FOR d IN @@collection LIMIT 0, @count RETURN d",
-                                  bind_vars={"@collection": collection, "count": sample_size})
+def get_schema_and_data(client: C8Client, collection: str, sample_size: int, workflow_run=False):
+    cursor = None
     schema_counts = defaultdict(int)
     records_by_schema = defaultdict(list)
+    while cursor is None or cursor.empty():
+        cursor = client.execute_query(f"FOR d IN @@collection LIMIT 0, @count RETURN d",
+                                      bind_vars={"@collection": collection, "count": sample_size})
+        if cursor.empty():
+            if workflow_run:
+                LOGGER.info("Cannot determine schema as no records found in collection %s, Retrying after 30 seconds ",
+                             collection)
+                time.sleep(30)
+            else:
+                raise Exception("Cannot determine schema as no records found in collection.")
+
     while not cursor.empty():
         rec = cursor.next()
         rec.pop('_id', None)
         rec.pop('_rev', None)
         # Skip empty records or records with no keys
         if not rec or not rec.keys():
             continue
@@ -174,23 +185,23 @@
         return SchemaAttributeType.BOOLEAN
     elif source_type == 'number':
         return SchemaAttributeType.DOUBLE
     else:
         return SchemaAttributeType.OBJECT
 
 
-def do_discovery(config):
+def do_discovery(config, workflow_run=False):
     collection_name = config['source_collection']
     schema, _ = get_schema_and_data(C8Client(
         "https",
         host=config["gdn_host"],
         port=443,
         geofabric=config["fabric"],
         apikey=config["api_key"]
-    ), collection_name, 50)
+    ), collection_name, 50, workflow_run)
     schema_properties = {
         k: SingerSchema(
             type=['null', 'string', 'integer', 'number', 'boolean', 'array', 'object'] if v == 'null' else (v if k == '_key' else ['null', v]),
             format=None
         )
         for k, v in schema.items()
     }
@@ -232,15 +243,15 @@
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     conn_config = {'api_key': args.config['api_key'],
                    'gdn_host': extract_gdn_host(args.config['gdn_host']),
                    'fabric': args.config['fabric'],
                    'source_collection': args.config['source_collection']}
 
     if args.discover:
-        do_discovery(conn_config)
+        do_discovery(conn_config, workflow_run=True)
     elif args.catalog:
         do_sync(conn_config, args.catalog, args.config.get('default_replication_method'))
     else:
         LOGGER.info("No properties were selected")
     return
```

### Comparing `macrometa-source-collection-0.0.38/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.39/macrometa_source_collection/client.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.38/pyproject.toml` & `macrometa-source-collection-0.0.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.38'
+version='0.0.39'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.38/setup.py` & `macrometa-source-collection-0.0.39/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.38',
+    'version': '0.0.39',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.38/PKG-INFO` & `macrometa-source-collection-0.0.39/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.38
+Version: 0.0.39
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

