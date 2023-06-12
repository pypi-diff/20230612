# Comparing `tmp/python_agency-0.1.0.tar.gz` & `tmp/python_agency-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_agency-0.1.0.tar", max compression
+gzip compressed data, was "python_agency-0.1.1.tar", max compression
```

## Comparing `python_agency-0.1.0.tar` & `python_agency-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 python_agency-0.1.0/LICENSE
--rw-r--r--   0        0        0    24885 2023-06-12 08:39:46.815847 python_agency-0.1.0/README.md
--rw-r--r--   0        0        0      575 2023-06-12 09:14:02.528866 python_agency-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 python_agency-0.1.0/python_agency/__init__.py
--rw-r--r--   0        0        0    10606 2023-06-12 08:15:54.594944 python_agency-0.1.0/python_agency/agent.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 python_agency-0.1.0/python_agency/agents/__init__.py
--rw-r--r--   0        0        0     2791 2023-06-12 08:15:54.595228 python_agency-0.1.0/python_agency/agents/chattyai.py
--rw-r--r--   0        0        0     2715 2023-06-12 08:15:54.595393 python_agency-0.1.0/python_agency/agents/demo_agent.py
--rw-r--r--   0        0        0     2202 2023-06-12 08:15:54.595538 python_agency-0.1.0/python_agency/agents/host.py
--rw-r--r--   0        0        0     1519 2023-06-12 08:15:54.595682 python_agency-0.1.0/python_agency/agents/prompt_methods.py
--rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 python_agency-0.1.0/python_agency/schema.py
--rwxr-xr-x   0        0        0     3232 2023-06-12 08:15:54.596001 python_agency-0.1.0/python_agency/space.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 python_agency-0.1.0/python_agency/spaces/__init__.py
--rw-r--r--   0        0        0     6149 2023-06-12 08:15:54.596300 python_agency-0.1.0/python_agency/spaces/templates/index.html
--rw-r--r--   0        0        0     4010 2023-06-12 08:15:54.596458 python_agency-0.1.0/python_agency/spaces/web_app.py
--rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 python_agency-0.1.0/python_agency/util.py
--rw-r--r--   0        0        0    25742 1970-01-01 00:00:00.000000 python_agency-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 python_agency-0.1.1/LICENSE
+-rw-r--r--   0        0        0    24786 2023-06-12 09:20:59.904493 python_agency-0.1.1/README.md
+-rw-r--r--   0        0        0      575 2023-06-12 19:18:56.314807 python_agency-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 python_agency-0.1.1/python_agency/__init__.py
+-rw-r--r--   0        0        0    10613 2023-06-12 09:30:12.366268 python_agency-0.1.1/python_agency/agent.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 python_agency-0.1.1/python_agency/agents/__init__.py
+-rw-r--r--   0        0        0     2820 2023-06-12 09:30:25.967905 python_agency-0.1.1/python_agency/agents/chattyai.py
+-rw-r--r--   0        0        0     2743 2023-06-12 09:30:12.376322 python_agency-0.1.1/python_agency/agents/demo_agent.py
+-rw-r--r--   0        0        0     2209 2023-06-12 09:30:12.376339 python_agency-0.1.1/python_agency/agents/host.py
+-rw-r--r--   0        0        0     1533 2023-06-12 09:30:12.376283 python_agency-0.1.1/python_agency/agents/prompt_methods.py
+-rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 python_agency-0.1.1/python_agency/schema.py
+-rwxr-xr-x   0        0        0     3246 2023-06-12 09:30:34.336025 python_agency-0.1.1/python_agency/space.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 python_agency-0.1.1/python_agency/spaces/__init__.py
+-rw-r--r--   0        0        0     6149 2023-06-12 08:15:54.596300 python_agency-0.1.1/python_agency/spaces/templates/index.html
+-rw-r--r--   0        0        0     4031 2023-06-12 09:30:12.366310 python_agency-0.1.1/python_agency/spaces/web_app.py
+-rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 python_agency-0.1.1/python_agency/util.py
+-rw-r--r--   0        0        0    25643 1970-01-01 00:00:00.000000 python_agency-0.1.1/PKG-INFO
```

### Comparing `python_agency-0.1.0/LICENSE` & `python_agency-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.0/README.md` & `python_agency-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,16 @@
 software and do not configure it for OS access otherwise.\
 \
 If you want to enable OS access, to allow for file I/O for example, I HIGHLY
 RECOMMEND running your project within a Docker container to prevent direct
 access to your host, allowing you to limit the resources and directories that
 may be accessed.
 
