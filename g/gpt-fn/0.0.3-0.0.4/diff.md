# Comparing `tmp/gpt_fn-0.0.3.tar.gz` & `tmp/gpt_fn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.0.3.tar", max compression
+gzip compressed data, was "gpt_fn-0.0.4.tar", max compression
```

## Comparing `gpt_fn-0.0.3.tar` & `gpt_fn-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1066 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/LICENSE
--rw-r--r--   0        0        0     3023 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/README.md
--rw-r--r--   0        0        0      668 2023-06-09 09:20:42.635795 gpt_fn-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/src/fn/__init__.py
--rw-r--r--   0        0        0      869 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/src/fn/ai_function.py
--rw-r--r--   0        0        0      537 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/src/fn/conftest.py
--rw-r--r--   0        0        0      625 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/src/fn/prompt.py
--rw-r--r--   0        0        0        0 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/src/fn/py.typed
--rw-r--r--   0        0        0        0 2023-06-09 09:20:14.023311 gpt_fn-0.0.3/src/fn/tests/__init__.py
--rw-r--r--   0        0        0      284 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0      330 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0     3356 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/tests/cassettes/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0     4299 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/tests/cassettes/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0      872 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/tests/test_ai_function.py
--rw-r--r--   0        0        0      490 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     2411 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/signature.py
--rw-r--r--   0        0        0        0 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/tests/__init__.py
--rw-r--r--   0        0        0      960 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0     5591 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0      892 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     1733 2023-06-09 09:20:14.027312 gpt_fn-0.0.3/src/fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 gpt_fn-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-12 00:37:42.039107 gpt_fn-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3023 2023-06-12 00:37:42.039107 gpt_fn-0.0.4/README.md
+-rw-r--r--   0        0        0      758 2023-06-12 00:38:06.795215 gpt_fn-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0      893 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0      537 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      641 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0      284 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0      330 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0     3356 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0     4299 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0      872 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0      522 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     2411 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0     5591 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0      892 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     1733 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 gpt_fn-0.0.4/PKG-INFO
```

### Comparing `gpt_fn-0.0.3/LICENSE` & `gpt_fn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/README.md` & `gpt_fn-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/pyproject.toml` & `gpt_fn-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
-packages = [{ include = "fn", from = "src" }]
+packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27"
 pydantic = "^1.0"
 jinja2 = "^3.0"
@@ -16,14 +16,16 @@
 [tool.poetry.group.test.dependencies]
 syrupy = "^4.0.2"
 pytest-vcr = "^1.0.2"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
+mkdocs-material = "^9.1.15"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 
 [tool.poetry-dynamic-versioning]
 enable = false
 pattern = "default-unprefixed"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
```

### Comparing `gpt_fn-0.0.3/src/fn/ai_function.py` & `gpt_fn-0.0.4/src/gpt_fn/ai_function.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import wraps
 from typing import Any, Callable, ParamSpec, TypeVar
 
 import openai
 
-from .prompt import ChatTemplate, Message
+from .prompt import ChatTemplate, MessageTemplate
 from .utils.signature import FunctionSignature
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
 def ai_fn(
@@ -15,16 +15,16 @@
 ) -> Callable[P, T]:
     sig = FunctionSignature(fn)
 
     @wraps(fn)
     def inner(*args: Any, **kwargs: Any) -> T:
         template = ChatTemplate(
             messages=[
-                Message(role="system", content=sig.instruction()),
-                Message(role="user", content=sig.call_line(*args, **kwargs)),
+                MessageTemplate(role="system", content=sig.instruction()),
+                MessageTemplate(role="user", content=sig.call_line(*args, **kwargs)),
             ]
         )
 
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=template.render(),
             temperature=0.0,
```

### Comparing `gpt_fn-0.0.3/src/fn/conftest.py` & `gpt_fn-0.0.4/src/gpt_fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/prompt.py` & `gpt_fn-0.0.4/src/gpt_fn/prompt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Literal
 
 import jinja2
 from pydantic import BaseModel
 
 
-class Message(BaseModel):
+class MessageTemplate(BaseModel):
     role: Literal["system", "user", "assistant"]
     content: str
 
     def render(self, **kwargs: str) -> dict[str, Any]:
         return {
             "role": self.role,
             "content": jinja2.Template(self.content).render(**kwargs),
@@ -16,11 +16,11 @@
 
     class Config:
         # remove whitespace
         anystr_strip_whitespace = True
 
 
 class ChatTemplate(BaseModel):
-    messages: list[Message]
+    messages: list[MessageTemplate]
 
     def render(self, **kwargs: str) -> list[dict[str, Any]]:
         return [m.render(**kwargs) for m in self.messages]
```

### Comparing `gpt_fn-0.0.3/src/fn/tests/cassettes/test_ai_fabnocci.yaml` & `gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/tests/cassettes/test_ai_fake_hero.yaml` & `gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/tests/test_ai_function.py` & `gpt_fn-0.0.4/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/utils/pydantic_parser.py` & `gpt_fn-0.0.4/src/gpt_fn/utils/pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/utils/signature.py` & `gpt_fn-0.0.4/src/gpt_fn/utils/signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/src/fn/utils/tests/test_signature.py` & `gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.3/PKG-INFO` & `gpt_fn-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

