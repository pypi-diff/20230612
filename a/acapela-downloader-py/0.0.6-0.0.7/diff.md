# Comparing `tmp/acapela_downloader_py-0.0.6.tar.gz` & `tmp/acapela_downloader_py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.0.6.tar", last modified: Thu Jun  8 15:01:04 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.0.7.tar", last modified: Mon Jun 12 20:29:03 2023, max compression
```

## Comparing `acapela_downloader_py-0.0.6.tar` & `acapela_downloader_py-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:01:04.791193 acapela_downloader_py-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 15:00:51.000000 acapela_downloader_py-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 15:01:04.791193 acapela_downloader_py-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 15:00:51.000000 acapela_downloader_py-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 15:00:51.000000 acapela_downloader_py-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:01:04.791193 acapela_downloader_py-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:01:04.791193 acapela_downloader_py-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 15:00:51.000000 acapela_downloader_py-0.0.6/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:01:04.791193 acapela_downloader_py-0.0.6/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-08 15:01:04.000000 acapela_downloader_py-0.0.6/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 15:01:04.000000 acapela_downloader_py-0.0.6/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:01:04.000000 acapela_downloader_py-0.0.6/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 15:01:04.000000 acapela_downloader_py-0.0.6/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-08 15:00:51.000000 acapela_downloader_py-0.0.6/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:29:03.011676 acapela_downloader_py-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 20:28:44.000000 acapela_downloader_py-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 20:29:03.011676 acapela_downloader_py-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-12 20:28:44.000000 acapela_downloader_py-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 20:28:44.000000 acapela_downloader_py-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:29:03.011676 acapela_downloader_py-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:29:03.011676 acapela_downloader_py-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 20:28:44.000000 acapela_downloader_py-0.0.7/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:29:03.011676 acapela_downloader_py-0.0.7/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 20:29:03.000000 acapela_downloader_py-0.0.7/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-12 20:29:03.000000 acapela_downloader_py-0.0.7/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:29:03.000000 acapela_downloader_py-0.0.7/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 20:29:03.000000 acapela_downloader_py-0.0.7/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-12 20:28:44.000000 acapela_downloader_py-0.0.7/src/utils.py
```

### Comparing `acapela_downloader_py-0.0.6/LICENSE` & `acapela_downloader_py-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.0.6/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.0.7/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: acapela-downloader-py
-Version: 0.0.6
+Version: 0.0.7
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
+Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Acapela Downloader but in Python
 Translated over to Python from C#: https://github.com/weespin/WillFromAfarDownloader
 
 # How to use
-It's pretty damn easy, just import the generate_audio function from the package and fill out the necessary arguments.
+
+First download the pip package.
+
+```
+pip install acapela-downloader-py
+```
+
+Then use the 'generate_audio' function from the 'acapela' library
 
 ``` python
 from acapela import generate_audio
 generate_audio("Great Test", "enu_willhappy_22k_ns.bvcu", "output.mp3")
 ```
 
 ## Other Stuff
```

### Comparing `acapela_downloader_py-0.0.6/src/utils.py` & `acapela_downloader_py-0.0.7/src/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,25 @@
         cached_nonce = nonce_response.json()["nonce"]
         cached_email = fake_email
 
 
 def get_sound_link(text, voice_id):
     if cached_email == "" or cached_nonce == "":
         update_nonce_token()
-    synthesizer_request_string = f"req_voice={voice_id}&cl_pwd=&cl_vers=1-30&req_echo=ON&cl_login=AcapelaGroup&req_comment=%7B%22nonce%22%3A%22{cached_nonce}%22%2C%22user%22%3A%22{cached_email}%22%7D&req_text={text}&cl_env=ACAPELA_VOICES&prot_vers=2&cl_app=AcapelaGroup_WebDemo_Android"
-    synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
-    headers = {'Content-type': 'application/x-www-form-urlencoded', 'Content-Length': str(len(synthesizer_request_bytes))}
-    synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
-    split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
-    return split_res[1]
+    finished = False
+    while not finished:
+        try:
+            synthesizer_request_string = f"req_voice={voice_id}&cl_pwd=&cl_vers=1-30&req_echo=ON&cl_login=AcapelaGroup&req_comment=%7B%22nonce%22%3A%22{cached_nonce}%22%2C%22user%22%3A%22{cached_email}%22%7D&req_text={text}&cl_env=ACAPELA_VOICES&prot_vers=2&cl_app=AcapelaGroup_WebDemo_Android"
+            synthesizer_request_bytes = bytes(synthesizer_request_string, 'utf-8')
+            headers = {'Content-type': 'application/x-www-form-urlencoded',
+                       'Content-Length': str(len(synthesizer_request_bytes))}
+            synthesizer_request = post(SYNTHESIZER_ENDPOINT, headers=headers, data=synthesizer_request_string)
+            split_res = re.split('&snd_url=|&snd_size', str(synthesizer_request.content))
+            finished = True
+            return split_res[1]
+        except:
+            print("generating new nonce")
+            update_nonce_token()
+    return ""
+
```

