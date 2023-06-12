# Comparing `tmp/oooenv-0.2.0.tar.gz` & `tmp/oooenv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooenv-0.2.0.tar", max compression
+gzip compressed data, was "oooenv-0.2.1.tar", max compression
```

## Comparing `oooenv-0.2.0.tar` & `oooenv-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-06-04 18:27:08.699098 oooenv-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.700098 oooenv-0.2.0/oooenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.701098 oooenv-0.2.0/oooenv/cli/__init__.py
--rw-r--r--   0        0        0     7915 2023-06-04 22:24:59.402702 oooenv-0.2.0/oooenv/cli/main.py
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.702098 oooenv-0.2.0/oooenv/cmds/__init__.py
--rw-r--r--   0        0        0      174 2023-06-04 18:27:08.703098 oooenv-0.2.0/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5103 2023-06-04 18:27:08.703098 oooenv-0.2.0/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
--rw-r--r--   0        0        0     2841 2023-06-04 18:27:08.704098 oooenv-0.2.0/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
--rw-r--r--   0        0        0     5767 2023-06-04 21:30:23.424740 oooenv-0.2.0/oooenv/cmds/manage_env_cfg.py
--rw-r--r--   0        0        0     4627 2023-06-04 18:55:26.719972 oooenv-0.2.0/oooenv/cmds/uno_lnk.py
--rw-r--r--   0        0        0     1255 2023-06-04 21:24:47.067335 oooenv-0.2.0/oooenv/cmds/updater.py
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.705098 oooenv-0.2.0/oooenv/utils/__init__.py
--rw-r--r--   0        0        0      175 2023-06-04 18:27:08.705098 oooenv-0.2.0/oooenv/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3710 2023-06-04 18:27:08.706099 oooenv-0.2.0/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
--rw-r--r--   0        0        0     1146 2023-06-04 18:27:08.706099 oooenv-0.2.0/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
--rw-r--r--   0        0        0     5887 2023-06-04 18:27:08.707099 oooenv-0.2.0/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
--rw-r--r--   0        0        0     3708 2023-06-04 18:27:08.707099 oooenv-0.2.0/oooenv/utils/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0     3169 2023-06-04 18:38:49.468518 oooenv-0.2.0/oooenv/utils/local_paths.py
--rw-r--r--   0        0        0      773 2023-06-04 18:47:20.056527 oooenv-0.2.0/oooenv/utils/sys_info.py
--rw-r--r--   0        0        0     8556 2023-06-04 18:46:57.785630 oooenv-0.2.0/oooenv/utils/uno_paths.py
--rw-r--r--   0        0        0     1419 2023-06-04 20:46:14.586346 oooenv-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1491 2023-06-04 22:31:23.476204 oooenv-0.2.0/README.md
--rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 oooenv-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-04 18:27:08.699098 oooenv-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.700098 oooenv-0.2.1/oooenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.701098 oooenv-0.2.1/oooenv/cli/__init__.py
+-rw-r--r--   0        0        0     8066 2023-06-12 21:27:05.393663 oooenv-0.2.1/oooenv/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.702098 oooenv-0.2.1/oooenv/cmds/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-04 18:27:08.703098 oooenv-0.2.1/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5103 2023-06-04 18:27:08.703098 oooenv-0.2.1/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
+-rw-r--r--   0        0        0     2841 2023-06-04 18:27:08.704098 oooenv-0.2.1/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
+-rw-r--r--   0        0        0      909 2023-06-12 21:32:53.696519 oooenv-0.2.1/oooenv/cmds/install.py
+-rw-r--r--   0        0        0     5767 2023-06-04 22:49:18.217130 oooenv-0.2.1/oooenv/cmds/manage_env_cfg.py
+-rw-r--r--   0        0        0     4627 2023-06-04 22:49:18.219134 oooenv-0.2.1/oooenv/cmds/uno_lnk.py
+-rw-r--r--   0        0        0     1216 2023-06-04 22:49:18.220132 oooenv-0.2.1/oooenv/cmds/updater.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:27:08.705098 oooenv-0.2.1/oooenv/utils/__init__.py
+-rw-r--r--   0        0        0      175 2023-06-04 18:27:08.705098 oooenv-0.2.1/oooenv/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3710 2023-06-04 18:27:08.706099 oooenv-0.2.1/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     1146 2023-06-04 18:27:08.706099 oooenv-0.2.1/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
+-rw-r--r--   0        0        0     5887 2023-06-04 18:27:08.707099 oooenv-0.2.1/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
+-rw-r--r--   0        0        0     3708 2023-06-04 18:27:08.707099 oooenv-0.2.1/oooenv/utils/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0     3169 2023-06-12 21:31:08.327054 oooenv-0.2.1/oooenv/utils/local_paths.py
+-rw-r--r--   0        0        0      773 2023-06-04 22:49:18.223133 oooenv-0.2.1/oooenv/utils/sys_info.py
+-rw-r--r--   0        0        0     8556 2023-06-04 22:49:18.224131 oooenv-0.2.1/oooenv/utils/uno_paths.py
+-rw-r--r--   0        0        0     1419 2023-06-12 20:44:28.886808 oooenv-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1804 2023-06-12 21:44:02.586192 oooenv-0.2.1/README.md
+-rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 oooenv-0.2.1/PKG-INFO
```

### Comparing `oooenv-0.2.0/LICENSE` & `oooenv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/cli/main.py` & `oooenv-0.2.1/oooenv/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # coding: utf-8
 from __future__ import annotations
 import importlib.metadata
 import argparse
 import sys
 import os
 from pathlib import Path
