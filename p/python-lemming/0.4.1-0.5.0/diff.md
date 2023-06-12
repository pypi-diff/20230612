# Comparing `tmp/python-lemming-0.4.1.tar.gz` & `tmp/python-lemming-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lemming-0.4.1.tar", last modified: Sun Apr  9 18:26:14 2023, max compression
+gzip compressed data, was "python-lemming-0.5.0.tar", last modified: Mon Jun 12 17:16:12 2023, max compression
```

## Comparing `python-lemming-0.4.1.tar` & `python-lemming-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.116500 python-lemming-0.4.1/
--rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     6320 2023-04-09 18:26:14.117501 python-lemming-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5356 2023-03-08 18:21:42.000000 python-lemming-0.4.1/README.md
--rw-rw-rw-   0        0        0     1126 2023-03-08 18:13:58.000000 python-lemming-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0     1447 2023-04-09 18:26:14.130500 python-lemming-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.042501 python-lemming-0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.074504 python-lemming-0.4.1/src/lemming/
--rw-rw-rw-   0        0        0      922 2023-04-09 18:25:14.000000 python-lemming-0.4.1/src/lemming/__init__.py
--rw-rw-rw-   0        0        0    11301 2023-03-08 18:14:19.000000 python-lemming-0.4.1/src/lemming/__main__.py
--rw-rw-rw-   0        0        0    11451 2023-04-09 18:17:18.000000 python-lemming-0.4.1/src/lemming/config.py
--rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.4.1/src/lemming/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-09 18:26:14.115501 python-lemming-0.4.1/src/python_lemming.egg-info/
--rw-rw-rw-   0        0        0     6320 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.4.1/src/python_lemming.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       85 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 18:26:14.000000 python-lemming-0.4.1/src/python_lemming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.808163 python-lemming-0.5.0/
+-rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     6305 2023-06-12 17:16:12.809163 python-lemming-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5341 2023-06-11 12:10:56.000000 python-lemming-0.5.0/README.md
+-rw-rw-rw-   0        0        0     1625 2023-06-12 17:12:49.000000 python-lemming-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1455 2023-06-12 17:16:12.823163 python-lemming-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.720165 python-lemming-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.742164 python-lemming-0.5.0/src/lemming/
+-rw-rw-rw-   0        0        0      922 2023-06-12 17:15:21.000000 python-lemming-0.5.0/src/lemming/__init__.py
+-rw-rw-rw-   0        0        0     9671 2023-06-12 17:12:49.000000 python-lemming-0.5.0/src/lemming/__main__.py
+-rw-rw-rw-   0        0        0    11252 2023-06-12 17:12:49.000000 python-lemming-0.5.0/src/lemming/config.py
+-rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.5.0/src/lemming/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-12 17:16:12.807165 python-lemming-0.5.0/src/python_lemming.egg-info/
+-rw-rw-rw-   0        0        0     6305 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.5.0/src/python_lemming.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 17:16:12.000000 python-lemming-0.5.0/src/python_lemming.egg-info/top_level.txt
```

### Comparing `python-lemming-0.4.1/LICENSE` & `python-lemming-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lemming-0.4.1/PKG-INFO` & `python-lemming-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.4.1
+Version: 0.5.0
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
@@ -61,23 +61,23 @@
 - in the `pyproject.toml` file
 
 Please note, that there must be a `lemming` or `tool.lemming` key in the config file.
 
 The config looks like this:
 
 ```toml
-fail_fast = false  # OPTIONAL, wheter or not immediately quit in case of an error
+fail_fast = false  # OPTIONAL, whether or not immediately quit in case of an error
 
-[[lemming.formatters]]
+[[formatters]]
 packages = ["example"]  # REQUIRED, the package(s) to install with pip (might include versions with "==x.y.z")
 format_command = "{pyexe} -m example {path}"  # REQUIRED, the command to run to format the code ({pyexe} will be replaced with the python executable, {path} with the path passed to Lemming (usually the current working directory: "."))
 check_command = "{pyexe} -m example --check {path}"  # OPTIONAL, the command to run to check the code (stuff will be replaced just like in format_command)
 allow_nonzero_on_format = true  # OPTIONAL, if true it is allowed for the format_command to return a non-zero exit status
 
-[[lemming.linters]]
+[[linters]]
 packages = ["example"]  # REQUIRED, same as for formatters
 command = "{pyexe} -m example {path}"  # REQUIRED, the command to run to lint the code (stuff will be replaced just like in format_command)
 run_first = true  # OPTIONAL, if true this linter will be ran BEFORE formatters, and linters with this being false. Defaults to false.
 ```
 
 ### 2. Run Lemming
