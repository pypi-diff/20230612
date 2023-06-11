# Comparing `tmp/kkutils-1.6.4.tar.gz` & `tmp/kkutils-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkutils-1.6.4.tar", last modified: Thu Apr 20 03:35:51 2023, max compression
+gzip compressed data, was "kkutils-1.6.5.tar", last modified: Sun Jun 11 23:10:38 2023, max compression
```

## Comparing `kkutils-1.6.4.tar` & `kkutils-1.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.044617 kkutils-1.6.4/
--rw-r--r--   0 root         (0) root         (0)      703 2023-04-20 03:35:51.044617 kkutils-1.6.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.040617 kkutils-1.6.4/kkutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      619 2023-04-20 03:35:51.000000 kkutils-1.6.4/kkutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-20 03:35:50.000000 kkutils-1.6.4/kkutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.4/processor.py
--rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 03:35:51.044617 kkutils-1.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-20 03:35:48.000000 kkutils-1.6.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.040617 kkutils-1.6.4/tornado_utils/
--rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.4/tornado_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.4/tornado_utils/application.py
--rw-r--r--   0 root         (0) root         (0)    10043 2023-03-06 03:11:06.000000 kkutils-1.6.4/tornado_utils/basehandler.py
--rw-r--r--   0 root         (0) root         (0)    12696 2023-03-16 13:15:20.000000 kkutils-1.6.4/tornado_utils/userhandler.py
--rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.4/tornado_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 03:35:51.044617 kkutils-1.6.4/utils/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.4/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10413 2023-04-20 03:33:38.000000 kkutils-1.6.4/utils/base_utils.py
--rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/cached_property.py
--rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-02-19 15:22:17.000000 kkutils-1.6.4/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)    10693 2022-11-04 03:27:22.000000 kkutils-1.6.4/utils/curl_utils.py
--rw-r--r--   0 root         (0) root         (0)    16416 2023-04-18 08:50:58.000000 kkutils-1.6.4/utils/db_utils.py
--rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)     4007 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/email_utils.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.4/utils/fire.py
--rw-r--r--   0 root         (0) root         (0)    26362 2023-02-19 15:22:17.000000 kkutils-1.6.4/utils/http_utils.py
--rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.4/utils/log_utils.py
--rw-r--r--   0 root         (0) root         (0)     6577 2022-07-14 13:13:22.000000 kkutils-1.6.4/utils/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.4/utils/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.4/utils/xdb_searcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.897494 kkutils-1.6.5/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-11 23:10:38.897494 kkutils-1.6.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.893493 kkutils-1.6.5/kkutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.5/processor.py
+-rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 23:10:38.897494 kkutils-1.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-11 23:10:36.000000 kkutils-1.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.893493 kkutils-1.6.5/tornado_utils/
+-rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.5/tornado_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.5/tornado_utils/application.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2023-06-03 05:59:58.000000 kkutils-1.6.5/tornado_utils/basehandler.py
+-rw-r--r--   0 root         (0) root         (0)    12696 2023-03-16 13:15:20.000000 kkutils-1.6.5/tornado_utils/userhandler.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.5/tornado_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.897494 kkutils-1.6.5/utils/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.5/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10493 2023-06-10 09:51:09.000000 kkutils-1.6.5/utils/base_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.5/utils/cached_property.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.5/utils/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-01 12:38:54.000000 kkutils-1.6.5/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)    10699 2023-06-11 01:44:37.000000 kkutils-1.6.5/utils/curl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16416 2023-04-18 08:50:58.000000 kkutils-1.6.5/utils/db_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.5/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-06-02 07:24:05.000000 kkutils-1.6.5/utils/email_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.5/utils/fire.py
+-rw-r--r--   0 root         (0) root         (0)    26557 2023-06-11 01:22:42.000000 kkutils-1.6.5/utils/http_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.5/utils/log_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6563 2023-06-03 06:12:56.000000 kkutils-1.6.5/utils/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.5/utils/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.5/utils/xdb_searcher.py
```

### Comparing `kkutils-1.6.4/PKG-INFO` & `kkutils-1.6.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.4
+Version: 1.6.5
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.4/kkutils.egg-info/PKG-INFO` & `kkutils-1.6.5/kkutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.4
+Version: 1.6.5
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.4/kkutils.egg-info/SOURCES.txt` & `kkutils-1.6.5/kkutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/processor.py` & `kkutils-1.6.5/processor.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/setup.py` & `kkutils-1.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Last modified: 2019-04-07 00:07:43
 '''
 
 from setuptools import setup
 
 setup(
     name="kkutils",
-    version="1.6.4",
+    version="1.6.5",
     description="python utils",
     author="digua",
     author_email="zkdfbb@qq.com",
     url="https://www.ishield.cn",
     license="MIT",
     python_requires='>=3.6',
     data_files=[('', ['requirements.txt'])],
```

### Comparing `kkutils-1.6.4/tornado_utils/application.py` & `kkutils-1.6.5/tornado_utils/application.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/tornado_utils/basehandler.py` & `kkutils-1.6.5/tornado_utils/basehandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,23 +79,14 @@
         if time.time() - int(self.args.t, 16) >= 3600:
             raise tornado.web.HTTPError(403)
 
         key = f'{prefix}_{self.args.t}_{self.args.n}'.encode()
         if self.args.s[:8] != getattr(hashlib, method)(key).hexdigest()[:8]:
             raise tornado.web.HTTPError(403)
 
-        '''
-        key = f'{self.prefix}_{self.args.s}'
-        value = await self.rd.get(key)
-        if value is None:
-            await self.rd.setex(key, 3600, self.args.ip)
-        elif value != self.args.ip:
-            raise tornado.web.HTTPError(403)
-        '''
-
     async def get_current_user(self):
         token = self.get_cookie('token', self.args.token)
         if token and hasattr(self.app, 'db') and isinstance(self.app.db, (Mongo, Motor)):
             user = await awaitable(self.app.db.users.find_one({'token': token}))
             if user:
                 if self.args.token and not self.get_cookie('token'):
                     expires = datetime.datetime.now() + datetime.timedelta(days=30)
@@ -104,26 +95,26 @@
         return Dict()
 
     async def prepare(self):
         self.current_user = await awaitable(self.get_current_user())
 
     @cached_property
     def ip(self):
-        if 'Cdn-Real-Ip' in self.request.headers:
-            return self.request.headers['Cdn-Real-Ip']
-        elif 'X-Forwarded-For' in self.request.headers:
+        if 'X-Forwarded-For' in self.request.headers:
             return self.request.headers['X-Forwarded-For'].split(',')[0]
         elif 'X-Real-Ip' in self.request.headers:
             return self.request.headers['X-Real-Ip']
         else:
             return self.request.remote_ip
 
     @cached_property
     def port(self):
-        return self.request.headers.get('X-Real-Port')
+        port = self.request.headers.get('X-Real-Port', '')
+        if port.isdigit():
+            return int(port)
 
     @cached_property
     def mobile(self):
         regexp = re.compile(r'Mobile|Android|iPhone|Windows Phone|iPad|Opera Mobi|iPod|UCBrowser|MQQBrowser|Quark|MicroMessenger', re.I)
         return True if regexp.search(self.ua) else False
 
     @cached_property
```

### Comparing `kkutils-1.6.4/tornado_utils/userhandler.py` & `kkutils-1.6.5/tornado_utils/userhandler.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/tornado_utils/utils.py` & `kkutils-1.6.5/tornado_utils/utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/__init__.py` & `kkutils-1.6.5/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/base_utils.py` & `kkutils-1.6.5/utils/base_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,21 +242,23 @@
 
 async def awaitable(ret):
     return await ret if inspect.isawaitable(ret) else ret
 
 
 def multi_apply(func, *args, **kwargs):
     workers = kwargs.pop('workers', os.cpu_count())
+    batch = kwargs.pop('batch', workers)
     backend = kwargs.pop('backend', 'thread')
     size = len(args[0])
-    args = [[x[i::workers] for i in range(workers)] for x in args]
+    step = math.ceil(size / batch)
+    iterables = [[x[i::step] for i in range(step)] for x in args]
     func = partial(func, **kwargs) if kwargs else func
     Executor = ThreadPoolExecutor if backend == 'thread' else ProcessPoolExecutor
     with Executor(workers) as executor:
-        results = executor.map(func, *args)
+        results = executor.map(func, *iterables)
     results = list(results)
     if all([isinstance(x, (list, tuple)) for x in results]):
         results = list(chain(*zip_longest(*results)))[:size]
     return results
 
 
 def floor(number, ndigits=0):
```

### Comparing `kkutils-1.6.4/utils/cached_property.py` & `kkutils-1.6.5/utils/cached_property.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/config_utils.py` & `kkutils-1.6.5/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/crypto.py` & `kkutils-1.6.5/utils/crypto.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 Author: zhangkai
 Last modified: 2020-06-14 19:33:33
 '''
 
