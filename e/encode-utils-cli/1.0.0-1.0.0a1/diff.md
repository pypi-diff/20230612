# Comparing `tmp/encode_utils_cli-1.0.0.tar.gz` & `tmp/encode_utils_cli-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encode_utils_cli-1.0.0.tar", max compression
+gzip compressed data, was "encode_utils_cli-1.0.0a1.tar", max compression
```

## Comparing `encode_utils_cli-1.0.0.tar` & `encode_utils_cli-1.0.0a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-06-12 16:20:38.964429 encode_utils_cli-1.0.0/LICENSE
--rw-r--r--   0        0        0      809 2023-06-12 16:20:38.964429 encode_utils_cli-1.0.0/README.md
--rw-r--r--   0        0        0     2595 2023-06-12 16:21:00.849536 encode_utils_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-12 16:20:38.964429 encode_utils_cli-1.0.0/src/encode_utils_cli/__init__.py
--rw-r--r--   0        0        0      177 2023-06-12 16:20:38.964429 encode_utils_cli-1.0.0/src/encode_utils_cli/__main__.py
--rw-r--r--   0        0        0      931 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/_cli.py
--rw-r--r--   0        0        0     2087 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/chapt2bmqpyml.py
--rw-r--r--   0        0        0      666 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/frames_denum.py
--rwxr-xr-x   0        0        0     1164 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/mpls2chap.py
--rw-r--r--   0        0        0      427 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/num_frames.py
--rw-r--r--   0        0        0     1163 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/re_chapters.py
--rwxr-xr-x   0        0        0     1042 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/re_titles.py
--rwxr-xr-x   0        0        0      966 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/screens2bm.py
--rw-r--r--   0        0        0       35 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/util/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/util/load_mpls.py
--rw-r--r--   0        0        0      312 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/util/source.py
--rw-r--r--   0        0        0      672 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/util/timeconv.py
--rw-r--r--   0        0        0     2203 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/vs_screens.py
--rwxr-xr-x   0        0        0      758 2023-06-12 16:20:38.968429 encode_utils_cli-1.0.0/src/encode_utils_cli/zones_validator.py
--rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 encode_utils_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0      809 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/README.md
+-rw-r--r--   0        0        0     2603 2023-06-12 16:13:29.698697 encode_utils_cli-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/__init__.py
+-rw-r--r--   0        0        0      177 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/__main__.py
+-rw-r--r--   0        0        0      931 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/_cli.py
+-rw-r--r--   0        0        0     2087 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/chapt2bmqpyml.py
+-rw-r--r--   0        0        0      666 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/frames_denum.py
+-rwxr-xr-x   0        0        0     1164 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/mpls2chap.py
+-rw-r--r--   0        0        0      427 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/num_frames.py
+-rw-r--r--   0        0        0     1163 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_chapters.py
+-rwxr-xr-x   0        0        0     1042 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_titles.py
+-rwxr-xr-x   0        0        0      966 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/screens2bm.py
+-rw-r--r--   0        0        0       35 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/load_mpls.py
+-rw-r--r--   0        0        0      312 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/source.py
+-rw-r--r--   0        0        0      672 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/timeconv.py
+-rw-r--r--   0        0        0     2203 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/vs_screens.py
+-rwxr-xr-x   0        0        0      758 2023-06-12 16:13:11.058568 encode_utils_cli-1.0.0a1/src/encode_utils_cli/zones_validator.py
+-rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 encode_utils_cli-1.0.0a1/PKG-INFO
```

### Comparing `encode_utils_cli-1.0.0/LICENSE` & `encode_utils_cli-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/README.md` & `encode_utils_cli-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/pyproject.toml` & `encode_utils_cli-1.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "encode-utils-cli"
-version = "1.0.0"
+version = "1.0.0-alpha.1"
 description = "Encode utils collection"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/encode-utils-cli"
 repository = "https://github.com/DeadNews/encode-utils-cli"
 keywords = ["cli", "encode", "vapoursynth", "mpls"]
```

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/_cli.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/chapt2bmqpyml.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/chapt2bmqpyml.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/frames_denum.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/frames_denum.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/mpls2chap.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/mpls2chap.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/re_chapters.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_chapters.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/re_titles.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/re_titles.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/screens2bm.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/screens2bm.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/util/load_mpls.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/load_mpls.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/util/timeconv.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/util/timeconv.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/vs_screens.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/vs_screens.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/src/encode_utils_cli/zones_validator.py` & `encode_utils_cli-1.0.0a1/src/encode_utils_cli/zones_validator.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.0/PKG-INFO` & `encode_utils_cli-1.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encode-utils-cli
-Version: 1.0.0
+Version: 1.0.0a1
 Summary: Encode utils collection
 Home-page: https://github.com/DeadNews/encode-utils-cli
 License: MIT
 Keywords: cli,encode,vapoursynth,mpls
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

