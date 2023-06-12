# Comparing `tmp/flask-http-middleware-0.2.1.tar.gz` & `tmp/flask-http-middleware-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-http-middleware-0.2.1.tar", last modified: Fri Dec 30 02:42:13 2022, max compression
+gzip compressed data, was "flask-http-middleware-0.2.2.tar", last modified: Mon Jun 12 14:21:51 2023, max compression
```

## Comparing `flask-http-middleware-0.2.1.tar` & `flask-http-middleware-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2022-12-30 02:42:13.975618 flask-http-middleware-0.2.1/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     9133 2022-12-30 02:42:13.975618 flask-http-middleware-0.2.1/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     6347 2022-12-30 02:41:47.000000 flask-http-middleware-0.2.1/README.md
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2022-12-30 02:42:13.971617 flask-http-middleware-0.2.1/flask_http_middleware/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2022-03-20 12:14:27.000000 flask-http-middleware-0.2.1/flask_http_middleware/__init__.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1707 2022-03-20 12:35:18.000000 flask-http-middleware-0.2.1/flask_http_middleware/base.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     6464 2022-12-30 02:40:40.000000 flask-http-middleware-0.2.1/flask_http_middleware/manager.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2022-12-30 02:42:13.971617 flask-http-middleware-0.2.1/flask_http_middleware.egg-info/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     9133 2022-12-30 02:42:12.000000 flask-http-middleware-0.2.1/flask_http_middleware.egg-info/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      339 2022-12-30 02:42:12.000000 flask-http-middleware-0.2.1/flask_http_middleware.egg-info/SOURCES.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2022-12-30 02:42:12.000000 flask-http-middleware-0.2.1/flask_http_middleware.egg-info/dependency_links.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2022-12-30 02:42:12.000000 flask-http-middleware-0.2.1/flask_http_middleware.egg-info/requires.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2022-12-30 02:42:12.000000 flask-http-middleware-0.2.1/flask_http_middleware.egg-info/top_level.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2022-12-30 02:42:13.975618 flask-http-middleware-0.2.1/setup.cfg
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1186 2022-12-30 02:40:59.000000 flask-http-middleware-0.2.1/setup.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:21:51.206378 flask-http-middleware-0.2.2/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1068 2022-03-20 12:47:01.000000 flask-http-middleware-0.2.2/LICENSE
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7286 2023-06-12 14:21:51.206378 flask-http-middleware-0.2.2/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     6347 2022-12-30 02:41:47.000000 flask-http-middleware-0.2.2/README.md
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:21:51.202379 flask-http-middleware-0.2.2/flask_http_middleware/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2022-03-20 12:14:27.000000 flask-http-middleware-0.2.2/flask_http_middleware/__init__.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1707 2022-03-20 12:35:18.000000 flask-http-middleware-0.2.2/flask_http_middleware/base.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7493 2023-06-12 14:20:09.000000 flask-http-middleware-0.2.2/flask_http_middleware/manager.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-12 14:21:51.202379 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7286 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      347 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       15 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/requires.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       22 2023-06-12 14:21:50.000000 flask-http-middleware-0.2.2/flask_http_middleware.egg-info/top_level.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-12 14:21:51.206378 flask-http-middleware-0.2.2/setup.cfg
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1384 2023-06-12 14:21:28.000000 flask-http-middleware-0.2.2/setup.py
```

### Comparing `flask-http-middleware-0.2.1/PKG-INFO` & `flask-http-middleware-0.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,272 +1,276 @@
 Metadata-Version: 2.1
 Name: flask-http-middleware
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module to create middleware with direct access to `request` and `response`
 Home-page: https://github.com/Danangjoyoo/flask-http-middleware
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
-License: UNKNOWN
-Description: # Flask HTTP Middleware
-        [![Downloads](https://static.pepy.tech/personalized-badge/flask-http-middleware?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/flask-http-middleware)
-        
-        
-        ## Installation
-        ```
-        pip install flask-http-middleware
-        ```
-        
-        ## Description
-        A module to create flask middleware with direct access to `request` and `response`.
-        
-        This module implement the starlette's (FastAPI) BaseHTTPMiddleware style to Flask.
-        
-        ## Changelogs
-        - v0.0
-            - First Upload
-        - v0.1
-            - Allow middlewares stacking
-        - v0.2
-            - Adjusting wsgi middleware update for `flask>=2.2.x`
-        
-        ## How to use ?
-        
-        ### Example: adding a response header
-        ```
-        import time
-        from flask import Flask
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class MetricsMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                t0 = time.time()
-                response = call_next(request)
-                response_time = time.time()-t0
-                response.headers.add("response_time", response_time)
-                return response
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(MetricsMiddleware)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        - Note: you can put your `MetricsMiddleware` class in different file
-        
-        Above example is equals with `app.before_request` and `app.after_request` decorated function.
-        
-        ```
-        @app.before_request
-        def start_metrics():
-            g.t0 = time.time()
-        
-        @app.after_request
-        def stop_metrics(response):
-            response_time = time.time()-g.t0
-            response.headers.add("response_time", response_time)
-            return response
-        ```
-        
-        ---
-        
-        ### Example: Authentication
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class AccessMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                if request.headers.get("token") == "secret":
-                    return call_next(request)
-                else:
-                    return jsonify({"message":"invalid token"})
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(AccessMiddleware)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        
-        ---
-        
-        ### Example: add some routers security
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class SecureRoutersMiddleware(BaseHTTPMiddleware):
-            def __init__(self, secured_routers = []):
-                super().__init__()
-                self.secured_routers = secured_routers
-        
-            def dispatch(self, request, call_next):
-                if request.path in self.secured_routers:
-                    if request.headers.get("token") == "secret":
-                        return call_next(request)
-                    else:
-                        return jsonify({"message":"invalid token"})
-                else:
-                    return call_next(request)
-        
-        secured_routers = ["/check_secured"]
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=secured_routers)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        @app.get("/check_secured")
-        def health():
-            return {"message":"Security bypassed"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        
-        ---
-        
-        ### Example: add error handling
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class AccessMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                if request.headers.get("token") == "secret":
-                    return call_next(request)
-                else:
-                    raise Exception("Authentication Failed")
-        
-            def error_handler(self, error):
-                return jsonify({"error": str(error)})
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(AccessMiddleware)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        
-        ### Example: Stacking Middleware
-        You can also stack your middleware
-        
-        `middleware.py`
-        ```
-        import time
-        from flask import jsonify
-        from flask_http_middleware import BaseHTTPMiddleware
-        
-        class AccessMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                if request.headers.get("token") == "secret":
-                    return call_next(request)
-                else:
-                    raise Exception("Authentication Failed")
-        
-            def error_handler(self, error):
-                return jsonify({"error": str(error)})
-        
-        
-        class MetricsMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                t0 = time.time()
-                response = call_next(request)
-                response_time = time.time()-t0
-                response.headers.add("response_time", response_time)
-                return response
-        
-        
-        class SecureRoutersMiddleware(BaseHTTPMiddleware):
-            def __init__(self, secured_routers = []):
-                super().__init__()
-                self.secured_routers = secured_routers
-        
-            def dispatch(self, request, call_next):
-                if request.path in self.secured_routers:
-                    if request.headers.get("token") == "secret":
-                        return call_next(request)
-                    else:
-                        return jsonify({"message":"invalid token"})
-                else:
-                    return call_next(request)
-        
-        ```
-        
-        your `main.py`
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager
-        from middleware import AccessMiddleware, MetricsMiddleware, SecureRoutersMiddleware
-        
-        app = Flask(__name__)
-        
-        my_secured_routers = ["/check_secured"]
-        
-        app.wsgi_app = MiddlewareManager(app)
-        
-        app.wsgi_app.add_middleware(AccessMiddleware)
-        app.wsgi_app.add_middleware(MetricsMiddleware)
-        app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=my_secured_routers)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        @app.get("/check_secured")
-        def health():
-            return {"message":"Security bypassed"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
 Keywords: flask,middleware,http,request,response
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Flask HTTP Middleware
+[![Downloads](https://static.pepy.tech/personalized-badge/flask-http-middleware?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/flask-http-middleware)
+
+
+## Installation
+```
+pip install flask-http-middleware
+```
+
+## Description
+A module to create flask middleware with direct access to `request` and `response`.
+
+This module implement the starlette's (FastAPI) BaseHTTPMiddleware style to Flask.
+
+## Changelogs
+- v0.0
+    - First Upload
+- v0.1
+    - Allow middlewares stacking
+- v0.2
+    - Adjusting wsgi middleware update for `flask>=2.2.x`
+
+## How to use ?
+
+### Example: adding a response header
+```
+import time
+from flask import Flask
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class MetricsMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        t0 = time.time()
+        response = call_next(request)
+        response_time = time.time()-t0
+        response.headers.add("response_time", response_time)
+        return response
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(MetricsMiddleware)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+if __name__ == "__main__":
+    app.run()
+```
+- Note: you can put your `MetricsMiddleware` class in different file
+
+Above example is equals with `app.before_request` and `app.after_request` decorated function.
+
+```
+@app.before_request
+def start_metrics():
+    g.t0 = time.time()
+
+@app.after_request
+def stop_metrics(response):
+    response_time = time.time()-g.t0
+    response.headers.add("response_time", response_time)
+    return response
+```
+
+---
+
+### Example: Authentication
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class AccessMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        if request.headers.get("token") == "secret":
+            return call_next(request)
+        else:
+            return jsonify({"message":"invalid token"})
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(AccessMiddleware)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+if __name__ == "__main__":
+    app.run()
+```
+
+---
+
+### Example: add some routers security
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class SecureRoutersMiddleware(BaseHTTPMiddleware):
+    def __init__(self, secured_routers = []):
+        super().__init__()
+        self.secured_routers = secured_routers
+
+    def dispatch(self, request, call_next):
+        if request.path in self.secured_routers:
+            if request.headers.get("token") == "secret":
+                return call_next(request)
+            else:
+                return jsonify({"message":"invalid token"})
+        else:
+            return call_next(request)
+
+secured_routers = ["/check_secured"]
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=secured_routers)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+@app.get("/check_secured")
+def health():
+    return {"message":"Security bypassed"}
+
+if __name__ == "__main__":
+    app.run()
+```
+
+---
+
+### Example: add error handling
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class AccessMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        if request.headers.get("token") == "secret":
+            return call_next(request)
+        else:
+            raise Exception("Authentication Failed")
+
+    def error_handler(self, error):
+        return jsonify({"error": str(error)})
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(AccessMiddleware)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+if __name__ == "__main__":
+    app.run()
+```
+
+### Example: Stacking Middleware
+You can also stack your middleware
+
+`middleware.py`
+```
+import time
+from flask import jsonify
+from flask_http_middleware import BaseHTTPMiddleware
+
+class AccessMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        if request.headers.get("token") == "secret":
+            return call_next(request)
+        else:
+            raise Exception("Authentication Failed")
+
+    def error_handler(self, error):
+        return jsonify({"error": str(error)})
+
+
+class MetricsMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        t0 = time.time()
+        response = call_next(request)
+        response_time = time.time()-t0
+        response.headers.add("response_time", response_time)
+        return response
+
+
+class SecureRoutersMiddleware(BaseHTTPMiddleware):
+    def __init__(self, secured_routers = []):
+        super().__init__()
+        self.secured_routers = secured_routers
+
+    def dispatch(self, request, call_next):
+        if request.path in self.secured_routers:
+            if request.headers.get("token") == "secret":
+                return call_next(request)
+            else:
+                return jsonify({"message":"invalid token"})
+        else:
+            return call_next(request)
+
+```
+
+your `main.py`
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager
+from middleware import AccessMiddleware, MetricsMiddleware, SecureRoutersMiddleware
+
+app = Flask(__name__)
+
+my_secured_routers = ["/check_secured"]
+
+app.wsgi_app = MiddlewareManager(app)
+
+app.wsgi_app.add_middleware(AccessMiddleware)
+app.wsgi_app.add_middleware(MetricsMiddleware)
+app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=my_secured_routers)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+@app.get("/check_secured")
+def health():
+    return {"message":"Security bypassed"}
+
+if __name__ == "__main__":
+    app.run()
+```
```

