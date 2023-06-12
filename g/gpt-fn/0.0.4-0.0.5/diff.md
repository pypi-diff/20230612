# Comparing `tmp/gpt_fn-0.0.4.tar.gz` & `tmp/gpt_fn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.0.4.tar", max compression
+gzip compressed data, was "gpt_fn-0.0.5.tar", max compression
```

## Comparing `gpt_fn-0.0.4.tar` & `gpt_fn-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0     1066 2023-06-12 00:37:42.039107 gpt_fn-0.0.4/LICENSE
--rw-r--r--   0        0        0     3023 2023-06-12 00:37:42.039107 gpt_fn-0.0.4/README.md
--rw-r--r--   0        0        0      758 2023-06-12 00:38:06.795215 gpt_fn-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/__init__.py
--rw-r--r--   0        0        0      893 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/ai_function.py
--rw-r--r--   0        0        0      537 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/conftest.py
--rw-r--r--   0        0        0      641 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/prompt.py
--rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/py.typed
--rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/__init__.py
--rw-r--r--   0        0        0      284 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0      330 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0     3356 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0     4299 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0      872 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/test_ai_function.py
--rw-r--r--   0        0        0      522 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/__init__.py
--rw-r--r--   0        0        0     1945 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     2411 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/signature.py
--rw-r--r--   0        0        0        0 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/__init__.py
--rw-r--r--   0        0        0      960 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0     5591 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0      892 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     1733 2023-06-12 00:37:42.043107 gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 gpt_fn-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-12 11:29:13.874951 gpt_fn-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3023 2023-06-12 11:29:13.874951 gpt_fn-0.0.5/README.md
+-rw-r--r--   0        0        0      758 2023-06-12 11:29:41.779048 gpt_fn-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0      767 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0     1212 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/completion.py
+-rw-r--r--   0        0        0      537 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      342 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/exceptions.py
+-rw-r--r--   0        0        0      655 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0      284 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0     1462 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__snapshots__/test_completion.ambr
+-rw-r--r--   0        0        0      330 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0     3423 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0     4360 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0     2794 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0     2656 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_chat_completion_incomplete.yaml
+-rw-r--r--   0        0        0      872 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0     1077 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/test_completion.py
+-rw-r--r--   0        0        0      522 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1945 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     2411 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0     5591 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0      892 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     1733 2023-06-12 11:29:13.878951 gpt_fn-0.0.5/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 gpt_fn-0.0.5/PKG-INFO
```

### Comparing `gpt_fn-0.0.4/LICENSE` & `gpt_fn-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/README.md` & `gpt_fn-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/pyproject.toml` & `gpt_fn-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `gpt_fn-0.0.4/src/gpt_fn/conftest.py` & `gpt_fn-0.0.5/src/gpt_fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/prompt.py` & `gpt_fn-0.0.5/src/gpt_fn/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from typing import Any, Literal
+from typing import Literal
 
 import jinja2
 from pydantic import BaseModel
 
+from .completion import Message
+
 
 class MessageTemplate(BaseModel):
     role: Literal["system", "user", "assistant"]
     content: str
 
-    def render(self, **kwargs: str) -> dict[str, Any]:
+    def render(self, **kwargs: str) -> Message:
         return {
             "role": self.role,
             "content": jinja2.Template(self.content).render(**kwargs),
         }
 
     class Config:
         # remove whitespace
         anystr_strip_whitespace = True
 
 
 class ChatTemplate(BaseModel):
     messages: list[MessageTemplate]
 
-    def render(self, **kwargs: str) -> list[dict[str, Any]]:
+    def render(self, **kwargs: str) -> list[Message]:
         return [m.render(**kwargs) for m in self.messages]
```

### Comparing `gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml` & `gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_ai_fabnocci.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 interactions:
 - request:
-    body: '{"model": "gpt-3.5-turbo", "messages": [{"role": "system", "content": "You
-      are now the following python function:\n```\n# return fabnocci number\ndef fabnocci(n:
-      int):\n```\nOnly respond with your `return` value.\nThe output should be formatted
-      as a JSON instance that conforms to the JSON schema below.\n\nAs an example,
-      for the schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\":
-      \"a list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
-      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
-      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
-      is not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\":
-      {\"ret\": {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
-      {"role": "user", "content": "fabnocci(10)"}], "temperature": 0.0}'
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# return fabnocci number\ndef fabnocci(n: int):\n```\nOnly
+      respond with your `return` value.\nThe output should be formatted as a JSON
+      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
+      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
+      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
+      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
+      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
+      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
+      {\"title\": \"Ret\", \"type\": \"integer\"}}, \"required\": [\"ret\"]}\n```"},
+      {"role": "user", "content": "fabnocci(10)"}], "model": "gpt-3.5-turbo", "temperature":
+      0.0, "top_p": 1.0, "frequency_penalty": 0.0, "presence_penalty": 0.0, "user":
+      "", "stop": null}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '884'
+      - '975'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.7
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
-        "3.11.3", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
-        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
+        "3.10.8", "platform": "Linux-5.15.0-72-generic-x86_64-with-glibc2.35", "publisher":
+        "openai", "uname": "Linux 5.15.0-72-generic #79-Ubuntu SMP Wed Apr 19 08:22:18
+        UTC 2023 x86_64"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7POvK29Ub10UemzsvNYhSCImY1xJh\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686288362,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+      string: "{\n  \"id\": \"chatcmpl-7QZLqAOMdygD2B0nE7xwIlZbI5dYJ\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686566774,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
         \ \"usage\": {\n    \"prompt_tokens\": 199,\n    \"completion_tokens\": 6,\n
         \   \"total_tokens\": 205\n  },\n  \"choices\": [\n    {\n      \"message\":
         {\n        \"role\": \"assistant\",\n        \"content\": \"{\\\"ret\\\":
         55}\"\n      },\n      \"finish_reason\": \"stop\",\n      \"index\": 0\n
         \   }\n  ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d46f515de330728-TPE
+      - 7d618241afc24a1e-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 09 Jun 2023 05:26:02 GMT
+      - Mon, 12 Jun 2023 10:46:14 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '817'
+      - '394'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
@@ -80,12 +82,12 @@
       x-ratelimit-remaining-tokens:
       - '89809'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
       - 126ms
       x-request-id:
-      - d1dc3dde477e92ba22a78a13f041b366
+      - 493e1bf4e826813b9d18a2843a8f3b9b
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.4/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml` & `gpt_fn-0.0.5/src/gpt_fn/tests/cassettes/test_ai_fake_hero.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 interactions:
 - request:
-    body: '{"model": "gpt-3.5-turbo", "messages": [{"role": "system", "content": "You
-      are now the following python function:\n```\n# generate fake hero.\ndef fake_hero(n:
-      int):\n```\nOnly respond with your `return` value.\nThe output should be formatted
-      as a JSON instance that conforms to the JSON schema below.\n\nAs an example,
-      for the schema {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\":
-      \"a list of strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}},
-      \"required\": [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted
-      instance of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}}
-      is not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\":
-      {\"ret\": {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
+    body: '{"messages": [{"role": "system", "content": "You are now the following
+      python function:\n```\n# generate fake hero.\ndef fake_hero(n: int):\n```\nOnly
+      respond with your `return` value.\nThe output should be formatted as a JSON
+      instance that conforms to the JSON schema below.\n\nAs an example, for the schema
+      {\"properties\": {\"foo\": {\"title\": \"Foo\", \"description\": \"a list of
+      strings\", \"type\": \"array\", \"items\": {\"type\": \"string\"}}}, \"required\":
+      [\"foo\"]}}\nthe object {\"foo\": [\"bar\", \"baz\"]} is a well-formatted instance
+      of the schema. The object {\"properties\": {\"foo\": [\"bar\", \"baz\"]}} is
+      not well-formatted.\n\nHere is the output schema:\n```\n{\"properties\": {\"ret\":
+      {\"title\": \"Ret\", \"type\": \"array\", \"items\": {\"$ref\": \"#/definitions/Hero\"}}},
       \"required\": [\"ret\"], \"definitions\": {\"Hero\": {\"title\": \"Hero\", \"description\":
       \"Hero model.\", \"type\": \"object\", \"properties\": {\"name\": {\"title\":
       \"Name\", \"type\": \"string\"}, \"age\": {\"title\": \"Age\", \"type\": \"integer\"}},
       \"required\": [\"name\", \"age\"]}}}\n```"}, {"role": "user", "content": "fake_hero(5)"}],
-      "temperature": 0.0}'
+      "model": "gpt-3.5-turbo", "temperature": 0.0, "top_p": 1.0, "frequency_penalty":
+      0.0, "presence_penalty": 0.0, "user": "", "stop": null}'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '1197'
+      - '1288'
       Content-Type:
       - application/json
       User-Agent:
       - OpenAI/v1 PythonBindings/0.27.7
       X-OpenAI-Client-User-Agent:
       - '{"bindings_version": "0.27.7", "httplib": "requests", "lang": "python", "lang_version":
-        "3.11.3", "platform": "macOS-13.4-x86_64-i386-64bit", "publisher": "openai",
-        "uname": "Darwin 22.5.0 Darwin Kernel Version 22.5.0: Mon Apr 24 20:53:44
-        PDT 2023; root:xnu-8796.121.2~5/RELEASE_ARM64_T8103 x86_64 i386"}'
+        "3.10.8", "platform": "Linux-5.15.0-72-generic-x86_64-with-glibc2.35", "publisher":
+        "openai", "uname": "Linux 5.15.0-72-generic #79-Ubuntu SMP Wed Apr 19 08:22:18
+        UTC 2023 x86_64"}'
     method: POST
     uri: https://api.openai.com/v1/chat/completions
   response:
     body:
-      string: "{\n  \"id\": \"chatcmpl-7POvLzz9bmjkVW62iee8coYLZUEsD\",\n  \"object\":
-        \"chat.completion\",\n  \"created\": 1686288363,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
+      string: "{\n  \"id\": \"chatcmpl-7QZLqztg5MYsSMGntIfhFHyEduL4n\",\n  \"object\":
+        \"chat.completion\",\n  \"created\": 1686566774,\n  \"model\": \"gpt-3.5-turbo-0301\",\n
         \ \"usage\": {\n    \"prompt_tokens\": 278,\n    \"completion_tokens\": 107,\n
         \   \"total_tokens\": 385\n  },\n  \"choices\": [\n    {\n      \"message\":
         {\n        \"role\": \"assistant\",\n        \"content\": \"```json\\n{\\n
         \   \\\"ret\\\": [\\n        {\\n            \\\"name\\\": \\\"Superman\\\",\\n
         \           \\\"age\\\": 35\\n        },\\n        {\\n            \\\"name\\\":
         \\\"Batman\\\",\\n            \\\"age\\\": 40\\n        },\\n        {\\n
         \           \\\"name\\\": \\\"Spiderman\\\",\\n            \\\"age\\\": 25\\n
@@ -51,37 +52,37 @@
         \\\"Iron Man\\\",\\n            \\\"age\\\": 45\\n        }\\n    ]\\n}\\n```\"\n
         \     },\n      \"finish_reason\": \"stop\",\n      \"index\": 0\n    }\n
         \ ]\n}\n"
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7d46f51cfa96a343-TPE
+      - 7d618245ab316b6e-TPE
       Cache-Control:
       - no-cache, must-revalidate
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 09 Jun 2023 05:26:08 GMT
+      - Mon, 12 Jun 2023 10:46:19 GMT
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       access-control-allow-origin:
       - '*'
       alt-svc:
       - h3=":443"; ma=86400
       openai-model:
       - gpt-3.5-turbo-0301
       openai-processing-ms:
-      - '5540'
+      - '4195'
       openai-version:
       - '2020-10-01'
       strict-transport-security:
       - max-age=15724800; includeSubDomains
       x-ratelimit-limit-requests:
       - '3500'
       x-ratelimit-limit-tokens:
@@ -91,12 +92,12 @@
       x-ratelimit-remaining-tokens:
       - '89743'
       x-ratelimit-reset-requests:
       - 17ms
       x-ratelimit-reset-tokens:
       - 170ms
       x-request-id:
-      - 87cb42ea1e3cc020be707c2c3121c079
+      - 017d559b51c138572998a217aeff9fb4
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `gpt_fn-0.0.4/src/gpt_fn/tests/test_ai_function.py` & `gpt_fn-0.0.5/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/tests/test_prompt.py` & `gpt_fn-0.0.5/src/gpt_fn/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/utils/pydantic_parser.py` & `gpt_fn-0.0.5/src/gpt_fn/utils/pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/utils/signature.py` & `gpt_fn-0.0.5/src/gpt_fn/utils/signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.0.5/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.0.5/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.0.5/src/gpt_fn/utils/tests/test_pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/src/gpt_fn/utils/tests/test_signature.py` & `gpt_fn-0.0.5/src/gpt_fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.0.4/PKG-INFO` & `gpt_fn-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