+import base64
 import binascii
 
 import rsa
 from Crypto.Cipher import AES, DES
 
 from .base_utils import to_bytes, to_str
 
@@ -30,45 +31,59 @@
     return to_str(binascii.b2a_hex(data))
 
 
 def hex_load(text):
     return binascii.a2b_hex(text)
 
 
-def des_encrypt(data, key):
+def des_encrypt(text, key, iv=None, mode=DES.MODE_CBC, encode='base64'):
     ''' key: 8位 '''
-    data = _pad(to_bytes(data), DES.block_size)
+    data = _pad(to_bytes(text), DES.block_size)
     key = to_bytes(key)
-    cipher = DES.new(key, DES.MODE_CBC, key)
+    iv = iv or key[:8]
+    cipher = DES.new(key, mode, iv)
     encrypt_data = cipher.encrypt(data)
-    return to_str(binascii.b2a_hex(encrypt_data))
+    if encode == 'base64':
+        return to_str(base64.b64encode(encrypt_data))
+    else:
+        return to_str(binascii.b2a_hex(encrypt_data))
 
 
-def des_decrypt(ciphertext, key):
-    data = binascii.a2b_hex(to_bytes(ciphertext))
+def des_decrypt(ciphertext, key, iv=None, mode=DES.MODE_CBC, encode='base64'):
+    if encode == 'base64':
+        data = base64.b64decode(ciphertext)
+    else:
+        data = binascii.a2b_hex(to_bytes(ciphertext))
     key = to_bytes(key)
