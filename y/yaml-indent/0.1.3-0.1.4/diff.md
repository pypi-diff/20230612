# Comparing `tmp/yaml_indent-0.1.3.tar.gz` & `tmp/yaml_indent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_indent-0.1.3.tar", max compression
+gzip compressed data, was "yaml_indent-0.1.4.tar", max compression
```

## Comparing `yaml_indent-0.1.3.tar` & `yaml_indent-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-06-08 11:39:30.751856 yaml_indent-0.1.3/LICENSE
--rw-r--r--   0        0        0     1606 2023-06-12 06:59:29.669152 yaml_indent-0.1.3/README.md
--rw-r--r--   0        0        0      663 2023-06-12 10:28:55.990697 yaml_indent-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       34 2023-06-12 07:30:40.480371 yaml_indent-0.1.3/yaml_indent/__init__.py
--rw-r--r--   0        0        0       22 2023-06-12 11:01:58.592620 yaml_indent-0.1.3/yaml_indent/_version.py
--rwxr-xr-x   0        0        0     3062 2023-06-12 10:19:59.516858 yaml_indent-0.1.3/yaml_indent/yaml_indent.py
--rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 yaml_indent-0.1.3/setup.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 yaml_indent-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 11:39:30.751856 yaml_indent-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1606 2023-06-12 06:59:29.669152 yaml_indent-0.1.4/README.md
+-rw-r--r--   0        0        0      663 2023-06-12 14:35:34.350260 yaml_indent-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-12 07:30:40.480371 yaml_indent-0.1.4/yaml_indent/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-12 14:33:39.358055 yaml_indent-0.1.4/yaml_indent/_version.py
+-rwxr-xr-x   0        0        0     4667 2023-06-12 14:31:10.149194 yaml_indent-0.1.4/yaml_indent/yaml_indent.py
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 yaml_indent-0.1.4/setup.py
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 yaml_indent-0.1.4/PKG-INFO
```

### Comparing `yaml_indent-0.1.3/LICENSE` & `yaml_indent-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_indent-0.1.3/README.md` & `yaml_indent-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `yaml_indent-0.1.3/pyproject.toml` & `yaml_indent-0.1.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yaml-indent"
-version = "0.1.3"
+version = "0.1.4"
 description = "Tool for making consistent indentation"
 authors = ["Knut Olav Bøhmer <bohmer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ruamel-yaml = "^0.17.31"
```

### Comparing `yaml_indent-0.1.3/setup.py` & `yaml_indent-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'toml>=0.10.2,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['yaml-indent = yaml_indent.yaml_indent:main']}
 
 setup_kwargs = {
     'name': 'yaml-indent',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Tool for making consistent indentation',
     'long_description': "# YAML Indent\n\n`yaml-indent` is a Python script to re-indent YAML files according to configurable or default indentation rules. It uses the `ruamel.yaml` library for parsing and writing YAML.\n\n## Installation\n\nThe script requires Python 3.\n\n``` sh\npip install yaml-indent\n```\n\n## Usage\n\nYou can run `yaml-indent` from the command line with the following syntax:\n\n``` sh\nyaml-indent <input_file> [-o <output_file>] [-i]\n```\n\nWhere:\n\n- `<input_file>` is the path to the input YAML file to be re-indented.\n- `-o <output_file>` (optional) is the path to the output file where the indented YAML will be written.\n- `-i` (optional) if set, the input file will be edited in place.\n\nIf no output file is specified and `-i` is not set, the indented YAML will be printed to the standard output.\n\n## Configuration\n\n`yaml-indent` looks for a `.yaml_indent.ini` configuration file in the\nthe yaml files directory and all parent directories up to the home\ndirectory. The configuration file should be in the INI format and can\nspecify the `mapping`, `sequence`, and `offset` indentation values\nunder the `YAML` section.\n\nHere's an example:\n\n```ini\n[YAML]\nmapping=4\nsequence=4\noffset=0\n```\n## Contributing\n\nContributions to this project are welcome. If you find a bug or think\nof a feature that this utility could benefit from, please open an\nissue or submit a pull request.\n\n## Source Code\n\nThe source code for this project is hosted on GitHub. You can access\nit at [https://github.com/knobo/yaml-indent](https://github.com/knobo/yaml-indent).\n\n## License\n\nThis project is open source under the terms of the GPL License.\n\n",
     'author': 'Knut Olav Bøhmer',
     'author_email': 'bohmer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `yaml_indent-0.1.3/PKG-INFO` & `yaml_indent-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-indent
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool for making consistent indentation
 Author: Knut Olav Bøhmer
 Author-email: bohmer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

