# Comparing `tmp/chima-0.0.7.tar.gz` & `tmp/chima-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chima-0.0.7.tar", max compression
+gzip compressed data, was "chima-0.0.8.tar", max compression
```

## Comparing `chima-0.0.7.tar` & `chima-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     2253 2023-06-08 03:14:29.940834 chima-0.0.7/README.md
--rw-r--r--   0        0        0      365 2023-06-08 03:14:29.940834 chima-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/__init__.py
--rw-r--r--   0        0        0     8944 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/client.py
--rw-r--r--   0        0        0      348 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      159 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/environment.py
--rw-r--r--   0        0        0        0 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/py.typed
--rw-r--r--   0        0        0      220 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/types/__init__.py
--rw-r--r--   0        0        0      757 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/types/generate_text_response.py
--rw-r--r--   0        0        0      920 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/types/search_response.py
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2253 2023-06-12 03:33:44.967216 chima-0.0.8/README.md
+-rw-r--r--   0        0        0      365 2023-06-12 03:33:44.967216 chima-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      275 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/__init__.py
+-rw-r--r--   0        0        0    11927 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/client.py
+-rw-r--r--   0        0        0      348 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      159 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/environment.py
+-rw-r--r--   0        0        0        0 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/py.typed
+-rw-r--r--   0        0        0      288 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/types/__init__.py
+-rw-r--r--   0        0        0      754 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/types/converse_response.py
+-rw-r--r--   0        0        0      757 2023-06-12 03:33:44.967216 chima-0.0.8/src/chima/types/generate_text_response.py
+-rw-r--r--   0        0        0      920 2023-06-12 03:33:44.971216 chima-0.0.8/src/chima/types/search_response.py
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.8/PKG-INFO
```

### Comparing `chima-0.0.7/README.md` & `chima-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `chima-0.0.7/src/chima/client.py` & `chima-0.0.8/src/chima/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from .core.api_error import ApiError
 from .core.jsonable_encoder import jsonable_encoder
+from .core.remove_none_from_headers import remove_none_from_headers
 from .environment import ChimaEnvironment
+from .types.converse_response import ConverseResponse
 from .types.generate_text_response import GenerateTextResponse
 from .types.search_response import SearchResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class Chima:
-    def __init__(self, *, environment: ChimaEnvironment = ChimaEnvironment.PRODUCTION):
+    def __init__(self, *, environment: ChimaEnvironment = ChimaEnvironment.PRODUCTION, token: str):
         self._environment = environment
+        self._token = token
 
     def search(
         self,
         group_id: str,
         *,
         query: str,
         provider: typing.Optional[str] = OMIT,
@@ -38,14 +41,17 @@
             _request["id"] = id
         if pdf is not OMIT:
             _request["pdf"] = pdf
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"search/{group_id}"),
             json=jsonable_encoder(_request),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
@@ -53,14 +59,17 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def stream(self, *, level_context: str) -> typing.Iterator[str]:
         with httpx.stream(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api_streaming"),
             json=jsonable_encoder({"level_context": level_context}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _text in _response.iter_text():
                     if len(_text) == 0:
                         continue
                     yield pydantic.parse_obj_as(str, json.loads(_text))  # type: ignore
@@ -108,28 +117,50 @@
                     "last_workout_completed": last_workout_completed,
                     "last_workout_week": last_workout_week,
                     "last_week_completed": last_week_completed,
                     "delta_moves": delta_moves,
                     "notification_type": notification_type,
                 }
             ),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateTextResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def converse(self, *, user_question: str) -> ConverseResponse:
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", "converse"),
+            json=jsonable_encoder({"user_question": user_question}),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ConverseResponse, _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncChima:
-    def __init__(self, *, environment: ChimaEnvironment = ChimaEnvironment.PRODUCTION):
+    def __init__(self, *, environment: ChimaEnvironment = ChimaEnvironment.PRODUCTION, token: str):
         self._environment = environment
+        self._token = token
 
     async def search(
         self,
         group_id: str,
         *,
         query: str,
         provider: typing.Optional[str] = OMIT,
@@ -144,14 +175,17 @@
         if pdf is not OMIT:
             _request["pdf"] = pdf
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"search/{group_id}"),
                 json=jsonable_encoder(_request),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
@@ -160,14 +194,17 @@
 
     async def stream(self, *, level_context: str) -> typing.AsyncIterator[str]:
         async with httpx.AsyncClient() as _client:
             async with _client.stream(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api_streaming"),
                 json=jsonable_encoder({"level_context": level_context}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             ) as _response:
                 if 200 <= _response.status_code < 300:
                     async for _text in _response.aiter_text():
                         if len(_text) == 0:
                             continue
                         yield pydantic.parse_obj_as(str, json.loads(_text))  # type: ignore
@@ -216,16 +253,38 @@
                         "last_workout_completed": last_workout_completed,
                         "last_workout_week": last_workout_week,
                         "last_week_completed": last_week_completed,
                         "delta_moves": delta_moves,
                         "notification_type": notification_type,
                     }
                 ),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GenerateTextResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def converse(self, *, user_question: str) -> ConverseResponse:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", "converse"),
+                json=jsonable_encoder({"user_question": user_question}),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ConverseResponse, _response_json)  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `chima-0.0.7/src/chima/core/datetime_utils.py` & `chima-0.0.8/src/chima/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.7/src/chima/core/jsonable_encoder.py` & `chima-0.0.8/src/chima/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.7/src/chima/types/generate_text_response.py` & `chima-0.0.8/src/chima/types/generate_text_response.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.7/src/chima/types/search_response.py` & `chima-0.0.8/src/chima/types/search_response.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.7/PKG-INFO` & `chima-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chima
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

