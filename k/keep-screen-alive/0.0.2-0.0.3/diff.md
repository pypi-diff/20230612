# Comparing `tmp/keep_screen_alive-0.0.2.tar.gz` & `tmp/keep_screen_alive-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keep_screen_alive-0.0.2.tar", max compression
+gzip compressed data, was "keep_screen_alive-0.0.3.tar", max compression
```

## Comparing `keep_screen_alive-0.0.2.tar` & `keep_screen_alive-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      420 2023-06-07 12:46:58.543143 keep_screen_alive-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-07 11:46:26.196161 keep_screen_alive-0.0.2/keep_alive/__init__.py
--rw-r--r--   0        0        0     1031 2023-06-07 11:46:26.196293 keep_screen_alive-0.0.2/keep_alive/run.py
--rw-r--r--   0        0        0      778 2023-06-07 13:25:28.967703 keep_screen_alive-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 keep_screen_alive-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-06-07 12:46:58.543143 keep_screen_alive-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 11:46:26.196161 keep_screen_alive-0.0.3/keep_alive/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-12 18:52:51.866839 keep_screen_alive-0.0.3/keep_alive/run.py
+-rw-r--r--   0        0        0      778 2023-06-12 18:55:54.616161 keep_screen_alive-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 keep_screen_alive-0.0.3/PKG-INFO
```

### Comparing `keep_screen_alive-0.0.2/keep_alive/run.py` & `keep_screen_alive-0.0.3/keep_alive/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     parser_settings = {
         'PREFER_DATES_FROM': 'future',
         'RETURN_AS_TIMEZONE_AWARE': True,
     }
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
-        later = dateparser.parse(input_value, settings=parser_settings)
         now = dateparser.parse('now', settings=parser_settings)
+        parser_settings['RELATIVE_BASE'] = now
+        later = dateparser.parse(input_value, settings=parser_settings)
 
     if later is None:
         print("Missing a target")
         sys.exit(1)
 
     if now >= later:
         print(f"{later} is in the past. It is currently {now}")
```

### Comparing `keep_screen_alive-0.0.2/pyproject.toml` & `keep_screen_alive-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keep-screen-alive"
-version = "0.0.2"
+version = "0.0.3"
 description = "A tool to keep your machine from going to sleep for some amount of time"
 authors = ["Tim Willis"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "keep_alive"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `keep_screen_alive-0.0.2/PKG-INFO` & `keep_screen_alive-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keep-screen-alive
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to keep your machine from going to sleep for some amount of time
 License: MIT
 Author: Tim Willis
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

