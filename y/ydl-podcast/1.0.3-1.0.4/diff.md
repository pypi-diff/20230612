# Comparing `tmp/ydl_podcast-1.0.3.tar.gz` & `tmp/ydl_podcast-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.0.3.tar", max compression
+gzip compressed data, was "ydl_podcast-1.0.4.tar", max compression
```

## Comparing `ydl_podcast-1.0.3.tar` & `ydl_podcast-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.3/LICENSE
--rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.3/README.md
--rw-r--r--   0        0        0      895 2023-06-12 02:15:43.271076 ydl_podcast-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    12290 2023-06-12 02:15:43.271076 ydl_podcast-1.0.3/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.3/ydl_podcast/__main__.py
--rw-r--r--   0        0        0      990 2023-06-12 02:15:43.271076 ydl_podcast-1.0.3/ydl_podcast/template.py
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/README.md
+-rw-r--r--   0        0        0      895 2023-06-12 02:23:54.572619 ydl_podcast-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    12290 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0      990 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/ydl_podcast/template.py
+-rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.4/PKG-INFO
```

### Comparing `ydl_podcast-1.0.3/LICENSE` & `ydl_podcast-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.3/README.md` & `ydl_podcast-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.3/pyproject.toml` & `ydl_podcast-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.0.3"
+version = "1.0.4"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.0.3/ydl_podcast/__init__.py` & `ydl_podcast-1.0.4/ydl_podcast/__init__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.3/ydl_podcast/__main__.py` & `ydl_podcast-1.0.4/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.3/ydl_podcast/template.py` & `ydl_podcast-1.0.4/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.3/PKG-INFO` & `ydl_podcast-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
```

