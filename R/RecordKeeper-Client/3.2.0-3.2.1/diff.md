# Comparing `tmp/RecordKeeper_Client-3.2.0.tar.gz` & `tmp/RecordKeeper_Client-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RecordKeeper_Client-3.2.0.tar", last modified: Wed Jun  7 14:01:01 2023, max compression
+gzip compressed data, was "RecordKeeper_Client-3.2.1.tar", last modified: Mon Jun 12 12:29:32 2023, max compression
```

## Comparing `RecordKeeper_Client-3.2.0.tar` & `RecordKeeper_Client-3.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/
--rw-r--r--   0 hubert    (1001) hubert    (1001)    35149 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.2.0/LICENSE
--rw-r--r--   0 hubert    (1001) hubert    (1001)       16 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.2.0/MANIFEST.in
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6500 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/PKG-INFO
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4545 2023-06-07 14:00:19.000000 RecordKeeper_Client-3.2.0/README.md
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.375995 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6500 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/PKG-INFO
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      434 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/SOURCES.txt
--rw-rw-r--   0 hubert    (1001) hubert    (1001)        1 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/dependency_links.txt
--rw-rw-r--   0 hubert    (1001) hubert    (1001)        9 2023-06-07 14:01:01.000000 RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/top_level.txt
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/rkclient/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      855 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/__init__.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     3806 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/admin.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)       97 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.2.0/rkclient/auth.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4439 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/client.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     3264 2023-06-07 12:22:19.000000 RecordKeeper_Client-3.2.0/rkclient/entities.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     2294 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.2.0/rkclient/factory.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)    12049 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/query.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4166 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/request.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     4770 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/rkclient/serialization.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)       38 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/setup.cfg
--rw-rw-r--   0 hubert    (1001) hubert    (1001)      894 2023-03-15 09:31:37.000000 RecordKeeper_Client-3.2.0/setup.py
-drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-07 14:01:01.379995 RecordKeeper_Client-3.2.0/test/
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     2665 2023-06-07 13:20:51.000000 RecordKeeper_Client-3.2.0/test/test_api.py
--rw-rw-r--   0 hubert    (1001) hubert    (1001)     6627 2023-06-07 12:22:19.000000 RecordKeeper_Client-3.2.0/test/test_serialization.py
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-12 12:29:32.506203 RecordKeeper_Client-3.2.1/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    35149 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.2.1/LICENSE
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       16 2021-09-21 18:37:33.000000 RecordKeeper_Client-3.2.1/MANIFEST.in
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6594 2023-06-12 12:29:32.506203 RecordKeeper_Client-3.2.1/PKG-INFO
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4615 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/README.md
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-12 12:29:32.506203 RecordKeeper_Client-3.2.1/RecordKeeper_Client.egg-info/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6594 2023-06-12 12:29:32.000000 RecordKeeper_Client-3.2.1/RecordKeeper_Client.egg-info/PKG-INFO
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      434 2023-06-12 12:29:32.000000 RecordKeeper_Client-3.2.1/RecordKeeper_Client.egg-info/SOURCES.txt
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)        1 2023-06-12 12:29:32.000000 RecordKeeper_Client-3.2.1/RecordKeeper_Client.egg-info/dependency_links.txt
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)        9 2023-06-12 12:29:32.000000 RecordKeeper_Client-3.2.1/RecordKeeper_Client.egg-info/top_level.txt
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-12 12:29:32.506203 RecordKeeper_Client-3.2.1/rkclient/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      855 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/rkclient/__init__.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     3806 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/rkclient/admin.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)       97 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.2.1/rkclient/auth.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4439 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/rkclient/client.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     3264 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/rkclient/entities.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     2294 2023-02-13 20:07:56.000000 RecordKeeper_Client-3.2.1/rkclient/factory.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)    12049 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/rkclient/query.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4166 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/rkclient/request.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     4770 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/rkclient/serialization.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)       38 2023-06-12 12:29:32.506203 RecordKeeper_Client-3.2.1/setup.cfg
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)      894 2023-03-15 09:31:37.000000 RecordKeeper_Client-3.2.1/setup.py
+drwxrwxr-x   0 hubert    (1001) hubert    (1001)        0 2023-06-12 12:29:32.506203 RecordKeeper_Client-3.2.1/test/
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     2665 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/test/test_api.py
+-rw-rw-r--   0 hubert    (1001) hubert    (1001)     6627 2023-06-12 12:28:29.000000 RecordKeeper_Client-3.2.1/test/test_serialization.py
```

### Comparing `RecordKeeper_Client-3.2.0/LICENSE` & `RecordKeeper_Client-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/PKG-INFO` & `RecordKeeper_Client-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecordKeeper_Client
-Version: 3.2.0
+Version: 3.2.1
 Summary: Client library for accessing Record Keepers Receiver
 Home-page: UNKNOWN
 Author: ERST
 Author-email: noreply@example.ecom
 License: GPLv3+
 Description: 
         # Context
