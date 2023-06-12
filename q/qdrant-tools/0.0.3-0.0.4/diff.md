# Comparing `tmp/qdrant_tools-0.0.3.tar.gz` & `tmp/qdrant_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_tools-0.0.3.tar", max compression
+gzip compressed data, was "qdrant_tools-0.0.4.tar", max compression
```

## Comparing `qdrant_tools-0.0.3.tar` & `qdrant_tools-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-06-08 09:46:17.915415 qdrant_tools-0.0.3/LICENSE
--rw-r--r--   0        0        0    17500 2023-06-12 10:00:14.636807 qdrant_tools-0.0.3/README.md
--rw-r--r--   0        0        0      391 2023-06-12 09:56:55.156983 qdrant_tools-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-08 09:43:33.573836 qdrant_tools-0.0.3/qdrant_tools/README.md
--rw-r--r--   0        0        0        0 2023-06-08 09:43:33.573544 qdrant_tools-0.0.3/qdrant_tools/__init__.py
--rw-r--r--   0        0        0       43 2023-06-08 09:43:33.573347 qdrant_tools-0.0.3/qdrant_tools/requirements.txt
--rw-r--r--   0        0        0     5898 2023-06-12 09:55:24.866264 qdrant_tools-0.0.3/qdrant_tools/vectordb.py
--rw-r--r--   0        0        0    18097 1970-01-01 00:00:00.000000 qdrant_tools-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-08 09:46:17.915415 qdrant_tools-0.0.4/LICENSE
+-rw-r--r--   0        0        0    17509 2023-06-12 11:21:49.653123 qdrant_tools-0.0.4/README.md
+-rw-r--r--   0        0        0      519 2023-06-12 11:27:52.821050 qdrant_tools-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-08 09:43:33.573836 qdrant_tools-0.0.4/qdrant_tools/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 09:43:33.573544 qdrant_tools-0.0.4/qdrant_tools/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-08 09:43:33.573347 qdrant_tools-0.0.4/qdrant_tools/requirements.txt
+-rw-r--r--   0        0        0     6606 2023-06-12 11:14:30.939886 qdrant_tools-0.0.4/qdrant_tools/vectordb.py
+-rw-r--r--   0        0        0    18106 1970-01-01 00:00:00.000000 qdrant_tools-0.0.4/PKG-INFO
```

### Comparing `qdrant_tools-0.0.3/LICENSE` & `qdrant_tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_tools-0.0.3/README.md` & `qdrant_tools-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 
 ```python
 pip install qdrant-tools
 ```
 
 ## Usage
 
-```
-from qdrant_tools.vectordb import PineconeExport, QdrantImport, QdrantMode
+```python
+from qdrant_tools.vectordb import PineconeExport, QdrantImport
 
 index_name = "hindi-search"  # Existing Pinecone index name
 
 # Init Pinecone
 pinecone_export = PineconeExport(index_name=index_name)
-print(pinecone_export.index.describe_index_stats())
-source_index = pinecone_export.index
 
-# Fetch all vector ids from Pinecone
 vector_ids = ["1", "2", "3", "4", "5"]  # Example vector ids
+points_information = pinecone_export.fetch_vectors(vector_ids)
+
+print(points_information["ids"], points_information["index_dimension"])
 
 # Init Qdrant
-qdrant = QdrantImport(mode=QdrantMode.local, source_index=source_index)
+qdrant = QdrantImport(**points_information)
 qdrant.create_collection()
-qdrant.upsert_vectors(vector_ids)
-
+qdrant.upsert_vectors()
 
-qdrant.qdrant_client.search(
+# Trying it out!
+response = qdrant.qdrant_client.search(
     collection_name=index_name,
     query_vector= # vector to search of same dimension as other vectors,
 )
 
+print(response)
 ```
 
 ## Introduction
 
 Are you considering a transition from Pinecone to Qdrant? If so, this article will guide you through the process, outlining the similarities and differences between the two systems, and providing a step-by-step migration plan.
 
 ### Understanding the Terminology
```

### Comparing `qdrant_tools-0.0.3/PKG-INFO` & `qdrant_tools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: MIT
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,38 +22,39 @@
 
 ```python
 pip install qdrant-tools
 ```
 
 ## Usage
 
-```
-from qdrant_tools.vectordb import PineconeExport, QdrantImport, QdrantMode
+```python
+from qdrant_tools.vectordb import PineconeExport, QdrantImport
 
 index_name = "hindi-search"  # Existing Pinecone index name
 
 # Init Pinecone
 pinecone_export = PineconeExport(index_name=index_name)
-print(pinecone_export.index.describe_index_stats())
-source_index = pinecone_export.index
 
-# Fetch all vector ids from Pinecone
 vector_ids = ["1", "2", "3", "4", "5"]  # Example vector ids
+points_information = pinecone_export.fetch_vectors(vector_ids)
+
+print(points_information["ids"], points_information["index_dimension"])
 
 # Init Qdrant
-qdrant = QdrantImport(mode=QdrantMode.local, source_index=source_index)
+qdrant = QdrantImport(**points_information)
 qdrant.create_collection()
-qdrant.upsert_vectors(vector_ids)
-
+qdrant.upsert_vectors()
 
-qdrant.qdrant_client.search(
+# Trying it out!
+response = qdrant.qdrant_client.search(
     collection_name=index_name,
     query_vector= # vector to search of same dimension as other vectors,
 )
 
+print(response)
 ```
 
 ## Introduction
 
 Are you considering a transition from Pinecone to Qdrant? If so, this article will guide you through the process, outlining the similarities and differences between the two systems, and providing a step-by-step migration plan.
 
 ### Understanding the Terminology
```