-    cipher = DES.new(key, DES.MODE_CBC, key)
+    iv = iv or key[:8]
+    cipher = DES.new(key, mode, iv)
     return to_str(_unpad(cipher.decrypt(data)))
 
 
-def aes_encrypt(data, key, iv=None):
+def aes_encrypt(text, key, iv=None, mode=AES.MODE_CBC, encode='base64'):
     ''' key: 32位, iv: 16位 '''
-    data = _pad(to_bytes(data), AES.block_size)
+    data = _pad(to_bytes(text), AES.block_size)
     key = to_bytes(key)
     iv = iv or key[:16]
-    cipher = AES.new(key, AES.MODE_CBC, iv)
+    cipher = AES.new(key, mode, iv)
     encrypt_data = cipher.encrypt(data)
-    return to_str(binascii.b2a_hex(encrypt_data))
+    if encode == 'base64':
+        return to_str(base64.b64encode(encrypt_data))
+    else:
+        return to_str(binascii.b2a_hex(encrypt_data))
 
 
-def aes_decrypt(ciphertext, key, iv=None):
-    data = binascii.a2b_hex(ciphertext)
+def aes_decrypt(ciphertext, key, iv=None, mode=AES.MODE_CBC, encode='base64'):
+    if encode == 'base64':
+        data = base64.b64decode(ciphertext)
+    else:
+        data = binascii.a2b_hex(to_bytes(ciphertext))
     key = to_bytes(key)
     iv = iv or key[:16]
-    cipher = AES.new(key, AES.MODE_CBC, iv)
+    cipher = AES.new(key, mode, iv)
     return to_str(_unpad(cipher.decrypt(data)))
 
 
 def gen_rsa_key(length=1024):
     pubkey, privkey = rsa.newkeys(length)
     return pubkey.save_pkcs1(), privkey.save_pkcs1()
```

### Comparing `kkutils-1.6.4/utils/curl_utils.py` & `kkutils-1.6.5/utils/curl_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,18 @@
         curl.setopt(pycurl.MAXREDIRS, 5)
         curl.setopt(pycurl.HEADER, 0)
         curl.setopt(pycurl.VERBOSE, 0)
         curl.setopt(pycurl.SSL_VERIFYPEER, 0)
         curl.setopt(pycurl.SSL_VERIFYHOST, 0)
         curl.setopt(pycurl.ACCEPT_ENCODING, "gzip,deflate,sdch")
         curl.setopt(pycurl.HTTP_CONTENT_DECODING, 0)
+        # 设置使用http1.1访问，在某些情况下入上传到qqdoc时使用http2会有问题
+        curl.setopt(pycurl.HTTP_VERSION, pycurl.CURL_HTTP_VERSION_1_1)
+        # 可能会导致403
         # curl.setopt(pycurl.AUTOREFERER, 1)
-        # 导致未知的403错误 https://video.wanmeikk.me/hls/a02689e5-d0f6-4a55-a590-75119b142a21/d6MJXL_kK9bOc1cTqAs3vVOWDA6wepIKOln9hG_oIT2vMXt81bvAsSaNmOVnaXAcM2BsEd87CSN9VlFIrLZuSw==.ts
         curl.setopt(pycurl.URL, urllib.parse.quote(url, safe='#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'))
         curl.setopt(pycurl.TRANSFER_ENCODING, int(kwargs.get('chunked', False)))
         curl.setopt(pycurl.FOLLOWLOCATION, kwargs['allow_redirects'])
         curl.setopt(pycurl.CONNECTTIMEOUT, kwargs['timeout'])
         curl.setopt(pycurl.TIMEOUT, kwargs['timeout'])
         self.load_cookie(curl)
         self.load_proxy(curl, kwargs.get('proxy'))
