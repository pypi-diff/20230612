# Comparing `tmp/elkm1_lib-2.2.4.tar.gz` & `tmp/elkm1_lib-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkm1_lib-2.2.4.tar", max compression
+gzip compressed data, was "elkm1_lib-2.2.5.tar", max compression
```

## Comparing `elkm1_lib-2.2.4.tar` & `elkm1_lib-2.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     9610 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     9289 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/README.md
--rw-r--r--   0        0        0    12509 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/bin/cmdr.py
--rwxr-xr-x   0        0        0     3088 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/bin/elk
--rwxr-xr-x   0        0        0     2165 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/bin/mkdoc
--rwxr-xr-x   0        0        0     1259 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/bin/simple
--rwxr-xr-x   0        0        0     2117 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/bin/test-serial
--rw-r--r--   0        0        0       41 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/__init__.py
--rw-r--r--   0        0        0     5127 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/areas.py
--rw-r--r--   0        0        0     7032 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/connection.py
--rw-r--r--   0        0        0    10373 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/const.py
--rw-r--r--   0        0        0     1424 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/counters.py
--rw-r--r--   0        0        0     5827 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/discovery.py
--rw-r--r--   0        0        0     5119 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/elements.py
--rw-r--r--   0        0        0     5183 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/elk.py
--rw-r--r--   0        0        0     3586 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/keypads.py
--rw-r--r--   0        0        0     1835 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/lights.py
--rw-r--r--   0        0        0    18619 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/message.py
--rw-r--r--   0        0        0     1478 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/notify.py
--rw-r--r--   0        0        0     1691 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/outputs.py
--rw-r--r--   0        0        0     4437 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/panel.py
--rw-r--r--   0        0        0        0 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/py.typed
--rw-r--r--   0        0        0     1848 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/settings.py
--rw-r--r--   0        0        0     1096 2023-06-10 15:16:58.641632 elkm1_lib-2.2.4/elkm1_lib/tasks.py
--rw-r--r--   0        0        0     3196 2023-06-10 15:16:58.645633 elkm1_lib-2.2.4/elkm1_lib/thermostats.py
--rw-r--r--   0        0        0      974 2023-06-10 15:16:58.645633 elkm1_lib-2.2.4/elkm1_lib/users.py
--rw-r--r--   0        0        0     2532 2023-06-10 15:16:58.645633 elkm1_lib-2.2.4/elkm1_lib/util.py
--rw-r--r--   0        0        0     4933 2023-06-10 15:16:58.645633 elkm1_lib-2.2.4/elkm1_lib/zones.py
--rw-r--r--   0        0        0     1943 2023-06-10 15:16:58.645633 elkm1_lib-2.2.4/pyproject.toml
--rw-r--r--   0        0        0    10027 1970-01-01 00:00:00.000000 elkm1_lib-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     9610 2023-06-11 23:30:53.046765 elkm1_lib-2.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     9289 2023-06-11 23:30:53.046765 elkm1_lib-2.2.5/README.md
+-rw-r--r--   0        0        0    12509 2023-06-11 23:30:53.046765 elkm1_lib-2.2.5/bin/cmdr.py
+-rwxr-xr-x   0        0        0     3088 2023-06-11 23:30:53.046765 elkm1_lib-2.2.5/bin/elk
+-rwxr-xr-x   0        0        0     2165 2023-06-11 23:30:53.046765 elkm1_lib-2.2.5/bin/mkdoc
+-rwxr-xr-x   0        0        0     1259 2023-06-11 23:30:53.046765 elkm1_lib-2.2.5/bin/simple
+-rwxr-xr-x   0        0        0     2117 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/bin/test-serial
+-rw-r--r--   0        0        0       41 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/__init__.py
+-rw-r--r--   0        0        0     5127 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/areas.py
+-rw-r--r--   0        0        0     7032 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/connection.py
+-rw-r--r--   0        0        0    10373 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/const.py
+-rw-r--r--   0        0        0     1424 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/counters.py
+-rw-r--r--   0        0        0     5856 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/discovery.py
+-rw-r--r--   0        0        0     5119 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/elements.py
+-rw-r--r--   0        0        0     5183 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/elk.py
+-rw-r--r--   0        0        0     3586 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/keypads.py
+-rw-r--r--   0        0        0     1835 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/lights.py
+-rw-r--r--   0        0        0    18619 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/message.py
+-rw-r--r--   0        0        0     1478 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/notify.py
+-rw-r--r--   0        0        0     1691 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/outputs.py
+-rw-r--r--   0        0        0     4437 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/panel.py
+-rw-r--r--   0        0        0        0 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/py.typed
+-rw-r--r--   0        0        0     1848 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/settings.py
+-rw-r--r--   0        0        0     1096 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/tasks.py
+-rw-r--r--   0        0        0     3196 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/thermostats.py
+-rw-r--r--   0        0        0      974 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/users.py
+-rw-r--r--   0        0        0     2426 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/util.py
+-rw-r--r--   0        0        0     4933 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/elkm1_lib/zones.py
+-rw-r--r--   0        0        0     1943 2023-06-11 23:30:53.050765 elkm1_lib-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0    10027 1970-01-01 00:00:00.000000 elkm1_lib-2.2.5/PKG-INFO
```

### Comparing `elkm1_lib-2.2.4/CHANGELOG.md` & `elkm1_lib-2.2.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/README.md` & `elkm1_lib-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/bin/cmdr.py` & `elkm1_lib-2.2.5/bin/cmdr.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/bin/elk` & `elkm1_lib-2.2.5/bin/elk`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/bin/mkdoc` & `elkm1_lib-2.2.5/bin/mkdoc`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/bin/simple` & `elkm1_lib-2.2.5/bin/simple`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/bin/test-serial` & `elkm1_lib-2.2.5/bin/test-serial`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/areas.py` & `elkm1_lib-2.2.5/elkm1_lib/areas.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/connection.py` & `elkm1_lib-2.2.5/elkm1_lib/connection.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/const.py` & `elkm1_lib-2.2.5/elkm1_lib/const.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/counters.py` & `elkm1_lib-2.2.5/elkm1_lib/counters.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/discovery.py` & `elkm1_lib-2.2.5/elkm1_lib/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,16 @@
                 destination=destination,
                 on_response=_on_response,
             ),
             sock=sock,
         )
         try:
             await self._async_run_scan(
-                cast(asyncio.DatagramTransport, transport),
+                # cast(asyncio.DatagramTransport, transport),
+                transport,
                 destination,
                 timeout,
                 found_all_future,
             )
         finally:
             transport.close()
