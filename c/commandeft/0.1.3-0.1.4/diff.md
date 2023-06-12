# Comparing `tmp/commandeft-0.1.3.tar.gz` & `tmp/commandeft-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandeft-0.1.3.tar", last modified: Mon Jun 12 01:48:54 2023, max compression
+gzip compressed data, was "commandeft-0.1.4.tar", last modified: Mon Jun 12 03:08:18 2023, max compression
```

## Comparing `commandeft-0.1.3.tar` & `commandeft-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,30 @@
--rw-r--r--   0        0        0     1078 2023-06-04 14:54:11.290505 commandeft-0.1.3/LICENSE
--rw-r--r--   0        0        0     3334 2023-06-12 01:21:44.524959 commandeft-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-06-04 15:07:15.290389 commandeft-0.1.3/commandeft/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.1.3/commandeft/constants/__init__.py
--rw-r--r--   0        0        0     3153 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/constants/consts.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.1.3/commandeft/core/__init__.py
--rw-r--r--   0        0        0     2319 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/core/cli.py
--rw-r--r--   0        0        0      823 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/core/decision.py
--rw-r--r--   0        0        0     1715 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/core/generation.py
--rw-r--r--   0        0        0     1123 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/main.py
--rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.1.3/commandeft/util/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/util/config_util.py
--rw-r--r--   0        0        0      437 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/util/gen_util.py
--rw-r--r--   0        0        0     2729 2023-06-12 01:21:44.524959 commandeft-0.1.3/commandeft/util/interactive_util.py
--rw-r--r--   0        0        0     1623 2023-06-12 01:48:54.788040 commandeft-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5113 1970-01-01 00:00:00.000000 commandeft-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-04 14:54:11.290505 commandeft-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-12 02:51:12.093999 commandeft-0.1.4/README.md
+-rw-r--r--   0        0        0       65 2023-06-12 02:20:42.863520 commandeft-0.1.4/commandeft/.pdm-python
+-rw-r--r--   0        0        0       40 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/.gitignore
+-rw-r--r--   0        0        0     2201 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/activate
+-rw-r--r--   0        0        0     1493 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3078 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3397 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1782 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1211 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/activate_this.py
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/python -> /usr/bin/python3.8
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/bin/python3.8 -> python
+-rw-r--r--   0        0        0       18 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4311 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/lib/python3.8/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      233 2023-06-12 02:20:42.855520 commandeft-0.1.4/commandeft/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0        0 2023-06-04 15:07:15.290389 commandeft-0.1.4/commandeft/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.1.4/commandeft/constants/__init__.py
+-rw-r--r--   0        0        0     3153 2023-06-12 01:21:44.524959 commandeft-0.1.4/commandeft/constants/consts.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.1.4/commandeft/core/__init__.py
+-rw-r--r--   0        0        0     2319 2023-06-12 01:21:44.524959 commandeft-0.1.4/commandeft/core/cli.py
+-rw-r--r--   0        0        0      823 2023-06-12 01:21:44.524959 commandeft-0.1.4/commandeft/core/decision.py
+-rw-r--r--   0        0        0     1715 2023-06-12 01:21:44.524959 commandeft-0.1.4/commandeft/core/generation.py
+-rw-r--r--   0        0        0     1123 2023-06-12 02:15:23.389295 commandeft-0.1.4/commandeft/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:39:15.217975 commandeft-0.1.4/commandeft/util/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-12 01:21:44.524959 commandeft-0.1.4/commandeft/util/config_util.py
+-rw-r--r--   0        0        0      437 2023-06-12 01:21:44.524959 commandeft-0.1.4/commandeft/util/gen_util.py
+-rw-r--r--   0        0        0     2729 2023-06-12 02:42:06.423316 commandeft-0.1.4/commandeft/util/interactive_util.py
+-rw-r--r--   0        0        0     1644 2023-06-12 03:08:18.623530 commandeft-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 commandeft-0.1.4/PKG-INFO
```

### Comparing `commandeft-0.1.3/LICENSE` & `commandeft-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.3/README.md` & `commandeft-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 CommanDeft is a simple Python CLI tool designed to generate useful shell commands based on user prompts. It utilizes OpenAI's chat models to provide intelligent suggestions and help users compose shell commands quickly and efficiently.
 
 ## Requirements
 
 - In order to use CommanDeft you will need an OpenAI API Key which will be asked of you during the initial configuration.
   You can easily get one from [HERE](https://platform.openai.com/account/api-keys)
 
+-If you are using Linux you might have to install `xclip` using your package manager.  
+For example, in Debian:
+`sudo apt-get install xclip`
+
 ## Installation
 
 To install CommanDeft, you can use the following command:
 
 ```sh
 pip install commandeft
 ```
@@ -50,15 +54,15 @@
 
 During the initial configuration or when running:
 
 ```sh
 commandeft --configure (or -c)
 ```
 
-- You can choose the generated answer's `temperature`. Because this tool is geared towards code generation, lowe temperatures perform better.
+- You can choose the generated answer's `temperature`. Because this tool is geared towards code generation, lower temperatures perform better.
   More information about temeratures [HERE](https://community.openai.com/t/cheat-sheet-mastering-temperature-and-top-p-in-chatgpt-api-a-few-tips-and-tricks-on-controlling-the-creativity-deterministic-output-of-prompt-responses/172683)
 - You can choose the `max_token` value.  
   ⚠️ Keep in Mind that the guided prompt consumes ~55 tokens. The value you specify won't include these tokens.
 - You will also be asked about the action that will be performed every time when you accept a generated command when running in interactive mode.  
   The available actions are:
 
 1. Running the generated command
```

### Comparing `commandeft-0.1.3/commandeft/constants/consts.py` & `commandeft-0.1.4/commandeft/constants/consts.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.3/commandeft/core/cli.py` & `commandeft-0.1.4/commandeft/core/cli.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.3/commandeft/core/decision.py` & `commandeft-0.1.4/commandeft/core/decision.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.3/commandeft/core/generation.py` & `commandeft-0.1.4/commandeft/core/generation.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.3/commandeft/main.py` & `commandeft-0.1.4/commandeft/main.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.3/commandeft/util/config_util.py` & `commandeft-0.1.4/commandeft/util/config_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.3/commandeft/util/interactive_util.py` & `commandeft-0.1.4/commandeft/util/interactive_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 
-from PyInquirer import prompt
+from InquirerPy import prompt
 from commandeft.constants.consts import init_messages
 
 
 def handle_escape(event):
     if event.name == "esc":
         raise KeyboardInterrupt()
```

### Comparing `commandeft-0.1.3/pyproject.toml` & `commandeft-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 [project]
 name = "commandeft"
-version = "0.1.3"
+version = "0.1.4"
 description = "CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models."
 readme = "README.md"
 authors = [
     { name = "Petros Sidirokastritis", email = "sidirope@gmail.com" },
 ]
-requires-python = ">=3.3, <=3.9"
+requires-python = ">=3.8.1, <=3.11.4"
 dependencies = [
-    "PyInquirer==1.0.3",
     "PyJWT==2.7.0",
     "Pygments==2.15.1",
     "aiohttp==3.8.4",
     "aiosignal==1.3.1",
     "async-timeout==4.0.2",
     "attrs==23.1.0",
     "cachetools==5.3.1",
     "certifi==2023.5.7",
     "cffi==1.15.1",
-    "charset-normalizer==3.1.0",
+    "charset-normalizer<4.0,>=2.0",
     "click==8.1.3",
     "cryptography==41.0.1",
     "diskcache==5.6.1",
     "frozenlist==1.3.3",
     "gptcache==0.1.29.1",
     "guidance==0.0.61",
     "idna==3.4",
     "msal==1.22.0",
-    "multidict==6.0.4",
+    "multidict<7.0,>=4.5",
     "nest-asyncio==1.5.6",
     "numpy==1.24.3",
     "openai==0.27.7",
     "parsimonious==0.10.0",
     "pip-licenses==4.3.2",
-    "platformdirs==3.5.1",
+    "platformdirs<4,>=3.2",
     "prettytable==3.7.0",
-    "prompt-toolkit==1.0.14",
+    "prompt-toolkit<4.0.0,>=3.0.1",
     "pycparser==2.21",
     "pygtrie==2.5.0",
     "pyperclip==1.8.2",
     "regex==2023.6.3",
     "requests==2.31.0",
     "six==1.16.0",
     "tiktoken==0.4.0",
     "tqdm==4.65.0",
     "urllib3==2.0.2",
     "wcwidth==0.2.6",
-    "yarl==1.9.2",
+    "yarl<2.0,>=1.0",
+    "InquirerPy>=0.3.4",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Ferrum-Citadel/commandeft"
```

### Comparing `commandeft-0.1.3/PKG-INFO` & `commandeft-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 Metadata-Version: 2.1
 Name: commandeft
-Version: 0.1.3
+Version: 0.1.4
 Summary: CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models.
 Author-Email: Petros Sidirokastritis <sidirope@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Ferrum-Citadel/commandeft
-Requires-Python: <=3.9,>=3.3
-Requires-Dist: PyInquirer==1.0.3
+Requires-Python: <=3.11.4,>=3.8.1
 Requires-Dist: PyJWT==2.7.0
 Requires-Dist: Pygments==2.15.1
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: async-timeout==4.0.2
 Requires-Dist: attrs==23.1.0
 Requires-Dist: cachetools==5.3.1
 Requires-Dist: certifi==2023.5.7
 Requires-Dist: cffi==1.15.1
-Requires-Dist: charset-normalizer==3.1.0
+Requires-Dist: charset-normalizer<4.0,>=2.0
 Requires-Dist: click==8.1.3
 Requires-Dist: cryptography==41.0.1
 Requires-Dist: diskcache==5.6.1
 Requires-Dist: frozenlist==1.3.3
 Requires-Dist: gptcache==0.1.29.1
 Requires-Dist: guidance==0.0.61
 Requires-Dist: idna==3.4
 Requires-Dist: msal==1.22.0
-Requires-Dist: multidict==6.0.4
+Requires-Dist: multidict<7.0,>=4.5
 Requires-Dist: nest-asyncio==1.5.6
 Requires-Dist: numpy==1.24.3
 Requires-Dist: openai==0.27.7
 Requires-Dist: parsimonious==0.10.0
 Requires-Dist: pip-licenses==4.3.2
-Requires-Dist: platformdirs==3.5.1
+Requires-Dist: platformdirs<4,>=3.2
 Requires-Dist: prettytable==3.7.0
-Requires-Dist: prompt-toolkit==1.0.14
+Requires-Dist: prompt-toolkit<4.0.0,>=3.0.1
 Requires-Dist: pycparser==2.21
 Requires-Dist: pygtrie==2.5.0
 Requires-Dist: pyperclip==1.8.2
 Requires-Dist: regex==2023.6.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: six==1.16.0
 Requires-Dist: tiktoken==0.4.0
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: urllib3==2.0.2
 Requires-Dist: wcwidth==0.2.6
-Requires-Dist: yarl==1.9.2
+Requires-Dist: yarl<2.0,>=1.0
+Requires-Dist: InquirerPy>=0.3.4
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-pep8; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # CommanDeft
@@ -56,14 +56,18 @@
 CommanDeft is a simple Python CLI tool designed to generate useful shell commands based on user prompts. It utilizes OpenAI's chat models to provide intelligent suggestions and help users compose shell commands quickly and efficiently.
 
 ## Requirements
 
 - In order to use CommanDeft you will need an OpenAI API Key which will be asked of you during the initial configuration.
   You can easily get one from [HERE](https://platform.openai.com/account/api-keys)
 
+-If you are using Linux you might have to install `xclip` using your package manager.  
+For example, in Debian:
+`sudo apt-get install xclip`
+
 ## Installation
 
 To install CommanDeft, you can use the following command:
 
 ```sh
 pip install commandeft
 ```
@@ -103,15 +107,15 @@
 
 During the initial configuration or when running:
 
 ```sh
 commandeft --configure (or -c)
 ```
 
-- You can choose the generated answer's `temperature`. Because this tool is geared towards code generation, lowe temperatures perform better.
+- You can choose the generated answer's `temperature`. Because this tool is geared towards code generation, lower temperatures perform better.
   More information about temeratures [HERE](https://community.openai.com/t/cheat-sheet-mastering-temperature-and-top-p-in-chatgpt-api-a-few-tips-and-tricks-on-controlling-the-creativity-deterministic-output-of-prompt-responses/172683)
 - You can choose the `max_token` value.  
   ⚠️ Keep in Mind that the guided prompt consumes ~55 tokens. The value you specify won't include these tokens.
 - You will also be asked about the action that will be performed every time when you accept a generated command when running in interactive mode.  
   The available actions are:
 
 1. Running the generated command
```

