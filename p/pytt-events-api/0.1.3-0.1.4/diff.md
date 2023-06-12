# Comparing `tmp/pytt_events_api-0.1.3.tar.gz` & `tmp/pytt_events_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytt_events_api-0.1.3.tar", last modified: Fri Jun  9 20:37:37 2023, max compression
+gzip compressed data, was "pytt_events_api-0.1.4.tar", last modified: Mon Jun 12 17:43:25 2023, max compression
```

## Comparing `pytt_events_api-0.1.3.tar` & `pytt_events_api-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.370321 pytt_events_api-0.1.3/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-01-28 12:24:47.000000 pytt_events_api-0.1.3/LICENSE
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-09 20:37:37.367320 pytt_events_api-0.1.3/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4017 2023-03-20 23:22:20.000000 pytt_events_api-0.1.3/README.md
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.090321 pytt_events_api-0.1.3/pytt_events/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:36:58.000000 pytt_events_api-0.1.3/pytt_events/__init__.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)      486 2023-06-09 18:59:59.000000 pytt_events_api-0.1.3/pytt_events/auth.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     2767 2023-06-09 20:35:54.000000 pytt_events_api-0.1.3/pytt_events/context.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1974 2023-06-09 20:35:54.000000 pytt_events_api-0.1.3/pytt_events/event.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1037 2023-06-09 19:25:47.000000 pytt_events_api-0.1.3/pytt_events/properties.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1457 2023-01-30 20:47:04.000000 pytt_events_api-0.1.3/pytt_events/supported_events.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.215321 pytt_events_api-0.1.3/pytt_events/tests/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:54:54.000000 pytt_events_api-0.1.3/pytt_events/tests/__init__.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     3071 2023-06-09 20:10:55.000000 pytt_events_api-0.1.3/pytt_events/tests/conftest.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4533 2023-06-09 20:15:56.000000 pytt_events_api-0.1.3/pytt_events/tests/test_event.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)      882 2023-02-01 07:33:30.000000 pytt_events_api-0.1.3/pytt_events/tests/test_tiktok_post_events.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     2886 2023-06-09 18:57:19.000000 pytt_events_api-0.1.3/pytt_events/tiktok_events_api.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-09 20:37:37.340320 pytt_events_api-0.1.3/pytt_events_api.egg-info/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)      536 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       81 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/requires.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       12 2023-06-09 20:37:36.000000 pytt_events_api-0.1.3/pytt_events_api.egg-info/top_level.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-06-09 20:37:37.371322 pytt_events_api-0.1.3/setup.cfg
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1522 2023-06-09 20:36:52.000000 pytt_events_api-0.1.3/setup.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.867176 pytt_events_api-0.1.4/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-01-28 12:24:47.000000 pytt_events_api-0.1.4/LICENSE
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-12 17:43:25.864175 pytt_events_api-0.1.4/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4017 2023-03-20 23:22:20.000000 pytt_events_api-0.1.4/README.md
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.630191 pytt_events_api-0.1.4/pytt_events/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:36:58.000000 pytt_events_api-0.1.4/pytt_events/__init__.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      486 2023-06-09 18:59:59.000000 pytt_events_api-0.1.4/pytt_events/auth.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     2767 2023-06-09 20:35:54.000000 pytt_events_api-0.1.4/pytt_events/context.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1974 2023-06-09 20:35:54.000000 pytt_events_api-0.1.4/pytt_events/event.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-06-12 17:35:51.000000 pytt_events_api-0.1.4/pytt_events/properties.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1509 2023-06-12 17:41:36.000000 pytt_events_api-0.1.4/pytt_events/supported_events.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.736176 pytt_events_api-0.1.4/pytt_events/tests/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:54:54.000000 pytt_events_api-0.1.4/pytt_events/tests/__init__.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     3071 2023-06-09 20:10:55.000000 pytt_events_api-0.1.4/pytt_events/tests/conftest.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4533 2023-06-09 20:15:56.000000 pytt_events_api-0.1.4/pytt_events/tests/test_event.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      882 2023-02-01 07:33:30.000000 pytt_events_api-0.1.4/pytt_events/tests/test_tiktok_post_events.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     2886 2023-06-09 18:57:19.000000 pytt_events_api-0.1.4/pytt_events/tiktok_events_api.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.839174 pytt_events_api-0.1.4/pytt_events_api.egg-info/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      536 2023-06-12 17:43:25.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       81 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/requires.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       12 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/top_level.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-06-12 17:43:25.868175 pytt_events_api-0.1.4/setup.cfg
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1522 2023-06-12 17:41:36.000000 pytt_events_api-0.1.4/setup.py
```

### Comparing `pytt_events_api-0.1.3/LICENSE` & `pytt_events_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/PKG-INFO` & `pytt_events_api-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytt_events_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python wrapper for the TikTok Events API
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,tiktok,events,api,tiktok ads,tiktok events api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytt_events_api-0.1.3/README.md` & `pytt_events_api-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/pytt_events/context.py` & `pytt_events_api-0.1.4/pytt_events/context.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/pytt_events/event.py` & `pytt_events_api-0.1.4/pytt_events/event.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/pytt_events/properties.py` & `pytt_events_api-0.1.4/pytt_events/properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     """
     PRODUCT = 'product'
     """
     For product groups (Items and variants).
     """
     PRODUCT_GROUP = 'product_group'
 
+    def __str__(self):
+        return self.value
+
 class Content(BaseModel):
     content_id: constr(strip_whitespace=True, min_length=1)
     quantity: PositiveInt
     price: PositiveFloat
     content_category: constr(min_length=1)
     content_name: constr(min_length=1)
```

### Comparing `pytt_events_api-0.1.3/pytt_events/supported_events.py` & `pytt_events_api-0.1.4/pytt_events/supported_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """
     When a search is made.
     """
     SEARCH = 'Search'
     """
     When an item is added to a wishlist.
     """
-    ADD_TO_WHISHLIST = 'AddToWishlist'
+    ADD_TO_WISHLIST = 'AddToWishlist'
     """
     When an item is added to the shopping cart.
     """
     ADD_TO_CART = 'AddToCart'
     """
     When the checkout process is started.
     """
@@ -55,8 +55,11 @@
     """
     When a registration is completed.
     """
     COMPLETE_REGISTRATION = 'CompleteRegistration'
     """
     When a subscription is made.
     """
-    SUBSCRIBE = 'Subscribe'
+    SUBSCRIBE = 'Subscribe'
+
+    def __str__(self):
+        return self.value
```

### Comparing `pytt_events_api-0.1.3/pytt_events/tests/conftest.py` & `pytt_events_api-0.1.4/pytt_events/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/pytt_events/tests/test_event.py` & `pytt_events_api-0.1.4/pytt_events/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/pytt_events/tests/test_tiktok_post_events.py` & `pytt_events_api-0.1.4/pytt_events/tests/test_tiktok_post_events.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/pytt_events/tiktok_events_api.py` & `pytt_events_api-0.1.4/pytt_events/tiktok_events_api.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/pytt_events_api.egg-info/PKG-INFO` & `pytt_events_api-0.1.4/pytt_events_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytt-events-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python wrapper for the TikTok Events API
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,tiktok,events,api,tiktok ads,tiktok events api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytt_events_api-0.1.3/pytt_events_api.egg-info/SOURCES.txt` & `pytt_events_api-0.1.4/pytt_events_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.3/setup.py` & `pytt_events_api-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 with open(requirements_filename) as f:
     # INSTALL_REQUIRES = [str(line[:-1]) for line in f]
     INSTALL_REQUIRES = ['requests', 'pytest', 'pydantic', 'phonenumbers', 'email-validator', 'ipaddress', 'pydantic[dotenv]']
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Python wrapper for the TikTok Events API'
 LONG_DESCRIPTION = long_description
 PACKAGE_LICENSE = 'LICENSE.txt'
 
 # Setting up
 setup(
     name="pytt_events_api",
```

