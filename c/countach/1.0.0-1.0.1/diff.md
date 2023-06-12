# Comparing `tmp/countach-1.0.0.tar.gz` & `tmp/countach-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countach-1.0.0.tar", last modified: Fri Mar 31 15:04:00 2023, max compression
+gzip compressed data, was "countach-1.0.1.tar", last modified: Mon Jun 12 21:23:23 2023, max compression
```

## Comparing `countach-1.0.0.tar` & `countach-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:00.534391 countach-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-31 15:03:42.000000 countach-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-31 15:04:00.534391 countach-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-31 15:03:42.000000 countach-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-31 15:03:42.000000 countach-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-31 15:04:00.534391 countach-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 15:03:42.000000 countach-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:00.526391 countach-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:00.530392 countach-1.0.0/src/countach/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 15:03:42.000000 countach-1.0.0/src/countach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-31 15:03:42.000000 countach-1.0.0/src/countach/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-31 15:03:42.000000 countach-1.0.0/src/countach/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-31 15:03:42.000000 countach-1.0.0/src/countach/fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-31 15:03:42.000000 countach-1.0.0/src/countach/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-31 15:03:42.000000 countach-1.0.0/src/countach/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-31 15:03:42.000000 countach-1.0.0/src/countach/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:00.530392 countach-1.0.0/src/countach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-31 15:04:00.000000 countach-1.0.0/src/countach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-31 15:04:00.000000 countach-1.0.0/src/countach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 15:04:00.000000 countach-1.0.0/src/countach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 15:04:00.000000 countach-1.0.0/src/countach.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-31 15:04:00.000000 countach-1.0.0/src/countach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 15:04:00.000000 countach-1.0.0/src/countach.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 15:04:00.534391 countach-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-31 15:03:42.000000 countach-1.0.0/tests/test_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-31 15:03:42.000000 countach-1.0.0/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-31 15:03:42.000000 countach-1.0.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:23.327182 countach-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-12 21:23:05.000000 countach-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-12 21:23:23.327182 countach-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 21:23:05.000000 countach-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-12 21:23:05.000000 countach-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-12 21:23:23.327182 countach-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-12 21:23:05.000000 countach-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:23.323182 countach-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:23.327182 countach-1.0.1/src/countach/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:05.000000 countach-1.0.1/src/countach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-12 21:23:05.000000 countach-1.0.1/src/countach/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-12 21:23:05.000000 countach-1.0.1/src/countach/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-12 21:23:05.000000 countach-1.0.1/src/countach/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 21:23:05.000000 countach-1.0.1/src/countach/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-12 21:23:05.000000 countach-1.0.1/src/countach/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-12 21:23:05.000000 countach-1.0.1/src/countach/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:23.327182 countach-1.0.1/src/countach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-12 21:23:23.000000 countach-1.0.1/src/countach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-12 21:23:23.000000 countach-1.0.1/src/countach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:23:23.000000 countach-1.0.1/src/countach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:23:23.000000 countach-1.0.1/src/countach.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 21:23:23.000000 countach-1.0.1/src/countach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 21:23:23.000000 countach-1.0.1/src/countach.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:23:23.327182 countach-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-12 21:23:05.000000 countach-1.0.1/tests/test_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-12 21:23:05.000000 countach-1.0.1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-12 21:23:05.000000 countach-1.0.1/tests/test_types.py
```

### Comparing `countach-1.0.0/LICENSE` & `countach-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `countach-1.0.0/PKG-INFO` & `countach-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countach
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for extracting data from EV2274A A2L files.
 Home-page: https://github.com/HWRacing/countach
 Author: Hamish Knox
 Author-email: hrjkknox@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HWRacing/countach/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countach-1.0.0/setup.cfg` & `countach-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = countach
-version = v1.0.0
+version = v1.0.1
 author = Hamish Knox
 author_email = hrjkknox@gmail.com
 description = A library for extracting data from EV2274A A2L files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HWRacing/countach
 license = MIT
```

### Comparing `countach-1.0.0/src/countach/fileops.py` & `countach-1.0.1/src/countach/fileops.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def _linesToSections(lines: List[str]) -> List[List[str]]:
 	# Whether or not the current line is inside a section
 	inSection = False
 	output = []
 	currentOutput = []
 	for rawline in lines:
 		# Remove leading and trailing whitespace
-		line = rawline.lstrip()[:-1]
+		line = rawline.strip()
 
 		if line == "/begin CHARACTERISTIC" or line == "/begin MEASUREMENT":
 			inSection = True
 		elif line == "/end CHARACTERISTIC" or line == "/end MEASUREMENT":
 			inSection = False
 			currentOutput.append(line)
 			output.append(currentOutput)
```

### Comparing `countach-1.0.0/src/countach/fixed.py` & `countach-1.0.1/src/countach/fixed.py`

 * *Files identical despite different names*

### Comparing `countach-1.0.0/src/countach/parse.py` & `countach-1.0.1/src/countach/parse.py`

 * *Files identical despite different names*

### Comparing `countach-1.0.0/src/countach.egg-info/PKG-INFO` & `countach-1.0.1/src/countach.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countach
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for extracting data from EV2274A A2L files.
 Home-page: https://github.com/HWRacing/countach
 Author: Hamish Knox
 Author-email: hrjkknox@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HWRacing/countach/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `countach-1.0.0/tests/test_fixed.py` & `countach-1.0.1/tests/test_fixed.py`

 * *Files identical despite different names*

### Comparing `countach-1.0.0/tests/test_types.py` & `countach-1.0.1/tests/test_types.py`

 * *Files identical despite different names*

