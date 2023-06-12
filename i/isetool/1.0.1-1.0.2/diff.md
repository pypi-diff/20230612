# Comparing `tmp/isetool-1.0.1.tar.gz` & `tmp/isetool-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isetool-1.0.1.tar", max compression
+gzip compressed data, was "isetool-1.0.2.tar", max compression
```

## Comparing `isetool-1.0.1.tar` & `isetool-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1322 2021-10-13 13:22:31.030089 isetool-1.0.1/LICENSE
--rw-r--r--   0        0        0        9 2021-10-13 13:22:31.030089 isetool-1.0.1/README.md
--rw-r--r--   0        0        0      682 2021-11-11 09:22:31.431913 isetool-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-11 09:17:36.101913 isetool-1.0.1/src/isetool/__init__.py
--rw-r--r--   0        0        0     6175 2021-10-13 13:22:31.030089 isetool-1.0.1/src/isetool/cli.py
--rw-r--r--   0        0        0     3848 2021-10-13 13:22:31.030089 isetool-1.0.1/src/isetool/ise.py
--rw-r--r--   0        0        0      880 2021-11-11 09:22:54.190293 isetool-1.0.1/setup.py
--rw-r--r--   0        0        0      786 2021-11-11 09:22:54.190644 isetool-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1322 2023-06-08 08:31:04.141307 isetool-1.0.2/LICENSE
+-rw-r--r--   0        0        0        9 2023-06-08 08:31:04.141307 isetool-1.0.2/README.md
+-rw-r--r--   0        0        0      683 2023-06-08 08:33:46.554143 isetool-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 08:31:04.142307 isetool-1.0.2/src/isetool/__init__.py
+-rw-r--r--   0        0        0     6336 2023-06-08 08:49:15.533325 isetool-1.0.2/src/isetool/cli.py
+-rw-r--r--   0        0        0     3941 2023-06-08 08:58:34.925984 isetool-1.0.2/src/isetool/ise.py
+-rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 isetool-1.0.2/PKG-INFO
```

### Comparing `isetool-1.0.1/LICENSE` & `isetool-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isetool-1.0.1/pyproject.toml` & `isetool-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "isetool"
-version = "1.0.1"
+version = "1.0.2"
 description = "Command line for querying a Cisco ISE server"
 authors = ["Rob Woodward <rob@emailplus.org>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 repository = "https://github.com/robwdwd/isetool"
 include = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 requests = "^2.26.0"
 click = "^8.0.1"
 urllib3 = "^1.26.6"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
+[tool.poetry.group.dev.dependencies]
+black = "^23.1.0"
+pytest = "^7.1.3"
+pylint = "^2.9.6"
 pydocstyle = "^6.1.1"
-flake8 = "^4.0.1"
-pylint = "^2.9.5"
-black = "^21.7b0"
-pycodestyle = "^2.8.0"
+flake8 = "^6.0.0"
+isort = "^5.12.0"
 
 [tool.poetry.scripts]
 isetool = "isetool.cli:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `isetool-1.0.1/src/isetool/cli.py` & `isetool-1.0.2/src/isetool/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env /usr/bin/python3
 
 import click
 import json
 from isetool.ise import ISE
 import os
 import pprint
+from json import JSONDecodeError
 
 pp = pprint.PrettyPrinter(indent=4)
 
 
 class Default(dict):
     def __missing__(self, key):
         return key
@@ -54,15 +55,18 @@
     help=filterOperatorChoices_help
 )
 @click.option("--filter-match", help="Filter match string.", metavar="MATCH")
 @click.pass_obj
 def userlist(obj, filter_field, filter_operator, filter_match):
     """List users on the ISE deployment."""
 
-    cfg = json.load(obj['config'])
+    try:
+        cfg = json.load(obj["config"])
+    except JSONDecodeError as err:
+        raise SystemExit(f"Unable to parse configuration file: {err}") from err
 
     if filter_match:
         filter = filter_field + "." + filter_operator + "." + filter_match
         print("Getting users with filter: " + filter)
     else:
         filter = None
         print("Getting all users.")
```

### Comparing `isetool-1.0.1/src/isetool/ise.py` & `isetool-1.0.2/src/isetool/ise.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         params = {"page": page, "size": 100}
 
         if filter:
             params["filter"] = filter
 
         resp = self.iseSession.get(url, verify=False, params=params)
 
+        if resp.status_code in (401, 403):
+          raise Exception('User not authorised')
+
         if resp.status_code != 200:
             result = resp.json()
             error = self.join_errors(result["ERSResponse"]["messages"])
             raise Exception("getPage: {} {}".format(resp.status_code, error))
 
         return resp.json()["SearchResult"]
```

### Comparing `isetool-1.0.1/PKG-INFO` & `isetool-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: isetool
-Version: 1.0.1
+Version: 1.0.2
 Summary: Command line for querying a Cisco ISE server
 Home-page: https://github.com/robwdwd/isetool
 License: BSD-2-Clause
 Author: Rob Woodward
 Author-email: rob@emailplus.org
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Project-URL: Repository, https://github.com/robwdwd/isetool
 Description-Content-Type: text/markdown
 
 # isetool
```