```

### Comparing `kkutils-1.6.4/utils/db_utils.py` & `kkutils-1.6.5/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/decorator.py` & `kkutils-1.6.5/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/email_utils.py` & `kkutils-1.6.5/utils/email_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 Author: zhangkai
 Last modified: 2019-09-24 18:56:04
 '''
+
 import asyncio
 import os
 import smtplib
+from email.header import Header
 from email.mime.application import MIMEApplication
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
-from email.utils import COMMASPACE, formatdate
+from email.utils import COMMASPACE, formataddr, formatdate, parseaddr
+from pathlib import Path
 
 import aiosmtplib
 
 __all__ = ['Email', 'AioEmail']
 
 
 class EmailBase:
@@ -24,87 +27,81 @@
         self.smtp = smtp or os.environ.get('EMAIL_SMTP')
         self.user = user or os.environ.get('EMAIL_USER')
         self.pwd = pwd or os.environ.get('EMAIL_PWD')
         self.use_tls = use_tls or os.environ.get('EMAIL_TLS')
         if isinstance(self.use_tls, str):
             self.use_tls = self.use_tls.lower() == 'true'
 
+    @staticmethod
+    def _format_addr(s):
+        # format: username<email address>
+        name, addr = parseaddr(s)
+        return formataddr((Header(name, 'utf-8').encode(), addr)) if name else addr
+
     def pack(self, receivers, title=None, content=None, files=None, cc=None):
         msg = MIMEMultipart()
         msg.set_charset('utf8')
 
         if content:
             mime = MIMEText(content, 'html', 'utf-8')
             msg.attach(mime)
 
         if files:
-            if isinstance(files, (str, bytes)):
+            if not isinstance(files, (list, tuple)):
                 files = [files]
             for i, fname in enumerate(files):
-                '''
-                _type, _ = mimetypes.guess_type(fname)
-                if _type:
-                    _type = _type.split('/')
-                    att = MIMEBase(_type[0], _type[1], filename=fname)
-                else:
-                    att = MIMEBase('application', 'octet-stream')
-                with open(fname, 'rb') as fp:
-                    att.set_payload(fp.read())
-                encoders.encode_base64(att)
-                att['Content-ID'] = str(i)
-                att["Content-Disposition"] = f'attachment; filename="{ os.path.basename(fname) }"'
-                '''
-                att = MIMEApplication(open(fname, 'rb').read())
+                fpath = Path(fname)
+                att = MIMEApplication(fpath.read_bytes())
                 # att.add_header('X-Attachment-Id', str(i))
                 att.add_header('Content-ID', str(i))
                 att.add_header('Content-Type', 'application/octet-stream')
-                att.add_header('Content-Disposition', 'attachment', filename=os.path.basename(fname))
+                att.add_header('Content-Disposition', 'attachment', filename=fpath.name)
                 msg.attach(att)
 
         if cc:
-            if not isinstance(cc, list):
+            if not isinstance(cc, (list, tuple)):
                 cc = [cc]
-            msg['cc'] = COMMASPACE.join(cc)
+            msg['cc'] = COMMASPACE.join([self._format_addr(c) for c in cc])
 
         msg['subject'] = title
         msg['date'] = formatdate(localtime=True)
-        msg['from'] = self.sender
-        if not isinstance(receivers, list):
+        sender = f'{self.sender}<{self.user}>' if self.sender else self.user
+        msg['from'] = self._format_addr(sender)
+        if not isinstance(receivers, (list, tuple)):
             receivers = [receivers]
-        msg['to'] = COMMASPACE.join(receivers)
+        msg['to'] = COMMASPACE.join([self._format_addr(r) for r in receivers])
         return msg
 
 
 class Email(EmailBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if self.use_tls:
             self.client = smtplib.SMTP_SSL(self.smtp, 465)
         else:
             self.client = smtplib.SMTP(self.smtp)
         # self.client = smtplib.SMTP('localhost')
-        # self.sender = self.client.local_hostname
 
     def send(self, *args, **kwargs):
         msg = self.pack(*args, **kwargs)
-        self.client.docmd('ehlo', self.smtp)
+        self.client.connect(self.smtp)
+        self.client.ehlo()
         self.client.login(self.user, self.pwd)
         self.client.send_message(msg)
         self.client.quit()
 
 
 class AioEmail(EmailBase):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         kwargs = {'port': 465, 'use_tls': True} if self.use_tls else {}
         self.client = aiosmtplib.SMTP(hostname=self.smtp, **kwargs)
         # self.client = smtplib.SMTP('localhost')
-        # self.sender = self.client.hostname
 
     async def send(self, *args, **kwargs):
         msg = self.pack(*args, **kwargs)
         await self.client.connect()
         await self.client.login(self.user, self.pwd)
         await self.client.send_message(msg)
         await self.client.quit()
```

### Comparing `kkutils-1.6.4/utils/fire.py` & `kkutils-1.6.5/utils/fire.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/http_utils.py` & `kkutils-1.6.5/utils/http_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 import random
 import re
 import socket
 import string
 import threading
 import time
 import urllib.parse
-import uuid
 import zlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial, reduce
 from http.cookiejar import MozillaCookieJar
 from http.cookies import SimpleCookie
 from pathlib import Path
 from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
 
 import aiohttp
 import chardet
 import requests
 from bs4 import BeautifulSoup
 from lxml import etree
+from requests.models import RequestEncodingMixin
 from requests.structures import CaseInsensitiveDict
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 from tornado import httputil
 from tornado.httpclient import HTTPClient, HTTPRequest, HTTPResponse
 
-from .base_utils import Dict, DictWrapper, to_bytes, to_str, tqdm
+from .base_utils import Dict, DictWrapper, to_str, tqdm
 from .cached_property import cached_property
 
 logging.getLogger("requests").setLevel(logging.WARNING)
 
 
 def patch_connection_pool(num_pools=100, maxsize=100):
     from urllib3 import connectionpool, poolmanager
@@ -395,14 +395,18 @@
         return self.request(url, method='options', **kwargs)
 
     def patch(self, url, **kwargs):
         return self.request(url, method='patch', **kwargs)
 
     @staticmethod
     def multipart(headers={}, data={}, files={}):
+        body, content_type = RequestEncodingMixin._encode_files(files, data)
+        headers['Content-Type'] = content_type
+        return body
+        '''
         boundary = uuid.uuid4().hex
         headers['Content-Type'] = 'multipart/form-data; boundary=%s' % boundary
         boundary_bytes = boundary.encode()
         if isinstance(data, dict):
             data = data.items()
         if isinstance(files, dict):
             files = files.items()
