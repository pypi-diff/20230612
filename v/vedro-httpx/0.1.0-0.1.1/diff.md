# Comparing `tmp/vedro-httpx-0.1.0.tar.gz` & `tmp/vedro-httpx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-httpx-0.1.0.tar", last modified: Mon Jun 12 15:34:24 2023, max compression
+gzip compressed data, was "vedro-httpx-0.1.1.tar", last modified: Mon Jun 12 15:51:48 2023, max compression
```

## Comparing `vedro-httpx-0.1.0.tar` & `vedro-httpx-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:34:24.206382 vedro-httpx-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-12 15:34:24.210382 vedro-httpx-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-12 15:34:24.210382 vedro-httpx-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:34:24.206382 vedro-httpx-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/tests/test_async_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/tests/test_format_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/tests/test_sync_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:34:24.206382 vedro-httpx-0.1.0/vedro_httpx/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/vedro_httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/vedro_httpx/_async_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/vedro_httpx/_render_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/vedro_httpx/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/vedro_httpx/_sync_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:34:09.000000 vedro-httpx-0.1.0/vedro_httpx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:34:24.206382 vedro-httpx-0.1.0/vedro_httpx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-12 15:34:24.000000 vedro-httpx-0.1.0/vedro_httpx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 15:34:24.000000 vedro-httpx-0.1.0/vedro_httpx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:34:24.000000 vedro-httpx-0.1.0/vedro_httpx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 15:34:24.000000 vedro-httpx-0.1.0/vedro_httpx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 15:34:24.000000 vedro-httpx-0.1.0/vedro_httpx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-12 15:51:48.613881 vedro-httpx-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_async_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_format_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_sync_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/vedro_httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_async_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_render_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_sync_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_vedro_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/vedro_httpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/top_level.txt
```

### Comparing `vedro-httpx-0.1.0/LICENSE` & `vedro-httpx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.0/setup.cfg` & `vedro-httpx-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 0.1.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-httpx-0.1.0/setup.py` & `vedro-httpx-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-httpx",
-    version="0.1.0",
-    description="",
+    version="0.1.1",
+    description="Vedro + HTTPX",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-httpx",
     project_urls={
```

### Comparing `vedro-httpx-0.1.0/tests/test_async_interface.py` & `vedro-httpx-0.1.1/tests/test_async_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.0/tests/test_format_response.py` & `vedro-httpx-0.1.1/tests/test_format_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.0/tests/test_response.py` & `vedro-httpx-0.1.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.0/tests/test_sync_interface.py` & `vedro-httpx-0.1.1/tests/test_sync_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.0/vedro_httpx/_async_http_interface.py` & `vedro-httpx-0.1.1/vedro_httpx/_async_http_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.0/vedro_httpx/_render_response.py` & `vedro-httpx-0.1.1/vedro_httpx/_render_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.0/vedro_httpx/_sync_http_interface.py` & `vedro-httpx-0.1.1/vedro_httpx/_sync_http_interface.py`

 * *Files identical despite different names*

