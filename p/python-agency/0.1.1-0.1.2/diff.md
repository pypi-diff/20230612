# Comparing `tmp/python_agency-0.1.1.tar.gz` & `tmp/python_agency-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_agency-0.1.1.tar", max compression
+gzip compressed data, was "python_agency-0.1.2.tar", max compression
```

## Comparing `python_agency-0.1.1.tar` & `python_agency-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 python_agency-0.1.1/LICENSE
--rw-r--r--   0        0        0    24786 2023-06-12 09:20:59.904493 python_agency-0.1.1/README.md
--rw-r--r--   0        0        0      575 2023-06-12 19:18:56.314807 python_agency-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 python_agency-0.1.1/python_agency/__init__.py
--rw-r--r--   0        0        0    10613 2023-06-12 09:30:12.366268 python_agency-0.1.1/python_agency/agent.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 python_agency-0.1.1/python_agency/agents/__init__.py
--rw-r--r--   0        0        0     2820 2023-06-12 09:30:25.967905 python_agency-0.1.1/python_agency/agents/chattyai.py
--rw-r--r--   0        0        0     2743 2023-06-12 09:30:12.376322 python_agency-0.1.1/python_agency/agents/demo_agent.py
--rw-r--r--   0        0        0     2209 2023-06-12 09:30:12.376339 python_agency-0.1.1/python_agency/agents/host.py
--rw-r--r--   0        0        0     1533 2023-06-12 09:30:12.376283 python_agency-0.1.1/python_agency/agents/prompt_methods.py
--rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 python_agency-0.1.1/python_agency/schema.py
--rwxr-xr-x   0        0        0     3246 2023-06-12 09:30:34.336025 python_agency-0.1.1/python_agency/space.py
--rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 python_agency-0.1.1/python_agency/spaces/__init__.py
--rw-r--r--   0        0        0     6149 2023-06-12 08:15:54.596300 python_agency-0.1.1/python_agency/spaces/templates/index.html
--rw-r--r--   0        0        0     4031 2023-06-12 09:30:12.366310 python_agency-0.1.1/python_agency/spaces/web_app.py
--rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 python_agency-0.1.1/python_agency/util.py
--rw-r--r--   0        0        0    25643 1970-01-01 00:00:00.000000 python_agency-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-12 08:15:54.594199 python_agency-0.1.2/LICENSE
+-rw-r--r--   0        0        0    24786 2023-06-12 09:20:59.904493 python_agency-0.1.2/README.md
+-rw-r--r--   0        0        0      575 2023-06-12 19:44:05.161613 python_agency-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-06-12 08:15:54.594765 python_agency-0.1.2/python_agency/__init__.py
+-rw-r--r--   0        0        0    10613 2023-06-12 09:30:12.366268 python_agency-0.1.2/python_agency/agent.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.595026 python_agency-0.1.2/python_agency/agents/__init__.py
+-rw-r--r--   0        0        0     2826 2023-06-12 19:36:28.084461 python_agency-0.1.2/python_agency/agents/chattyai.py
+-rw-r--r--   0        0        0     2743 2023-06-12 09:30:12.376322 python_agency-0.1.2/python_agency/agents/demo_agent.py
+-rw-r--r--   0        0        0     2209 2023-06-12 09:30:12.376339 python_agency-0.1.2/python_agency/agents/host.py
+-rw-r--r--   0        0        0     1533 2023-06-12 09:30:12.376283 python_agency-0.1.2/python_agency/agents/prompt_methods.py
+-rw-r--r--   0        0        0      801 2023-06-12 08:15:54.595850 python_agency-0.1.2/python_agency/schema.py
+-rwxr-xr-x   0        0        0     3246 2023-06-12 09:30:34.336025 python_agency-0.1.2/python_agency/space.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:15:54.596076 python_agency-0.1.2/python_agency/spaces/__init__.py
+-rw-r--r--   0        0        0     6149 2023-06-12 08:15:54.596300 python_agency-0.1.2/python_agency/spaces/templates/index.html
+-rw-r--r--   0        0        0     4031 2023-06-12 09:30:12.366310 python_agency-0.1.2/python_agency/spaces/web_app.py
+-rw-r--r--   0        0        0     4280 2023-06-12 08:15:54.596618 python_agency-0.1.2/python_agency/util.py
+-rw-r--r--   0        0        0    25643 1970-01-01 00:00:00.000000 python_agency-0.1.2/PKG-INFO
```

### Comparing `python_agency-0.1.1/LICENSE` & `python_agency-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/README.md` & `python_agency-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/pyproject.toml` & `python_agency-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_agency"
-version = "0.1.1"
+version = "0.1.2"
 description = "A fast and minimal foundation for unifying human, AI, and other computing systems, in python"
 authors = ["Daniel Rodriguez"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `python_agency-0.1.1/python_agency/agent.py` & `python_agency-0.1.2/python_agency/agent.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/agents/chattyai.py` & `python_agency-0.1.2/python_agency/agents/chattyai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from python_agency.agent import ACCESS_PERMITTED, access_policy
 from python_agency.agent import Agent
 from python_agency.agents.prompt_methods import PromptMethods
 from python_agency.schema import MessageSchema
 from transformers import AutoTokenizer, AutoModelForCausalLM
-import pagency.util as util
 import os
+import python_agency.util as util
 import textwrap
 
 
 os.environ['TOKENIZERS_PARALLELISM'] = 'true'
 
 
 class ChattyAI(Agent, PromptMethods):
```

### Comparing `python_agency-0.1.1/python_agency/agents/demo_agent.py` & `python_agency-0.1.2/python_agency/agents/demo_agent.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/agents/host.py` & `python_agency-0.1.2/python_agency/agents/host.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/agents/prompt_methods.py` & `python_agency-0.1.2/python_agency/agents/prompt_methods.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/schema.py` & `python_agency-0.1.2/python_agency/schema.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/space.py` & `python_agency-0.1.2/python_agency/space.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/spaces/templates/index.html` & `python_agency-0.1.2/python_agency/spaces/templates/index.html`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/spaces/web_app.py` & `python_agency-0.1.2/python_agency/spaces/web_app.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/python_agency/util.py` & `python_agency-0.1.2/python_agency/util.py`

 * *Files identical despite different names*

### Comparing `python_agency-0.1.1/PKG-INFO` & `python_agency-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-agency
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast and minimal foundation for unifying human, AI, and other computing systems, in python
 License: GPL-3.0
 Author: Daniel Rodriguez
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