@@ -420,14 +424,15 @@
             lines.append(b'Content-Type: %s\r\n' % to_bytes(value[2]))
             value[1].seek(0)
             lines.append(value[1].read())
 
         lines.append(b'--%s--' % boundary_bytes)
         body = b'\r\n'.join(lines)
         return body
+        '''
 
 
 class AsyncRequest(BaseRequest):
 
     async def _retry(self, url, kwargs, retry):
         reason = 'OK'
         for i in range(retry + 1):
```

### Comparing `kkutils-1.6.4/utils/log_utils.py` & `kkutils-1.6.5/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/rabbitmq.py` & `kkutils-1.6.5/utils/rabbitmq.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 logging.getLogger('pika').setLevel(logging.ERROR)
 
 __all__ = ['Pika', 'AioPika']
 
 
 class Pika:
 
-    def __init__(self, queue='test', **kwargs):
+    def __init__(self, queue, **kwargs):
         if any([key in kwargs for key in ['host', 'port', 'user', 'pwd', 'vhost']]):
             host = kwargs.pop('host', 'localhost')
             port = kwargs.pop('port', 5672)
             user = kwargs.pop('user', 'guest')
             pwd = kwargs.pop('pwd', 'guest')
             vhost = kwargs.pop('vhost', '/')
             self.uri = f'amqp://{user}:{pwd}@{host}:{port}{vhost}'
@@ -112,15 +112,15 @@
                 channel.close()
         if self._connection is not None and not self._connection.is_closed:
             self._connection.close()
 
 
 class AioPika(Pika):
 
-    def __init__(self, queue='test', workers=1, **kwargs):
+    def __init__(self, queue, workers=1, **kwargs):
         super().__init__(queue, **kwargs)
         self.workers = workers
         self.loop = asyncio.get_event_loop()
         self.lock = asyncio.Lock()
 
     async def connect(self):
         async with self.lock:
```

### Comparing `kkutils-1.6.4/utils/stopwatch.py` & `kkutils-1.6.5/utils/stopwatch.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.4/utils/xdb_searcher.py` & `kkutils-1.6.5/utils/xdb_searcher.py`

 * *Files identical despite different names*

