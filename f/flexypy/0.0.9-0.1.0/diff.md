# Comparing `tmp/flexypy-0.0.9.tar.gz` & `tmp/flexypy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexypy-0.0.9.tar", last modified: Tue Apr 25 09:48:23 2023, max compression
+gzip compressed data, was "flexypy-0.1.0.tar", last modified: Mon Jun 12 15:52:02 2023, max compression
```

## Comparing `flexypy-0.0.9.tar` & `flexypy-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.329828 flexypy-0.0.9/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-25 09:48:23.329828 flexypy-0.0.9/PKG-INFO
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.057825 flexypy-0.0.9/flexypy/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.9/flexypy/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.9/flexypy/cli.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.181826 flexypy-0.0.9/flexypy/exceptions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.9/flexypy/exceptions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.9/flexypy/exceptions/baseexceptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.9/flexypy/exceptions/extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.9/flexypy/exceptions/render.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.9/flexypy/exceptions/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.9/flexypy/exceptions/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.189827 flexypy-0.0.9/flexypy/exceptions/web/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.9/flexypy/exceptions/web/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.9/flexypy/exceptions/web/baseexseptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.9/flexypy/exceptions/web/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.209827 flexypy-0.0.9/flexypy/generate_templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.9/flexypy/generate_templates/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.9/flexypy/generate_templates/generator.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.229827 flexypy-0.0.9/flexypy/generate_templates/templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.9/flexypy/generate_templates/templates/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.253827 flexypy-0.0.9/flexypy/generate_templates/templates/config/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.9/flexypy/generate_templates/templates/config/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       86 2023-04-23 08:22:28.000000 flexypy-0.0.9/flexypy/generate_templates/templates/config/apps.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.9/flexypy/generate_templates/templates/config/dirs.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      201 2023-04-23 08:23:04.000000 flexypy-0.0.9/flexypy/generate_templates/templates/main.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.289828 flexypy-0.0.9/flexypy/http/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.9/flexypy/http/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.0.9/flexypy/http/cookie.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2431 2023-04-23 10:12:45.000000 flexypy-0.0.9/flexypy/http/request.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2688 2023-04-25 09:44:33.000000 flexypy-0.0.9/flexypy/http/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     9797 2023-04-24 10:05:14.000000 flexypy-0.0.9/flexypy/http/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.289828 flexypy-0.0.9/flexypy/http/template/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.9/flexypy/http/template/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.301828 flexypy-0.0.9/flexypy/http/template/extensions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.9/flexypy/http/template/extensions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.9/flexypy/http/template/extensions/base_extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.9/flexypy/http/template/extensions/template_ext.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.9/flexypy/http/template/render.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.321828 flexypy-0.0.9/flexypy/middlewares/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.9/flexypy/middlewares/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.9/flexypy/middlewares/mddl.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-25 09:48:23.133826 flexypy-0.0.9/flexypy.egg-info/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-25 09:48:23.000000 flexypy-0.0.9/flexypy.egg-info/PKG-INFO
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-04-25 09:48:23.000000 flexypy-0.0.9/flexypy.egg-info/SOURCES.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-25 09:48:23.000000 flexypy-0.0.9/flexypy.egg-info/dependency_links.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       34 2023-04-25 09:48:23.000000 flexypy-0.0.9/flexypy.egg-info/requires.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-25 09:48:23.000000 flexypy-0.0.9/flexypy.egg-info/top_level.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      405 2023-04-25 09:48:07.000000 flexypy-0.0.9/pyproject.toml
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-25 09:48:23.329828 flexypy-0.0.9/setup.cfg
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-06-12 15:52:02.266679 flexypy-0.1.0/PKG-INFO
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.230679 flexypy-0.1.0/flexypy/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.1.0/flexypy/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.1.0/flexypy/cli.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/exceptions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.1.0/flexypy/exceptions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.1.0/flexypy/exceptions/baseexceptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.1.0/flexypy/exceptions/extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.1.0/flexypy/exceptions/render.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.1.0/flexypy/exceptions/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.1.0/flexypy/exceptions/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/exceptions/web/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.1.0/flexypy/exceptions/web/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.1.0/flexypy/exceptions/web/baseexseptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.1.0/flexypy/exceptions/web/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/generate_templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.1.0/flexypy/generate_templates/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      953 2023-04-27 09:44:58.000000 flexypy-0.1.0/flexypy/generate_templates/generator.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/generate_templates/templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.1.0/flexypy/generate_templates/templates/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.262679 flexypy-0.1.0/flexypy/generate_templates/templates/config/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.1.0/flexypy/generate_templates/templates/config/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       86 2023-04-23 08:22:28.000000 flexypy-0.1.0/flexypy/generate_templates/templates/config/apps.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.1.0/flexypy/generate_templates/templates/config/dirs.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      201 2023-04-23 08:23:04.000000 flexypy-0.1.0/flexypy/generate_templates/templates/main.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/http/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.1.0/flexypy/http/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.1.0/flexypy/http/cookie.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2552 2023-06-12 15:43:55.000000 flexypy-0.1.0/flexypy/http/request.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2645 2023-04-27 09:44:59.000000 flexypy-0.1.0/flexypy/http/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)    10059 2023-06-12 15:35:09.000000 flexypy-0.1.0/flexypy/http/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/http/template/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.1.0/flexypy/http/template/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/http/template/extensions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.1.0/flexypy/http/template/extensions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      764 2023-04-27 09:44:58.000000 flexypy-0.1.0/flexypy/http/template/extensions/base_extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.1.0/flexypy/http/template/extensions/template_ext.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.1.0/flexypy/http/template/render.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/middlewares/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.1.0/flexypy/middlewares/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.1.0/flexypy/middlewares/mddl.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.250679 flexypy-0.1.0/flexypy.egg-info/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/PKG-INFO
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       34 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/requires.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/top_level.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      405 2023-06-12 15:47:57.000000 flexypy-0.1.0/pyproject.toml
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-06-12 15:52:02.266679 flexypy-0.1.0/setup.cfg
```

### Comparing `flexypy-0.0.9/flexypy/exceptions/web/server.py` & `flexypy-0.1.0/flexypy/exceptions/web/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.9/flexypy/generate_templates/generator.py` & `flexypy-0.1.0/flexypy/generate_templates/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,11 +25,7 @@
             os.mkdir(dir_path)
 
         if os.path.exists(dir_path):
             if not os.path.exists(os.path.join(dir_path, file['name'])) and file['name']:
                 with open(os.path.join(dir_path, file['name']), 'w+') as wf:
                     with open(file['path'], 'r') as rf:
                         wf.write(rf.read())
