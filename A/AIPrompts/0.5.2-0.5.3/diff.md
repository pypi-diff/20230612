# Comparing `tmp/AIPrompts-0.5.2.tar.gz` & `tmp/AIPrompts-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPrompts-0.5.2.tar", last modified: Mon Jun 12 14:21:51 2023, max compression
+gzip compressed data, was "AIPrompts-0.5.3.tar", last modified: Mon Jun 12 18:34:58 2023, max compression
```

## Comparing `AIPrompts-0.5.2.tar` & `AIPrompts-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.558069 AIPrompts-0.5.2/AIPrompts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/tests/test_turbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:34:58.661110 AIPrompts-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:34:58.657110 AIPrompts-0.5.3/AIPrompts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 18:34:58.000000 AIPrompts-0.5.3/AIPrompts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 18:34:58.000000 AIPrompts-0.5.3/AIPrompts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:34:58.000000 AIPrompts-0.5.3/AIPrompts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 18:34:58.000000 AIPrompts-0.5.3/AIPrompts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 18:34:58.000000 AIPrompts-0.5.3/AIPrompts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 18:34:58.661110 AIPrompts-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:34:58.661110 AIPrompts-0.5.3/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/prompts/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/prompts/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/prompts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/prompts/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/prompts/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 18:34:58.661110 AIPrompts-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:34:58.661110 AIPrompts-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-12 18:34:44.000000 AIPrompts-0.5.3/tests/test_turbo.py
```

### Comparing `AIPrompts-0.5.2/AIPrompts.egg-info/PKG-INFO` & `AIPrompts-0.5.3/AIPrompts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.5.2
+Version: 0.5.3
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.5.2/PKG-INFO` & `AIPrompts-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.5.2
+Version: 0.5.3
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.5.2/README.md` & `AIPrompts-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.2/prompts/dynamic.py` & `AIPrompts-0.5.3/prompts/dynamic.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.2/prompts/ensemble.py` & `AIPrompts-0.5.3/prompts/ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.2/prompts/exceptions.py` & `AIPrompts-0.5.3/prompts/exceptions.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.2/prompts/schemas.py` & `AIPrompts-0.5.3/prompts/schemas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from typing import TypedDict, NotRequired
 
 from pydantic import BaseModel, Field
 
 
 # ==== Generic classes ====
 class OpenAIModelSettings(BaseModel):
     # TODO: these defaults are terrible. We must remove them.
@@ -37,20 +38,20 @@
 
 class PromptRole(str, Enum):
     USER = "user"
     SYSTEM = "system"
     ASSISTANT = "assistant"
 
 
-class TemplateInputs(BaseModel):
+class TemplateInputs(TypedDict):
     inputs: dict[str, str]
-    name: str | None = None
+    name: NotRequired[str]
     role: PromptRole
     # advanced usage: select sub-templates
-    template_name: str = "default"
+    template_name: NotRequired[str]
 
 
 class ChatMLMessage(BaseModel):
     content: str
     name: str | None = None
     role: PromptRole
```

### Comparing `AIPrompts-0.5.2/prompts/turbo.py` & `AIPrompts-0.5.3/prompts/turbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,26 +204,26 @@
             return
 
         for hist in initial_template_data:
             if isinstance(hist, ChatMLMessage):
                 prompt.add_raw_content(hist)
                 continue
 
-            if hist.role == PromptRole.SYSTEM:
+            if hist["role"] == PromptRole.SYSTEM:
                 prompt.add_system_message(
-                    template_name=hist.template_name, **hist.inputs
+                    template_name=hist.get("template_name"), **hist["inputs"]
                 )
-            elif hist.role == PromptRole.USER:
-                prompt.add_user_message(template_name=hist.template_name, **hist.inputs)
-            elif hist.role == PromptRole.ASSISTANT:
+            elif hist["role"] == PromptRole.USER:
+                prompt.add_user_message(template_name=hist.get("template_name"), **hist["inputs"])
+            elif hist["role"] == PromptRole.ASSISTANT:
                 prompt.add_assistant_message(
-                    template_name=hist.template_name, **hist.inputs
+                    template_name=hist.get("template_name"), **hist["inputs"]
                 )
             else:
-                raise ValueError(f"Invalid role in initial_template_data: {hist.role}")
+                raise ValueError(f"Invalid role in initial_template_data: {hist['role']}")
 
     @classmethod
     def from_file(cls, file_path: str):
         with open(file_path, "r") as f:
             prompt_data = yaml.safe_load(f)
 
         tb = TurboSchema(**prompt_data)
@@ -231,15 +231,15 @@
 
     @classmethod
     def from_settings(
         cls,
         name: str,
         description: str,
         settings: OpenAIModelSettings,
-        initial_template_data: list[TemplateInputs | ChatMLMessage],
+        initial_template_data: list[TemplateInputs] | list[ChatMLMessage],
         system_template: list[Template] | str = "",
         user_template: list[Template] | str = "",
         assistant_template: list[Template] | str = "",
     ):
         tbs = TurboSchema(
             name=name,
             description=description,
```

### Comparing `AIPrompts-0.5.2/setup.py` & `AIPrompts-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.2/tests/test_ensemble.py` & `AIPrompts-0.5.3/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.2/tests/test_prompt.py` & `AIPrompts-0.5.3/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.2/tests/test_turbo.py` & `AIPrompts-0.5.3/tests/test_turbo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from prompts import (
     DynamicPrompt,
     OpenAIModelSettings,
     PromptRole,
-    TemplateContent,
+    TemplateInputs,
     TurboPrompt,
 )
 
 
 def test_turbo_all_none():
     tp = TurboPrompt()
     assert len(tp.prompts) == 0
@@ -141,25 +141,25 @@
     assert isinstance(built[0], dict)
     assert len(built) == 3
     assert built[-1]["role"] == "assistant"
 
     tp = TurboPrompt.from_settings(
         name="turbo_prompt_inline",
         description="",
-        system_template="You are an AI",
+        system_template="<message>",
         user_template="Q:<message>",
         assistant_template="A:",
         settings=OpenAIModelSettings(model="gpt-4"),
         initial_template_data=[
-            TemplateContent(
-                content="hey", template_name="default", role=PromptRole.SYSTEM
+            TemplateInputs(
+                inputs={"message": "You are an AI."}, role=PromptRole.SYSTEM
             )
         ],
     )
 
     content = tp.build()
     assert len(content) == 1
     print(content)
     assert content[0] == {
         "role": "system",
-        "content": "hey",
+        "content": "You are an AI.",
     }
```

