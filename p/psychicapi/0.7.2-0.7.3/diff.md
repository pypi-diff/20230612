# Comparing `tmp/psychicapi-0.7.2.tar.gz` & `tmp/psychicapi-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychicapi-0.7.2.tar", last modified: Sat Jun 10 02:01:32 2023, max compression
+gzip compressed data, was "psychicapi-0.7.3.tar", last modified: Sun Jun 11 22:39:11 2023, max compression
```

## Comparing `psychicapi-0.7.2.tar` & `psychicapi-0.7.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-10 02:01:32.073785 psychicapi-0.7.2/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1842 2023-06-10 02:01:32.073650 psychicapi-0.7.2/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)     1575 2023-06-07 19:40:18.000000 psychicapi-0.7.2/README.md
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-10 02:01:32.072607 psychicapi-0.7.2/psychicapi/
--rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.7.2/psychicapi/__init__.py
--rw-r--r--   0 jasonfan   (501) staff       (20)     2940 2023-06-10 02:01:10.000000 psychicapi-0.7.2/psychicapi/psychic.py
-drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-10 02:01:32.073421 psychicapi-0.7.2/psychicapi.egg-info/
--rw-r--r--   0 jasonfan   (501) staff       (20)     1842 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/requires.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-06-10 02:01:32.000000 psychicapi-0.7.2/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-06-10 02:01:32.073831 psychicapi-0.7.2/setup.cfg
--rw-r--r--   0 jasonfan   (501) staff       (20)      666 2023-06-10 02:01:27.000000 psychicapi-0.7.2/setup.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-11 22:39:11.520756 psychicapi-0.7.3/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1842 2023-06-11 22:39:11.520627 psychicapi-0.7.3/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1575 2023-06-07 19:40:18.000000 psychicapi-0.7.3/README.md
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-11 22:39:11.519648 psychicapi-0.7.3/psychicapi/
+-rw-r--r--   0 jasonfan   (501) staff       (20)       41 2023-05-19 18:59:00.000000 psychicapi-0.7.3/psychicapi/__init__.py
+-rw-r--r--   0 jasonfan   (501) staff       (20)     2924 2023-06-11 22:38:00.000000 psychicapi-0.7.3/psychicapi/psychic.py
+drwxr-xr-x   0 jasonfan   (501) staff       (20)        0 2023-06-11 22:39:11.520443 psychicapi-0.7.3/psychicapi.egg-info/
+-rw-r--r--   0 jasonfan   (501) staff       (20)     1842 2023-06-11 22:39:11.000000 psychicapi-0.7.3/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 jasonfan   (501) staff       (20)      232 2023-06-11 22:39:11.000000 psychicapi-0.7.3/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        1 2023-06-11 22:39:11.000000 psychicapi-0.7.3/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)        9 2023-06-11 22:39:11.000000 psychicapi-0.7.3/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       11 2023-06-11 22:39:11.000000 psychicapi-0.7.3/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 jasonfan   (501) staff       (20)       38 2023-06-11 22:39:11.520792 psychicapi-0.7.3/setup.cfg
+-rw-r--r--   0 jasonfan   (501) staff       (20)      666 2023-06-11 22:38:57.000000 psychicapi-0.7.3/setup.py
```

### Comparing `psychicapi-0.7.2/PKG-INFO` & `psychicapi-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.2
+Version: 0.7.3
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.7.2/README.md` & `psychicapi-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `psychicapi-0.7.2/psychicapi/psychic.py` & `psychicapi-0.7.3/psychicapi/psychic.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     slack = "slack"
 
 class Psychic:
     def __init__(self, secret_key: str):
         self.api_url = "https://api.psychic.dev/"
         self.secret_key = secret_key
 
-    def get_documents(self, *, account_id: str, connector_id: Optional[ConnectorId] = None, pre_chunked: Optional[bool] = False, min_chunk_size: Optional[int] = None, max_chunk_size: Optional[int] = None):
+    def get_documents(self, *, account_id: str, connector_id: Optional[ConnectorId] = None, chunked: Optional[bool] = False, min_chunk_size: Optional[int] = None, max_chunk_size: Optional[int] = None):
         body = {
             "account_id": account_id
         }
         if connector_id is not None:
             body["connector_id"] = connector_id.value
-        if pre_chunked is not None:
-            body["pre_chunked"] = pre_chunked
+        if chunked is not None:
+            body["chunked"] = chunked
         if min_chunk_size is not None:
             body["min_chunk_size"] = min_chunk_size
         if max_chunk_size is not None:
             body["max_chunk_size"] = max_chunk_size
         response = requests.post(
             self.api_url + "get-documents",
             json=body,
```

### Comparing `psychicapi-0.7.2/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.7.3/psychicapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.2
+Version: 0.7.3
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 Description-Content-Type: text/markdown
 
 # Psychic
```

### Comparing `psychicapi-0.7.2/setup.py` & `psychicapi-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.7.2',
+    version='0.7.3',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