### Comparing `flask-http-middleware-0.2.1/README.md` & `flask-http-middleware-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.2.1/flask_http_middleware/base.py` & `flask-http-middleware-0.2.2/flask_http_middleware/base.py`

 * *Files identical despite different names*

### Comparing `flask-http-middleware-0.2.1/flask_http_middleware/manager.py` & `flask-http-middleware-0.2.2/flask_http_middleware/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,16 +39,38 @@
 
     def process_request_and_handle_exception(self, error) -> Response:
         rv = self.app.handle_user_exception(error)
         return self.app.make_response(rv)
 
     def __call__(self, environ, start_response):
         # version 2.2
-        if flask_version.startswith("2.2"):
+        if flask_version.startswith("2.3"):
+            ctx = self.app.request_context(environ)
+            error: BaseException | None = None
+            try:
+                try:
+                    ctx.push()
+                    response = self.app.full_dispatch_request()
+                except Exception as e:
+                    error = e
+                    response = self.app.handle_exception(e)
+                except:  # noqa: B001
+                    error = sys.exc_info()[1]
+                    raise
+                return response(environ, start_response)
+            finally:
+                if "werkzeug.debug.preserve_context" in environ:
+                    from flask.globals import _cv_app, _cv_request
+                    environ["werkzeug.debug.preserve_context"](_cv_app.get())
+                    environ["werkzeug.debug.preserve_context"](_cv_request.get())
+                if error is not None and self.app.should_ignore_error(error):
+                    error = None
+                ctx.pop(error)
 
