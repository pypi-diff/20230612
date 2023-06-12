# Comparing `tmp/superinvoke-1.0.1.tar.gz` & `tmp/superinvoke-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superinvoke-1.0.1.tar", max compression
+gzip compressed data, was "superinvoke-1.0.2.tar", max compression
```

## Comparing `superinvoke-1.0.1.tar` & `superinvoke-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2021-11-05 22:01:21.839383 superinvoke-1.0.1/LICENSE
--rw-r--r--   0        0        0       75 2021-11-05 22:01:43.303591 superinvoke-1.0.1/README.md
--rw-r--r--   0        0        0     2518 2023-06-11 16:58:51.388126 superinvoke-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      331 2023-06-11 16:59:00.628236 superinvoke-1.0.1/superinvoke/__init__.py
--rw-r--r--   0        0        0       30 2022-04-06 17:00:43.796843 superinvoke-1.0.1/superinvoke/collections/__init__.py
--rw-r--r--   0        0        0     1488 2022-08-24 22:29:27.352392 superinvoke-1.0.1/superinvoke/collections/env.py
--rw-r--r--   0        0        0      160 2021-11-05 19:11:04.153864 superinvoke-1.0.1/superinvoke/collections/misc.py
--rw-r--r--   0        0        0     7087 2023-06-11 16:54:26.768939 superinvoke-1.0.1/superinvoke/collections/tool.py
--rw-r--r--   0        0        0      699 2023-02-10 15:52:26.982795 superinvoke-1.0.1/superinvoke/constants.py
--rw-r--r--   0        0        0       40 2022-04-06 21:27:18.109926 superinvoke-1.0.1/superinvoke/extensions/__init__.py
--rw-r--r--   0        0        0       44 2023-05-19 11:24:00.575959 superinvoke-1.0.1/superinvoke/extensions/collection.py
--rw-r--r--   0        0        0     6182 2023-02-12 00:38:54.165150 superinvoke-1.0.1/superinvoke/extensions/context.py
--rw-r--r--   0        0        0      944 2021-11-05 17:48:25.409401 superinvoke-1.0.1/superinvoke/extensions/task.py
--rw-r--r--   0        0        0     1220 2023-05-19 11:23:40.827730 superinvoke-1.0.1/superinvoke/main.py
--rw-r--r--   0        0        0       82 2022-04-06 16:46:10.227621 superinvoke-1.0.1/superinvoke/objects/__init__.py
--rw-r--r--   0        0        0      731 2022-08-24 23:38:36.765460 superinvoke-1.0.1/superinvoke/objects/common.py
--rw-r--r--   0        0        0     1676 2023-05-19 11:21:45.118391 superinvoke-1.0.1/superinvoke/objects/env.py
--rw-r--r--   0        0        0     1819 2023-02-10 15:57:47.706638 superinvoke-1.0.1/superinvoke/objects/tool.py
--rw-r--r--   0        0        0     2477 2022-04-08 21:57:15.050683 superinvoke-1.0.1/superinvoke/utils.py
--rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 superinvoke-1.0.1/setup.py
--rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 superinvoke-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2021-11-05 22:01:21.839383 superinvoke-1.0.2/LICENSE
+-rw-r--r--   0        0        0       75 2021-11-05 22:01:43.303591 superinvoke-1.0.2/README.md
+-rw-r--r--   0        0        0     2536 2023-06-12 12:05:46.029617 superinvoke-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-06-12 11:40:57.745260 superinvoke-1.0.2/superinvoke/__init__.py
+-rw-r--r--   0        0        0       30 2022-04-06 17:00:43.796843 superinvoke-1.0.2/superinvoke/collections/__init__.py
+-rw-r--r--   0        0        0     1488 2022-08-24 22:29:27.352392 superinvoke-1.0.2/superinvoke/collections/env.py
+-rw-r--r--   0        0        0      413 2023-06-12 11:40:33.828956 superinvoke-1.0.2/superinvoke/collections/misc.py
+-rw-r--r--   0        0        0     7087 2023-06-11 16:54:26.768939 superinvoke-1.0.2/superinvoke/collections/tool.py
+-rw-r--r--   0        0        0      699 2023-02-10 15:52:26.982795 superinvoke-1.0.2/superinvoke/constants.py
+-rw-r--r--   0        0        0       40 2022-04-06 21:27:18.109926 superinvoke-1.0.2/superinvoke/extensions/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-19 11:24:00.575959 superinvoke-1.0.2/superinvoke/extensions/collection.py
+-rw-r--r--   0        0        0     6320 2023-06-12 12:15:38.686018 superinvoke-1.0.2/superinvoke/extensions/context.py
+-rw-r--r--   0        0        0      944 2021-11-05 17:48:25.409401 superinvoke-1.0.2/superinvoke/extensions/task.py
+-rw-r--r--   0        0        0     1264 2023-06-12 11:29:55.724880 superinvoke-1.0.2/superinvoke/main.py
+-rw-r--r--   0        0        0       82 2022-04-06 16:46:10.227621 superinvoke-1.0.2/superinvoke/objects/__init__.py
+-rw-r--r--   0        0        0      731 2022-08-24 23:38:36.765460 superinvoke-1.0.2/superinvoke/objects/common.py
+-rw-r--r--   0        0        0     1676 2023-05-19 11:21:45.118391 superinvoke-1.0.2/superinvoke/objects/env.py
+-rw-r--r--   0        0        0     1819 2023-02-10 15:57:47.706638 superinvoke-1.0.2/superinvoke/objects/tool.py
+-rw-r--r--   0        0        0     2477 2022-04-08 21:57:15.050683 superinvoke-1.0.2/superinvoke/utils.py
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 superinvoke-1.0.2/setup.py
+-rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 superinvoke-1.0.2/PKG-INFO
```

### Comparing `superinvoke-1.0.1/LICENSE` & `superinvoke-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/pyproject.toml` & `superinvoke-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superinvoke"
-version = "1.0.1"
+version = "1.0.2"
 description = "An Invoke wrapper with extra handy features."
 license = "MIT"
 authors = ["Alex <alex@neoxelox.com>"]
 maintainers = ["Alex <alex@neoxelox.com>"]
 readme = "README.md"
 homepage = "https://github.com/neoxelox/superinvoke"
 repository = "https://github.com/neoxelox/superinvoke"
