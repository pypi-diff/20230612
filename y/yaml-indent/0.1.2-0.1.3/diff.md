# Comparing `tmp/yaml_indent-0.1.2.tar.gz` & `tmp/yaml_indent-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_indent-0.1.2.tar", max compression
+gzip compressed data, was "yaml_indent-0.1.3.tar", max compression
```

## Comparing `yaml_indent-0.1.2.tar` & `yaml_indent-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-11 08:48:40.402953 yaml_indent-0.1.2/LICENSE
--rw-r--r--   0        0        0     1599 2023-06-11 08:48:40.402953 yaml_indent-0.1.2/README.md
--rw-r--r--   0        0        0      608 2023-06-11 09:22:19.042831 yaml_indent-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 08:48:40.402953 yaml_indent-0.1.2/yaml_indent/__init__.py
--rwxr-xr-x   0        0        0     2914 2023-06-11 09:14:11.152191 yaml_indent-0.1.2/yaml_indent/yaml_indent.py
--rw-r--r--   0        0        0     2277 1970-01-01 00:00:00.000000 yaml_indent-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 11:39:30.751856 yaml_indent-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1606 2023-06-12 06:59:29.669152 yaml_indent-0.1.3/README.md
+-rw-r--r--   0        0        0      663 2023-06-12 10:28:55.990697 yaml_indent-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-12 07:30:40.480371 yaml_indent-0.1.3/yaml_indent/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-12 11:01:58.592620 yaml_indent-0.1.3/yaml_indent/_version.py
+-rwxr-xr-x   0        0        0     3062 2023-06-12 10:19:59.516858 yaml_indent-0.1.3/yaml_indent/yaml_indent.py
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 yaml_indent-0.1.3/setup.py
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 yaml_indent-0.1.3/PKG-INFO
```

### Comparing `yaml_indent-0.1.2/LICENSE` & `yaml_indent-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_indent-0.1.2/README.md` & `yaml_indent-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 - `-i` (optional) if set, the input file will be edited in place.
 
 If no output file is specified and `-i` is not set, the indented YAML will be printed to the standard output.
 
 ## Configuration
 
 `yaml-indent` looks for a `.yaml_indent.ini` configuration file in the
-current directory and all parent directories up to the home
+the yaml files directory and all parent directories up to the home
 directory. The configuration file should be in the INI format and can
 specify the `mapping`, `sequence`, and `offset` indentation values
 under the `YAML` section.
 
 Here's an example:
 
 ```ini
```

### Comparing `yaml_indent-0.1.2/pyproject.toml` & `yaml_indent-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "yaml-indent"
-version = "0.1.2"
-description = ""
+version = "0.1.3"
+description = "Tool for making consistent indentation"
 authors = ["Knut Olav Bøhmer <bohmer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ruamel-yaml = "^0.17.31"
 configparser = "^5.3.0"
 argparse = "^1.4.0"
+toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 yaml-indent = "yaml_indent.yaml_indent:main"
```

### Comparing `yaml_indent-0.1.2/yaml_indent/yaml_indent.py` & `yaml_indent-0.1.3/yaml_indent/yaml_indent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#!/usr/bin/env python3
 """ A program to indent yaml files """
 import argparse
 import configparser
 import os
 import sys
 from ruamel.yaml import YAML
-
+from . import __version__
 
 def find_config_file(dir_path):
     '''Finds config file for files in dir_path'''
     home_dir = os.path.expanduser("~")  # Home directory path
-    while dir_path != home_dir:  # Stop at the home directory
+    while dir_path != home_dir and dir_path != "/" and dir_path != "":  # Stop at the home directory
+        print(dir_path)
         config_path = os.path.join(dir_path, '.yaml_indent.ini')
         if os.path.exists(config_path):
             return config_path
         # Go up to the parent directory
         dir_path = os.path.dirname(dir_path)
     return None
 
@@ -66,14 +66,16 @@
             print(exc)
 
 
 def main():
     '''Parse arguments and indent files'''
 
     parser = argparse.ArgumentParser()
+    parser.add_argument("-v", "--version", action="version", version=__version__)
+
     parser.add_argument(
         'input_file',
         help='The input YAML file to be indented'
     )
     parser.add_argument(
         '-o', '--output_file', nargs='?',
         default=argparse.SUPPRESS,
```

### Comparing `yaml_indent-0.1.2/PKG-INFO` & `yaml_indent-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: yaml-indent
-Version: 0.1.2
-Summary: 
+Version: 0.1.3
+Summary: Tool for making consistent indentation
 Author: Knut Olav Bøhmer
 Author-email: bohmer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.31,<0.18.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Bug Tracker, https://github.com/knobo/yaml-indent/issues
 Project-URL: Documentation, https://github.com/knobo/yaml-indent/wiki
 Project-URL: Repository, https://github.com/knobo/yaml-indent
 Description-Content-Type: text/markdown
 
 # YAML Indent
 
@@ -43,15 +44,15 @@
 - `-i` (optional) if set, the input file will be edited in place.
 
 If no output file is specified and `-i` is not set, the indented YAML will be printed to the standard output.
 
 ## Configuration
 
 `yaml-indent` looks for a `.yaml_indent.ini` configuration file in the
-current directory and all parent directories up to the home
+the yaml files directory and all parent directories up to the home
 directory. The configuration file should be in the INI format and can
 specify the `mapping`, `sequence`, and `offset` indentation values
 under the `YAML` section.
 
 Here's an example:
 
 ```ini
```