-from oooenv.cmds import uno_lnk, manage_env_cfg, updater
+from oooenv.cmds import uno_lnk, manage_env_cfg, updater, install
 from oooenv.utils import local_paths
 
+
 # region parser
 
 # region        Create Parsers
 
 
 def _create_parser(name: str) -> argparse.ArgumentParser:
     return argparse.ArgumentParser(description=name)
@@ -104,22 +105,14 @@
         "-c",
         "--custom-env",
         help="Set a custom environment. cfg file must exist and be manually configured. Value is suffix of cfg file. For example: -c myenv will use pyenv_myenv.cfg",
         action="store",
         dest="custom_env",
         required=False,
     )
-    parser.add_argument(
-        "-v",
-        "--version",
-        help="Displays the current version of LiberOffice Python. This is parsed from LibreOffice Python executable.",
-        action="store_true",
-        dest="lo_py_version",
-        default=False,
-    )
 
 
 def _args_action_cmd_toggle_env(a_parser: argparse.ArgumentParser, args: argparse.Namespace) -> None:
     if args.uno_env:
         if manage_env_cfg.is_env_uno_python():
             print("UNO Environment")
         else:
@@ -210,21 +203,34 @@
         "-v",
         "--version",
         help="Show the current version of oooenv.",
         action="store_true",
         dest="show_version",
         default=False,
     )
+    parser.add_argument(
+        "-e",
+        "--editable",
+        help="Install a project in editable mode from the local project path. Similar to pip install -e .",
+        action="store_true",
+        dest="editable",
+        default=False,
+    )
 
 
 def _args_action_global(a_parser: argparse.ArgumentParser, args: argparse.Namespace) -> str | None:
     # sourcery skip: assign-if-exp, reintroduce-else
     if args.show_version:
         # return importlib.metadata.version(__package__ or __name__)
         return importlib.metadata.version("oooenv")
+    if args.editable:
+        if result := install.pip_e():
+            return result
+        else:
+            return "Install Failed for unknown reason."
     return None
 
 
 # endregion process arg command for global
 
 # endregion parser
```

### Comparing `oooenv-0.2.0/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc` & `oooenv-0.2.1/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc` & `oooenv-0.2.1/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/cmds/manage_env_cfg.py` & `oooenv-0.2.1/oooenv/cmds/manage_env_cfg.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/cmds/uno_lnk.py` & `oooenv-0.2.1/oooenv/cmds/uno_lnk.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/utils/__pycache__/local_paths.cpython-310.pyc` & `oooenv-0.2.1/oooenv/utils/__pycache__/local_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/utils/__pycache__/sys_info.cpython-310.pyc` & `oooenv-0.2.1/oooenv/utils/__pycache__/sys_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc` & `oooenv-0.2.1/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/utils/__pycache__/util.cpython-310.pyc` & `oooenv-0.2.1/oooenv/utils/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/utils/local_paths.py` & `oooenv-0.2.1/oooenv/utils/local_paths.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/utils/sys_info.py` & `oooenv-0.2.1/oooenv/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/oooenv/utils/uno_paths.py` & `oooenv-0.2.1/oooenv/utils/uno_paths.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.0/pyproject.toml` & `oooenv-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooenv"
-version = "0.2.0"
+version = "0.2.1"
 description = "Configures a project python environment for LibreOffice UNO."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 keywords = ["libreoffice", "macro", "uno", "ooouno", "venv"]
 homepage = "https://github.com/Amourspirit/python_oooenv"
 documentation = "https://github.com/Amourspirit/python_oooenv"
 repository = "https://github.com/Amourspirit/python_oooenv"
 license = "MIT"