@@ -43,17 +43,17 @@
 jobs = "auto"
 exclude = ["**/__pycache__/*", "**/__init__.py"]
 
 [tool.flakehell.plugins]
 "flake8-black" = ["+*"]
 "flake8-isort" = ["+*"]
 mccabe = ["+*"]
-pycodestyle = ["+*", "-W0621", "-E203", "-E1101"]
+pycodestyle = ["+*", "-W0621", "-E203", "-E1101", "-W503"]
 pyflakes = ["+*"]
-pylint = ["+*", "-W0621", "-E1101"]
+pylint = ["+*", "-W0621", "-E1101", "-W503"]
 
 [tool.isort]
 profile = "black"
 py_version = "39"
 line_length = 120
 multi_line_output = 3
 known_first_party = ["superinvoke"]
```

### Comparing `superinvoke-1.0.1/superinvoke/collections/env.py` & `superinvoke-1.0.2/superinvoke/collections/env.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/superinvoke/collections/tool.py` & `superinvoke-1.0.2/superinvoke/collections/tool.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/superinvoke/constants.py` & `superinvoke-1.0.2/superinvoke/constants.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/superinvoke/extensions/context.py` & `superinvoke-1.0.2/superinvoke/extensions/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import fnmatch
 import os
 import sys
 from typing import List, Literal, Optional
 
 from invoke.context import Context
 
 from .. import constants, utils
@@ -62,15 +63,19 @@
 
     return stdout or stderr
 
 
 # Checks whether a certain version of a program is installed.
 def has(context: Context, program: str, version: Optional[str] = None) -> bool:
     if version:
-        return version in context.attempt(f"{program} --version") or version in context.attempt(f"{program} version")
+        version = f"*{version}*"
+        return (  # noqa: BLK100
+            fnmatch.fnmatchcase(context.attempt(f"{program} --version"), version)
+            or fnmatch.fnmatchcase(context.attempt(f"{program} version"), version)
+        )
     else:
         result = context.attempt(f"which {program}")
         return result and "not found" not in result
 
 
 # Gets the root path of the current repository.
 def repository(context: Context) -> str:
```

### Comparing `superinvoke-1.0.1/superinvoke/extensions/task.py` & `superinvoke-1.0.2/superinvoke/extensions/task.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/superinvoke/main.py` & `superinvoke-1.0.2/superinvoke/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     root.configure({  # noqa: BLK100
         "run": {
             "shell": os.environ.get("COMSPEC", os.environ.get("SHELL")),
             "encoding": "utf-8"
         }
     })
     root.add_task(collections.misc.help)
+    root.add_task(collections.misc.version)
 
     if tools:
         # Tool collection
         tool = Collection()
         tool.add_task(collections.tool.install)
         tool.add_task(collections.tool.list)
         tool.add_task(collections.tool.remove)
```

### Comparing `superinvoke-1.0.1/superinvoke/objects/common.py` & `superinvoke-1.0.2/superinvoke/objects/common.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/superinvoke/objects/env.py` & `superinvoke-1.0.2/superinvoke/objects/env.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/superinvoke/objects/tool.py` & `superinvoke-1.0.2/superinvoke/objects/tool.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/superinvoke/utils.py` & `superinvoke-1.0.2/superinvoke/utils.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.1/setup.py` & `superinvoke-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['download==0.3.5', 'neoxelox-invoke==2.0.0', 'rich==12.5.1']
 
 setup_kwargs = {
     'name': 'superinvoke',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'An Invoke wrapper with extra handy features.',
     'long_description': '# superinvoke\n\nAn Invoke wrapper with extra handy features.\n\nTODO: EXPLAIN\n',
     'author': 'Alex',
     'author_email': 'alex@neoxelox.com',
     'maintainer': 'Alex',
     'maintainer_email': 'alex@neoxelox.com',
     'url': 'https://github.com/neoxelox/superinvoke',
```

### Comparing `superinvoke-1.0.1/PKG-INFO` & `superinvoke-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superinvoke
-Version: 1.0.1
+Version: 1.0.2
 Summary: An Invoke wrapper with extra handy features.
 Home-page: https://github.com/neoxelox/superinvoke
 License: MIT
 Keywords: plugin,wrapper,invoke,pyinvoke,superinvoke
 Author: Alex
 Author-email: alex@neoxelox.com
 Maintainer: Alex
```