```

### Comparing `python-lemming-0.4.1/README.md` & `python-lemming-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 - in the `pyproject.toml` file
 
 Please note, that there must be a `lemming` or `tool.lemming` key in the config file.
 
 The config looks like this:
 
 ```toml
-fail_fast = false  # OPTIONAL, wheter or not immediately quit in case of an error
+fail_fast = false  # OPTIONAL, whether or not immediately quit in case of an error
 
-[[lemming.formatters]]
+[[formatters]]
 packages = ["example"]  # REQUIRED, the package(s) to install with pip (might include versions with "==x.y.z")
 format_command = "{pyexe} -m example {path}"  # REQUIRED, the command to run to format the code ({pyexe} will be replaced with the python executable, {path} with the path passed to Lemming (usually the current working directory: "."))
 check_command = "{pyexe} -m example --check {path}"  # OPTIONAL, the command to run to check the code (stuff will be replaced just like in format_command)
 allow_nonzero_on_format = true  # OPTIONAL, if true it is allowed for the format_command to return a non-zero exit status
 
-[[lemming.linters]]
+[[linters]]
 packages = ["example"]  # REQUIRED, same as for formatters
 command = "{pyexe} -m example {path}"  # REQUIRED, the command to run to lint the code (stuff will be replaced just like in format_command)
 run_first = true  # OPTIONAL, if true this linter will be ran BEFORE formatters, and linters with this being false. Defaults to false.
 ```
 
 ### 2. Run Lemming
```

### Comparing `python-lemming-0.4.1/pyproject.toml` & `python-lemming-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,33 +6,60 @@
 profile = "black"
 
 [tool.ruff]
 select = ["ALL"]
 ignore = [
     "ANN101",
     "ANN102",
-    "COM812",
+    "COM",
     "D",
     "EM102",
     "FBT",
-    "G004",
-    "PGH003",
-    "PLR2004",
-    "RUF100",
-    "TCH002",
+    "T",
     "TRY003",
-    "TRY400",
+    "PLR0913",
 ]
 line-length = 79
 target-version = "py38"
 
-[[tool.lemming.linters]]
-packages = ["ruff"]
-command = "{pyexe} -m ruff check . --show-source"
-run_first = true
+fixable = [
+    "F632",
+    "E711",
+    "F901",
+    "E703",
+    "E712",
+    "E713",
+    "E714",
+    "W291",
+    "W292",
+    "W293",
+    "I001",
+    "PT001",
+    "PT003",
+    "PT006",
+    "PT009",
+    "PT023",
+    "Q",
+    "RSE102",
+    "SIM101",
+    "SIM103",
+    "SIM109",
+    "SIM112",
+    "SIM117",
+    "SIM118",
+    "SIM201",
+    "SIM202",
+    "SIM208",
+    "SIM210",
+    "SIM211",
+    "SIM212",
+]
+
+[tool.ruff.flake8-quotes]
+inline-quotes = "double"
 
 [[tool.lemming.formatters]]
 packages = ["black"]
 format_command = "{pyexe} -m black -l 79 {path}"
 check_command = "{pyexe} -m black -l 79 --check --extend-exclude .*venv.* {path}"
 
 [[tool.lemming.formatters]]
@@ -41,10 +68,15 @@
 # no check
 
 [[tool.lemming.formatters]]
 packages = ["isort"]
 format_command = "{pyexe} -m isort --profile black {path}"
 check_command = "{pyexe} -m isort --profile black -c {path}"
 
+[[tool.lemming.formatters]]
+packages = ["ruff"]
+format_command = "{pyexe} -m ruff check . --show-source --fix -n"
+check_command = "{pyexe} -m ruff check . --show-source --show-fixes -n"
+
 [[tool.lemming.linters]]
 packages = ["pyroma"]
 command = "{pyexe} -m pyroma {path}"
```

### Comparing `python-lemming-0.4.1/setup.cfg` & `python-lemming-0.5.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -58,34 +58,34 @@
 00000390: 670d 0a69 6e73 7461 6c6c 5f72 6571 7569  g..install_requi
 000003a0: 7265 7320 3d20 0d0a 0974 6f6d 6c69 3b20  res = ...tomli; 
 000003b0: 7079 7468 6f6e 5f76 6572 7369 6f6e 3c27  python_version<'
 000003c0: 332e 3131 270d 0a09 7079 7468 6f6e 2d6d  3.11'...python-m
 000003d0: 796c 6f67 3e3d 302e 372e 300d 0a09 636f  ylog>=0.7.0...co
 000003e0: 6e66 7a0d 0a09 7479 7069 6e67 2d65 7874  nfz...typing-ext
 000003f0: 656e 7369 6f6e 733e 3d34 2e34 2e30 0d0a  ensions>=4.4.0..