@@ -100,14 +100,17 @@
         >>> for pem in pems:
         >>>   print(pem)
         ```
         ## Changelog
         
         ### Unreleased
         
+        ### [3.2.1] - 2023-06-12
+        - Version updated to match other components
+        
         ### [3.2.0] - 2023-06-07
         - Moved "getter" functions to new class RKQuery. RKAdmin is left with truly low-level functions.
         - Added helper function RKQuery.get_artifact_latest().
         
         ## [3.1.0] - 2023-04-06 and 2023-05-17
         - Improved error logging, by creating less irrelevant logs. 
         - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
```

### Comparing `RecordKeeper_Client-3.2.0/README.md` & `RecordKeeper_Client-3.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 >>> for pem in pems:
 >>>   print(pem)
 ```
 ## Changelog
 
 ### Unreleased
 
+### [3.2.1] - 2023-06-12
+- Version updated to match other components
+
 ### [3.2.0] - 2023-06-07
 - Moved "getter" functions to new class RKQuery. RKAdmin is left with truly low-level functions.
 - Added helper function RKQuery.get_artifact_latest().
 
 ## [3.1.0] - 2023-04-06 and 2023-05-17
 - Improved error logging, by creating less irrelevant logs. 
 - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
```

### Comparing `RecordKeeper_Client-3.2.0/RecordKeeper_Client.egg-info/PKG-INFO` & `RecordKeeper_Client-3.2.1/RecordKeeper_Client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecordKeeper-Client
-Version: 3.2.0
+Version: 3.2.1
 Summary: Client library for accessing Record Keepers Receiver
 Home-page: UNKNOWN
 Author: ERST
 Author-email: noreply@example.ecom
 License: GPLv3+
 Description: 
         # Context
@@ -100,14 +100,17 @@
         >>> for pem in pems:
         >>>   print(pem)
         ```
         ## Changelog
         
         ### Unreleased
         
+        ### [3.2.1] - 2023-06-12
+        - Version updated to match other components
+        
         ### [3.2.0] - 2023-06-07
         - Moved "getter" functions to new class RKQuery. RKAdmin is left with truly low-level functions.
         - Added helper function RKQuery.get_artifact_latest().
         
         ## [3.1.0] - 2023-04-06 and 2023-05-17
         - Improved error logging, by creating less irrelevant logs. 
         - Add default User-Agent to requests to be equal to `recordkeeper-client-{version}`.
```

### Comparing `RecordKeeper_Client-3.2.0/rkclient/__init__.py` & `RecordKeeper_Client-3.2.1/rkclient/__init__.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/rkclient/admin.py` & `RecordKeeper_Client-3.2.1/rkclient/admin.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/rkclient/client.py` & `RecordKeeper_Client-3.2.1/rkclient/client.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/rkclient/entities.py` & `RecordKeeper_Client-3.2.1/rkclient/entities.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/rkclient/factory.py` & `RecordKeeper_Client-3.2.1/rkclient/factory.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/rkclient/query.py` & `RecordKeeper_Client-3.2.1/rkclient/query.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/rkclient/request.py` & `RecordKeeper_Client-3.2.1/rkclient/request.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/rkclient/serialization.py` & `RecordKeeper_Client-3.2.1/rkclient/serialization.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/setup.py` & `RecordKeeper_Client-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/test/test_api.py` & `RecordKeeper_Client-3.2.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `RecordKeeper_Client-3.2.0/test/test_serialization.py` & `RecordKeeper_Client-3.2.1/test/test_serialization.py`

 * *Files identical despite different names*

