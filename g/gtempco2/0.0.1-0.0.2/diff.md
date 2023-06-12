# Comparing `tmp/gtempco2-0.0.1.tar.gz` & `tmp/gtempco2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtempco2-0.0.1.tar", last modified: Mon Jun 12 03:42:25 2023, max compression
+gzip compressed data, was "gtempco2-0.0.2.tar", last modified: Mon Jun 12 04:43:43 2023, max compression
```

## Comparing `gtempco2-0.0.1.tar` & `gtempco2-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 03:42:25.449922 gtempco2-0.0.1/
--rw-r--r--   0 yt        (1000) yt        (1000)     1781 2023-06-12 03:42:25.449031 gtempco2-0.0.1/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)     1250 2023-06-12 03:41:45.000000 gtempco2-0.0.1/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-12 03:42:25.449922 gtempco2-0.0.1/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-06-12 03:03:39.000000 gtempco2-0.0.1/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 03:42:25.432011 gtempco2-0.0.1/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 03:42:25.447585 gtempco2-0.0.1/src/gtempco2.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1781 2023-06-12 03:42:25.000000 gtempco2-0.0.1/src/gtempco2.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-06-12 03:42:25.000000 gtempco2-0.0.1/src/gtempco2.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-12 03:42:25.000000 gtempco2-0.0.1/src/gtempco2.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-06-12 03:42:25.000000 gtempco2-0.0.1/src/gtempco2.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-06-12 03:42:25.000000 gtempco2-0.0.1/src/gtempco2.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     2702 2023-06-12 01:39:39.000000 gtempco2-0.0.1/src/gtempco2.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 04:43:43.618582 gtempco2-0.0.2/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-06-12 04:43:43.617761 gtempco2-0.0.2/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     1249 2023-06-12 04:40:13.000000 gtempco2-0.0.2/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-12 04:43:43.618582 gtempco2-0.0.2/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      951 2023-06-12 04:42:39.000000 gtempco2-0.0.2/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 04:43:43.601524 gtempco2-0.0.2/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-12 04:43:43.616707 gtempco2-0.0.2/src/gtempco2.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     1780 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      217 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       44 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        9 2023-06-12 04:43:43.000000 gtempco2-0.0.2/src/gtempco2.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     2702 2023-06-12 01:39:39.000000 gtempco2-0.0.2/src/gtempco2.py
```

### Comparing `gtempco2-0.0.1/PKG-INFO` & `gtempco2-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
@@ -40,11 +40,11 @@
 enter end_date: e.g. 2023-04
 yyyy-mo: 1965-06
 start_date= 1960-06 end_date= 1965-06
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
 
-<img src='https://github.com/ytakefuji/gtempco2/blob/main/1960-06_1965-06.png' height=450 width=600>
+<img src='https://github.com/ytakefuji/gtempco2/raw/main/1960-06_1965-06.png' height=450 width=600>
```

### Comparing `gtempco2-0.0.1/README.md` & `gtempco2-0.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 enter end_date: e.g. 2023-04
 yyyy-mo: 1965-06
 start_date= 1960-06 end_date= 1965-06
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
 
-<img src='https://github.com/ytakefuji/gtempco2/blob/main/1960-06_1965-06.png' height=450 width=600>
+<img src='https://github.com/ytakefuji/gtempco2/raw/main/1960-06_1965-06.png' height=450 width=600>
```

### Comparing `gtempco2-0.0.1/setup.py` & `gtempco2-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gtempco2",
-    version="0.0.1",
+    version="0.0.2",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for displaying global temperature and co2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/gtempco2",
     project_urls={
```

### Comparing `gtempco2-0.0.1/src/gtempco2.egg-info/PKG-INFO` & `gtempco2-0.0.2/src/gtempco2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtempco2
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for displaying global temperature and co2
 Home-page: https://github.com/ytakefuji/gtempco2
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ytakefuji/gtempco2
 Platform: UNKNOWN
@@ -40,11 +40,11 @@
 enter end_date: e.g. 2023-04
 yyyy-mo: 1965-06
 start_date= 1960-06 end_date= 1965-06
 </pre>
 
 The system will ask the start-date and end-date. The result will be shown and saved in the directory as follows.
 
-<img src='https://github.com/ytakefuji/gtempco2/blob/main/1960-06_1965-06.png' height=450 width=600>
+<img src='https://github.com/ytakefuji/gtempco2/raw/main/1960-06_1965-06.png' height=450 width=600>
```

### Comparing `gtempco2-0.0.1/src/gtempco2.py` & `gtempco2-0.0.2/src/gtempco2.py`

 * *Files identical despite different names*

