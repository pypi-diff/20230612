# Comparing `tmp/macrometa-source-collection-0.0.42.tar.gz` & `tmp/macrometa-source-collection-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.42.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.43.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.42.tar` & `macrometa-source-collection-0.0.43.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9606 2023-06-12 16:59:26.768277 macrometa-source-collection-0.0.42/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     9087 2023-06-12 16:59:26.768277 macrometa-source-collection-0.0.42/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-12 16:59:27.024284 macrometa-source-collection-0.0.42/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.42/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.42/PKG-INFO
+-rw-r--r--   0        0        0     9533 2023-06-12 17:15:41.145646 macrometa-source-collection-0.0.43/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     9087 2023-06-12 17:15:41.145646 macrometa-source-collection-0.0.43/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-12 17:15:41.437644 macrometa-source-collection-0.0.43/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.43/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.43/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.42/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.43/macrometa_source_collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,23 +136,21 @@
             raise KeyError(f'Integration property `{e}` not found.')
 
 
 def get_schema_and_data(client: C8Client, collection: str, sample_size: int, workflow_run=False):
     cursor = None
     schema_counts = defaultdict(int)
     records_by_schema = defaultdict(list)
-    LOGGER.warn("Determining schema..")
-    LOGGER.error("Determining schema..")
     LOGGER.info("Determining schema..")
     while cursor is None or cursor.empty():
         cursor = client.execute_query(f"FOR d IN @@collection LIMIT 0, @count RETURN d",
                                       bind_vars={"@collection": collection, "count": sample_size})
         if cursor.empty():
             if workflow_run:
-                LOGGER.warn("Cannot determine schema as no records found in collection. Retrying after 30 seconds..")
+                LOGGER.info("Cannot determine schema as no records found in collection. Retrying after 30 seconds..")
                 time.sleep(30)
             else:
                 raise Exception("Cannot determine schema as no records found in collection.")
 
     while not cursor.empty():
         rec = cursor.next()
         rec.pop('_id', None)
@@ -244,22 +242,23 @@
 def main_impl():
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     conn_config = {'api_key': args.config['api_key'],
                    'gdn_host': extract_gdn_host(args.config['gdn_host']),
                    'fabric': args.config['fabric'],
                    'source_collection': args.config['source_collection']}
 
+    LOGGER.info("Testing 123..")
     if args.discover:
-        LOGGER.info("Discovery started..")
         do_discovery(conn_config, workflow_run=True)
     elif args.catalog:
         do_sync(conn_config, args.catalog, args.config.get('default_replication_method'))
     else:
         LOGGER.info("No properties were selected")
     return
 
 
 def main():
     try:
         main_impl()
     except Exception as exc:
         LOGGER.critical(exc)
+        raise exc
```

### Comparing `macrometa-source-collection-0.0.42/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.43/macrometa_source_collection/client.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.42/pyproject.toml` & `macrometa-source-collection-0.0.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.42'
+version='0.0.43'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.42/setup.py` & `macrometa-source-collection-0.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.42',
+    'version': '0.0.43',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.42/PKG-INFO` & `macrometa-source-collection-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.42
+Version: 0.0.43
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