+        elif flask_version.startswith("2.2"):
             ctx = self.app.request_context(environ)
             error: t.Optional[BaseException] = None
             try:
                 try:
                     ctx.push()
                     if not self.app._got_first_request:
                         with self.app._before_request_lock:
```

### Comparing `flask-http-middleware-0.2.1/flask_http_middleware.egg-info/PKG-INFO` & `flask-http-middleware-0.2.2/flask_http_middleware.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,272 +1,276 @@
 Metadata-Version: 2.1
 Name: flask-http-middleware
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module to create middleware with direct access to `request` and `response`
 Home-page: https://github.com/Danangjoyoo/flask-http-middleware
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
-License: UNKNOWN
-Description: # Flask HTTP Middleware
-        [![Downloads](https://static.pepy.tech/personalized-badge/flask-http-middleware?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/flask-http-middleware)
-        
-        
-        ## Installation
-        ```
-        pip install flask-http-middleware
-        ```
-        
-        ## Description
-        A module to create flask middleware with direct access to `request` and `response`.
-        
-        This module implement the starlette's (FastAPI) BaseHTTPMiddleware style to Flask.
-        
-        ## Changelogs
-        - v0.0
-            - First Upload
-        - v0.1
-            - Allow middlewares stacking
-        - v0.2
-            - Adjusting wsgi middleware update for `flask>=2.2.x`
-        
-        ## How to use ?
-        
-        ### Example: adding a response header
-        ```
-        import time
-        from flask import Flask
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class MetricsMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                t0 = time.time()
-                response = call_next(request)
-                response_time = time.time()-t0
-                response.headers.add("response_time", response_time)
-                return response
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(MetricsMiddleware)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        - Note: you can put your `MetricsMiddleware` class in different file
-        
-        Above example is equals with `app.before_request` and `app.after_request` decorated function.
-        
-        ```
-        @app.before_request
-        def start_metrics():
-            g.t0 = time.time()
-        
-        @app.after_request
-        def stop_metrics(response):
-            response_time = time.time()-g.t0
-            response.headers.add("response_time", response_time)
-            return response
-        ```
-        
-        ---
-        
-        ### Example: Authentication
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class AccessMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                if request.headers.get("token") == "secret":
-                    return call_next(request)
-                else:
-                    return jsonify({"message":"invalid token"})
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(AccessMiddleware)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        
-        ---
-        
-        ### Example: add some routers security
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class SecureRoutersMiddleware(BaseHTTPMiddleware):
-            def __init__(self, secured_routers = []):
-                super().__init__()
-                self.secured_routers = secured_routers
-        
-            def dispatch(self, request, call_next):
-                if request.path in self.secured_routers:
-                    if request.headers.get("token") == "secret":
-                        return call_next(request)
-                    else:
-                        return jsonify({"message":"invalid token"})
-                else:
-                    return call_next(request)
-        
-        secured_routers = ["/check_secured"]
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=secured_routers)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        @app.get("/check_secured")
-        def health():
-            return {"message":"Security bypassed"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        
-        ---
-        
-        ### Example: add error handling
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
-        
-        app = Flask(__name__)
-        
-        class AccessMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                if request.headers.get("token") == "secret":
-                    return call_next(request)
-                else:
-                    raise Exception("Authentication Failed")
-        
-            def error_handler(self, error):
-                return jsonify({"error": str(error)})
-        
-        app.wsgi_app = MiddlewareManager(app)
-        app.wsgi_app.add_middleware(AccessMiddleware)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
-        
-        ### Example: Stacking Middleware
-        You can also stack your middleware
-        
-        `middleware.py`
-        ```
-        import time
-        from flask import jsonify
-        from flask_http_middleware import BaseHTTPMiddleware
-        
-        class AccessMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                if request.headers.get("token") == "secret":
-                    return call_next(request)
-                else:
-                    raise Exception("Authentication Failed")
-        
-            def error_handler(self, error):
-                return jsonify({"error": str(error)})
-        
-        
-        class MetricsMiddleware(BaseHTTPMiddleware):
-            def __init__(self):
-                super().__init__()
-        
-            def dispatch(self, request, call_next):
-                t0 = time.time()
-                response = call_next(request)
-                response_time = time.time()-t0
-                response.headers.add("response_time", response_time)
-                return response
-        
-        
-        class SecureRoutersMiddleware(BaseHTTPMiddleware):
-            def __init__(self, secured_routers = []):
-                super().__init__()
-                self.secured_routers = secured_routers
-        
-            def dispatch(self, request, call_next):
-                if request.path in self.secured_routers:
-                    if request.headers.get("token") == "secret":
-                        return call_next(request)
-                    else:
-                        return jsonify({"message":"invalid token"})
-                else:
-                    return call_next(request)
-        
-        ```
-        
-        your `main.py`
-        ```
-        import time
-        from flask import Flask, jsonify
-        from flask_http_middleware import MiddlewareManager
-        from middleware import AccessMiddleware, MetricsMiddleware, SecureRoutersMiddleware
-        
-        app = Flask(__name__)
-        
-        my_secured_routers = ["/check_secured"]
-        
-        app.wsgi_app = MiddlewareManager(app)
-        
-        app.wsgi_app.add_middleware(AccessMiddleware)
-        app.wsgi_app.add_middleware(MetricsMiddleware)
-        app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=my_secured_routers)
-        
-        @app.get("/health")
-        def health():
-            return {"message":"I'm healthy"}
-        
-        @app.get("/check_secured")
-        def health():
-            return {"message":"Security bypassed"}
-        
-        if __name__ == "__main__":
-            app.run()
-        ```
 Keywords: flask,middleware,http,request,response
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Flask HTTP Middleware
+[![Downloads](https://static.pepy.tech/personalized-badge/flask-http-middleware?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/flask-http-middleware)
+
+
+## Installation
+```
+pip install flask-http-middleware
+```
+
+## Description
+A module to create flask middleware with direct access to `request` and `response`.
+
+This module implement the starlette's (FastAPI) BaseHTTPMiddleware style to Flask.
+
+## Changelogs
+- v0.0
+    - First Upload
+- v0.1
+    - Allow middlewares stacking
+- v0.2
+    - Adjusting wsgi middleware update for `flask>=2.2.x`
+
+## How to use ?
+
+### Example: adding a response header
+```
+import time
+from flask import Flask
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class MetricsMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        t0 = time.time()
+        response = call_next(request)
+        response_time = time.time()-t0
+        response.headers.add("response_time", response_time)
+        return response
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(MetricsMiddleware)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+if __name__ == "__main__":
+    app.run()
+```
+- Note: you can put your `MetricsMiddleware` class in different file
+
+Above example is equals with `app.before_request` and `app.after_request` decorated function.
+
+```
+@app.before_request
+def start_metrics():
+    g.t0 = time.time()
+
+@app.after_request
+def stop_metrics(response):
+    response_time = time.time()-g.t0
+    response.headers.add("response_time", response_time)
+    return response
+```
+
+---
+
+### Example: Authentication
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class AccessMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        if request.headers.get("token") == "secret":
+            return call_next(request)
+        else:
+            return jsonify({"message":"invalid token"})
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(AccessMiddleware)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+if __name__ == "__main__":
+    app.run()
+```
+
+---
+
+### Example: add some routers security
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class SecureRoutersMiddleware(BaseHTTPMiddleware):
+    def __init__(self, secured_routers = []):
+        super().__init__()
+        self.secured_routers = secured_routers
+
+    def dispatch(self, request, call_next):
+        if request.path in self.secured_routers:
+            if request.headers.get("token") == "secret":
+                return call_next(request)
+            else:
+                return jsonify({"message":"invalid token"})
+        else:
+            return call_next(request)
+
+secured_routers = ["/check_secured"]
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=secured_routers)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+@app.get("/check_secured")
+def health():
+    return {"message":"Security bypassed"}
+
+if __name__ == "__main__":
+    app.run()
+```
+
+---
+
+### Example: add error handling
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager, BaseHTTPMiddleware
+
+app = Flask(__name__)
+
+class AccessMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        if request.headers.get("token") == "secret":
+            return call_next(request)
+        else:
+            raise Exception("Authentication Failed")
+
+    def error_handler(self, error):
+        return jsonify({"error": str(error)})
+
+app.wsgi_app = MiddlewareManager(app)
+app.wsgi_app.add_middleware(AccessMiddleware)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+if __name__ == "__main__":
+    app.run()
+```
+
+### Example: Stacking Middleware
+You can also stack your middleware
+
+`middleware.py`
+```
+import time
+from flask import jsonify
+from flask_http_middleware import BaseHTTPMiddleware
+
+class AccessMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        if request.headers.get("token") == "secret":
+            return call_next(request)
+        else:
+            raise Exception("Authentication Failed")
+
+    def error_handler(self, error):
+        return jsonify({"error": str(error)})
+
+
+class MetricsMiddleware(BaseHTTPMiddleware):
+    def __init__(self):
+        super().__init__()
+
+    def dispatch(self, request, call_next):
+        t0 = time.time()
+        response = call_next(request)
+        response_time = time.time()-t0
+        response.headers.add("response_time", response_time)
+        return response
+
+
+class SecureRoutersMiddleware(BaseHTTPMiddleware):
+    def __init__(self, secured_routers = []):
+        super().__init__()
+        self.secured_routers = secured_routers
+
+    def dispatch(self, request, call_next):
+        if request.path in self.secured_routers:
+            if request.headers.get("token") == "secret":
+                return call_next(request)
+            else:
+                return jsonify({"message":"invalid token"})
+        else:
+            return call_next(request)
+
+```
+
+your `main.py`
+```
+import time
+from flask import Flask, jsonify
+from flask_http_middleware import MiddlewareManager
+from middleware import AccessMiddleware, MetricsMiddleware, SecureRoutersMiddleware
+
+app = Flask(__name__)
+
+my_secured_routers = ["/check_secured"]
+
+app.wsgi_app = MiddlewareManager(app)
+
+app.wsgi_app.add_middleware(AccessMiddleware)
+app.wsgi_app.add_middleware(MetricsMiddleware)
+app.wsgi_app.add_middleware(SecureRoutersMiddleware, secured_routers=my_secured_routers)
+
+@app.get("/health")
+def health():
+    return {"message":"I'm healthy"}
+
+@app.get("/check_secured")
+def health():
+    return {"message":"Security bypassed"}
+
+if __name__ == "__main__":
+    app.run()
+```
```

### Comparing `flask-http-middleware-0.2.1/setup.py` & `flask-http-middleware-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 DESCRIPTION = "A module to create middleware with direct access to `request` and `response`"
 
 # Setting up
 setup(
     name="flask-http-middleware",
     version=VERSION,
     author="danangjoyoo (Agus Danangjoyo)",
@@ -22,14 +22,18 @@
     packages=find_packages(),
     install_requires=["flask","werkzeug"],
     keywords=['flask', 'middleware', 'http', 'request', "response"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Environment :: Web Environment",
         "Operating System :: OS Independent",
         "Typing :: Typed"
     ],
     url="https://github.com/Danangjoyoo/flask-http-middleware"
 )
```

