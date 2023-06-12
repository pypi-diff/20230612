# Comparing `tmp/zhipuai-1.0.4.tar.gz` & `tmp/zhipuai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-1.0.4.tar", last modified: Fri Jun  9 06:06:24 2023, max compression
+gzip compressed data, was "zhipuai-1.0.7.tar", last modified: Mon Jun 12 12:15:09 2023, max compression
```

## Comparing `zhipuai-1.0.4.tar` & `zhipuai-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.369118 zhipuai-1.0.4/
--rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-09 06:06:24.368965 zhipuai-1.0.4/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.4/README.md
--rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-09 06:06:24.369154 zhipuai-1.0.4/setup.cfg
--rw-r--r--   0 haowangai   (501) staff       (20)      899 2023-06-09 06:05:00.000000 zhipuai-1.0.4/setup.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.366192 zhipuai-1.0.4/zhipuai/
--rw-r--r--   0 haowangai   (501) staff       (20)      221 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/__init__.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.367183 zhipuai-1.0.4/zhipuai/examples/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/examples/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1466 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/examples/chatglm6b_example.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1427 2023-06-09 02:23:14.000000 zhipuai-1.0.4/zhipuai/examples/model_api_example.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.367939 zhipuai-1.0.4/zhipuai/model_api/
--rw-r--r--   0 haowangai   (501) staff       (20)      102 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/model_api/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1858 2023-06-09 02:21:28.000000 zhipuai-1.0.4/zhipuai/model_api/api.py
--rw-r--r--   0 haowangai   (501) staff       (20)      246 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/model_api/chatglm_params.py
--rw-r--r--   0 haowangai   (501) staff       (20)      272 2023-06-09 02:21:28.000000 zhipuai-1.0.4/zhipuai/model_api/params.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.368598 zhipuai-1.0.4/zhipuai/utils/
--rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-05 13:56:33.000000 zhipuai-1.0.4/zhipuai/utils/__init__.py
--rw-r--r--   0 haowangai   (501) staff       (20)     1252 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/utils/http_client.py
--rw-r--r--   0 haowangai   (501) staff       (20)      700 2023-06-08 03:38:31.000000 zhipuai-1.0.4/zhipuai/utils/jwt_token.py
--rw-r--r--   0 haowangai   (501) staff       (20)     4531 2023-06-08 10:53:33.000000 zhipuai-1.0.4/zhipuai/utils/sse_client.py
-drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-09 06:06:24.366802 zhipuai-1.0.4/zhipuai.egg-info/
--rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/PKG-INFO
--rw-r--r--   0 haowangai   (501) staff       (20)      526 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/SOURCES.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/dependency_links.txt
--rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/requires.txt
--rw-r--r--   0 haowangai   (501) staff       (20)        8 2023-06-09 06:06:24.000000 zhipuai-1.0.4/zhipuai.egg-info/top_level.txt
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-12 12:15:09.915959 zhipuai-1.0.7/
+-rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-12 12:15:09.915830 zhipuai-1.0.7/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)       11 2023-04-26 12:22:24.000000 zhipuai-1.0.7/README.md
+-rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-12 12:15:09.915994 zhipuai-1.0.7/setup.cfg
+-rw-r--r--   0 haowangai   (501) staff       (20)      899 2023-06-12 12:14:41.000000 zhipuai-1.0.7/setup.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-12 12:15:09.913043 zhipuai-1.0.7/zhipuai/
+-rw-r--r--   0 haowangai   (501) staff       (20)      221 2023-06-08 03:38:31.000000 zhipuai-1.0.7/zhipuai/__init__.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-12 12:15:09.914065 zhipuai-1.0.7/zhipuai/examples/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-08 03:38:31.000000 zhipuai-1.0.7/zhipuai/examples/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1466 2023-06-08 03:38:31.000000 zhipuai-1.0.7/zhipuai/examples/chatglm6b_example.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1427 2023-06-09 02:23:14.000000 zhipuai-1.0.7/zhipuai/examples/model_api_example.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-12 12:15:09.914837 zhipuai-1.0.7/zhipuai/model_api/
+-rw-r--r--   0 haowangai   (501) staff       (20)      102 2023-06-08 03:38:31.000000 zhipuai-1.0.7/zhipuai/model_api/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1754 2023-06-12 10:36:58.000000 zhipuai-1.0.7/zhipuai/model_api/api.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      246 2023-06-08 03:38:31.000000 zhipuai-1.0.7/zhipuai/model_api/chatglm_params.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      272 2023-06-09 02:21:28.000000 zhipuai-1.0.7/zhipuai/model_api/params.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-12 12:15:09.915496 zhipuai-1.0.7/zhipuai/utils/
+-rw-r--r--   0 haowangai   (501) staff       (20)        0 2023-06-05 13:56:33.000000 zhipuai-1.0.7/zhipuai/utils/__init__.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     1432 2023-06-12 10:24:29.000000 zhipuai-1.0.7/zhipuai/utils/http_client.py
+-rw-r--r--   0 haowangai   (501) staff       (20)      700 2023-06-08 03:38:31.000000 zhipuai-1.0.7/zhipuai/utils/jwt_token.py
+-rw-r--r--   0 haowangai   (501) staff       (20)     4531 2023-06-08 10:53:33.000000 zhipuai-1.0.7/zhipuai/utils/sse_client.py
+drwxr-xr-x   0 haowangai   (501) staff       (20)        0 2023-06-12 12:15:09.913682 zhipuai-1.0.7/zhipuai.egg-info/
+-rw-r--r--   0 haowangai   (501) staff       (20)      488 2023-06-12 12:15:09.000000 zhipuai-1.0.7/zhipuai.egg-info/PKG-INFO
+-rw-r--r--   0 haowangai   (501) staff       (20)      526 2023-06-12 12:15:09.000000 zhipuai-1.0.7/zhipuai.egg-info/SOURCES.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)        1 2023-06-12 12:15:09.000000 zhipuai-1.0.7/zhipuai.egg-info/dependency_links.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)       38 2023-06-12 12:15:09.000000 zhipuai-1.0.7/zhipuai.egg-info/requires.txt
+-rw-r--r--   0 haowangai   (501) staff       (20)        8 2023-06-12 12:15:09.000000 zhipuai-1.0.7/zhipuai.egg-info/top_level.txt
```

### Comparing `zhipuai-1.0.4/setup.py` & `zhipuai-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 with open("requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
 
 setup(
     name="zhipuai",
-    version="v1.0.4",
+    version="v1.0.7",
     description="A SDK library for accessing big model apis from ZhipuAI",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Zhipu AI",
     url="https://open.bigmodel.cn/",
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
```

### Comparing `zhipuai-1.0.4/zhipuai/examples/chatglm6b_example.py` & `zhipuai-1.0.7/zhipuai/examples/chatglm6b_example.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.4/zhipuai/examples/model_api_example.py` & `zhipuai-1.0.7/zhipuai/examples/model_api_example.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.4/zhipuai/model_api/api.py` & `zhipuai-1.0.7/zhipuai/model_api/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding:utf-8 -*-
-import json
-import os.path
+import posixpath
 
 import zhipuai
 from zhipuai.utils import jwt_token
 from zhipuai.utils.http_client import get, post, stream
 from zhipuai.utils.sse_client import SSEClient
 
 
@@ -14,28 +13,25 @@
     SSE = "sse-invoke"
 
 
 class ModelAPI:
     @classmethod
     def invoke(cls, **kwargs):
         url = cls._build_api_url(kwargs, InvokeType.SYNC)
-        data = post(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
-        return json.loads(data)
+        return post(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
 
     @classmethod
     def async_invoke(cls, **kwargs):
         url = cls._build_api_url(kwargs, InvokeType.ASYNC)
-        data = post(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
-        return json.loads(data)
+        return post(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
 
     @classmethod
     def query_async_invoke_result(cls, task_id: str):
         url = cls._build_api_url(None, InvokeType.ASYNC, task_id)
-        data = get(url, cls._generate_token(), zhipuai.api_timeout_seconds)
-        return json.loads(data)
+        return get(url, cls._generate_token(), zhipuai.api_timeout_seconds)
 
     @classmethod
     def sse_invoke(cls, **kwargs):
         url = cls._build_api_url(kwargs, InvokeType.SSE)
         data = stream(url, cls._generate_token(), kwargs, zhipuai.api_timeout_seconds)
         return SSEClient(data)
 
@@ -44,15 +40,15 @@
         if kwargs:
             if "model" not in kwargs:
                 raise Exception("model param missed")
             model = kwargs.pop("model")
         else:
             model = "-"
 
-        return os.path.join(zhipuai.model_api_url, model, *path)
+        return posixpath.join(zhipuai.model_api_url, model, *path)
 
     @staticmethod
     def _generate_token():
         if not zhipuai.api_key:
             raise Exception(
                 "api_key not provided, you could provide it with `shell: export API_KEY=xxx` or `code: zhipuai.api_key=xxx`"
             )
```

### Comparing `zhipuai-1.0.4/zhipuai/utils/http_client.py` & `zhipuai-1.0.7/zhipuai/utils/http_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,36 +12,39 @@
 
 def post(api_url, token, params, timeout):
     try:
         headers.update({"Authorization": token})
         resp = requests.post(
             url=api_url, data=json.dumps(params), headers=headers, timeout=timeout
         )
-        if requests.codes.ok == resp.status_code:
-            return resp.text
+        if requests.codes.ok != resp.status_code:
+            raise Exception("响应异常：" + resp.content)
+        return json.loads(resp.text)
     except Exception as e:
         logging.exception("请求异常", e)
 
 
 def stream(api_url, token, params, timeout):
     try:
         resp = requests.post(
             api_url,
             stream=True,
             headers={"Authorization": token},
             json=params,
             timeout=timeout,
         )
-        if requests.codes.ok == resp.status_code:
-            return resp
+        if requests.codes.ok != resp.status_code:
+            raise Exception("请求异常")
+        return resp
     except Exception as e:
         logging.exception("请求异常", e)
 
 
 def get(api_url, token, timeout):
     try:
         headers.update({"Authorization": token})
         resp = requests.get(api_url, headers=headers, timeout=timeout)
-        if requests.codes.ok == resp.status_code:
-            return resp.text
+        if requests.codes.ok != resp.status_code:
+            raise Exception("响应异常：" + resp.content)
+        return json.loads(resp.text)
     except Exception as e:
         logging.exception("请求异常", e)
```

### Comparing `zhipuai-1.0.4/zhipuai/utils/jwt_token.py` & `zhipuai-1.0.7/zhipuai/utils/jwt_token.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.4/zhipuai/utils/sse_client.py` & `zhipuai-1.0.7/zhipuai/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `zhipuai-1.0.4/zhipuai.egg-info/SOURCES.txt` & `zhipuai-1.0.7/zhipuai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

