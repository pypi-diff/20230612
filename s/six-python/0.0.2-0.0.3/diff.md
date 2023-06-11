# Comparing `tmp/six-python-0.0.2.tar.gz` & `tmp/six-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/six-python-0.0.2.tar", last modified: Sun Jun 11 22:41:36 2023, max compression
+gzip compressed data, was "dist/six-python-0.0.3.tar", last modified: Sun Jun 11 22:52:22 2023, max compression
```

## Comparing `six-python-0.0.2.tar` & `six-python-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:41:36.000000 six-python-0.0.2/
--rw-r--r--   0 mac        (501) staff       (20)      758 2023-06-11 22:41:36.000000 six-python-0.0.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       20 2023-06-09 19:50:05.000000 six-python-0.0.2/README.md
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-11 22:41:36.000000 six-python-0.0.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     2027 2023-06-11 22:41:26.000000 six-python-0.0.2/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python/
--rw-r--r--   0 mac        (501) staff       (20)       30 2023-06-11 22:37:24.000000 six-python-0.0.2/six_python/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python/middlewares/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 six-python-0.0.2/six_python/middlewares/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3738 2023-06-11 22:37:24.000000 six-python-0.0.2/six_python/middlewares/encryption_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 six-python-0.0.2/six_python/middlewares/six_base_http_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)     3986 2023-06-10 21:31:40.000000 six-python-0.0.2/six_python/middlewares/six_independent_rate_limiter.py
--rw-r--r--   0 mac        (501) staff       (20)     4104 2023-06-10 21:31:40.000000 six-python-0.0.2/six_python/middlewares/six_rate_limiter_middleware.py
--rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 six-python-0.0.2/six_python/schemas.py
--rw-r--r--   0 mac        (501) staff       (20)     3151 2023-06-11 22:37:24.000000 six-python-0.0.2/six_python/six.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 six-python-0.0.2/six_python/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4309 2023-06-10 10:44:01.000000 six-python-0.0.2/six_python/utils/encryption_utils.py
--rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 six-python-0.0.2/six_python/utils/time_utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      758 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      590 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      617 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2023-06-11 22:41:36.000000 six-python-0.0.2/six_python.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:52:22.000000 six-python-0.0.3/
+-rw-r--r--   0 mac        (501) staff       (20)      758 2023-06-11 22:52:22.000000 six-python-0.0.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)       20 2023-06-09 19:50:05.000000 six-python-0.0.3/README.md
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-11 22:52:22.000000 six-python-0.0.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     2013 2023-06-11 22:52:19.000000 six-python-0.0.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python/
+-rw-r--r--   0 mac        (501) staff       (20)       30 2023-06-11 22:37:24.000000 six-python-0.0.3/six_python/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python/middlewares/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:12:54.000000 six-python-0.0.3/six_python/middlewares/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3738 2023-06-11 22:37:24.000000 six-python-0.0.3/six_python/middlewares/encryption_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     5121 2023-06-10 17:10:19.000000 six-python-0.0.3/six_python/middlewares/six_base_http_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)     3986 2023-06-10 21:31:40.000000 six-python-0.0.3/six_python/middlewares/six_independent_rate_limiter.py
+-rw-r--r--   0 mac        (501) staff       (20)     4104 2023-06-10 21:31:40.000000 six-python-0.0.3/six_python/middlewares/six_rate_limiter_middleware.py
+-rw-r--r--   0 mac        (501) staff       (20)      624 2023-06-10 23:02:11.000000 six-python-0.0.3/six_python/schemas.py
+-rw-r--r--   0 mac        (501) staff       (20)     3151 2023-06-11 22:37:24.000000 six-python-0.0.3/six_python/six.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-10 23:13:17.000000 six-python-0.0.3/six_python/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     4309 2023-06-10 10:44:01.000000 six-python-0.0.3/six_python/utils/encryption_utils.py
+-rw-rw-r--   0 mac        (501) staff       (20)     1707 2023-06-09 19:33:11.000000 six-python-0.0.3/six_python/utils/time_utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      758 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      590 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      610 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2023-06-11 22:52:22.000000 six-python-0.0.3/six_python.egg-info/top_level.txt
```

### Comparing `six-python-0.0.2/PKG-INFO` & `six-python-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: six-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Six offical python ackage
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.
 Keywords: python,cybersecurity,pentesting,encryption,rate limiting,xss prevention
```

### Comparing `six-python-0.0.2/setup.py` & `six-python-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import setup, find_packages
 from pip._internal.req import parse_requirements
 
 
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Six offical python ackage'
 LONG_DESCRIPTION = 'Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.'
 
 # Setting up
 setup(
     name="six-python",
     version=VERSION,
     author="6thSense",
     author_email="tech@withsix.co",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=["anyio",
-    "bcrypt",
     "CacheControl",
     "cachetools",
     "certifi",
     "cffi",
     "charset-normalizer",
     "click",
     "crypto",
```

### Comparing `six-python-0.0.2/six_python/middlewares/encryption_middleware.py` & `six-python-0.0.3/six_python/middlewares/encryption_middleware.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python/middlewares/six_base_http_middleware.py` & `six-python-0.0.3/six_python/middlewares/six_base_http_middleware.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python/middlewares/six_independent_rate_limiter.py` & `six-python-0.0.3/six_python/middlewares/six_independent_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python/middlewares/six_rate_limiter_middleware.py` & `six-python-0.0.3/six_python/middlewares/six_rate_limiter_middleware.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python/schemas.py` & `six-python-0.0.3/six_python/schemas.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python/six.py` & `six-python-0.0.3/six_python/six.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python/utils/encryption_utils.py` & `six-python-0.0.3/six_python/utils/encryption_utils.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python/utils/time_utils.py` & `six-python-0.0.3/six_python/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python.egg-info/PKG-INFO` & `six-python-0.0.3/six_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: six-python
-Version: 0.0.2
+Version: 0.0.3
 Summary: Six offical python ackage
 Home-page: UNKNOWN
 Author: 6thSense
 Author-email: tech@withsix.co
 License: UNKNOWN
 Description: Six is a package that helps you automate pen testing and also helps you protect your API from cybersecurity threats. Visit https://withsix.co to get started.
 Keywords: python,cybersecurity,pentesting,encryption,rate limiting,xss prevention
```

### Comparing `six-python-0.0.2/six_python.egg-info/SOURCES.txt` & `six-python-0.0.3/six_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `six-python-0.0.2/six_python.egg-info/requires.txt` & `six-python-0.0.3/six_python.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 anyio
-bcrypt
 CacheControl
 cachetools
 certifi
 cffi
 charset-normalizer
 click
 crypto
```

