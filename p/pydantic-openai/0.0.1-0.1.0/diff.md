# Comparing `tmp/pydantic_openai-0.0.1.tar.gz` & `tmp/pydantic_openai-0.1.0.tar.gz`

## Comparing `pydantic_openai-0.0.1.tar` & `pydantic_openai-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/.python3@3.10.pkg -> hermit
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/README.hermit.md
--rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/activate-hermit
--rwxr-xr-x   0        0        0     1512 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/hermit
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/hermit.hcl
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/pip -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/pip3 -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/pip3.10 -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/pydoc3 -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/pydoc3.10 -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/python -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/python3 -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/python3-config -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/python3.10 -> .python3@3.10.pkg
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/bin/python3.10-config -> .python3@3.10.pkg
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/src/pydantic_openai/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/src/pydantic_openai/chat.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/src/pydantic_openai/common.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/src/pydantic_openai/completion.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/src/pydantic_openai/embeddings.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/src/pydantic_openai/moderation.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/LICENSE
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 pydantic_openai-0.0.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/.python3@3.10.pkg -> hermit
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/README.hermit.md
+-rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/activate-hermit
+-rwxr-xr-x   0        0        0     1512 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/hermit
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/hermit.hcl
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/pip -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/pip3 -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/pip3.10 -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/pydoc3 -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/pydoc3.10 -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/python -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/python3 -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/python3-config -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/python3.10 -> .python3@3.10.pkg
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/bin/python3.10-config -> .python3@3.10.pkg
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/src/pydantic_openai/__init__.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/src/pydantic_openai/chat.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/src/pydantic_openai/common.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/src/pydantic_openai/completion.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/src/pydantic_openai/embeddings.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/src/pydantic_openai/moderation.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/LICENSE
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 pydantic_openai-0.1.0/PKG-INFO
```

### Comparing `pydantic_openai-0.0.1/bin/activate-hermit` & `pydantic_openai-0.1.0/bin/activate-hermit`

 * *Files identical despite different names*

### Comparing `pydantic_openai-0.0.1/bin/hermit` & `pydantic_openai-0.1.0/bin/hermit`

 * *Files identical despite different names*

### Comparing `pydantic_openai-0.0.1/src/pydantic_openai/chat.py` & `pydantic_openai-0.1.0/src/pydantic_openai/chat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Chat completion related APIs.
 
 Reference: https://platform.openai.com/docs/api-reference/completions
 """
 from typing import List, Dict, Optional
 from enum import Enum
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from .common import Usage
 
+
 class ChatMessageRole(str, Enum):
     System = "system"
     User = "user"
     Assistant = "assistant"
 
 class ChatCompletionMessage(BaseModel):
     role: ChatMessageRole
     content: str
-    name: Optional[str] = None
+    name: Optional[str] = Field(None, alias="name")
 
 class ChatCompletionRequest(BaseModel):
     model: str
     messages: List[ChatCompletionMessage]
-    max_tokens: Optional[int] = None
-    temperature: Optional[float] = None
-    top_p: Optional[float] = None
-    n: Optional[int] = None
-    stream: bool = False
-    stop: Optional[List[str]] = None
-    presence_penalty: Optional[float] = None
-    frequency_penalty: Optional[float] = None
-    logit_bias: Optional[Dict[str, int]] = None
-    user: Optional[str] = None
+    max_tokens: Optional[int] = Field(None, alias="max_tokens")
+    temperature: Optional[float] = Field(None, alias="temperature")
+    top_p: Optional[float] = Field(None, alias="top_p")
+    n: Optional[int] = Field(None, alias="n")
+    stream: Optional[bool] = Field(None, alias="stream")
+    stop: Optional[List[str]] = Field(None, alias="stop")
+    presence_penalty: Optional[float] = Field(None, alias="presence_penalty")
+    frequency_penalty: Optional[float] = Field(None, alias="frequency_penalty")
+    logit_bias: Optional[Dict[str, int]] = Field(None, alias="logit_bias")
+    user: Optional[str] = Field(None, alias="user")
 
 class ChatCompletionChoice(BaseModel):
     index: int
     message: ChatCompletionMessage
-    finish_reason: str
+    finish_reason: str = Field(..., alias="finish_reason")
 
 class ChatCompletionResponse(BaseModel):
-    id: str
-    object: str
-    created: int
-    model: str
+    id: str = Field(..., alias="id")
+    object: str = Field(..., alias="object")
+    created: int = Field(..., alias="created")
+    model: str = Field(..., alias="model")
     choices: List[ChatCompletionChoice]
     usage: Usage
-
```

### Comparing `pydantic_openai-0.0.1/src/pydantic_openai/completion.py` & `pydantic_openai-0.1.0/src/pydantic_openai/completion.py`

 * *Files identical despite different names*

### Comparing `pydantic_openai-0.0.1/src/pydantic_openai/embeddings.py` & `pydantic_openai-0.1.0/src/pydantic_openai/embeddings.py`

 * *Files identical despite different names*

### Comparing `pydantic_openai-0.0.1/src/pydantic_openai/moderation.py` & `pydantic_openai-0.1.0/src/pydantic_openai/moderation.py`

 * *Files identical despite different names*

### Comparing `pydantic_openai-0.0.1/.gitignore` & `pydantic_openai-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic_openai-0.0.1/LICENSE` & `pydantic_openai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_openai-0.0.1/pyproject.toml` & `pydantic_openai-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydantic_openai"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Chris Hua", email="hua.christopher@gmail.com" },
 ]
 description = "Pydantic models for OpenAI's API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `pydantic_openai-0.0.1/PKG-INFO` & `pydantic_openai-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_openai
-Version: 0.0.1
+Version: 0.1.0
 Summary: Pydantic models for OpenAI's API
 Project-URL: Homepage, https://github.com/stillmatic/pydantic-openai
 Project-URL: Bug Tracker, https://github.com/stillmatic/pydantic-openai/issues
 Author-email: Chris Hua <hua.christopher@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,8 +15,20 @@
 
 # pydantic-openai
 
 Pydantic models for OpenAI's API. These make it easier to construct requests and parse responses, as well as set up API-compatible servers.
 
 Making requests is explicitly out of scope.
 
-This is mostly translated from [sashabaranov/go-openai](https://github.com/sashabaranov/go-openai/tree/master), by ChatGPT.
+This is mostly translated from [sashabaranov/go-openai](https://github.com/sashabaranov/go-openai/tree/master), by ChatGPT. I welcome translating the rest over, I just don't really use the other API's.
+
+# Usage
+
+See the package on [PyPI](https://pypi.org/project/pydantic-openai/). 
+
+```bash
+pip install pydantic-openai
+```
+
+```python
+from pydantic_openai import ChatCompletionRequest
+```
```

