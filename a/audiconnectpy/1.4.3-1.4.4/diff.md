# Comparing `tmp/audiconnectpy-1.4.3.tar.gz` & `tmp/audiconnectpy-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.4.3.tar", last modified: Mon May 22 06:56:27 2023, max compression
+gzip compressed data, was "audiconnectpy-1.4.4.tar", last modified: Mon Jun 12 17:18:07 2023, max compression
```

## Comparing `audiconnectpy-1.4.3.tar` & `audiconnectpy-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.118575 audiconnectpy-1.4.3/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32074 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 06:56:27.000000 audiconnectpy-1.4.3/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-22 06:56:26.000000 audiconnectpy-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:56:27.122575 audiconnectpy-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 06:56:14.000000 audiconnectpy-1.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:18:07.475040 audiconnectpy-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-12 17:18:07.475040 audiconnectpy-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:18:07.475040 audiconnectpy-1.4.4/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22833 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26809 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32108 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:18:07.475040 audiconnectpy-1.4.4/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-12 17:18:07.000000 audiconnectpy-1.4.4/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 17:18:07.000000 audiconnectpy-1.4.4/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:18:07.000000 audiconnectpy-1.4.4/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:18:07.000000 audiconnectpy-1.4.4/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 17:18:07.000000 audiconnectpy-1.4.4/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:18:07.475040 audiconnectpy-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-12 17:18:05.000000 audiconnectpy-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:18:07.475040 audiconnectpy-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 17:17:56.000000 audiconnectpy-1.4.4/tests/__init__.py
```

### Comparing `audiconnectpy-1.4.3/LICENSE` & `audiconnectpy-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.3/PKG-INFO` & `audiconnectpy-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.3/README.md` & `audiconnectpy-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.3/audiconnectpy/api.py` & `audiconnectpy-1.4.4/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.3/audiconnectpy/auth.py` & `audiconnectpy-1.4.4/audiconnectpy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             rsp = await response.json(loads=json_loads)
         elif (
             headers
             and "application/json" in headers.get("Accept", "")
             and contents == ""
         ):
             _LOGGER.debug("JSON FIX: Accept is JSON but Response is None")
-            rsp = ExtendedDict({})
+            rsp = ExtendedDict()
         else:
             rsp = await response.text()
 
         if raw_reply and raw_rsp:
             return response, rsp
         return rsp
```

### Comparing `audiconnectpy-1.4.3/audiconnectpy/helpers.py` & `audiconnectpy-1.4.4/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.3/audiconnectpy/models.py` & `audiconnectpy-1.4.4/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.3/audiconnectpy/services.py` & `audiconnectpy-1.4.4/audiconnectpy/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,19 +157,19 @@
         }
         data = await self._auth.get(
             f"{url}/bs/tripstatistics/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/tripdata/{knd}",
             params=params,
         )
         data = data if data else ExtendedDict()
         td_sorted = sorted(
-            data.getr("tripDataList.tripData"),
+            data.getr("tripDataList.tripData", []),
             key=lambda k: k["overallMileage"],  # type: ignore[no-any-return]
             reverse=True,
         )
-        td_current = td_sorted[0]
+        td_current = td_sorted[0] if len(td_sorted) > 0 else {}
         td_reset_trip = {}
 
         for trip in td_sorted:
             if (td_current["startMileage"] - trip["startMileage"]) > 2:
                 td_reset_trip = trip
                 break
             td_current["tripID"] = trip["tripID"]
```

### Comparing `audiconnectpy-1.4.3/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.4.4/audiconnectpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.4.3
+Version: 1.4.4
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.4.3/pyproject.toml` & `audiconnectpy-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.4.3/setup.py` & `audiconnectpy-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.4.3",
+    version="1.4.4",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

