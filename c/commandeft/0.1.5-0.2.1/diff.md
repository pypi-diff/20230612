# Comparing `tmp/commandeft-0.1.5.tar.gz` & `tmp/commandeft-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandeft-0.1.5.tar", last modified: Mon Jun 12 03:29:50 2023, max compression
+gzip compressed data, was "commandeft-0.2.1.tar", last modified: Mon Jun 12 20:03:57 2023, max compression
```

## Comparing `commandeft-0.1.5.tar` & `commandeft-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,30 @@
--rw-r--r--   0        0        0     1078 2023-06-10 01:12:32.215348 commandeft-0.1.5/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-12 03:13:58.678920 commandeft-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-11 23:37:24.840096 commandeft-0.1.5/commandeft/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009549 commandeft-0.1.5/commandeft/constants/__init__.py
--rw-r--r--   0        0        0     3153 2023-06-11 23:38:27.793749 commandeft-0.1.5/commandeft/constants/consts.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009834 commandeft-0.1.5/commandeft/core/__init__.py
--rw-r--r--   0        0        0     2557 2023-06-12 03:25:45.776795 commandeft-0.1.5/commandeft/core/cli.py
--rw-r--r--   0        0        0      823 2023-06-11 23:38:27.796254 commandeft-0.1.5/commandeft/core/decision.py
--rw-r--r--   0        0        0     1715 2023-06-11 23:38:27.804139 commandeft-0.1.5/commandeft/core/generation.py
--rw-r--r--   0        0        0     1128 2023-06-12 03:26:22.574486 commandeft-0.1.5/commandeft/main.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.010171 commandeft-0.1.5/commandeft/util/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-11 23:38:27.808831 commandeft-0.1.5/commandeft/util/config_util.py
--rw-r--r--   0        0        0      437 2023-06-11 23:38:27.809677 commandeft-0.1.5/commandeft/util/gen_util.py
--rw-r--r--   0        0        0     2729 2023-06-12 03:13:58.680953 commandeft-0.1.5/commandeft/util/interactive_util.py
--rw-r--r--   0        0        0     1664 2023-06-12 03:29:50.096178 commandeft-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 commandeft-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-04 14:54:11.290505 commandeft-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-12 02:51:12.093999 commandeft-0.2.1/README.md
+-rw-r--r--   0        0        0       65 2023-06-12 02:20:42.863520 commandeft-0.2.1/commandeft/.pdm-python
+-rw-r--r--   0        0        0       40 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/.gitignore
+-rw-r--r--   0        0        0     2201 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate
+-rw-r--r--   0        0        0     1493 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3078 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3397 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1782 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1211 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/activate_this.py
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/python -> /usr/bin/python3.8
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/bin/python3.8 -> python
+-rw-r--r--   0        0        0       18 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4311 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      233 2023-06-12 02:20:42.855520 commandeft-0.2.1/commandeft/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0        0 2023-06-04 15:07:15.290389 commandeft-0.2.1/commandeft/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.2.1/commandeft/constants/__init__.py
+-rw-r--r--   0        0        0     3153 2023-06-12 19:43:48.156337 commandeft-0.2.1/commandeft/constants/consts.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.2.1/commandeft/core/__init__.py
+-rw-r--r--   0        0        0     2420 2023-06-12 19:57:38.569171 commandeft-0.2.1/commandeft/core/cli.py
+-rw-r--r--   0        0        0      823 2023-06-12 01:21:44.524959 commandeft-0.2.1/commandeft/core/decision.py
+-rw-r--r--   0        0        0     1715 2023-06-12 01:21:44.524959 commandeft-0.2.1/commandeft/core/generation.py
+-rw-r--r--   0        0        0     1132 2023-06-12 19:57:19.149060 commandeft-0.2.1/commandeft/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.2.1/commandeft/util/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-12 01:21:44.524959 commandeft-0.2.1/commandeft/util/config_util.py
+-rw-r--r--   0        0        0      624 2023-06-12 18:13:27.860557 commandeft-0.2.1/commandeft/util/gen_util.py
+-rw-r--r--   0        0        0     2729 2023-06-12 02:42:06.423316 commandeft-0.2.1/commandeft/util/interactive_util.py
+-rw-r--r--   0        0        0     1644 2023-06-12 20:03:57.355324 commandeft-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 commandeft-0.2.1/PKG-INFO
```

### Comparing `commandeft-0.1.5/LICENSE` & `commandeft-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/README.md` & `commandeft-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/constants/consts.py` & `commandeft-0.2.1/commandeft/constants/consts.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/core/cli.py` & `commandeft-0.2.1/commandeft/core/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 import json
+from importlib.metadata import version
 import click
 import pyperclip
