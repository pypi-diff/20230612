# Comparing `tmp/fabric_fss_utils-1.5.0.tar.gz` & `tmp/fabric_fss_utils-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_fss_utils-1.5.0.tar", last modified: Mon Jun 12 14:59:31 2023, max compression
+gzip compressed data, was "fabric_fss_utils-1.5.0rc1.tar", last modified: Wed May 10 22:00:48 2023, max compression
```

## Comparing `fabric_fss_utils-1.5.0.tar` & `fabric_fss_utils-1.5.0rc1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0        0 2023-06-12 14:58:25.229249 fabric_fss_utils-1.5.0/AUTHORS
--rw-r--r--   0        0        0     1071 2023-06-12 14:58:25.229407 fabric_fss_utils-1.5.0/LICENSE
--rw-r--r--   0        0        0      851 2023-06-12 14:58:25.229523 fabric_fss_utils-1.5.0/README.md
--rw-r--r--   0        0        0      118 2023-06-12 14:59:02.569664 fabric_fss_utils-1.5.0/fss_utils/__init__.py
--rw-r--r--   0        0        0     3290 2023-06-12 14:58:25.229793 fabric_fss_utils-1.5.0/fss_utils/http_errors.py
--rw-r--r--   0        0        0     8288 2023-06-12 14:58:25.230056 fabric_fss_utils-1.5.0/fss_utils/jwt_manager.py
--rw-r--r--   0        0        0     3678 2023-06-12 14:58:25.230296 fabric_fss_utils-1.5.0/fss_utils/jwt_validate.py
--rw-r--r--   0        0        0     8429 2023-06-12 14:58:25.230463 fabric_fss_utils-1.5.0/fss_utils/sshkey.py
--rw-r--r--   0        0        0     5090 2023-06-12 14:58:25.230609 fabric_fss_utils-1.5.0/fss_utils/vouch_encoder.py
--rw-r--r--   0        0        0      776 2023-06-12 14:58:25.230721 fabric_fss_utils-1.5.0/pyproject.toml
--rw-r--r--   0        0        0       57 2023-06-12 14:58:25.230816 fabric_fss_utils-1.5.0/requirements.txt
--rw-r--r--   0        0        0        2 2023-06-12 14:58:25.230986 fabric_fss_utils-1.5.0/test/__init__.py
--rw-r--r--   0        0        0     3272 2023-06-12 14:58:25.231155 fabric_fss_utils-1.5.0/test/data/privkey.pem
--rw-r--r--   0        0        0      800 2023-06-12 14:58:25.231274 fabric_fss_utils-1.5.0/test/data/pubkey.pem
--rw-r--r--   0        0        0     7811 2023-06-12 14:58:25.231511 fabric_fss_utils-1.5.0/test/jwt_decode_test.py
--rw-r--r--   0        0        0     4583 2023-06-12 14:58:25.231763 fabric_fss_utils-1.5.0/test/jwt_manager_test.py
--rw-r--r--   0        0        0     6964 2023-06-12 14:58:25.231899 fabric_fss_utils-1.5.0/test/ssh_test.py
--rw-r--r--   0        0        0     9404 2023-06-12 14:58:25.232050 fabric_fss_utils-1.5.0/test/vouch_encoder_test.py
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 fabric_fss_utils-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-12-11 22:04:09.114297 fabric_fss_utils-1.5.0rc1/AUTHORS
+-rw-r--r--   0        0        0     1071 2020-12-11 22:04:42.289179 fabric_fss_utils-1.5.0rc1/LICENSE
+-rw-r--r--   0        0        0       59 2022-06-08 19:53:51.796455 fabric_fss_utils-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0        0        0      851 2021-01-13 21:58:26.743332 fabric_fss_utils-1.5.0rc1/README.md
+-rw-r--r--   0        0        0      121 2023-05-10 22:00:20.624356 fabric_fss_utils-1.5.0rc1/fss_utils/__init__.py
+-rw-r--r--   0        0        0     3290 2021-05-05 20:19:27.853971 fabric_fss_utils-1.5.0rc1/fss_utils/http_errors.py
+-rw-r--r--   0        0        0     8288 2023-05-10 21:50:19.899928 fabric_fss_utils-1.5.0rc1/fss_utils/jwt_manager.py
+-rw-r--r--   0        0        0     3678 2021-01-13 21:34:16.970111 fabric_fss_utils-1.5.0rc1/fss_utils/jwt_validate.py
+-rw-r--r--   0        0        0     8429 2022-06-08 19:53:51.802302 fabric_fss_utils-1.5.0rc1/fss_utils/sshkey.py
+-rw-r--r--   0        0        0     5090 2021-01-13 21:34:16.970600 fabric_fss_utils-1.5.0rc1/fss_utils/vouch_encoder.py
+-rw-r--r--   0        0        0      776 2023-05-10 21:56:38.451610 fabric_fss_utils-1.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-05-10 21:58:14.762074 fabric_fss_utils-1.5.0rc1/requirements.txt
+-rw-r--r--   0        0        0      826 2022-06-08 17:21:57.693221 fabric_fss_utils-1.5.0rc1/setup.py
+-rw-r--r--   0        0        0        2 2020-12-13 06:15:01.062052 fabric_fss_utils-1.5.0rc1/test/__init__.py
+-rw-r--r--   0        0        0     3272 2021-01-13 21:34:16.972211 fabric_fss_utils-1.5.0rc1/test/data/privkey.pem
+-rw-r--r--   0        0        0      800 2021-01-13 21:34:16.972648 fabric_fss_utils-1.5.0rc1/test/data/pubkey.pem
+-rw-r--r--   0        0        0     7811 2023-05-10 21:39:23.714894 fabric_fss_utils-1.5.0rc1/test/jwt_decode_test.py
+-rw-r--r--   0        0        0     4583 2023-05-10 21:33:57.843225 fabric_fss_utils-1.5.0rc1/test/jwt_manager_test.py
+-rw-r--r--   0        0        0     6964 2022-01-09 16:48:43.909205 fabric_fss_utils-1.5.0rc1/test/ssh_test.py
+-rw-r--r--   0        0        0     9404 2021-01-13 21:34:16.974329 fabric_fss_utils-1.5.0rc1/test/vouch_encoder_test.py
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 fabric_fss_utils-1.5.0rc1/PKG-INFO
```

### Comparing `fabric_fss_utils-1.5.0/LICENSE` & `fabric_fss_utils-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/README.md` & `fabric_fss_utils-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/fss_utils/http_errors.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/http_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/fss_utils/jwt_manager.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/jwt_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/fss_utils/jwt_validate.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/jwt_validate.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/fss_utils/sshkey.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/sshkey.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/fss_utils/vouch_encoder.py` & `fabric_fss_utils-1.5.0rc1/fss_utils/vouch_encoder.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/pyproject.toml` & `fabric_fss_utils-1.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/test/data/privkey.pem` & `fabric_fss_utils-1.5.0rc1/test/data/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/test/data/pubkey.pem` & `fabric_fss_utils-1.5.0rc1/test/data/pubkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/test/jwt_decode_test.py` & `fabric_fss_utils-1.5.0rc1/test/jwt_decode_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/test/jwt_manager_test.py` & `fabric_fss_utils-1.5.0rc1/test/jwt_manager_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/test/ssh_test.py` & `fabric_fss_utils-1.5.0rc1/test/ssh_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/test/vouch_encoder_test.py` & `fabric_fss_utils-1.5.0rc1/test/vouch_encoder_test.py`

 * *Files identical despite different names*

### Comparing `fabric_fss_utils-1.5.0/PKG-INFO` & `fabric_fss_utils-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_fss_utils
-Version: 1.5.0
+Version: 1.5.0rc1
 Summary: FABRIC System Service Utilities - JWT and SSH key handling
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

