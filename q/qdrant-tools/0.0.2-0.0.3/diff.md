# Comparing `tmp/qdrant_tools-0.0.2.tar.gz` & `tmp/qdrant_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_tools-0.0.2.tar", max compression
+gzip compressed data, was "qdrant_tools-0.0.3.tar", max compression
```

## Comparing `qdrant_tools-0.0.2.tar` & `qdrant_tools-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-06-08 09:46:17.915415 qdrant_tools-0.0.2/LICENSE
--rw-r--r--   0        0        0    17801 2023-06-09 06:38:08.001002 qdrant_tools-0.0.2/README.md
--rw-r--r--   0        0        0      391 2023-06-09 06:38:55.494069 qdrant_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      110 2023-06-08 09:43:33.573836 qdrant_tools-0.0.2/qdrant_tools/README.md
--rw-r--r--   0        0        0        0 2023-06-08 09:43:33.573544 qdrant_tools-0.0.2/qdrant_tools/__init__.py
--rw-r--r--   0        0        0       43 2023-06-08 09:43:33.573347 qdrant_tools-0.0.2/qdrant_tools/requirements.txt
--rw-r--r--   0        0        0     4041 2023-06-08 13:27:04.352078 qdrant_tools-0.0.2/qdrant_tools/vectordb.py
--rw-r--r--   0        0        0    18398 1970-01-01 00:00:00.000000 qdrant_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-08 09:46:17.915415 qdrant_tools-0.0.3/LICENSE
+-rw-r--r--   0        0        0    17500 2023-06-12 10:00:14.636807 qdrant_tools-0.0.3/README.md
+-rw-r--r--   0        0        0      391 2023-06-12 09:56:55.156983 qdrant_tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-08 09:43:33.573836 qdrant_tools-0.0.3/qdrant_tools/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 09:43:33.573544 qdrant_tools-0.0.3/qdrant_tools/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-08 09:43:33.573347 qdrant_tools-0.0.3/qdrant_tools/requirements.txt
+-rw-r--r--   0        0        0     5898 2023-06-12 09:55:24.866264 qdrant_tools-0.0.3/qdrant_tools/vectordb.py
+-rw-r--r--   0        0        0    18097 1970-01-01 00:00:00.000000 qdrant_tools-0.0.3/PKG-INFO
```

### Comparing `qdrant_tools-0.0.2/LICENSE` & `qdrant_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_tools-0.0.2/README.md` & `qdrant_tools-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,42 +6,36 @@
 pip install qdrant-tools
 ```
 
 ## Usage
 
 ```
 from qdrant_tools.vectordb import PineconeExport, QdrantImport, QdrantMode
-index_name = "hindi-search" # Existing Pinecone index name
 
-# Init Pinecone
+index_name = "hindi-search"  # Existing Pinecone index name
 
+# Init Pinecone
 pinecone_export = PineconeExport(index_name=index_name)
 print(pinecone_export.index.describe_index_stats())
 source_index = pinecone_export.index
 
 # Fetch all vector ids from Pinecone
-
-vector_ids = ["1", "2", "3", "4", "5"] # Example vector ids, list of strings -- this is the main input for the replication
-points = pinecone_export.fetch_vectors(vector_ids) # Fetch vectors from Pinecone
+vector_ids = ["1", "2", "3", "4", "5"]  # Example vector ids
 
 # Init Qdrant
+qdrant = QdrantImport(mode=QdrantMode.local, source_index=source_index)
+qdrant.create_collection()
+qdrant.upsert_vectors(vector_ids)
 
-vector_dimension = source_index.describe_index_stats()[
-"dimension"
-] # Get dimension from existing index
-qdrant = QdrantImport(mode=QdrantMode.local)
-qdrant.create_collection(index_name, vector_dimension)
-qdrant.upsert_vectors(index_name, vector_ids, source_index) # source_index is a pinecone index object
 
-
-# Testing if it works!
 qdrant.qdrant_client.search(
     collection_name=index_name,
-    query_vector= # query_vector
+    query_vector= # vector to search of same dimension as other vectors,
 )
+
 ```
 
 ## Introduction
 
 Are you considering a transition from Pinecone to Qdrant? If so, this article will guide you through the process, outlining the similarities and differences between the two systems, and providing a step-by-step migration plan.
 
 ### Understanding the Terminology
```

### Comparing `qdrant_tools-0.0.2/PKG-INFO` & `qdrant_tools-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,42 +24,36 @@
 pip install qdrant-tools
 ```
 
 ## Usage
 
 ```
 from qdrant_tools.vectordb import PineconeExport, QdrantImport, QdrantMode
-index_name = "hindi-search" # Existing Pinecone index name
 
-# Init Pinecone
+index_name = "hindi-search"  # Existing Pinecone index name
 
+# Init Pinecone
 pinecone_export = PineconeExport(index_name=index_name)
 print(pinecone_export.index.describe_index_stats())
 source_index = pinecone_export.index
 
 # Fetch all vector ids from Pinecone
-
-vector_ids = ["1", "2", "3", "4", "5"] # Example vector ids, list of strings -- this is the main input for the replication
-points = pinecone_export.fetch_vectors(vector_ids) # Fetch vectors from Pinecone
+vector_ids = ["1", "2", "3", "4", "5"]  # Example vector ids
 
 # Init Qdrant
+qdrant = QdrantImport(mode=QdrantMode.local, source_index=source_index)
+qdrant.create_collection()
+qdrant.upsert_vectors(vector_ids)
 
-vector_dimension = source_index.describe_index_stats()[
-"dimension"
-] # Get dimension from existing index
-qdrant = QdrantImport(mode=QdrantMode.local)
-qdrant.create_collection(index_name, vector_dimension)
-qdrant.upsert_vectors(index_name, vector_ids, source_index) # source_index is a pinecone index object
 
-
-# Testing if it works!
 qdrant.qdrant_client.search(
     collection_name=index_name,
-    query_vector= # query_vector
+    query_vector= # vector to search of same dimension as other vectors,
 )
+
 ```
 
 ## Introduction
 
 Are you considering a transition from Pinecone to Qdrant? If so, this article will guide you through the process, outlining the similarities and differences between the two systems, and providing a step-by-step migration plan.
 
 ### Understanding the Terminology
```

