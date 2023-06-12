# Comparing `tmp/owlml-0.1.2.dev1685654240.tar.gz` & `tmp/owlml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.2.dev1685654240.tar", last modified: Thu Jun  1 21:17:33 2023, max compression
+gzip compressed data, was "owlml-0.2.0.tar", last modified: Mon Jun 12 19:23:31 2023, max compression
```

## Comparing `owlml-0.1.2.dev1685654240.tar` & `owlml-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:17:33.683187 owlml-0.1.2.dev1685654240/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-01 21:17:33.683187 owlml-0.1.2.dev1685654240/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:17:33.683187 owlml-0.1.2.dev1685654240/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/dataset_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/images.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/owlml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:17:33.683187 owlml-0.1.2.dev1685654240/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-01 21:17:33.000000 owlml-0.1.2.dev1685654240/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-01 21:17:33.000000 owlml-0.1.2.dev1685654240/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:17:33.000000 owlml-0.1.2.dev1685654240/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 21:17:33.000000 owlml-0.1.2.dev1685654240/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 21:17:33.000000 owlml-0.1.2.dev1685654240/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 21:17:33.000000 owlml-0.1.2.dev1685654240/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-01 21:17:33.683187 owlml-0.1.2.dev1685654240/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:16:40.000000 owlml-0.1.2.dev1685654240/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:23:31.208250 owlml-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 19:22:33.000000 owlml-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 19:23:31.208250 owlml-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-12 19:22:33.000000 owlml-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:23:31.208250 owlml-0.2.0/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/dataset_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-12 19:22:33.000000 owlml-0.2.0/owlml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:23:31.208250 owlml-0.2.0/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-12 19:23:31.000000 owlml-0.2.0/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-12 19:23:31.000000 owlml-0.2.0/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:23:31.000000 owlml-0.2.0/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 19:23:31.000000 owlml-0.2.0/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-12 19:23:31.000000 owlml-0.2.0/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 19:23:31.000000 owlml-0.2.0/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-12 19:23:31.212250 owlml-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:22:33.000000 owlml-0.2.0/setup.py
```

### Comparing `owlml-0.1.2.dev1685654240/LICENSE` & `owlml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1685654240/README.md` & `owlml-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1685654240/owlml/__main__.py` & `owlml-0.2.0/owlml/__main__.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1685654240/owlml/annotations.py` & `owlml-0.2.0/owlml/annotations.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1685654240/owlml/api.py` & `owlml-0.2.0/owlml/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """API class for OwlML."""
 import os
 from typing import Any
 
 import requests
+from requests.auth import HTTPBasicAuth
 
 
 def _get_required_env_var(env_var: str) -> str:
     """Get an environment variable or raise an error if it doesn't exist."""
     value = os.getenv(env_var)
     if value is None:
         raise ValueError(f"Missing required environment variable: {env_var}")
@@ -24,25 +25,30 @@
 
 
 class OwlMLAPI:
     """API class for OwlML."""
 
     base_url: str = _get_required_env_var("OWLML_URL")
     api_url: str = os.path.join(base_url, "api")
+    basic_auth: HTTPBasicAuth = HTTPBasicAuth(
+        _get_required_env_var("OWLML_USERNAME"), _get_required_env_var("OWLML_PASSWORD")
+    )
 
     @classmethod
     def get(cls, route: str) -> dict[str, Any]:
         """Make a GET request to the OwlML API."""
-        response = requests.get(os.path.join(cls.api_url, route))
+        response = requests.get(os.path.join(cls.api_url, route), auth=cls.basic_auth)
         raise_for_status(response)
         if response.status_code == 204:
             return {}
         return response.json()
 
     @classmethod
     def post(cls, route: str, payload: dict[str, Any] = dict()) -> dict[str, Any]:
         """Make a POST request to the OwlML API."""
-        response = requests.post(os.path.join(cls.api_url, route), json=payload)
+        response = requests.post(
+            os.path.join(cls.api_url, route), auth=cls.basic_auth, json=payload
+        )
         raise_for_status(response)
         if response.status_code == 204:
             return {}
         return response.json()
```

### Comparing `owlml-0.1.2.dev1685654240/owlml/auth.py` & `owlml-0.2.0/owlml/auth.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1685654240/owlml/dataset_versions.py` & `owlml-0.2.0/owlml/dataset_versions.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1685654240/owlml/datasets.py` & `owlml-0.2.0/owlml/datasets.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1685654240/owlml/images.py` & `owlml-0.2.0/owlml/images.py`

 * *Files identical despite different names*