-**Please note that `agency` is not yet published to pip.**
-
 ```sh
-git clone git@github.com:operand/agency.git
-pip install ./agency
+pip install python_agency
 ```
 
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) intended for integrating AI,
```

### Comparing `python_agency-0.1.0/pyproject.toml` & `python_agency-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_agency"
-version = "0.1.0"
+version = "0.1.1"
 description = "A fast and minimal foundation for unifying human, AI, and other computing systems, in python"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `python_agency-0.1.0/python_agency/agent.py` & `python_agency-0.1.1/python_agency/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import abstractmethod
-from agency.schema import ActionSchema, MessageSchema
+from python_agency.schema import ActionSchema, MessageSchema
 import inspect
 import queue
 import re
 import threading
 
 
 # access keys
```

### Comparing `python_agency-0.1.0/python_agency/agents/chattyai.py` & `python_agency-0.1.1/python_agency/agents/chattyai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from agency.agent import ACCESS_PERMITTED, access_policy
-from agency.agent import Agent
-from agency.agents.prompt_methods import PromptMethods
-from agency.schema import MessageSchema
+from python_agency.agent import ACCESS_PERMITTED, access_policy
+from python_agency.agent import Agent
+from python_agency.agents.prompt_methods import PromptMethods
+from python_agency.schema import MessageSchema
 from transformers import AutoTokenizer, AutoModelForCausalLM
-import agency.util as util
+import pagency.util as util
 import os
 import textwrap
 
 
 os.environ['TOKENIZERS_PARALLELISM'] = 'true'
```

### Comparing `python_agency-0.1.0/python_agency/agents/demo_agent.py` & `python_agency-0.1.1/python_agency/agents/demo_agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
-from agency import util
-from agency.agent import ACCESS_PERMITTED, access_policy
-from agency.agent import Agent
-from agency.agents.prompt_methods import PromptMethods
+from python_agency import util
+from python_agency.agent import ACCESS_PERMITTED, access_policy
+from python_agency.agent import Agent
+from python_agency.agents.prompt_methods import PromptMethods
 import json
 import openai
 import textwrap
 
 
 class DemoAgent(Agent, PromptMethods):
```

### Comparing `python_agency-0.1.0/python_agency/agents/host.py` & `python_agency-0.1.1/python_agency/agents/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from colorama import Fore, Style
-from agency.agent import ACCESS_REQUESTED, Agent, access_policy
+from python_agency.agent import ACCESS_REQUESTED, Agent, access_policy
 import json
 import os
 import re
 import subprocess
 
 
 class Host(Agent):
```

### Comparing `python_agency-0.1.0/python_agency/agents/prompt_methods.py` & `python_agency-0.1.1/python_agency/agents/prompt_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from datetime import datetime
-from agency import util
-from agency.schema import MessageSchema
+from python_agency import util
+from python_agency.schema import MessageSchema
 
 
 class PromptMethods:
     """
     Contains methods for constructing prompts from message logs"""
 
     def _full_prompt(self):
```

### Comparing `python_agency-0.1.0/python_agency/schema.py` & `python_agency-0.1.1/python_agency/schema.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.0/python_agency/space.py` & `python_agency-0.1.1/python_agency/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from agency.agent import Agent
-from agency.schema import MessageSchema
+from python_agency.agent import Agent
+from python_agency.schema import MessageSchema
 
 
 class Space(Agent):
     """
     A Space is itself an Agent and is responsible for:
     - starting/stopping itself and its member agents
     - routing all messages for its member agents
```

### Comparing `python_agency-0.1.0/python_agency/spaces/templates/index.html` & `python_agency-0.1.1/python_agency/spaces/templates/index.html`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.0/python_agency/spaces/web_app.py` & `python_agency-0.1.1/python_agency/spaces/web_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from eventlet import wsgi
-from agency.agent import ACCESS_PERMITTED, Agent, access_policy
-from agency.schema import MessageSchema
-from agency.space import Space
+from python_agency.agent import ACCESS_PERMITTED, Agent, access_policy
+from python_agency.schema import MessageSchema
+from python_agency.space import Space
 from flask import Flask, render_template, request
 from flask.logging import default_handler
 from flask_socketio import SocketIO
 import eventlet
 import logging
```

### Comparing `python_agency-0.1.0/python_agency/util.py` & `python_agency-0.1.1/python_agency/util.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.0/PKG-INFO` & `python_agency-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-agency
-Version: 0.1.0
+Version: 0.1.1
 Summary: A fast and minimal foundation for unifying human, AI, and other computing systems, in python
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -57,19 +57,16 @@
 software and do not configure it for OS access otherwise.\
 \
 If you want to enable OS access, to allow for file I/O for example, I HIGHLY
 RECOMMEND running your project within a Docker container to prevent direct
 access to your host, allowing you to limit the resources and directories that
 may be accessed.
 
-**Please note that `agency` is not yet published to pip.**
-
 ```sh
-git clone git@github.com:operand/agency.git
-pip install ./agency
+pip install python_agency
 ```
 
 
 # API Overview
 
 `agency` is an implementation of the [Actor
 model](https://en.wikipedia.org/wiki/Actor_model) intended for integrating AI,
```