```

### Comparing `elkm1_lib-2.2.4/elkm1_lib/elements.py` & `elkm1_lib-2.2.5/elkm1_lib/elements.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/elk.py` & `elkm1_lib-2.2.5/elkm1_lib/elk.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/keypads.py` & `elkm1_lib-2.2.5/elkm1_lib/keypads.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/lights.py` & `elkm1_lib-2.2.5/elkm1_lib/lights.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/message.py` & `elkm1_lib-2.2.5/elkm1_lib/message.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/notify.py` & `elkm1_lib-2.2.5/elkm1_lib/notify.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/outputs.py` & `elkm1_lib-2.2.5/elkm1_lib/outputs.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/panel.py` & `elkm1_lib-2.2.5/elkm1_lib/panel.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/settings.py` & `elkm1_lib-2.2.5/elkm1_lib/settings.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/tasks.py` & `elkm1_lib-2.2.5/elkm1_lib/tasks.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/thermostats.py` & `elkm1_lib-2.2.5/elkm1_lib/thermostats.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/users.py` & `elkm1_lib-2.2.5/elkm1_lib/users.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/elkm1_lib/util.py` & `elkm1_lib-2.2.5/elkm1_lib/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,15 @@
     for future use since we only have a few schemes.
     """
     ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
     if tls := TLS_VERSIONS.get(scheme):
         ssl_context.minimum_version = tls
         ssl_context.maximum_version = tls
 
-    ssl_context.set_ciphers("ALL")
-    # ssl_context.set_ciphers(
-    #     "DEFAULT:!aNULL:!eNULL:!MD5:!3DES:!DES:!RC4:!IDEA:!SEED:!aDSS:!SRP:!PSK"
-    # )
+    ssl_context.set_ciphers("DEFAULT:@SECLEVEL=0")
 
     # ssl.OP_LEGACY_SERVER_CONNECT is only available in Python 3.12a4+
     ssl_context.options |= getattr(ssl, "OP_LEGACY_SERVER_CONNECT", 0x4)
     return ssl_context
 
 
 def parse_url(url: str) -> tuple[str, str, int, ssl.SSLContext | None]:
```

### Comparing `elkm1_lib-2.2.4/elkm1_lib/zones.py` & `elkm1_lib-2.2.5/elkm1_lib/zones.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.4/pyproject.toml` & `elkm1_lib-2.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elkm1-lib"
-version = "2.2.4"
+version = "2.2.5"
 description = "Library for interacting with ElkM1 alarm/automation panel."
 homepage = "https://github.com/gwww/elkm1"
 authors = ["Glenn Waters <gwwaters+elkm1@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   'Development Status :: 5 - Production/Stable',
```

### Comparing `elkm1_lib-2.2.4/PKG-INFO` & `elkm1_lib-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkm1-lib
-Version: 2.2.4
+Version: 2.2.5
 Summary: Library for interacting with ElkM1 alarm/automation panel.
 Home-page: https://github.com/gwww/elkm1
 License: MIT
 Author: Glenn Waters
 Author-email: gwwaters+elkm1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