-
-
-if __name__ == '__main__':
-    generate('/home/uwine/Documents/python/flexypy/')
```

### Comparing `flexypy-0.0.9/flexypy/http/cookie.py` & `flexypy-0.1.0/flexypy/http/cookie.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.9/flexypy/http/request.py` & `flexypy-0.1.0/flexypy/http/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,34 +71,37 @@
         return cls._set_cookie
 
     @classmethod
     def clear_request_cookie(cls):
         cls._set_cookie = {}
 
     @classmethod
-    def set_cookie(cls, name, value, expires=None):
+    def set_cookie(cls, name, value, expires=None, max_age=None):
         c = cookies.SimpleCookie()
         c[name] = Cookie.encrypt_cookie(value).decode()
         c[name]['expires'] = (datetime.datetime.now() + datetime.timedelta(days=365)). \
             strftime('%a, %d-%b-%Y %H:%M:%S GMT')
         c[name]['secure'] = True
         c[name]['path'] = '/'
+        if max_age is not None:
+            c[name]['max-age'] = max_age
         if expires:
             c[name]['expires'] = expires
         cls._set_cookie.update(c)
 
     @classmethod
     def set_server_cookie(cls, cookie):
         c = cookies.SimpleCookie()
-        c.load(cookie)
+        if cookie:
+            c.load(cookie)
         cls._server_cookie = c
 
     @classmethod
     def get_server_cookie(cls, name):
         try:
             return Cookie.decrypt_cookie(cls._server_cookie.get(name).value.encode())
         except:
             return None
 
     @classmethod
     def delete_cookie(cls, name):
-        cls.set_cookie(name, '', expires='Thu, 01, Jan 1970 00:00:00 GMT')
+        cls.set_cookie(name, '', expires='Thu, 01, Jan 1970 00:00:00 GMT', max_age=0)
```

### Comparing `flexypy-0.0.9/flexypy/http/routing.py` & `flexypy-0.1.0/flexypy/http/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,12 +89,7 @@
         if self.parent_route:
             return self.parent_route().path.strip('/') + '/' + path.lstrip('/')
         else:
             return path
 
     def post(self):
         pass
-
-
-# def redirect(path):
-#     return path
-
```

### Comparing `flexypy-0.0.9/flexypy/http/server.py` & `flexypy-0.1.0/flexypy/http/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os
 from flexypy.exceptions.web.server import PathNotFound
 from urllib import parse
 from cgi import FieldStorage
 from flexypy.middlewares.mddl import Middleware
 import re
 from flexypy.http.cookie import Cookie
+from http import cookies
 
 
 @dataclass
 class HtmlResponse:
     code: str
     header: list[tuple[str, str]]
     html: bytes
@@ -45,15 +46,22 @@
         self._get_fxp_apps()
         self.router = Router(self.environ, self.routes, self.full_url)
         self._set_server_cookie()
 
     def _set_server_cookie(self):
         try:
             if 'HTTP_COOKIE' in self.environ:
+                c = cookies.SimpleCookie()
+                c.load(self.environ['HTTP_COOKIE'])
+                for i in list(c.keys()):
+                    if Cookie.decrypt_cookie(c.get(i).value.encode()) == '':
+                        c.pop(i)
                 self.request.set_server_cookie(self.environ['HTTP_COOKIE'])
+            else:
+                self.request.set_server_cookie(None)
         except Exception as e:
             pass
 
     def _route(self) -> HtmlResponse:
         path_found = False
         match self.environ['REQUEST_METHOD']:
             case 'GET':
@@ -160,17 +168,16 @@
                 m.start()
                 mddl_app = m.app
                 redirect = MddlRedirect(m.redirect_from, m.redirect_to)
         return [mddl_app, redirect]
 
     def start(self):
         resp = self._route()
+        self._set_server_cookie()
 
-        if 'HTTP_COOKIE' in self.environ:
-            self.request.set_server_cookie(self.environ['HTTP_COOKIE'])
         if resp:
             # set header cookies
             header = Cookie(self.request).set_server_cookie(resp.header)
             if header:
                 resp.header = header
 
             self.start_response(resp.code, resp.header)
```

### Comparing `flexypy-0.0.9/flexypy/http/template/extensions/base_extension.py` & `flexypy-0.1.0/flexypy/http/template/extensions/base_extension.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
         return nodes.Output([nodes.MarkSafe(call)]).set_lineno(lineno)
 
     @abstractmethod
     def handler(self) -> str:
         """
         Extension handler.
         """
-        pass
+        pass
```

### Comparing `flexypy-0.0.9/flexypy/http/template/extensions/template_ext.py` & `flexypy-0.1.0/flexypy/http/template/extensions/template_ext.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.9/flexypy/http/template/render.py` & `flexypy-0.1.0/flexypy/http/template/render.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.9/flexypy.egg-info/SOURCES.txt` & `flexypy-0.1.0/flexypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

