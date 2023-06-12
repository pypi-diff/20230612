# Comparing `tmp/HTTP-PyServer-0.1.4.2.1.tar.gz` & `tmp/HTTP-PyServer-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.4.2.1.tar", last modified: Sun Jun 11 02:13:36 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.4.3.tar", last modified: Mon Jun 12 00:05:29 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.4.2.1.tar` & `HTTP-PyServer-0.1.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.298981 HTTP-PyServer-0.1.4.2.1/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.2.1/LICENSE
--rw-rw-rw-   0        0        0     2108 2023-06-11 02:13:36.296988 HTTP-PyServer-0.1.4.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.2.1/README.md
--rw-rw-rw-   0        0        0      645 2023-06-11 02:13:12.000000 HTTP-PyServer-0.1.4.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 02:13:36.299979 HTTP-PyServer-0.1.4.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.225150 HTTP-PyServer-0.1.4.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.255585 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2108 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 02:13:36.000000 HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 02:13:36.293993 HTTP-PyServer-0.1.4.2.1/src/server/
--rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.2.1/src/server/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.2.1/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.2.1/src/server/render.py
--rw-rw-rw-   0        0        0     4565 2023-06-11 02:11:17.000000 HTTP-PyServer-0.1.4.2.1/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.2.1/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.2.1/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.2.1/src/server/response_messages.py
--rw-rw-rw-   0        0        0     8864 2023-05-17 20:18:32.000000 HTTP-PyServer-0.1.4.2.1/src/server/routes.py
--rw-rw-rw-   0        0        0     7449 2023-06-11 02:12:16.000000 HTTP-PyServer-0.1.4.2.1/src/server/server.py
--rw-rw-rw-   0        0        0     3608 2023-05-17 19:38:59.000000 HTTP-PyServer-0.1.4.2.1/src/server/sessions.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.2.1/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.343387 HTTP-PyServer-0.1.4.3/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     2106 2023-06-12 00:05:29.342388 HTTP-PyServer-0.1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-06-11 01:47:44.000000 HTTP-PyServer-0.1.4.3/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-12 00:05:06.000000 HTTP-PyServer-0.1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 00:05:29.344383 HTTP-PyServer-0.1.4.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.282549 HTTP-PyServer-0.1.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.306484 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2106 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 00:05:29.000000 HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 00:05:29.340394 HTTP-PyServer-0.1.4.3/src/server/
+-rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4.3/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4.3/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4.3/src/server/render.py
+-rw-rw-rw-   0        0        0     4667 2023-06-12 00:04:01.000000 HTTP-PyServer-0.1.4.3/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4.3/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4.3/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4.3/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     8866 2023-06-11 23:42:15.000000 HTTP-PyServer-0.1.4.3/src/server/routes.py
+-rw-rw-rw-   0        0        0     7406 2023-06-11 23:52:43.000000 HTTP-PyServer-0.1.4.3/src/server/server.py
+-rw-rw-rw-   0        0        0     3588 2023-06-11 23:50:14.000000 HTTP-PyServer-0.1.4.3/src/server/sessions.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4.3/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.4.2.1/LICENSE` & `HTTP-PyServer-0.1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2.1/PKG-INFO` & `HTTP-PyServer-0.1.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.2.1
+Version: 0.1.4.3
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.2.1/README.md` & `HTTP-PyServer-0.1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2.1/pyproject.toml` & `HTTP-PyServer-0.1.4.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.4.2.1"
+version = "0.1.4.3"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.4.2.1/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.4.3/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.4.2.1
+Version: 0.1.4.3
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/cache.py` & `HTTP-PyServer-0.1.4.3/src/server/cache.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/render.py` & `HTTP-PyServer-0.1.4.3/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/request.py` & `HTTP-PyServer-0.1.4.3/src/server/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from typing import Self
 import urllib
 import json
 
 class Request:
     '''Represents an HTTP request.'''
 
     def __init__(self,
                  *,
                  address: tuple = (),
                  method: str = '',
                  path: str = '',
                  version: float = '',
                  headers: dict = {},
                  body: str = '',
-                 query: dict = {}):
+                 query: dict = {}) -> None:
         '''Initializes the request class.'''
 
         self.address: tuple[str, int] = address
 
         self.method: str = method
 
         self.path: str = path
@@ -29,15 +30,15 @@
 
         self.query: dict[str, str] = query
 
     @classmethod
     def from_bytestring(cls,
                          *,
                          address: tuple = (),
-                         request: bytes):
+                         request: bytes) -> Self:
         '''Creates a request object from an HTTP request string.'''
 
         lines = request.split(b'\r\n')
 
         method, path, version = lines[0].decode(encoding = 'utf-8',
                                                 errors = 'ignore').split(' ')
 
@@ -76,57 +77,55 @@
                    method = method,
                    path = path,
                    version = float(version.split('/')[1]),
                    headers = headers,
                    body = body,
                    query = query)
     
