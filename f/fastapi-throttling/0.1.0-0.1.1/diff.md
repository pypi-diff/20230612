# Comparing `tmp/fastapi_throttling-0.1.0.tar.gz` & `tmp/fastapi_throttling-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.1.tar", max compression
```

## Comparing `fastapi_throttling-0.1.0.tar` & `fastapi_throttling-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-10 10:35:09.660298 fastapi_throttling-0.1.0/LICENSE
--rw-r--r--   0        0        0       63 2023-06-10 10:35:09.660298 fastapi_throttling-0.1.0/README.md
--rw-r--r--   0        0        0     1751 2023-06-10 10:35:09.660298 fastapi_throttling-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-10 10:35:09.660298 fastapi_throttling-0.1.0/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     2720 2023-06-10 10:35:09.664299 fastapi_throttling-0.1.0/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1343 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/README.md
+-rw-r--r--   0        0        0     1803 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     3068 2023-06-12 07:21:12.250480 fastapi_throttling-0.1.1/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.1/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.0/LICENSE` & `fastapi_throttling-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.0/pyproject.toml` & `fastapi_throttling-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.0"
+version = "0.1.1"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -18,14 +18,16 @@
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 httpx = "^0.24.1"
 pytest-redis = "^3.0.2"
 debugpy = "^1.6.7"
 types-redis = "^4.5.5.2"
+pytest-asyncio = "^0.21.0"
+asgi-lifespan = "^2.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
```

### Comparing `fastapi_throttling-0.1.0/src/fastapi_throttling/throttle.py` & `fastapi_throttling-0.1.1/src/fastapi_throttling/throttle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,97 @@
-from fastapi import HTTPException, Request, Response
-from redis import Redis
-from starlette.middleware.base import (
-    BaseHTTPMiddleware,
-    RequestResponseEndpoint,
-)
-from starlette.types import ASGIApp
+from typing import Any, Awaitable
 
+from redis.asyncio import Redis
+from starlette.datastructures import Headers
+from starlette.responses import JSONResponse
+from starlette.types import ASGIApp, Receive, Scope, Send
 
-class ThrottlingError(HTTPException):
+ResponseT = Awaitable | Any
+
+
+class ThrottlingResponse(JSONResponse):
     def __init__(self):
-        super().__init__(status_code=429, detail="Too Many Requests")
+        content = {"detail": "Too Many Requests"}
+        status_code = 429
+        super().__init__(status_code=status_code, content=content)
 
 
-class ThrottlingMiddleware(BaseHTTPMiddleware):
+class ThrottlingMiddleware:
     """
     Middleware for throttling requests based on IP address and access token.
 
     The middleware uses a Redis server to keep track of the request counts.
     If a limit is reached within a specified time window, further requests
     are blocked until the window is expired.
 
     Attributes:
         app: The FastAPI application to apply the middleware to.
         limit: The maximum number of requests allowed within the time window.
         window: The time window in seconds.
-        redis: The Redis server instance.
+        redis: The Redis client instance.
 
     Methods:
         __call__: Intercept incoming requests and apply the rate limiting.
-        is_rate_limited: Check if the number of requests has exceeded the limit for
-            a given identifier.
+        has_exceeded_rate_limit: Check if the number of requests has exceeded the limit
+            for a given identifier.
     """
 
     def __init__(
         self,
         app: ASGIApp,
         limit: int = 100,
         window: int = 60,
-        redis_host: str | None = 'localhost',
-        redis_port: int | None = 6379,
+        token_header: str = "Authorization",
         redis: Redis | None = None,
-    ):
+    ) -> None:
         self.app = app
+        self.token_header = token_header
         self.limit = limit
         self.window = window
-
         if redis:
             self.redis = redis
-        elif redis_host and redis_port:
-            self.redis = Redis(host=redis_host, port=redis_port)
         else:
-            raise ValueError('Redis server not configured')
-
-        super().__init__(app)
-
-    async def dispatch(
-        self, request: Request, call_next: RequestResponseEndpoint
-    ) -> Response:
-        client_ip = request.client.host
-        token = request.headers.get('Authorization')
+            self.redis = Redis()
 
+    async def __call__(
+        self, scope: Scope, receive: Receive, send: Send
+    ) -> None:
+        if scope["type"] != "http":
+            await self.app(scope, receive, send)
+
+        headers = Headers(scope=scope)
+
+        client_ip = headers.get(
+            "x-forwarded-for", next(iter(scope["client"][0]), None)
+        )
         # Throttle by IP
-        if self.has_exceeded_rate_limit(client_ip):
-            raise ThrottlingError
+        if client_ip and await self.has_exceeded_rate_limit(client_ip):
+            response = ThrottlingResponse()
+            await response(scope, receive, send)
+            return
 
+        token = headers.get(self.token_header)
         # Throttle by Token
-        if token and self.has_exceeded_rate_limit(token):
-            raise ThrottlingError
+        if token and await self.has_exceeded_rate_limit(token):
+            response = ThrottlingResponse()
+            await response(scope, receive, send)
+            return
 
-        response = await call_next(request)
-        return response
+        await self.app(scope, receive, send)
+        return
 
-    def has_exceeded_rate_limit(self, identifier: str) -> bool:
-        current_count = self.redis.get(identifier)
+    async def has_exceeded_rate_limit(self, identifier: str) -> bool:
+        current_count = await self.redis.get(identifier)
 
         if current_count is None:
             # This is the first request with this identifier within the window
-            self.redis.set(identifier, 1, ex=self.window)  # Start a new window
+            await self.redis.set(
+                identifier, 1, ex=self.window
+            )  # Start a new window
             return False
 
         if int(current_count) < self.limit:
             # Increase the request count
-            self.redis.incr(identifier)
+            await self.redis.incr(identifier)
             return False
 
         return True
```