-00000400: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000410: 3d20 3e3d 332e 3131 0d0a 7061 636b 6167  = >=3.11..packag
-00000420: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
-00000430: 0a7a 6970 5f73 6166 6520 3d20 6e6f 0d0a  .zip_safe = no..
-00000440: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000450: 6765 5f64 6174 615d 0d0a 6c65 6d6d 696e  ge_data]..lemmin
-00000460: 6720 3d20 7079 2e74 7970 6564 0d0a 0d0a  g = py.typed....
-00000470: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-00000480: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-00000490: 7363 7269 7074 7320 3d20 0d0a 096c 656d  scripts = ...lem
-000004a0: 6d69 6e67 203d 206c 656d 6d69 6e67 2e5f  ming = lemming._
-000004b0: 5f6d 6169 6e5f 5f3a 6d61 696e 0d0a 0d0a  _main__:main....
-000004c0: 5b70 7963 6f64 6573 7479 6c65 5d0d 0a69  [pycodestyle]..i
-000004d0: 676e 6f72 6520 3d20 4532 3033 0d0a 0d0a  gnore = E203....
-000004e0: 5b70 796c 616d 615d 0d0a 6967 6e6f 7265  [pylama]..ignore
-000004f0: 203d 2057 3530 330d 0a0d 0a5b 666c 616b   = W503....[flak
-00000500: 6538 5d0d 0a65 7874 656e 642d 6967 6e6f  e8]..extend-igno
-00000510: 7265 203d 2057 3530 330d 0a65 7874 656e  re = W503..exten
-00000520: 642d 6578 636c 7564 6520 3d20 7665 6e76  d-exclude = venv
-00000530: 2c2a 6361 6368 652a 0d0a 7065 722d 6669  ,*cache*..per-fi
-00000540: 6c65 2d69 676e 6f72 6573 203d 200d 0a09  le-ignores = ...
-00000550: 7465 7374 732f 2a3a 2053 3130 310d 0a0d  tests/*: S101...
-00000560: 0a5b 6973 6f72 745d 0d0a 7072 6f66 696c  .[isort]..profil
-00000570: 6520 3d20 626c 6163 6b0d 0a0d 0a5b 6567  e = black....[eg
-00000580: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000590: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000005a0: 3d20 300d 0a0d 0a                        = 0....
+00000400: 0974 7970 6572 0d0a 7079 7468 6f6e 5f72  .typer..python_r
+00000410: 6571 7569 7265 7320 3d20 3e3d 332e 3131  equires = >=3.11
+00000420: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000430: 0d0a 093d 7372 630d 0a7a 6970 5f73 6166  ...=src..zip_saf
+00000440: 6520 3d20 6e6f 0d0a 0d0a 5b6f 7074 696f  e = no....[optio
+00000450: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+00000460: 0d0a 6c65 6d6d 696e 6720 3d20 7079 2e74  ..lemming = py.t
+00000470: 7970 6564 0d0a 0d0a 5b6f 7074 696f 6e73  yped....[options
+00000480: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
+00000490: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
+000004a0: 3d20 0d0a 096c 656d 6d69 6e67 203d 206c  = ...lemming = l
+000004b0: 656d 6d69 6e67 2e5f 5f6d 6169 6e5f 5f3a  emming.__main__:
+000004c0: 6d61 696e 0d0a 0d0a 5b70 7963 6f64 6573  main....[pycodes
+000004d0: 7479 6c65 5d0d 0a69 676e 6f72 6520 3d20  tyle]..ignore = 
+000004e0: 4532 3033 0d0a 0d0a 5b70 796c 616d 615d  E203....[pylama]
+000004f0: 0d0a 6967 6e6f 7265 203d 2057 3530 330d  ..ignore = W503.
+00000500: 0a0d 0a5b 666c 616b 6538 5d0d 0a65 7874  ...[flake8]..ext
+00000510: 656e 642d 6967 6e6f 7265 203d 2057 3530  end-ignore = W50
+00000520: 330d 0a65 7874 656e 642d 6578 636c 7564  3..extend-exclud
+00000530: 6520 3d20 7665 6e76 2c2a 6361 6368 652a  e = venv,*cache*
+00000540: 0d0a 7065 722d 6669 6c65 2d69 676e 6f72  ..per-file-ignor
+00000550: 6573 203d 200d 0a09 7465 7374 732f 2a3a  es = ...tests/*:
+00000560: 2053 3130 310d 0a0d 0a5b 6973 6f72 745d   S101....[isort]
+00000570: 0d0a 7072 6f66 696c 6520 3d20 626c 6163  ..profile = blac
+00000580: 6b0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  k....[egg_info].
+00000590: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000005a0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `python-lemming-0.4.1/src/lemming/__init__.py` & `python-lemming-0.5.0/src/lemming/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 __all__ = ["__version__", "logger"]
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 import mylog
 
 logger = mylog.root.get_child("lemming")
 logger.threshold = mylog.Level.info
```

### Comparing `python-lemming-0.4.1/src/lemming/__main__.py` & `python-lemming-0.5.0/src/lemming/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,83 +12,62 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-# SPDX-License-Identifier: GPL-3.0-or-later
-import argparse
 import pathlib
+import sys
 import time
-from typing import List, Literal, Tuple
+from typing import Annotated, Optional, Self, TypedDict
 
 import mylog
-from confz import ConfZFileSource
-from typing_extensions import Self
 
-from . import __version__, config, logger
+# SPDX-License-Identifier: GPL-3.0-or-later
+import typer
 
-PARSER = argparse.ArgumentParser(
-    description="Lemming is a tool for formatting and linting code.",
-    prog="lemming",
-)
-PARSER.add_argument(
-    "task",
-    choices=("format", "check"),
-    help="format the code with the formatters, or check the code with the"
-    " formatters (linters will be ran in all cases)",
-)
-PARSER.add_argument(
-    "path",
-    action="append",
-    type=pathlib.Path,
-    help="the paths (files and directories) to check. These arguments will be"
-    " passed to the formatters and linters as arguments where {path} is used",
-)
-PARSER.add_argument(
-    "-v",
-    "--verbose",
-    action="store_true",
-    help="log more information",
-)
-PARSER.add_argument(
-    "-q",
-    "--quiet",
-    action="count",
-    help="log less information. Can be passed multiple times",
-    default=0,
-)
-PARSER.add_argument(
-    "--quiet-commands",
-    action="store_true",
-    help="don't let ran commands write to stdout and stderr. Use --quiet-pip"
-    " to quiet `pip`",
-)
-PARSER.add_argument(
-    "--quiet-pip",
-    action="store_true",
-    help="don't let pip write to stdout and stderr. Use --quiet-commands"
-    " to quiet the formatters and linters",
-)
-PARSER.add_argument(
-    "-c",
-    "--config",
-    default=None,
-    help="the config file to use. If passed all other config files will be"
-    " ignored",
-)
-PARSER.add_argument(
-    "-V",
-    "--version",
-    action="version",
-    help="print the program's version and exit",
-    version=__version__,
+from . import __version__, logger
+from .config import (
+    Config,
+    Formatter,
+    Linter,
+    WhatToQuiet,
+    get_config,
+    get_config_dot_lemming,
+    get_config_pyproject,
 )
 
+PRE_COMMIT_FILE = """#!/bin/sh
+#!/usr/bin/env bash
+# File generated by Lemming: https://github.com/koviubi56/lemming
+
+set -e
+PYTHON='{}'
+
+if [[ -n $LEMMING_VERBOSE ]]; then
+    exec $PYTHON -m lemming format -v $(pwd)
+    ret_code=$?
+else
+    exec $PYTHON -m lemming -q --quiet-pip format "$(pwd)"
+    ret_code=$?
+fi
+exit $ret_code
+"""
+
+app = typer.Typer(no_args_is_help=True)
+
+
+class _Settings(TypedDict):
+    what_to_quiet: WhatToQuiet
+    config: Config
+
+
+SETTINGS: _Settings
+
 
 class Timer:
     def __init__(self) -> None:
         self.start = None
         self.time = None
 
     def __enter__(self) -> Self:
@@ -96,254 +75,242 @@
         return self
 
     def __exit__(self, *_: object) -> None:
         assert self.start  # noqa: S101
         self.time = time.perf_counter() - self.start
 
 
-def parse_args() -> argparse.Namespace:
-    return PARSER.parse_args()
-
-
-def _get_paths_to_check(args: argparse.Namespace) -> List[pathlib.Path]:
-    paths_to_check = args.path
-    logger.debug(f"{paths_to_check = !r}")
-    if not (
-        isinstance(paths_to_check, list)
-        and all(isinstance(path, pathlib.Path) for path in paths_to_check)
-    ):
-        PARSER.error("invalid paths")
-    return paths_to_check
-
-
-def _set_logger(args: argparse.Namespace) -> None:
-    verbose = args.verbose
-    quiet = args.quiet
-    logger.debug(f"{verbose = !r}")
-    logger.debug(f"{quiet = !r}")
-    if verbose and quiet:
-        PARSER.error("cannot have both verbose and quiet")
-    if quiet >= 4:
-        logger.handlers = []
-    elif quiet == 3:
-        logger.threshold = mylog.Level.critical
-    elif quiet == 2:
-        logger.threshold = mylog.Level.error
-    elif quiet == 1:
-        logger.threshold = mylog.Level.warning
-    if verbose:
-        logger.threshold = mylog.Level.debug
-    logger.debug(f"{logger.threshold = !r}")
-
-
-def _get_what_to_quiet(args: argparse.Namespace) -> config.WhatToQuiet:
-    return config.WhatToQuiet(args.quiet_commands, args.quiet_pip)
-
-
-def _get_config_file(args: argparse.Namespace) -> pathlib.Path:
-    config_file = args.config
-    logger.debug(f"{config_file = !r}")
-    if config_file is not None:
-        config_file = pathlib.Path(config_file).resolve()
-        if not config_file.exists():
-            PARSER.error(f"config file {config_file} doesn't exist")
-        if not config_file.is_file():
-            PARSER.error(f"config file {config_file} isn't a file")
-    logger.debug(f"{config_file = !r}")
-    return config_file
-
-
-def _get_configuration_configprovided(
-    config_file: pathlib.Path,
-) -> config.Config:
-    logger.debug("config_file is provided, using that")
-    return config.Config(ConfZFileSource(file=config_file))
-
-
-def _get_configuration_confignotprovided() -> config.Config:
-    logger.debug("config_file is None, searching for it")
-    return config.get_config(".")
-
-
-def _get_configuration(args: argparse.Namespace) -> config.Config:
-    # sourcery skip: assign-if-exp, inline-immediately-returned-variable
-    config_file = _get_config_file(args)
-
-    if config_file:
-        return _get_configuration_configprovided(config_file)
-    return _get_configuration_confignotprovided()
-
-
-def get_configuration() -> (
-    Tuple[
-        config.Config,
-        List[pathlib.Path],
-        config.WhatToQuiet,
-        Literal["format", "check"],
-    ]
-):
-    logger.debug("Parsing args")
-    with logger.ctxmgr:
-        args = parse_args()
-
-        paths_to_check = _get_paths_to_check(args)
-
-        _set_logger(args)
-
-        configuration = _get_configuration(args)
-
-        what_to_quiet = _get_what_to_quiet(args)
-
-        task = args.task
-    return configuration, paths_to_check, what_to_quiet, task
-
-
-def _formatters(
-    configuration: config.Config,
-    paths_to_check: List[pathlib.Path],
-    what_to_quiet: config.WhatToQuiet,
-    task: Literal["format", "check"],
-) -> bool:
-    logger.info(f"Running formatters ({task})")
-    with logger.ctxmgr:
-        with Timer() as formatters_timer:
-            for formatter in configuration.formatters:
-                logger.info(f"Running formatter {formatter.packages} ({task})")
-                with logger.ctxmgr:
-                    with Timer() as formatter_timer:
-                        if task == "format":
-                            success = formatter.run_format(
-                                paths_to_check, what_to_quiet
-                            )
-                        elif task == "check":
-                            success = formatter.run_check(
-                                paths_to_check, what_to_quiet
-                            )
-                        else:
-                            PARSER.error(f"unknown task: {task!r}")
-
-                        if not success:
-                            logger.error(
-                                "Could not run formatter"
-                                f" {formatter.packages}!"
-                            )
-                            if configuration.fail_fast:
-                                PARSER.exit(1, "\nFAILED!\n")
-                            else:
-                                return False
-                    logger.info(
-                        f"Ran formatter in {formatter_timer.time} seconds"
-                    )
-        logger.info(f"Ran all formatters in {formatters_timer.time} seconds")
-        return True
-
-
-def _run_linter(
-    configuration: config.Config,
-    paths_to_check: List[pathlib.Path],
-    what_to_quiet: config.WhatToQuiet,
-    linter: config.Linter,
-) -> bool:
+def run_linter(linter: Linter, paths: list[pathlib.Path]) -> bool:
     with logger.ctxmgr:
         with Timer() as linter_timer:
-            success = linter.run(paths_to_check, what_to_quiet)
+            success = linter.run(paths, SETTINGS["what_to_quiet"])
             if not success:
                 logger.error(
                     f"Could not run linter {linter.packages}!"
                     " Please see the linter's output for more"
                     " details."
                 )
-                if configuration.fail_fast:
-                    PARSER.exit(1, "\nFAILED!\n")
-                else:
-                    return False
+                if SETTINGS["config"].fail_fast:
+                    raise typer.Exit(1)
+                return False
         logger.info(f"Ran linter in {linter_timer.time} seconds")
         return True
 
 
-def _linters_first(
-    configuration: config.Config,
-    paths_to_check: List[pathlib.Path],
-    what_to_quiet: config.WhatToQuiet,
-) -> bool:
-    logger.info("Running (first) linters")
+def linter_first(paths: list[pathlib.Path]) -> bool:
+    logger.info("Running first linters")
     return_value = True
     with logger.ctxmgr:
         with Timer() as linters_timer:
-            for linter in configuration.get_first_linters():
-                logger.info(f"Running (first) linter {linter.packages}")
-                success = _run_linter(
-                    configuration, paths_to_check, what_to_quiet, linter
-                )
+            for linter in SETTINGS["config"].get_first_linters():
+                logger.info(f"Running first linter {linter.packages}")
+                success = run_linter(linter, paths)
                 if not success:
                     return_value = False
         logger.info(f"Ran all (first) linters in {linters_timer.time} seconds")
         return return_value
 
 
-def _linters_other(
-    configuration: config.Config,
-    paths_to_check: List[pathlib.Path],
-    what_to_quiet: config.WhatToQuiet,
-) -> None:
-    logger.info("Running (other) linters")
-    return_value = True
+def run_formatter(
+    formatter: Formatter, paths: list[pathlib.Path], format_: bool
+) -> bool:
     with logger.ctxmgr:
-        with Timer() as linters_timer:
-            for linter in configuration.get_other_linters():
-                logger.info(f"Running (other) linter {linter.packages}")
-                success = _run_linter(
-                    configuration, paths_to_check, what_to_quiet, linter
+        with Timer() as formatter_timer:
+            if format_:
+                success = formatter.run_format(
+                    paths, SETTINGS["what_to_quiet"]
                 )
+            else:
+                success = formatter.run_check(paths, SETTINGS["what_to_quiet"])
+
+            if not success:
+                logger.error(f"Could not run formatter {formatter.packages}!")
+                if SETTINGS["config"].fail_fast:
+                    raise typer.Exit(1)
+                return False
+        logger.info(f"Ran formatter in {formatter_timer.time} seconds")
+        return True
+
+
+def formatter(format_: bool, paths: list[pathlib.Path]) -> bool:
+    logger.info("Running formatters")
+    return_value = True
+    with logger.ctxmgr:
+        with Timer() as formatters_timer:
+            for formatter in SETTINGS["config"].formatters:
+                logger.info(f"Running formatter {formatter.packages}")
+                success = run_formatter(formatter, paths, format_)
                 if not success:
                     return_value = False
-        logger.info(f"Ran all (other) linters in {linters_timer.time} seconds")
+        logger.info(f"Ran all formatters in {formatters_timer.time} seconds")
         return return_value
 
 
-def main() -> None:
-    with Timer() as all_timer:
-        with Timer() as config_timer:
-            (
-                configuration,
-                paths_to_check,
-                what_to_quiet,
-                task,
-            ) = get_configuration()
-        logger.debug(
-            f"Got configuration {configuration} in {config_timer.time} seconds"
-        )
-
-        linter_first_success = _linters_first(
-            configuration, paths_to_check, what_to_quiet
-        )
+def linter_other(paths: list[pathlib.Path]) -> bool:
+    logger.info("Running other linters")
+    return_value = True
+    with logger.ctxmgr:
+        with Timer() as linters_timer:
+            for linter in SETTINGS["config"].get_other_linters():
+                logger.info(f"Running other linter {linter.packages}")
+                success = run_linter(linter, paths)
+                if not success:
+                    return_value = False
+        logger.info(f"Ran all other linters in {linters_timer.time} seconds")
+        return return_value
 
-        formatter_success = _formatters(
-            configuration, paths_to_check, what_to_quiet, task
-        )
 
-        linter_other_success = _linters_other(
-            configuration, paths_to_check, what_to_quiet
-        )
+def run(paths: list[pathlib.Path], format_: bool) -> None:
+    with Timer() as all_timer:
+        success = True
+        if linter_first(paths) is False:
+            success = False
+        if formatter(format_, paths) is False:
+            success = False
+        if linter_other(paths) is False:
+            success = False
 
-        if not all(
-            (linter_first_success, formatter_success, linter_other_success)
-        ):
+        if not success:
             logger.error(
-                "Failed, due to one or more linters/formatters failing."
+                "Failed, due to one or more linters/formatters failing. (HINT:"
+                " Set fail_fast=true to disable this behavior)"
             )
-            logger.error("HINT: Set fail_fast=true to disable this behavior")
-            PARSER.exit(1, "\nFAILED\n")
-
+            raise typer.Exit(1)
     logger.info(
         f"Successfully ran all formatters and linters in {all_timer.time}"
         " seconds with no errors. Good job!"
     )
-    if not what_to_quiet.pip:
-        logger.info(
-            "*!*!* HINT: Do you get overwhelmed by pip's output? Consider"
-            " using the --quiet-pip argument for Lemming !*!*!"
+
+
+def quiet_callback(value: bool) -> None:
+    if value:
+        logger.threshold += 10
+
+
+def version_callback(value: bool) -> None:
+    if value:
+        print(__version__)
+        raise typer.Exit(0)
+
+
+@app.command("format")
+def format_(
+    paths: Annotated[list[pathlib.Path], typer.Argument(exists=True)]
+) -> None:
+    """Format your code and run linters."""
+    run(paths, True)
+
+
+@app.command()
+def check(
+    paths: Annotated[list[pathlib.Path], typer.Argument(exists=True)]
+) -> None:
+    """Check the formatting of your code and run linters."""
+    run(paths, False)
+
+
+def install_pre_commit(git_repository: pathlib.Path) -> None:
+    if not git_repository.exists():
+        logger.critical(f"Directory {git_repository} does not exist!")
+        raise typer.Exit(1)
+    git_directory = git_repository / ".git"
+    if not git_directory.exists():
+        logger.critical(f"Directory {git_repository} is not a git repository!")
+        raise typer.Exit(1)
+    pre_commit = git_directory / "hooks" / "pre-commit"
+    if pre_commit.exists():
+        logger.warning(
+            f"pre-commit file {pre_commit} already exists! Overwriting..."
+        )
+    logger.info(f"Creating pre-commit git hook (it will use {sys.executable})")
+    try:
+        pre_commit.write_text(PRE_COMMIT_FILE.format(sys.executable))
+    except OSError as exception:
+        logger.critical("Could not write pre-commit file!", True)
+        raise typer.Exit(1) from exception
+    logger.info("Successfully written pre-commit!")
+
+
+@app.command("pre-commit")
+def pre_commit(
+    git_repository: Annotated[
+        pathlib.Path,
+        typer.Option(
+            default_factory=pathlib.Path.cwd, exists=True, file_okay=False
+        ),
+    ]
+) -> None:
+    """Install a pre-commit git hook which will run Lemming."""
+    install_pre_commit(git_repository)
+
+
+@app.callback()
+def callback(
+    _version: Annotated[
+        bool,
+        typer.Option(
+            "--version",
+            "-V",
+            help="Print the version of Lemming and exit.",
+            callback=version_callback,
+        ),
+    ] = False,
+    quiet_commands: Annotated[
+        bool,
+        typer.Option(
+            help="If passed the output of the formatters and linters will be"
+            " hidden.",
+        ),
+    ] = False,
+    quiet_pip: Annotated[
+        bool,
+        typer.Option(
+            help="If passed the output of pip will be hidden.",
+        ),
+    ] = False,
+    verbose: Annotated[
+        bool,
+        typer.Option(
+            "--verbose",
+            "-v",
+            help="If passed the logger's threshold will be set to debug.",
+        ),
+    ] = False,
+    quiet: Annotated[
+        bool,
+        typer.Option(
+            "--quiet",
+            "-q",
+            callback=quiet_callback,
+            help="When passed the logger's threshold will be increased by 10"
+            " (may be passed multiple times)",
+        ),
+    ] = False,
+    config: Annotated[
+        Optional[pathlib.Path],
+        typer.Option(
+            exists=True, dir_okay=False, help="The config file to use."
+        ),
+    ] = None,
+) -> None:
+    if verbose:
+        if quiet:
+            logger.critical("Verbose and quiet are mutually exclusive!")
+            raise typer.Exit(2)
+        logger.threshold = mylog.Level.debug
+    if config:
+        config_ = (
+            get_config_pyproject(config)
+            if config.name == "pyproject.toml"
+            else get_config_dot_lemming(config.parent)
         )
+    else:
+        config_ = get_config(".")
+    global SETTINGS  # noqa: PLW0603
+    SETTINGS = _Settings(
+        what_to_quiet=WhatToQuiet(commands=quiet_commands, pip=quiet_pip),
+        config=config_,
+    )
 
 
 if __name__ == "__main__":
-    main()
+    app()
```

### Comparing `python-lemming-0.4.1/src/lemming/config.py` & `python-lemming-0.5.0/src/lemming/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,21 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import pathlib
 import shlex
-import subprocess  # noqa: S404
+import subprocess
 import sys
-from typing import (
-    AnyStr,
-    Iterable,
-    List,
-    Mapping,
-    MutableSequence,
-    Optional,
-    Protocol,
-    Union,
-)
+from typing import Iterable, List, Mapping, MutableSequence, Optional, Union
 
 from confz import ConfZ, ConfZFileSource
 from confz.exceptions import ConfZFileException
-from typing_extensions import NamedTuple, Self, TypeAlias, TypeVar
+from typing_extensions import NamedTuple, Self, TypeVar
 
 from . import logger
 
 try:
     import tomllib  # novermin
 except Exception:  # noqa: BLE001
     import tomli as tomllib
@@ -53,22 +44,14 @@
     "The found pyproject.toml file has no tool.lemming key!"
     # we don't actually check for "tool.lemming" key.
     # we search for config["tool"]["lemming"]
 )
 T = TypeVar("T")
 
 
-class _PathLike(Protocol):
-    def __fspath__(self) -> AnyStr:
-        ...
-
-
-PathLike: TypeAlias = Union[_PathLike, AnyStr]
-
-
 class WhatToQuiet(NamedTuple):
     commands: bool
     pip: bool
 
 
 def assert_dict_keys(
     dictionary: Iterable[T], keys: MutableSequence[T]
@@ -161,19 +144,19 @@
         Returns:
             bool: `exit_status == 0`
         """
         command = self.replace_command(command, paths_to_check)
 
         splitted = shlex.split(command, posix=os.name != "nt")
         logger.debug(f"Running command {splitted!r}")
-        completed_process = subprocess.run(  # noqa: S603
+        completed_process = subprocess.run(
             splitted,
             check=False,
             capture_output=quiet,
-            shell=False,
+            shell=False,  # noqa: S603
         )
         exit_status = completed_process.returncode
         if exit_status == 0:
             logger.info(f"Successfully ran command {command!r}")
             return True
         logger.error(
             f"Command {command!r} returned non-zero exit status {exit_status}"
@@ -342,16 +325,16 @@
     try:
         lemming_config = pyproject_config["tool"]["lemming"]
     except KeyError as exception:
         raise CONFIG_HAS_NO_LEMMING_STUFF from exception
     return Config(**lemming_config)
 
 
-def get_config(folder: PathLike) -> None:
-    folder = pathlib.Path(folder)
+def get_config(_folder: Union[os.PathLike[str], str]) -> Config:
+    folder = pathlib.Path(_folder)
     try:
         # try .lemming.toml
         return get_config_dot_lemming(folder)
     except ConfZFileException:
         # try pyproject.toml
         pyproject = folder / "pyproject.toml"
         if not pyproject.exists():
```

### Comparing `python-lemming-0.4.1/src/python_lemming.egg-info/PKG-INFO` & `python-lemming-0.5.0/src/python_lemming.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.4.1
+Version: 0.5.0
 Summary: Lemming is a tool for formatting and linting code.
 Home-page: https://github.com/koviubi56/lemming
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: lemming,format,formatter,lint,linting,linter
 Platform: unix
@@ -61,23 +61,23 @@
 - in the `pyproject.toml` file
 
 Please note, that there must be a `lemming` or `tool.lemming` key in the config file.
 
 The config looks like this:
 
 ```toml
-fail_fast = false  # OPTIONAL, wheter or not immediately quit in case of an error
+fail_fast = false  # OPTIONAL, whether or not immediately quit in case of an error
 
-[[lemming.formatters]]
+[[formatters]]
 packages = ["example"]  # REQUIRED, the package(s) to install with pip (might include versions with "==x.y.z")
 format_command = "{pyexe} -m example {path}"  # REQUIRED, the command to run to format the code ({pyexe} will be replaced with the python executable, {path} with the path passed to Lemming (usually the current working directory: "."))
 check_command = "{pyexe} -m example --check {path}"  # OPTIONAL, the command to run to check the code (stuff will be replaced just like in format_command)
 allow_nonzero_on_format = true  # OPTIONAL, if true it is allowed for the format_command to return a non-zero exit status
 
-[[lemming.linters]]
+[[linters]]
 packages = ["example"]  # REQUIRED, same as for formatters
 command = "{pyexe} -m example {path}"  # REQUIRED, the command to run to lint the code (stuff will be replaced just like in format_command)
 run_first = true  # OPTIONAL, if true this linter will be ran BEFORE formatters, and linters with this being false. Defaults to false.
 ```
 
 ### 2. Run Lemming
```

