# Comparing `tmp/pyneoncli-0.1.0a2.tar.gz` & `tmp/pyneoncli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneoncli-0.1.0a2.tar", max compression
+gzip compressed data, was "pyneoncli-0.1.1.tar", max compression
```

## Comparing `pyneoncli-0.1.0a2.tar` & `pyneoncli-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     8278 2023-06-09 09:31:15.780474 pyneoncli-0.1.0a2/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.1.0a2/pyneoncli/__init__.py
--rw-r--r--   0        0        0     6910 2023-06-10 11:23:53.263947 pyneoncli-0.1.0a2/pyneoncli/clicommands.py
--rw-r--r--   0        0        0     3038 2023-06-11 18:26:54.787575 pyneoncli-0.1.0a2/pyneoncli/clidispatcher.py
--rw-r--r--   0        0        0     3245 2023-06-09 18:11:47.236682 pyneoncli-0.1.0a2/pyneoncli/clilist.py
--rw-r--r--   0        0        0     5677 2023-06-07 20:06:42.981654 pyneoncli-0.1.0a2/pyneoncli/climain.py
--rw-r--r--   0        0        0     2886 2023-06-07 11:02:46.695750 pyneoncli-0.1.0a2/pyneoncli/colortext.py
--rw-r--r--   0        0        0     1080 2023-06-07 20:07:20.413137 pyneoncli-0.1.0a2/pyneoncli/configfile.py
--rw-r--r--   0        0        0        0 2023-06-06 17:23:56.004114 pyneoncli-0.1.0a2/pyneoncli/endpoint_template.json
--rw-r--r--   0        0        0        1 2023-06-11 16:34:26.267305 pyneoncli-0.1.0a2/pyneoncli/exceptions.py
--rw-r--r--   0        0        0     1478 2023-06-07 12:01:09.344156 pyneoncli-0.1.0a2/pyneoncli/msg.py
--rw-r--r--   0        0        0     2205 2023-06-10 10:34:02.048055 pyneoncli-0.1.0a2/pyneoncli/neon.py
--rw-r--r--   0        0        0     4445 2023-06-11 18:25:19.573798 pyneoncli-0.1.0a2/pyneoncli/neonapi.py
--rw-r--r--   0        0        0     1580 2023-06-11 16:34:26.268625 pyneoncli-0.1.0a2/pyneoncli/neonapiexceptions.py
--rw-r--r--   0        0        0     1237 2023-06-10 11:20:45.709200 pyneoncli-0.1.0a2/pyneoncli/neonliterals.py
--rw-r--r--   0        0        0     4558 2023-06-07 08:56:54.007032 pyneoncli-0.1.0a2/pyneoncli/printer.py
--rw-r--r--   0        0        0     7496 2023-06-11 16:34:26.266017 pyneoncli-0.1.0a2/pyneoncli/rawneonapi.py
--rw-r--r--   0        0        0     5235 2023-06-11 21:46:14.385802 pyneoncli-0.1.0a2/pyneoncli/requester.py
--rw-r--r--   0        0        0     1335 2023-06-11 17:05:54.225765 pyneoncli-0.1.0a2/pyneoncli/threadedcreate.py
--rw-r--r--   0        0        0     3557 2023-06-11 21:08:18.995480 pyneoncli-0.1.0a2/pyneoncli/threadedneonapi.py
--rw-r--r--   0        0        0       23 2023-06-11 22:02:57.017160 pyneoncli-0.1.0a2/pyneoncli/version.py
--rw-r--r--   0        0        0      703 2023-06-11 22:02:57.014809 pyneoncli-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     9092 1970-01-01 00:00:00.000000 pyneoncli-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8305 2023-06-11 22:32:51.277285 pyneoncli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.1.1/pyneoncli/__init__.py
+-rw-r--r--   0        0        0     6910 2023-06-10 11:23:53.263947 pyneoncli-0.1.1/pyneoncli/clicommands.py
+-rw-r--r--   0        0        0     3038 2023-06-11 18:26:54.787575 pyneoncli-0.1.1/pyneoncli/clidispatcher.py
+-rw-r--r--   0        0        0     3245 2023-06-09 18:11:47.236682 pyneoncli-0.1.1/pyneoncli/clilist.py
+-rw-r--r--   0        0        0     5677 2023-06-07 20:06:42.981654 pyneoncli-0.1.1/pyneoncli/climain.py
+-rw-r--r--   0        0        0     2886 2023-06-07 11:02:46.695750 pyneoncli-0.1.1/pyneoncli/colortext.py
+-rw-r--r--   0        0        0     1080 2023-06-07 20:07:20.413137 pyneoncli-0.1.1/pyneoncli/configfile.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:23:56.004114 pyneoncli-0.1.1/pyneoncli/endpoint_template.json
+-rw-r--r--   0        0        0        1 2023-06-11 16:34:26.267305 pyneoncli-0.1.1/pyneoncli/exceptions.py
+-rw-r--r--   0        0        0     1478 2023-06-07 12:01:09.344156 pyneoncli-0.1.1/pyneoncli/msg.py
+-rw-r--r--   0        0        0     2205 2023-06-10 10:34:02.048055 pyneoncli-0.1.1/pyneoncli/neon.py
+-rw-r--r--   0        0        0     4445 2023-06-11 18:25:19.573798 pyneoncli-0.1.1/pyneoncli/neonapi.py
+-rw-r--r--   0        0        0     1580 2023-06-11 16:34:26.268625 pyneoncli-0.1.1/pyneoncli/neonapiexceptions.py
+-rw-r--r--   0        0        0     1237 2023-06-10 11:20:45.709200 pyneoncli-0.1.1/pyneoncli/neonliterals.py
+-rw-r--r--   0        0        0     4558 2023-06-07 08:56:54.007032 pyneoncli-0.1.1/pyneoncli/printer.py
+-rw-r--r--   0        0        0     7496 2023-06-11 16:34:26.266017 pyneoncli-0.1.1/pyneoncli/rawneonapi.py
+-rw-r--r--   0        0        0     5235 2023-06-11 21:46:14.385802 pyneoncli-0.1.1/pyneoncli/requester.py
+-rw-r--r--   0        0        0     1335 2023-06-11 17:05:54.225765 pyneoncli-0.1.1/pyneoncli/threadedcreate.py
+-rw-r--r--   0        0        0     3557 2023-06-11 21:08:18.995480 pyneoncli-0.1.1/pyneoncli/threadedneonapi.py
+-rw-r--r--   0        0        0       21 2023-06-11 22:32:06.276352 pyneoncli-0.1.1/pyneoncli/version.py
+-rw-r--r--   0        0        0      701 2023-06-11 22:32:06.273455 pyneoncli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9117 1970-01-01 00:00:00.000000 pyneoncli-0.1.1/PKG-INFO
```

### Comparing `pyneoncli-0.1.0a2/LICENSE` & `pyneoncli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/README.md` & `pyneoncli-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 A python package and command line tool for interaction with the [Neon](https://neon.tech) Serverless Postgres [API](https://api-docs.neon.tech/reference/getting-started-with-neon-api).
 
 This is a work in progress and this version is incomplete. 
 
 This version only supports the Neon V2 API. 
 
-The program can read the NEON_API_KEY from the environment or it can he loaded from a .env field in the current working directory.
+The program can read the NEON_API_KEY from the environment or it can he loaded from a `neoncli.conf` in your home directory or
+the current working directory.
 
 ## Installation
 
 You can install the package from PyPi using pip:
 ```commandline
 pip install pyneoncli
 ```
```

### Comparing `pyneoncli-0.1.0a2/pyneoncli/clicommands.py` & `pyneoncli-0.1.1/pyneoncli/clicommands.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/clidispatcher.py` & `pyneoncli-0.1.1/pyneoncli/clidispatcher.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/clilist.py` & `pyneoncli-0.1.1/pyneoncli/clilist.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/climain.py` & `pyneoncli-0.1.1/pyneoncli/climain.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/colortext.py` & `pyneoncli-0.1.1/pyneoncli/colortext.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/configfile.py` & `pyneoncli-0.1.1/pyneoncli/configfile.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/msg.py` & `pyneoncli-0.1.1/pyneoncli/msg.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/neon.py` & `pyneoncli-0.1.1/pyneoncli/neon.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/neonapi.py` & `pyneoncli-0.1.1/pyneoncli/neonapi.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/neonapiexceptions.py` & `pyneoncli-0.1.1/pyneoncli/neonapiexceptions.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/neonliterals.py` & `pyneoncli-0.1.1/pyneoncli/neonliterals.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/printer.py` & `pyneoncli-0.1.1/pyneoncli/printer.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/rawneonapi.py` & `pyneoncli-0.1.1/pyneoncli/rawneonapi.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/requester.py` & `pyneoncli-0.1.1/pyneoncli/requester.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/threadedcreate.py` & `pyneoncli-0.1.1/pyneoncli/threadedcreate.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyneoncli/threadedneonapi.py` & `pyneoncli-0.1.1/pyneoncli/threadedneonapi.py`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.1.0a2/pyproject.toml` & `pyneoncli-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "pyneoncli"
-version = "0.1.0a2"
+version = "0.1.1"
 description = "A Python CLI for the Neon API"
 authors = ["Joe Drumgoole <Joe.Drumgoole@neon.tech>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `pyneoncli-0.1.0a2/PKG-INFO` & `pyneoncli-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneoncli
-Version: 0.1.0a2
+Version: 0.1.1
 Summary: A Python CLI for the Neon API
 License: Apache-2.0
 Author: Joe Drumgoole
 Author-email: Joe.Drumgoole@neon.tech
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -24,15 +24,16 @@
 
 A python package and command line tool for interaction with the [Neon](https://neon.tech) Serverless Postgres [API](https://api-docs.neon.tech/reference/getting-started-with-neon-api).
 
 This is a work in progress and this version is incomplete. 
 
 This version only supports the Neon V2 API. 
 
-The program can read the NEON_API_KEY from the environment or it can he loaded from a .env field in the current working directory.
+The program can read the NEON_API_KEY from the environment or it can he loaded from a `neoncli.conf` in your home directory or
+the current working directory.
 
 ## Installation
 
 You can install the package from PyPi using pip:
 ```commandline
 pip install pyneoncli
 ```
```

