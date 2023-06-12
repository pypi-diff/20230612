# Comparing `tmp/acapela_downloader_py-0.0.8.tar.gz` & `tmp/acapela_downloader_py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.0.8.tar", last modified: Mon Jun 12 21:10:02 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.0.9.tar", last modified: Mon Jun 12 21:53:35 2023, max compression
```

## Comparing `acapela_downloader_py-0.0.8.tar` & `acapela_downloader_py-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:10:02.318991 acapela_downloader_py-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 21:09:51.000000 acapela_downloader_py-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 21:10:02.318991 acapela_downloader_py-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 21:09:51.000000 acapela_downloader_py-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 21:09:51.000000 acapela_downloader_py-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:10:02.322991 acapela_downloader_py-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:10:02.318991 acapela_downloader_py-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 21:09:51.000000 acapela_downloader_py-0.0.8/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:10:02.318991 acapela_downloader_py-0.0.8/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 21:10:02.000000 acapela_downloader_py-0.0.8/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 21:10:02.000000 acapela_downloader_py-0.0.8/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:10:02.000000 acapela_downloader_py-0.0.8/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 21:10:02.000000 acapela_downloader_py-0.0.8/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-12 21:09:51.000000 acapela_downloader_py-0.0.8/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:53:35.085016 acapela_downloader_py-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:53:35.089016 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 21:53:35.000000 acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-12 21:53:25.000000 acapela_downloader_py-0.0.9/src/utils.py
```

### Comparing `acapela_downloader_py-0.0.8/LICENSE` & `acapela_downloader_py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.0.8/PKG-INFO` & `acapela_downloader_py-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela_downloader_py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.0.8/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.0.9/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acapela-downloader-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.0.8/src/utils.py` & `acapela_downloader_py-0.0.9/src/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import random
 import string
 import re
+from datetime import time
+
 from requests import post
 
 NONCE_ENDPOINT = "https://acapelavoices.acapela-group.com/index/getnonce/"
 SYNTHESIZER_ENDPOINT = "https://www.acapela-group.com:8443/Services/Synthesizer"
 cached_nonce = ""
 cached_email = ""
 
@@ -37,13 +39,13 @@
             headers = {'Content-type': 'application/x-www-form-urlencoded',
                        'Content-Length': str(len(synthesizer_request_bytes))}
             synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
             split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
             finished = True
             return split_res[1]
         except:
-            print("generating new nonce")
-            update_nonce_token()
+            print("one minute delay...")
+            time.sleep(60)
     return ""
```

