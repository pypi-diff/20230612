# Comparing `tmp/django-nextjs-2.2.3.tar.gz` & `tmp/django-nextjs-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nextjs-2.2.3.tar", last modified: Sun May 28 15:16:01 2023, max compression
+gzip compressed data, was "django-nextjs-2.3.0.tar", last modified: Mon Jun 12 18:50:33 2023, max compression
```

## Comparing `django-nextjs-2.2.3.tar` & `django-nextjs-2.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/
--rw-r--r--   0 danial    (1000) danial    (1000)     1076 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/LICENSE
--rw-r--r--   0 danial    (1000) danial    (1000)       62 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/MANIFEST.in
--rw-r--r--   0 danial    (1000) danial    (1000)     8973 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/PKG-INFO
--rw-r--r--   0 danial    (1000) danial    (1000)     7914 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/README.md
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.047196 django-nextjs-2.2.3/django_nextjs/
--rw-r--r--   0 danial    (1000) danial    (1000)       22 2023-05-28 15:15:39.000000 django-nextjs-2.2.3/django_nextjs/__init__.py
--rw-r--r--   0 danial    (1000) danial    (1000)      191 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/app_settings.py
--rw-r--r--   0 danial    (1000) danial    (1000)      135 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/apps.py
--rw-r--r--   0 danial    (1000) danial    (1000)       54 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/exceptions.py
--rw-r--r--   0 danial    (1000) danial    (1000)     3797 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/proxy.py
--rw-r--r--   0 danial    (1000) danial    (1000)     6347 2023-05-28 15:10:19.000000 django-nextjs-2.2.3/django_nextjs/render.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.047196 django-nextjs-2.2.3/django_nextjs/templates/
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/django_nextjs/templates/django_nextjs/
--rw-r--r--   0 danial    (1000) danial    (1000)      246 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/templates/django_nextjs/document_base.html
--rw-r--r--   0 danial    (1000) danial    (1000)      287 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/django_nextjs/urls.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/django_nextjs.egg-info/
--rw-r--r--   0 danial    (1000) danial    (1000)     8973 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/PKG-INFO
--rw-r--r--   0 danial    (1000) danial    (1000)      490 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/SOURCES.txt
--rw-r--r--   0 danial    (1000) danial    (1000)        1 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/dependency_links.txt
--rw-r--r--   0 danial    (1000) danial    (1000)      108 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/requires.txt
--rw-r--r--   0 danial    (1000) danial    (1000)       14 2023-05-28 15:16:01.000000 django-nextjs-2.2.3/django_nextjs.egg-info/top_level.txt
--rw-r--r--   0 danial    (1000) danial    (1000)      281 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/pyproject.toml
--rw-r--r--   0 danial    (1000) danial    (1000)       38 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/setup.cfg
--rw-r--r--   0 danial    (1000) danial    (1000)     1802 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/setup.py
-drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-05-28 15:16:01.050532 django-nextjs-2.2.3/tests/
--rw-r--r--   0 danial    (1000) danial    (1000)     1119 2022-12-17 14:25:24.000000 django-nextjs-2.2.3/tests/test_render.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/
+-rw-r--r--   0 danial    (1000) danial    (1000)     1076 2022-03-05 14:42:22.000000 django-nextjs-2.3.0/LICENSE
+-rw-r--r--   0 danial    (1000) danial    (1000)       62 2022-03-05 14:42:22.000000 django-nextjs-2.3.0/MANIFEST.in
+-rw-r--r--   0 danial    (1000) danial    (1000)     9967 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/PKG-INFO
+-rw-r--r--   0 danial    (1000) danial    (1000)     8919 2023-06-12 18:38:49.000000 django-nextjs-2.3.0/README.md
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/django_nextjs/
+-rw-r--r--   0 danial    (1000) danial    (1000)       22 2023-06-12 18:41:27.000000 django-nextjs-2.3.0/django_nextjs/__init__.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      191 2022-03-05 14:42:22.000000 django-nextjs-2.3.0/django_nextjs/app_settings.py
+-rw-r--r--   0 danial    (1000) danial    (1000)      135 2022-09-16 11:04:07.000000 django-nextjs-2.3.0/django_nextjs/apps.py
+-rw-r--r--   0 danial    (1000) danial    (1000)       54 2022-03-05 14:42:22.000000 django-nextjs-2.3.0/django_nextjs/exceptions.py
+-rw-r--r--   0 danial    (1000) danial    (1000)     3893 2023-06-12 18:38:49.000000 django-nextjs-2.3.0/django_nextjs/proxy.py
+-rw-r--r--   0 danial    (1000) danial    (1000)     6387 2023-06-12 18:38:49.000000 django-nextjs-2.3.0/django_nextjs/render.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/django_nextjs/templates/
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/django_nextjs/templates/django_nextjs/
+-rw-r--r--   0 danial    (1000) danial    (1000)      246 2022-03-05 14:42:22.000000 django-nextjs-2.3.0/django_nextjs/templates/django_nextjs/document_base.html
+-rw-r--r--   0 danial    (1000) danial    (1000)      287 2022-03-05 14:42:22.000000 django-nextjs-2.3.0/django_nextjs/urls.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/django_nextjs.egg-info/
+-rw-r--r--   0 danial    (1000) danial    (1000)     9967 2023-06-12 18:50:33.000000 django-nextjs-2.3.0/django_nextjs.egg-info/PKG-INFO
+-rw-r--r--   0 danial    (1000) danial    (1000)      490 2023-06-12 18:50:33.000000 django-nextjs-2.3.0/django_nextjs.egg-info/SOURCES.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)        1 2023-06-12 18:50:33.000000 django-nextjs-2.3.0/django_nextjs.egg-info/dependency_links.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)      120 2023-06-12 18:50:33.000000 django-nextjs-2.3.0/django_nextjs.egg-info/requires.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)       14 2023-06-12 18:50:33.000000 django-nextjs-2.3.0/django_nextjs.egg-info/top_level.txt
+-rw-r--r--   0 danial    (1000) danial    (1000)      281 2022-09-16 11:04:07.000000 django-nextjs-2.3.0/pyproject.toml
+-rw-r--r--   0 danial    (1000) danial    (1000)       38 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/setup.cfg
+-rw-r--r--   0 danial    (1000) danial    (1000)     1814 2023-06-12 18:38:49.000000 django-nextjs-2.3.0/setup.py
+drwxr-xr-x   0 danial    (1000) danial    (1000)        0 2023-06-12 18:50:33.082221 django-nextjs-2.3.0/tests/
+-rw-r--r--   0 danial    (1000) danial    (1000)     3386 2023-06-12 18:38:49.000000 django-nextjs-2.3.0/tests/test_render.py
```

### Comparing `django-nextjs-2.2.3/LICENSE` & `django-nextjs-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-nextjs-2.2.3/PKG-INFO` & `django-nextjs-2.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: django-nextjs
-Version: 2.2.3
-Summary: Next.js + Django integration
-Home-page: https://github.com/QueraTeam/django-nextjs
-Download-URL: https://github.com/QueraTeam/django-nextjs
-Author: Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>
-Keywords: django,next,nextjs,django-nextjs
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Django Next.js
 
 [![](https://img.shields.io/pypi/v/django-nextjs.svg)](https://pypi.python.org/pypi/django-nextjs/)
 [![](https://github.com/QueraTeam/django-nextjs/workflows/tests/badge.svg)](https://github.com/QueraTeam/django-nextjs/actions)
 [![](https://img.shields.io/github/license/QueraTeam/django-nextjs.svg)](https://github.com/QueraTeam/django-nextjs/blob/master/LICENSE)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -64,76 +38,96 @@
 
   ```shell
   pip install django-nextjs
   ```
 
 - Add `django_nextjs.apps.DjangoNextJSConfig` to `INSTALLED_APPS`.
 
-- **In Development Environment:**
+- Set up Next.js URLs depending on your environment.
 
-  - If you're using django channels (after Nextjs v12 you need this to be able to use hot-reload), add `NextJSProxyHttpConsumer` and `NextJSProxyWebsocketConsumer` to `asgi.py`:
+### Setup Next.js URLs (Development Environment)
 
-    ```python
-    import os
+If you're serving your site under ASGI during development,
+use [Django Channels](https://channels.readthedocs.io/en/stable/) and
+add `NextJSProxyHttpConsumer`, `NextJSProxyWebsocketConsumer` to `asgi.py` like the following example.
 
-    from django.core.asgi import get_asgi_application
-    from django.urls import re_path, path
+**Note:** We recommend using ASGI and Django Channels,
+because it is required for [fast refresh](https://nextjs.org/docs/architecture/fast-refresh) (hot module replacement) to work properly in Nextjs 12+.
 
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "myproject.settings")
-    django_asgi_app = get_asgi_application()
+```python
+import os
 
-    from channels.auth import AuthMiddlewareStack
-    from channels.routing import ProtocolTypeRouter, URLRouter
-    from django_nextjs.proxy import NextJSProxyHttpConsumer, NextJSProxyWebsocketConsumer
+from django.core.asgi import get_asgi_application
+from django.urls import re_path, path
 
-    from django.conf import settings
+os.environ.setdefault("DJANGO_SETTINGS_MODULE", "myproject.settings")
+django_asgi_app = get_asgi_application()
 
-    # put your custom routes here if you need
-    http_routes = [re_path(r"", django_asgi_app)]
-    websocket_routers = []
+from channels.auth import AuthMiddlewareStack
+from channels.routing import ProtocolTypeRouter, URLRouter
+from django_nextjs.proxy import NextJSProxyHttpConsumer, NextJSProxyWebsocketConsumer
 
-    if settings.DEBUG:
-        http_routes.insert(0, re_path(r"^(?:_next|__next|next).*", NextJSProxyHttpConsumer.as_asgi()))
-        websocket_routers.insert(0, path("_next/webpack-hmr", NextJSProxyWebsocketConsumer.as_asgi()))
+from django.conf import settings
 
+# put your custom routes here if you need
+http_routes = [re_path(r"", django_asgi_app)]
+websocket_routers = []
 
-    application = ProtocolTypeRouter(
-        {
-            # Django's ASGI application to handle traditional HTTP and websocket requests.
-            "http": URLRouter(http_routes),
-            "websocket": AuthMiddlewareStack(URLRouter(websocket_routers)),
-            # ...
-        }
-    )
-    ```
+if settings.DEBUG:
+    http_routes.insert(0, re_path(r"^(?:_next|__next|next).*", NextJSProxyHttpConsumer.as_asgi()))
+    websocket_routers.insert(0, path("_next/webpack-hmr", NextJSProxyWebsocketConsumer.as_asgi()))
 
-  - Otherwise, add the following to the beginning of `urls.py`:
 
-    ```python
-    path("", include("django_nextjs.urls"))
-    ```
+application = ProtocolTypeRouter(
+    {
+        # Django's ASGI application to handle traditional HTTP and websocket requests.
+        "http": URLRouter(http_routes),
+        "websocket": AuthMiddlewareStack(URLRouter(websocket_routers)),
+        # ...
+    }
+)
+```
 
-- **In Production:**
+Otherwise (if serving under WSGI during development), add the following to the beginning of `urls.py`:
 
-  - Use a reverse proxy like nginx:
+```python
+path("", include("django_nextjs.urls"))
+```
 
-    | URL                 | Action                                     |
-    | ------------------- | ------------------------------------------ |
-    | `/_next/static/...` | Serve `NEXTJS_PATH/.next/static` directory |
-    | `/_next/...`        | Proxy to `http://localhost:3000`           |
-    | `/next/...`         | Serve `NEXTJS_PATH/public/next` directory  |
+**Warning:** If you are serving under ASGI, do NOT add this
+to your `urls.py`. It may cause deadlocks.
 
-    Pass `x-real-ip` header when proxying `/_next/`:
+### Setup Next.js URLs (Production Environment)
 
-    ```conf
-    location /_next/ {
-        proxy_set_header  x-real-ip $remote_addr;
-        proxy_pass  http://127.0.0.1:3000;
-    }
-    ```
+In production, use a reverse proxy like Nginx or Caddy:
+
+| URL                 | Action                                     |
+| ------------------- | ------------------------------------------ |
+| `/_next/static/...` | Serve `NEXTJS_PATH/.next/static` directory |
+| `/_next/...`        | Proxy to `http://localhost:3000`           |
+| `/next/...`         | Serve `NEXTJS_PATH/public/next` directory  |
+
+Pass `x-real-ip` header when proxying `/_next/`. Example config for Nginx:
+
+```conf
+location /_next/static/ {
+    alias NEXTJS_PATH/.next/static/;
+    expires max;
+    add_header Cache-Control "public";
+}
+location /_next/ {
+    proxy_set_header  x-real-ip $remote_addr;
+    proxy_pass  http://127.0.0.1:3000;
+}
+location /next/ {
+    alias NEXTJS_PATH/public/next/;
+    expires max;
+    add_header Cache-Control "public";
+}
+```
 
 ## Usage
 
 Start Next.js server:
 
 ```shell
 # Development:
@@ -141,99 +135,102 @@
 
 # Production:
 $ npm run build
 $ npm run start
 ```
 
 Develop your pages in Next.js.
-Write a django URL and view for each page like this:
+Write a django URL and an async view for each page like this:
 
 ```python
-# If you're using django channels
 from django.http import HttpResponse
-from django_nextjs.render import render_nextjs_page_async
+from django_nextjs.render import render_nextjs_page
 
 async def jobs(request):
-    return await render_nextjs_page_async(request)
+    return await render_nextjs_page(request)
 ```
 
-```python
-# If you're not using django channels
-from django.http import HttpResponse
-from django_nextjs.render import render_nextjs_page_sync
-
-def jobs(request):
-    return render_nextjs_page_sync(request)
-```
+## Customizing the HTML Response
 
-## Customizing Document
+You can modify the HTML code that Next.js returns in your Django code.
 
-If you want to customize the HTML document (e.g. add header or footer), read this section.
+Avoiding duplicate code for the navbar and footer is a common use case
+for this if you are using both Next.js and Django templates.
+Without it, you would have to write and maintain two separate versions
+of your navbar and footer (a Django template version and a Next.js version).
+However, you can simply create a Django template for your navbar and insert its code
+at the beginning of `<body>` tag returned from Next.js.
 
-You need to [customize Next's document]:
+To enable this feature, you need to customize the document and root layout
+in Next.js and make the following adjustments:
 
 - Add `id="__django_nextjs_body"` as the first attribute of `<body>` element.
 - Add `<div id="__django_nextjs_body_begin" />` as the first element inside `<body>`.
 - Add `<div id="__django_nextjs_body_end" />` as the last element inside `<body>`.
 
-```jsx
-import Document, { Html, Head, Main, NextScript } from "next/document";
+NOTE: Currently HTML customization is not working with [app router](https://nextjs.org/docs/app) (Next.js 13+).
 
-// https://nextjs.org/docs/advanced-features/custom-document
-class MyDocument extends Document {
-  render() {
-    return (
-      <Html>
-        <Head />
-        <body id="__django_nextjs_body" dir="rtl">
-          <div id="__django_nextjs_body_begin" />
-          <Main />
-          <NextScript />
-          <div id="__django_nextjs_body_end" />
-        </body>
-      </Html>
-    );
-  }
-}
+Read
+[this doc](https://nextjs.org/docs/pages/building-your-application/routing/custom-document)
+and customize your Next.js document:
 
-export default MyDocument;
+```jsx
+// pages/_document.jsx (or .tsx)
+...
+<body id="__django_nextjs_body">
+  <div id="__django_nextjs_body_begin" />
+  <Main />
+  <NextScript />
+  <div id="__django_nextjs_body_end" />
+</body>
+...
 ```
 
+<!-- If you are using Next.js 13+, you also need to
+[customize the root layout](https://nextjs.org/docs/app/api-reference/file-conventions/layout)
+in `app` directory:
+
+```jsx
+// app/layout.jsx (or .tsx)
+...
+<body id="__django_nextjs_body" className={inter.className}>
+  <div id="__django_nextjs_body_begin" />
+  {children}
+  <div id="__django_nextjs_body_end" />
+</body>
+...
+``` -->
+
 Write a django template that extends `django_nextjs/document_base.html`:
 
 ```django
 {% extends "django_nextjs/document_base.html" %}
 
 
 {% block head %}
-  ... the content you want to add to the beginning of <head> tag ...
+  <!-- ... the content you want to place at the beginning of "head" tag ... -->
   {{ block.super }}
-  ... the content you want to add to the end of <head> tag ...
+  <!-- ... the content you want to place at the end of "head" tag ... -->
 {% endblock %}
 
 
 {% block body %}
-  ... the content you want to add to the beginning of <body> tag ...
+  ... the content you want to place at the beginning of "body" tag ...
+  ... e.g. include the navbar template ...
   {{ block.super }}
-  ... the content you want to add to the end of <body> tag ...
+  ... the content you want to place at the end of "body" tag ...
+  ... e.g. include the footer template ...
 {% endblock %}
 ```
 
-Pass the template name to `render_nextjs_page_async` or `render_nextjs_page_sync`:
+Pass the template name to `render_nextjs_page`:
 
 ```python
-# If you're using django channels
 async def jobs(request):
-    return await render_nextjs_page_async(request, "path/to/template.html")
-```
-
-```python
-# If you're not using django channels
-def jobs(request):
-    return render_nextjs_page_sync(request, "path/to/template.html")
+    return await render_nextjs_page(request, "path/to/template.html")
 ```
 
 ## Notes
 
 - If you want to add a file to `public` directory of Next.js,
   that file should be in `public/next` subdirectory to work correctly.
 - If you're using django channels, make sure all your middlewares are
@@ -263,12 +260,11 @@
 
 ## References
 
 - https://github.com/yourlabs/djnext
 - [comment on StackOverflow]
 
 [comment on stackoverflow]: https://stackoverflow.com/questions/54252943/is-there-a-way-to-integrate-django-with-next-js#comment110078700_54252943
-[customize next's document]: https://nextjs.org/docs/advanced-features/custom-document
 
 ## License
 
 MIT
```

### Comparing `django-nextjs-2.2.3/django_nextjs/proxy.py` & `django-nextjs-2.3.0/django_nextjs/proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import re
+import urllib.request
+from http.client import HTTPResponse
 
 import aiohttp
-import requests
 import websockets
 from channels.generic.http import AsyncHttpConsumer
 from channels.generic.websocket import AsyncWebsocketConsumer
 from django import http
 from django.conf import settings
 from django.views import View
 
@@ -85,19 +86,22 @@
         if not settings.DEBUG:
             raise NextJSImproperlyConfigured("This proxy is for development only.")
         return super().dispatch(request, *args, **kwargs)
 
     def get(self, request):
         url = NEXTJS_SERVER_URL + request.path + "?" + request.GET.urlencode()
 
-        if request.headers.get("Accept", None) == "text/event-stream":
-            response = requests.get(url, stream=True, cookies=request.COOKIES)
-            ret = http.StreamingHttpResponse(response.iter_content())
-        else:
-            response = requests.get(url, cookies=request.COOKIES)
-            ret = http.HttpResponse(
-                content=bytes(response.content),
-            )
-
-        if "Content-Type" in response.headers:
-            ret["Content-Type"] = response.headers["Content-Type"]
-        return ret
+        urllib_response = urllib.request.urlopen(
+            urllib.request.Request(url, headers={"Cookie": request.headers.get("Cookie")})
+        )
+
+        return http.StreamingHttpResponse(
+            self._iter_content(urllib_response), headers={"Content-Type": urllib_response.headers.get("Content-Type")}
+        )
+
+    def _iter_content(self, urllib_response: HTTPResponse):
+        while True:
+            chunk = urllib_response.read(urllib_response.length or 1)
+            if not chunk:
+                urllib_response.close()
+                break
+            yield chunk
```

### Comparing `django-nextjs-2.2.3/django_nextjs/render.py` & `django-nextjs-2.3.0/django_nextjs/render.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,178 @@
-import typing
+import warnings
+from typing import Dict, Tuple, Union
+from urllib.parse import quote
 
 import aiohttp
-import requests
-from asgiref.sync import sync_to_async
+from asgiref.sync import async_to_sync, sync_to_async
 from django.conf import settings
 from django.http import HttpRequest, HttpResponse
 from django.middleware.csrf import get_token as get_csrf_token
 from django.template.loader import render_to_string
+from multidict import MultiMapping
 
 from .app_settings import NEXTJS_SERVER_URL
 
 
-def _get_context(html: str, context: typing.Union[dict, None] = None) -> typing.Union[dict, None]:
+def _get_render_context(html: str, extra_context: Union[Dict, None] = None):
     a = html.find("<head>")
     b = html.find('</head><body id="__django_nextjs_body"', a)
     c = html.find('<div id="__django_nextjs_body_begin"', b)
     d = html.find('<div id="__django_nextjs_body_end"', c)
-    if a == -1 or b == -1 or c == -1 or d == -1:
+
+    if any(i == -1 for i in (a, b, c, d)):
         return None
 
-    context = context or {}
-    context["django_nextjs__"] = {
-        "section1": html[: a + len("<head>")],
-        "section2": html[a + len("<head>") : b],
-        "section3": html[b:c],
-        "section4": html[c:d],
-        "section5": html[d:],
+    return {
+        **(extra_context or {}),
+        "django_nextjs__": {
+            "section1": html[: a + len("<head>")],
+            "section2": html[a + len("<head>") : b],
+            "section3": html[b:c],
+            "section4": html[c:d],
+            "section5": html[d:],
+        },
     }
 
-    return context
-
 
-def _get_cookies(request: HttpRequest):
+def _get_nextjs_request_cookies(request: HttpRequest):
     """
     Ensure we always send a CSRF cookie to Next.js server (if there is none in `request` object, generate one)
     Reason: We are going to issue GraphQL POST requests to fetch data in NextJS getServerSideProps.
             If this is the first request of user, there is no CSRF cookie and request fails,
             since GraphQL uses POST even for data fetching.
     Isn't this a vulnerability?
     No, as long as getServerSideProps functions are side effect free
     (i.e. dont use HTTP unsafe methods or GraphQL mutations).
     https://docs.djangoproject.com/en/3.2/ref/csrf/#is-posting-an-arbitrary-csrf-token-pair-cookie-and-post-data-a-vulnerability
     """
     return {**request.COOKIES, settings.CSRF_COOKIE_NAME: get_csrf_token(request)}
 
 
-def _get_headers(request: HttpRequest, headers=None):
-    """
-    Headers that we will send in request to Next.js
-    """
+def _get_nextjs_request_headers(request: HttpRequest, headers: Union[Dict, None] = None):
     return {
         "x-real-ip": request.headers.get("X-Real-Ip", "") or request.META.get("REMOTE_ADDR", ""),
         "user-agent": request.headers.get("User-Agent", ""),
         **({} if headers is None else headers),
     }
 
 
-def _get_nextjs_response_headers(headers):
-    useful_header_keys = [
-        "Location",
-    ]
+def _get_nextjs_response_headers(headers: MultiMapping[str]) -> Dict:
+    useful_header_keys = ("Location",)
     return {key: headers[key] for key in useful_header_keys if key in headers}
 
 
-def _render_nextjs_page_to_string_sync(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
-) -> typing.Tuple[str, int, typing.Dict[str, str]]:
-    page = requests.utils.quote(request.path_info.lstrip("/"))
-    params = {k: request.GET.getlist(k) for k in request.GET.keys()}
-
-    # Get HTML from Next.js server
-    response = requests.get(
-        f"{NEXTJS_SERVER_URL}/{page}",
-        params=params,
-        cookies=_get_cookies(request),
-        headers=_get_headers(request, headers),
-        allow_redirects=allow_redirects,
-    )
-    html = response.text
-    response_headers = _get_nextjs_response_headers(response.headers)
-
-    # Apply template_name if provided
-    if template_name:
-        final_context = _get_context(html, context)
-        if final_context is not None:
-            html = render_to_string(template_name, context=final_context, request=request, using=using)
-
-    return html, response.status_code, response_headers
-
-
-def render_nextjs_page_to_string_sync(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
-) -> str:
-    html, _, _ = _render_nextjs_page_to_string_sync(
-        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
-    )
-    return html
-
-
-def render_nextjs_page_sync(
+async def _render_nextjs_page_to_string(
     request: HttpRequest,
     template_name: str = "",
-    context=None,
-    content_type=None,
-    override_status=None,
-    using=None,
-    allow_redirects=False,
-    headers=None,
-) -> HttpResponse:
-    content, status, response_headers = _render_nextjs_page_to_string_sync(
-        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
-    )
-    final_status = status if override_status is None else override_status
-    return HttpResponse(content, content_type, final_status, headers=response_headers)
-
-
-async def _render_nextjs_page_to_string_async(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
-) -> typing.Tuple[str, int, typing.Dict[str, str]]:
-    page = requests.utils.quote(request.path_info.lstrip("/"))
+    context: Union[Dict, None] = None,
+    using: Union[str, None] = None,
+    allow_redirects: bool = False,
+    headers: Union[Dict, None] = None,
+) -> Tuple[str, int, Dict[str, str]]:
+    page_path = quote(request.path_info.lstrip("/"))
     params = [(k, v) for k in request.GET.keys() for v in request.GET.getlist(k)]
 
     # Get HTML from Next.js server
     async with aiohttp.ClientSession(
-        cookies=_get_cookies(request),
-        headers=_get_headers(request, headers),
+        cookies=_get_nextjs_request_cookies(request),
+        headers=_get_nextjs_request_headers(request, headers),
     ) as session:
         async with session.get(
-            f"{NEXTJS_SERVER_URL}/{page}", params=params, allow_redirects=allow_redirects
+            f"{NEXTJS_SERVER_URL}/{page_path}", params=params, allow_redirects=allow_redirects
         ) as response:
             html = await response.text()
             response_headers = _get_nextjs_response_headers(response.headers)
 
-    # Apply template_name if provided
+    # Apply template rendering (HTML customization) if template_name is provided
     if template_name:
-        final_context = _get_context(html, context)
-        if final_context is not None:
+        render_context = _get_render_context(html, context)
+        if render_context is not None:
             html = await sync_to_async(render_to_string)(
-                template_name, context=final_context, request=request, using=using
+                template_name, context=render_context, request=request, using=using
             )
     return html, response.status, response_headers
 
 
-async def render_nextjs_page_to_string_async(
-    request: HttpRequest, template_name: str = "", context=None, using=None, allow_redirects=False, headers=None
-) -> str:
-    html, _, _ = await _render_nextjs_page_to_string_async(
-        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
+async def render_nextjs_page_to_string(
+    request: HttpRequest,
+    template_name: str = "",
+    context: Union[Dict, None] = None,
+    using: Union[str, None] = None,
+    allow_redirects: bool = False,
+    headers: Union[Dict, None] = None,
+):
+    html, _, _ = await _render_nextjs_page_to_string(
+        request,
+        template_name,
+        context,
+        using=using,
+        allow_redirects=allow_redirects,
+        headers=headers,
     )
     return html
 
 
-async def render_nextjs_page_async(
+async def render_nextjs_page(
     request: HttpRequest,
     template_name: str = "",
-    context=None,
-    content_type=None,
-    override_status=None,
-    using=None,
-    allow_redirects=False,
-    headers=None,
-) -> HttpResponse:
-    content, status, response_headers = await _render_nextjs_page_to_string_async(
-        request, template_name, context, using=using, allow_redirects=allow_redirects, headers=headers
+    context: Union[Dict, None] = None,
+    content_type: Union[str, None] = None,
+    override_status: Union[int, None] = None,
+    using: Union[str, None] = None,
+    allow_redirects: bool = False,
+    headers: Union[Dict, None] = None,
+):
+    content, status, response_headers = await _render_nextjs_page_to_string(
+        request,
+        template_name,
+        context,
+        using=using,
+        allow_redirects=allow_redirects,
+        headers=headers,
     )
     final_status = status if override_status is None else override_status
     return HttpResponse(content, content_type, final_status, headers=response_headers)
+
+
+async def render_nextjs_page_to_string_async(*args, **kwargs):
+    warnings.warn(
+        (
+            "render_nextjs_page_to_string_async is deprecated and will be removed in a future release. "
+            "Use render_nextjs_page_to_string instead."
+        ),
+        DeprecationWarning,
+    )
+    return await render_nextjs_page_to_string(*args, **kwargs)
+
+
+async def render_nextjs_page_async(*args, **kwargs):
+    warnings.warn(
+        (
+            "render_nextjs_page_async is deprecated and will be removed in a future release. "
+            "Use render_nextjs_page instead."
+        ),
+        DeprecationWarning,
+    )
+    return await render_nextjs_page(*args, **kwargs)
+
+
+def render_nextjs_page_to_string_sync(*args, **kwargs):
+    warnings.warn(
+        (
+            "render_nextjs_page_to_string_sync is deprecated and will be removed in a future release. "
+            "Use render_nextjs_page_to_string in an async view, or use async_to_sync(render_nextjs_page_to_string)."
+        ),
+        DeprecationWarning,
+    )
+    return async_to_sync(render_nextjs_page_to_string)(*args, **kwargs)
+
+
+def render_nextjs_page_sync(*args, **kwargs):
+    warnings.warn(
+        (
+            "render_nextjs_page_sync is deprecated and will be removed in a future release. "
+            "Use render_nextjs_page in an async view, or use async_to_sync(render_nextjs_page)."
+        ),
+        DeprecationWarning,
+    )
+    return async_to_sync(render_nextjs_page)(*args, **kwargs)
```

### Comparing `django-nextjs-2.2.3/django_nextjs.egg-info/PKG-INFO` & `django-nextjs-2.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: django-nextjs
-Version: 2.2.3
+Version: 2.3.0
 Summary: Next.js + Django integration
 Home-page: https://github.com/QueraTeam/django-nextjs
 Download-URL: https://github.com/QueraTeam/django-nextjs
 Author: Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>
 Keywords: django,next,nextjs,django-nextjs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -64,76 +64,96 @@
 
   ```shell
   pip install django-nextjs
   ```
 
 - Add `django_nextjs.apps.DjangoNextJSConfig` to `INSTALLED_APPS`.
 
-- **In Development Environment:**
+- Set up Next.js URLs depending on your environment.
 
-  - If you're using django channels (after Nextjs v12 you need this to be able to use hot-reload), add `NextJSProxyHttpConsumer` and `NextJSProxyWebsocketConsumer` to `asgi.py`:
+### Setup Next.js URLs (Development Environment)
 
-    ```python
-    import os
+If you're serving your site under ASGI during development,
+use [Django Channels](https://channels.readthedocs.io/en/stable/) and
+add `NextJSProxyHttpConsumer`, `NextJSProxyWebsocketConsumer` to `asgi.py` like the following example.
 
-    from django.core.asgi import get_asgi_application
-    from django.urls import re_path, path
+**Note:** We recommend using ASGI and Django Channels,
+because it is required for [fast refresh](https://nextjs.org/docs/architecture/fast-refresh) (hot module replacement) to work properly in Nextjs 12+.
 
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "myproject.settings")
-    django_asgi_app = get_asgi_application()
+```python
+import os
 
-    from channels.auth import AuthMiddlewareStack
-    from channels.routing import ProtocolTypeRouter, URLRouter
-    from django_nextjs.proxy import NextJSProxyHttpConsumer, NextJSProxyWebsocketConsumer
+from django.core.asgi import get_asgi_application
+from django.urls import re_path, path
 
-    from django.conf import settings
+os.environ.setdefault("DJANGO_SETTINGS_MODULE", "myproject.settings")
+django_asgi_app = get_asgi_application()
 
-    # put your custom routes here if you need
-    http_routes = [re_path(r"", django_asgi_app)]
-    websocket_routers = []
+from channels.auth import AuthMiddlewareStack
+from channels.routing import ProtocolTypeRouter, URLRouter
+from django_nextjs.proxy import NextJSProxyHttpConsumer, NextJSProxyWebsocketConsumer
 
-    if settings.DEBUG:
-        http_routes.insert(0, re_path(r"^(?:_next|__next|next).*", NextJSProxyHttpConsumer.as_asgi()))
-        websocket_routers.insert(0, path("_next/webpack-hmr", NextJSProxyWebsocketConsumer.as_asgi()))
+from django.conf import settings
 
+# put your custom routes here if you need
+http_routes = [re_path(r"", django_asgi_app)]
+websocket_routers = []
 
-    application = ProtocolTypeRouter(
-        {
-            # Django's ASGI application to handle traditional HTTP and websocket requests.
-            "http": URLRouter(http_routes),
-            "websocket": AuthMiddlewareStack(URLRouter(websocket_routers)),
-            # ...
-        }
-    )
-    ```
+if settings.DEBUG:
+    http_routes.insert(0, re_path(r"^(?:_next|__next|next).*", NextJSProxyHttpConsumer.as_asgi()))
+    websocket_routers.insert(0, path("_next/webpack-hmr", NextJSProxyWebsocketConsumer.as_asgi()))
 
-  - Otherwise, add the following to the beginning of `urls.py`:
 
-    ```python
-    path("", include("django_nextjs.urls"))
-    ```
+application = ProtocolTypeRouter(
+    {
+        # Django's ASGI application to handle traditional HTTP and websocket requests.
+        "http": URLRouter(http_routes),
+        "websocket": AuthMiddlewareStack(URLRouter(websocket_routers)),
+        # ...
+    }
+)
+```
 
-- **In Production:**
+Otherwise (if serving under WSGI during development), add the following to the beginning of `urls.py`:
 
-  - Use a reverse proxy like nginx:
+```python
+path("", include("django_nextjs.urls"))
+```
 
-    | URL                 | Action                                     |
-    | ------------------- | ------------------------------------------ |
-    | `/_next/static/...` | Serve `NEXTJS_PATH/.next/static` directory |
-    | `/_next/...`        | Proxy to `http://localhost:3000`           |
-    | `/next/...`         | Serve `NEXTJS_PATH/public/next` directory  |
+**Warning:** If you are serving under ASGI, do NOT add this
+to your `urls.py`. It may cause deadlocks.
 
-    Pass `x-real-ip` header when proxying `/_next/`:
+### Setup Next.js URLs (Production Environment)
 
-    ```conf
-    location /_next/ {
-        proxy_set_header  x-real-ip $remote_addr;
-        proxy_pass  http://127.0.0.1:3000;
-    }
-    ```
+In production, use a reverse proxy like Nginx or Caddy:
+
+| URL                 | Action                                     |
+| ------------------- | ------------------------------------------ |
+| `/_next/static/...` | Serve `NEXTJS_PATH/.next/static` directory |
+| `/_next/...`        | Proxy to `http://localhost:3000`           |
+| `/next/...`         | Serve `NEXTJS_PATH/public/next` directory  |
+
+Pass `x-real-ip` header when proxying `/_next/`. Example config for Nginx:
+
+```conf
+location /_next/static/ {
+    alias NEXTJS_PATH/.next/static/;
+    expires max;
+    add_header Cache-Control "public";
+}
+location /_next/ {
+    proxy_set_header  x-real-ip $remote_addr;
+    proxy_pass  http://127.0.0.1:3000;
+}
+location /next/ {
+    alias NEXTJS_PATH/public/next/;
+    expires max;
+    add_header Cache-Control "public";
+}
+```
 
 ## Usage
 
 Start Next.js server:
 
 ```shell
 # Development:
@@ -141,99 +161,102 @@
 
 # Production:
 $ npm run build
 $ npm run start
 ```
 
 Develop your pages in Next.js.
-Write a django URL and view for each page like this:
+Write a django URL and an async view for each page like this:
 
 ```python
-# If you're using django channels
 from django.http import HttpResponse
-from django_nextjs.render import render_nextjs_page_async
+from django_nextjs.render import render_nextjs_page
 
 async def jobs(request):
-    return await render_nextjs_page_async(request)
+    return await render_nextjs_page(request)
 ```
 
-```python
-# If you're not using django channels
-from django.http import HttpResponse
-from django_nextjs.render import render_nextjs_page_sync
-
-def jobs(request):
-    return render_nextjs_page_sync(request)
-```
+## Customizing the HTML Response
 
-## Customizing Document
+You can modify the HTML code that Next.js returns in your Django code.
 
-If you want to customize the HTML document (e.g. add header or footer), read this section.
+Avoiding duplicate code for the navbar and footer is a common use case
+for this if you are using both Next.js and Django templates.
+Without it, you would have to write and maintain two separate versions
+of your navbar and footer (a Django template version and a Next.js version).
+However, you can simply create a Django template for your navbar and insert its code
+at the beginning of `<body>` tag returned from Next.js.
 
-You need to [customize Next's document]:
+To enable this feature, you need to customize the document and root layout
+in Next.js and make the following adjustments:
 
 - Add `id="__django_nextjs_body"` as the first attribute of `<body>` element.
 - Add `<div id="__django_nextjs_body_begin" />` as the first element inside `<body>`.
 - Add `<div id="__django_nextjs_body_end" />` as the last element inside `<body>`.
 
-```jsx
-import Document, { Html, Head, Main, NextScript } from "next/document";
+NOTE: Currently HTML customization is not working with [app router](https://nextjs.org/docs/app) (Next.js 13+).
 
-// https://nextjs.org/docs/advanced-features/custom-document
-class MyDocument extends Document {
-  render() {
-    return (
-      <Html>
-        <Head />
-        <body id="__django_nextjs_body" dir="rtl">
-          <div id="__django_nextjs_body_begin" />
-          <Main />
-          <NextScript />
-          <div id="__django_nextjs_body_end" />
-        </body>
-      </Html>
-    );
-  }
-}
+Read
+[this doc](https://nextjs.org/docs/pages/building-your-application/routing/custom-document)
+and customize your Next.js document:
 
-export default MyDocument;
+```jsx
+// pages/_document.jsx (or .tsx)
+...
+<body id="__django_nextjs_body">
+  <div id="__django_nextjs_body_begin" />
+  <Main />
+  <NextScript />
+  <div id="__django_nextjs_body_end" />
+</body>
+...
 ```
 
+<!-- If you are using Next.js 13+, you also need to
+[customize the root layout](https://nextjs.org/docs/app/api-reference/file-conventions/layout)
+in `app` directory:
+
+```jsx
+// app/layout.jsx (or .tsx)
+...
+<body id="__django_nextjs_body" className={inter.className}>
+  <div id="__django_nextjs_body_begin" />
+  {children}
+  <div id="__django_nextjs_body_end" />
+</body>
+...
+``` -->
+
 Write a django template that extends `django_nextjs/document_base.html`:
 
 ```django
 {% extends "django_nextjs/document_base.html" %}
 
 
 {% block head %}
-  ... the content you want to add to the beginning of <head> tag ...
+  <!-- ... the content you want to place at the beginning of "head" tag ... -->
   {{ block.super }}
-  ... the content you want to add to the end of <head> tag ...
+  <!-- ... the content you want to place at the end of "head" tag ... -->
 {% endblock %}
 
 
 {% block body %}
-  ... the content you want to add to the beginning of <body> tag ...
+  ... the content you want to place at the beginning of "body" tag ...
+  ... e.g. include the navbar template ...
   {{ block.super }}
-  ... the content you want to add to the end of <body> tag ...
+  ... the content you want to place at the end of "body" tag ...
+  ... e.g. include the footer template ...
 {% endblock %}
 ```
 
-Pass the template name to `render_nextjs_page_async` or `render_nextjs_page_sync`:
+Pass the template name to `render_nextjs_page`:
 
 ```python
-# If you're using django channels
 async def jobs(request):
-    return await render_nextjs_page_async(request, "path/to/template.html")
-```
-
-```python
-# If you're not using django channels
-def jobs(request):
-    return render_nextjs_page_sync(request, "path/to/template.html")
+    return await render_nextjs_page(request, "path/to/template.html")
 ```
 
 ## Notes
 
 - If you want to add a file to `public` directory of Next.js,
   that file should be in `public/next` subdirectory to work correctly.
 - If you're using django channels, make sure all your middlewares are
@@ -263,12 +286,11 @@
 
 ## References
 
 - https://github.com/yourlabs/djnext
 - [comment on StackOverflow]
 
 [comment on stackoverflow]: https://stackoverflow.com/questions/54252943/is-there-a-way-to-integrate-django-with-next-js#comment110078700_54252943
-[customize next's document]: https://nextjs.org/docs/advanced-features/custom-document
 
 ## License
 
 MIT
```

### Comparing `django-nextjs-2.2.3/setup.py` & `django-nextjs-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,43 @@
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 dev_requirements = [
     "pre-commit",
     "pytest>=7",
     "pytest-cov",
     "pytest-django",
+    "pytest-asyncio",
     "black",
+    "isort",
 ]
 
 setup(
     name="django-nextjs",
     version=__version__,
     description="Next.js + Django integration",
     long_description=README,
     long_description_content_type="text/markdown",
     keywords=["django", "next", "nextjs", "django-nextjs"],
     author="Mohammad Javad Naderi <mjnaderi@gmail.com>, Danial Keimasi <danialkeimasi@gmail.com>",
     url="https://github.com/QueraTeam/django-nextjs",
     download_url="https://github.com/QueraTeam/django-nextjs",
     packages=find_packages(".", include=("django_nextjs", "django_nextjs.*")),
     include_package_data=True,
-    install_requires=["Django >= 3.2", "requests", "aiohttp", "channels", "websockets"],
+    install_requires=["Django >= 3.2", "aiohttp", "channels", "websockets"],
     extras_require={"dev": dev_requirements},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
 )
```