-import toml
 
 
 from commandeft.constants.consts import COMMANDEFT_ASCII_DESC, COMMANDEFT_NORMAL_DESC, CONFIG_FILE_PATH
 from commandeft.core.decision import decide_and_apply_action
 from commandeft.core.generation import generate_command
 from commandeft.util.config_util import validate_configuration
 from commandeft.util.interactive_util import get_configuration_answers, get_prompt
@@ -67,12 +67,9 @@
         validate_configuration()
     command = generate_command(prompt)
     click.echo(click.style("> " + command, fg="green"))
     pyperclip.copy(command)
     click.echo("Command copied to clipboard!")
 
 
-def get_version():
-    with open("pyproject.toml", "r", encoding="utf-8") as pyproject:
-        pyproject_data = toml.load(pyproject)
-        version = pyproject_data["project"]["version"]
-        click.echo(f"v{version}")
+def print_version():
+    click.echo(version("commandeft"))
```

### Comparing `commandeft-0.1.5/commandeft/core/decision.py` & `commandeft-0.2.1/commandeft/core/decision.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/core/generation.py` & `commandeft-0.2.1/commandeft/core/generation.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/main.py` & `commandeft-0.2.1/commandeft/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import click
 
-from commandeft.core.cli import CustomCommand, configuration_mode, get_version, prompt_in_line, interactive_mode
+from commandeft.core.cli import CustomCommand, configuration_mode, print_version, prompt_in_line, interactive_mode
 
 
 def custom_exception_handler(exc_value):
     # Handle the exception
     click.echo(click.style(f"An error occurred:{str(exc_value),}", fg="red"))
     sys.exit(1)
 
@@ -17,15 +17,15 @@
 @click.help_option("-h", "--help")
 @click.option("-v", "--version", help="Show version and exit", is_flag=True)
 @click.option("-c", "--configure", help="Configure commandeft", is_flag=True)
 @click.option("-i", "--interactive", help="Run in interactive mode", is_flag=True)
 @click.option("-p", "--prompt", help="Specify your prompt inline")
 def commandeft(version, configure, interactive, prompt):
     if version:
-        get_version()
+        print_version()
     elif configure:
         configuration_mode()
     elif interactive:
         interactive_mode()
     elif prompt:
         prompt_in_line(prompt)
     else:
```

### Comparing `commandeft-0.1.5/commandeft/util/config_util.py` & `commandeft-0.2.1/commandeft/util/config_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/util/interactive_util.py` & `commandeft-0.2.1/commandeft/util/interactive_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/pyproject.toml` & `commandeft-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "commandeft"
-version = "0.1.5"
+version = "0.2.1"
 description = "CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models."
 readme = "README.md"
 authors = [
     { name = "Petros Sidirokastritis", email = "sidirope@gmail.com" },
 ]
 requires-python = ">=3.8.1, <=3.11.4"
 dependencies = [
@@ -43,15 +43,14 @@
     "six==1.16.0",
     "tiktoken==0.4.0",
     "tqdm==4.65.0",
     "urllib3==2.0.2",
     "wcwidth==0.2.6",
     "yarl<2.0,>=1.0",
     "InquirerPy>=0.3.4",
-    "toml>=0.10.2",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Ferrum-Citadel/commandeft"
```

### Comparing `commandeft-0.1.5/PKG-INFO` & `commandeft-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandeft
-Version: 0.1.5
+Version: 0.2.1
 Summary: CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models.
 Author-Email: Petros Sidirokastritis <sidirope@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Ferrum-Citadel/commandeft
 Requires-Python: <=3.11.4,>=3.8.1
 Requires-Dist: PyJWT==2.7.0
 Requires-Dist: Pygments==2.15.1
@@ -41,15 +41,14 @@
 Requires-Dist: six==1.16.0
 Requires-Dist: tiktoken==0.4.0
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: urllib3==2.0.2
 Requires-Dist: wcwidth==0.2.6
 Requires-Dist: yarl<2.0,>=1.0
 Requires-Dist: InquirerPy>=0.3.4
-Requires-Dist: toml>=0.10.2
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-pep8; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # CommanDeft
```