```

### Comparing `oooenv-0.2.0/README.md` & `oooenv-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 # OOOENV
 
 This project is strictly for LibreOffice python projects that need to set UNO environment.
 
 A project as [OOO Development Tools](https://python-ooo-dev-tools.readthedocs.io/en/latest/index.html) would use this project
 
-See also [OOO Development Tools - Develop Docs](https://python-ooo-dev-tools.readthedocs.io/en/latest/dev_docs/dev_notes.html)
+See also:
+
+- [LibreOffice Virtual Environment Guides](https://python-ooo-dev-tools.readthedocs.io/en/latest/guide/virtual_env/index.html)
+- [OOO Development Tools - Develop Docs](https://python-ooo-dev-tools.readthedocs.io/en/latest/dev_docs/dev_notes.html)
+- [LibreOffice Python Script Modern Code Editor Examples](https://github.com/Amourspirit/libreoffice-modern-code-editing-py)
 
 ## Installation
 
 **oooenv** [PyPI](https://pypi.org/project/oooenv)
 
-```
+```shell
 pip install oooenv
 ```
 
 ## Usage
 
+View command options
+
+```shell
+oooenv -h
+```
+
 ### Linux/Mac
 
 In Linux and Mac all that is needed to run a project that requires LibreOffice UNO
 is to link the UNO files into virtual environment.
 
 To add UNO links to virtual environment run command:
 
-```sh
+```shell
 oooenv cmd-link -a
 ```
 
 To remove UNO links from virtual environment run command:
 
-```sh
+```shell
 oooenv cmd-link -r
 ```
 
 ### Windows
 
 Windows python projects cannot use linking to UNO Files.
 
@@ -41,15 +51,15 @@
 
 The Follow command toggles between original configuration and UNO environment configuration.
 
 ```powershell
 oooenv env -t
 ```
 
-To update the configuration to match the installed verison of LibreOffice's python.
+To update the configuration to match the installed version of LibreOffice's python.
 
 This command should not be run until `oooenv env -t` has be run at least once.
 
 ```powershell
 oooenv update --update
 ```
```

### Comparing `oooenv-0.2.0/PKG-INFO` & `oooenv-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oooenv
-Version: 0.2.0
+Version: 0.2.1
 Summary: Configures a project python environment for LibreOffice UNO.
 Home-page: https://github.com/Amourspirit/python_oooenv
 License: MIT
 Keywords: libreoffice,macro,uno,ooouno,venv
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -25,40 +25,50 @@
 
 # OOOENV
 
 This project is strictly for LibreOffice python projects that need to set UNO environment.
 
 A project as [OOO Development Tools](https://python-ooo-dev-tools.readthedocs.io/en/latest/index.html) would use this project
 
-See also [OOO Development Tools - Develop Docs](https://python-ooo-dev-tools.readthedocs.io/en/latest/dev_docs/dev_notes.html)
+See also:
+
+- [LibreOffice Virtual Environment Guides](https://python-ooo-dev-tools.readthedocs.io/en/latest/guide/virtual_env/index.html)
+- [OOO Development Tools - Develop Docs](https://python-ooo-dev-tools.readthedocs.io/en/latest/dev_docs/dev_notes.html)
+- [LibreOffice Python Script Modern Code Editor Examples](https://github.com/Amourspirit/libreoffice-modern-code-editing-py)
 
 ## Installation
 
 **oooenv** [PyPI](https://pypi.org/project/oooenv)
 
-```
+```shell
 pip install oooenv
 ```
 
 ## Usage
 
+View command options
+
+```shell
+oooenv -h
+```
+
 ### Linux/Mac
 
 In Linux and Mac all that is needed to run a project that requires LibreOffice UNO
 is to link the UNO files into virtual environment.
 
 To add UNO links to virtual environment run command:
 
-```sh
+```shell
 oooenv cmd-link -a
 ```
 
 To remove UNO links from virtual environment run command:
 
-```sh
+```shell
 oooenv cmd-link -r
 ```
 
 ### Windows
 
 Windows python projects cannot use linking to UNO Files.
 
@@ -66,15 +76,15 @@
 
 The Follow command toggles between original configuration and UNO environment configuration.
 
 ```powershell
 oooenv env -t
 ```
 
-To update the configuration to match the installed verison of LibreOffice's python.
+To update the configuration to match the installed version of LibreOffice's python.
 
 This command should not be run until `oooenv env -t` has be run at least once.
 
 ```powershell
 oooenv update --update
 ```
```