-    def __str__(self):
+    def __str__(self) -> str:
         '''Returns the request as an HTTP request string.'''
 
         return f'{self.method} {self.path if self.path else "/"} {self.version}\r\n' + \
 '\r\n'.join([f'{key}: {value}' for key, value in self.headers.items()]) + \
 '\r\n\r\n' + \
 self.body.decode(encoding = 'utf-8',
                  errors = 'ignore')
 
-    def cookies(self):
+    def cookies(self) -> dict[str, list[str]]:
         '''Returns the request cookies as a dictionary.'''
 
         try:
 
             cookies = {}
 
             for cookie in self.headers.get('Cookie').split(';'):
 
                 key, value = list(urllib.parse.parse_qs(cookie.strip()).items())[0]
 
                 cookies[key] = value[0]
 
             return cookies
         
-        except Exception as e:
-
-            print(e)
+        except Exception:
 
             return {}
 
-    def json(self):
+    def json(self) -> dict | list:
         '''Returns the request body as a JSON object.'''
 
         return json.loads(self.body.decode(encoding = 'utf-8',
                                            errors = 'ignore'))
     
-    def form(self):
+    def form(self) -> dict[str, list[str]]:
         '''Returns the request body as parsed urlencoded form data.'''
 
         return urllib.parse.parse_qs(self.body.decode(encoding = 'utf-8',
                                                       errors = 'ignore'))
     
-    def files(self):
+    def files(self) -> dict[str, bytes]:
 
         try:
         
             boundry = self.headers.get('Content-Type').split('; ')[1].split('=')[1]
 
             parts = self.body.split(b'--' + boundry.encode(encoding = 'utf-8',
                                     errors = 'ignore') + b'\r\n')[1:]
```

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/response.py` & `HTTP-PyServer-0.1.4.3/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/response_codes.py` & `HTTP-PyServer-0.1.4.3/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/response_messages.py` & `HTTP-PyServer-0.1.4.3/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/routes.py` & `HTTP-PyServer-0.1.4.3/src/server/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
                             self._root(request, session)
 
                         else:
                         
                             self._root(request)
 
-                    message = self._routes[path](request,
+                    message = self._routes[route](request,
                                                  session,
                                                  *wildcard_values)
                     
                     if isinstance(message, str):
 
                         message = render.text(text = message)
 
@@ -205,15 +205,15 @@
 
                             self._root(request, self.sessions.get(self.sessions.add()))
 
                         else:
                         
                             self._root(request)
 
-                    message = self._routes[path](request,
+                    message = self._routes[route](request,
                                                  *wildcard_values)
 
                     if isinstance(message, str):
 
                         message = render.text(text = message)
 
                 if isinstance(message, response.Response):
```

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/server.py` & `HTTP-PyServer-0.1.4.3/src/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,27 +146,27 @@
 
                     if b'\r\n\r\n' in raw_request or raw_request == b'':
 
                         break
 
                 if not raw_request:
                         
-                        if self._logger:
+                    if self._logger:
 
-                            self._logger.debug(f'Connection closed by client \
+                        self._logger.debug(f'Connection closed by client \
 {address[0]}:{address[1]}.')
 
-                        connection.close()
+                    connection.close()
 
-                        return None
+                    return None
 
                 try:
 
                     parsed_request = request.Request.from_bytestring(address = address,
-                                                                request = raw_request)
+                                     request = raw_request)
 
                 except Exception:
 
                     if self._logger:
 
                         self._logger.error(f'Invalid request from \
 {address[0]}:{address[1]}, closing connection.')
```

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/sessions.py` & `HTTP-PyServer-0.1.4.3/src/server/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import threading
 import time
 from typing import Any
 
 class Session:
      
     def __init__(self,
-                session_id: str) -> None:
+                 session_id: str) -> None:
         '''Initializes the session class.'''
         
         self._session_id: str = session_id
         
         self._items: dict[str, Any] = {}
 
     @property
@@ -25,32 +25,30 @@
         '''Adds an item to the session.
         If the item already exists, it is overwritten.'''
         
         self._items[key] = value
 
     def remove(self,
                key: str) -> None:
-         
         '''Removes an item from the session.'''
 
         self._items.pop(key)
 
     def get(self,
             key: str) -> Any:
-         
         '''Gets an item from the session. Returns "None" if the item does not exist.'''
 
         return self._items.get(key)
     
     def update(self) -> None: 
         '''Updates the session id, and resets the timer.'''
 
         self._parent.remove(self._session_id)
 
-        while self._parent._session.get(session_id := secrets.token_urlsafe(128)):
+        while self._parent._sessions.get(session_id := secrets.token_urlsafe(128)):
              pass
         
         self._session_id = session_id
 
         self._parent._sessions[self._session_id] = self
 
         remove_timer = threading.Timer(self._parent._remove_after,
```

### Comparing `HTTP-PyServer-0.1.4.2.1/src/server/template.py` & `HTTP-PyServer-0.1.4.3/src/server/template.py`

 * *Files identical despite different names*

