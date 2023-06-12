# Comparing `tmp/AIPrompts-0.5.1.tar.gz` & `tmp/AIPrompts-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPrompts-0.5.1.tar", last modified: Tue May 30 19:16:06 2023, max compression
+gzip compressed data, was "AIPrompts-0.5.2.tar", last modified: Mon Jun 12 14:21:51 2023, max compression
```

## Comparing `AIPrompts-0.5.1.tar` & `AIPrompts-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.475989 AIPrompts-0.5.1/AIPrompts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 19:16:06.000000 AIPrompts-0.5.1/AIPrompts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:16:06.479989 AIPrompts-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-30 19:15:50.000000 AIPrompts-0.5.1/tests/test_turbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.558069 AIPrompts-0.5.2/AIPrompts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 14:21:51.000000 AIPrompts-0.5.2/AIPrompts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:21:51.562069 AIPrompts-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-12 14:21:36.000000 AIPrompts-0.5.2/tests/test_turbo.py
```

### Comparing `AIPrompts-0.5.1/AIPrompts.egg-info/PKG-INFO` & `AIPrompts-0.5.2/AIPrompts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.5.1
+Version: 0.5.2
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.5.1/PKG-INFO` & `AIPrompts-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.5.1
+Version: 0.5.2
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.5.1/README.md` & `AIPrompts-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/prompts/dynamic.py` & `AIPrompts-0.5.2/prompts/dynamic.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/prompts/ensemble.py` & `AIPrompts-0.5.2/prompts/ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/prompts/exceptions.py` & `AIPrompts-0.5.2/prompts/exceptions.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/prompts/schemas.py` & `AIPrompts-0.5.2/prompts/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from enum import Enum
-from typing import Optional
 
 from pydantic import BaseModel, Field
 
 
 # ==== Generic classes ====
 class OpenAIModelSettings(BaseModel):
+    # TODO: these defaults are terrible. We must remove them.
     model: str
     max_tokens: int = 256
-    temperature: float = 0.0
-    top_p: float = 1
-    frequency_penalty: float = 0
-    presence_penalty: float = 0
-    logit_bias: dict[int, int] | None = None
-    stop: list[str] = Field(default_factory=list)
-    n: int = 1
-    user: str | None = None
+    temperature: float = 0.2
+    # top_p: float = 1
+    # frequency_penalty: float = 0
+    # presence_penalty: float = 0
+    # logit_bias: dict[int, int] | None = None
+    # stop: list[str] = Field(default_factory=list)
+    # n: int = 1
+    # user: str | None = None
 
 
 # ==== Dynamic classes ====
 class DynamicSchema(BaseModel):
     # Prompt identification
     name: str
     description: str = ""
```

### Comparing `AIPrompts-0.5.1/prompts/turbo.py` & `AIPrompts-0.5.2/prompts/turbo.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/setup.py` & `AIPrompts-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/tests/test_ensemble.py` & `AIPrompts-0.5.2/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/tests/test_prompt.py` & `AIPrompts-0.5.2/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.5.1/tests/test_turbo.py` & `AIPrompts-0.5.2/tests/test_turbo.py`

 * *Files identical despite different names*

