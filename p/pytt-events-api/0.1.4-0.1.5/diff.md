# Comparing `tmp/pytt_events_api-0.1.4.tar.gz` & `tmp/pytt_events_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytt_events_api-0.1.4.tar", last modified: Mon Jun 12 17:43:25 2023, max compression
+gzip compressed data, was "pytt_events_api-0.1.5.tar", last modified: Mon Jun 12 18:42:17 2023, max compression
```

## Comparing `pytt_events_api-0.1.4.tar` & `pytt_events_api-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.867176 pytt_events_api-0.1.4/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-01-28 12:24:47.000000 pytt_events_api-0.1.4/LICENSE
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-12 17:43:25.864175 pytt_events_api-0.1.4/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4017 2023-03-20 23:22:20.000000 pytt_events_api-0.1.4/README.md
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.630191 pytt_events_api-0.1.4/pytt_events/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:36:58.000000 pytt_events_api-0.1.4/pytt_events/__init__.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)      486 2023-06-09 18:59:59.000000 pytt_events_api-0.1.4/pytt_events/auth.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     2767 2023-06-09 20:35:54.000000 pytt_events_api-0.1.4/pytt_events/context.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1974 2023-06-09 20:35:54.000000 pytt_events_api-0.1.4/pytt_events/event.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-06-12 17:35:51.000000 pytt_events_api-0.1.4/pytt_events/properties.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1509 2023-06-12 17:41:36.000000 pytt_events_api-0.1.4/pytt_events/supported_events.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.736176 pytt_events_api-0.1.4/pytt_events/tests/
--rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:54:54.000000 pytt_events_api-0.1.4/pytt_events/tests/__init__.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     3071 2023-06-09 20:10:55.000000 pytt_events_api-0.1.4/pytt_events/tests/conftest.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4533 2023-06-09 20:15:56.000000 pytt_events_api-0.1.4/pytt_events/tests/test_event.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)      882 2023-02-01 07:33:30.000000 pytt_events_api-0.1.4/pytt_events/tests/test_tiktok_post_events.py
--rwxrwxrwx   0 valar     (1000) valar     (1000)     2886 2023-06-09 18:57:19.000000 pytt_events_api-0.1.4/pytt_events/tiktok_events_api.py
-drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 17:43:25.839174 pytt_events_api-0.1.4/pytt_events_api.egg-info/
--rwxrwxrwx   0 valar     (1000) valar     (1000)     4607 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/PKG-INFO
--rwxrwxrwx   0 valar     (1000) valar     (1000)      536 2023-06-12 17:43:25.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       81 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/requires.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       12 2023-06-12 17:43:24.000000 pytt_events_api-0.1.4/pytt_events_api.egg-info/top_level.txt
--rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-06-12 17:43:25.868175 pytt_events_api-0.1.4/setup.cfg
--rwxrwxrwx   0 valar     (1000) valar     (1000)     1522 2023-06-12 17:41:36.000000 pytt_events_api-0.1.4/setup.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 18:42:17.592899 pytt_events_api-0.1.5/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-01-28 12:24:47.000000 pytt_events_api-0.1.5/LICENSE
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4848 2023-06-12 18:42:17.589900 pytt_events_api-0.1.5/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4258 2023-06-12 18:02:36.000000 pytt_events_api-0.1.5/README.md
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 18:42:17.305900 pytt_events_api-0.1.5/pytt_events/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:36:58.000000 pytt_events_api-0.1.5/pytt_events/__init__.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      486 2023-06-09 18:59:59.000000 pytt_events_api-0.1.5/pytt_events/auth.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     2767 2023-06-09 20:35:54.000000 pytt_events_api-0.1.5/pytt_events/context.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1974 2023-06-09 20:35:54.000000 pytt_events_api-0.1.5/pytt_events/event.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1090 2023-06-12 17:58:32.000000 pytt_events_api-0.1.5/pytt_events/properties.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1509 2023-06-12 17:41:36.000000 pytt_events_api-0.1.5/pytt_events/supported_events.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 18:42:17.435900 pytt_events_api-0.1.5/pytt_events/tests/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-01-28 17:54:54.000000 pytt_events_api-0.1.5/pytt_events/tests/__init__.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     3071 2023-06-09 20:10:55.000000 pytt_events_api-0.1.5/pytt_events/tests/conftest.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4533 2023-06-09 20:15:56.000000 pytt_events_api-0.1.5/pytt_events/tests/test_event.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      882 2023-02-01 07:33:30.000000 pytt_events_api-0.1.5/pytt_events/tests/test_tiktok_post_events.py
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     2886 2023-06-09 18:57:19.000000 pytt_events_api-0.1.5/pytt_events/tiktok_events_api.py
+drwxrwxrwx   0 valar     (1000) valar     (1000)        0 2023-06-12 18:42:17.562900 pytt_events_api-0.1.5/pytt_events_api.egg-info/
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     4848 2023-06-12 18:42:16.000000 pytt_events_api-0.1.5/pytt_events_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 valar     (1000) valar     (1000)      536 2023-06-12 18:42:16.000000 pytt_events_api-0.1.5/pytt_events_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)        1 2023-06-12 18:42:16.000000 pytt_events_api-0.1.5/pytt_events_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       81 2023-06-12 18:42:16.000000 pytt_events_api-0.1.5/pytt_events_api.egg-info/requires.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       12 2023-06-12 18:42:16.000000 pytt_events_api-0.1.5/pytt_events_api.egg-info/top_level.txt
+-rwxrwxrwx   0 valar     (1000) valar     (1000)       38 2023-06-12 18:42:17.593901 pytt_events_api-0.1.5/setup.cfg
+-rwxrwxrwx   0 valar     (1000) valar     (1000)     1522 2023-06-12 18:03:47.000000 pytt_events_api-0.1.5/setup.py
```

### Comparing `pytt_events_api-0.1.4/LICENSE` & `pytt_events_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/PKG-INFO` & `pytt_events_api-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytt_events_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python wrapper for the TikTok Events API
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,tiktok,events,api,tiktok ads,tiktok events api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -102,14 +102,17 @@
     event_id='123456789',
     timestamp='2023-02-01T00:00:00-03:00', # str or datetime object
     context=context,
     properties=properties
 )
 ```
 
+#### Errors in the Docs
+[TikTok's documentation](https://ads.tiktok.com/marketing_api/docs?id=1741601162187777) says that content_type should be a parameter of the Properties object, but it actually is a parameter of the Content object.
+
 ### Sending an event
 ``` python
 response = api.post_event(
     event=event,
     auth=auth
 )
 ```
```

### Comparing `pytt_events_api-0.1.4/README.md` & `pytt_events_api-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
     event_id='123456789',
     timestamp='2023-02-01T00:00:00-03:00', # str or datetime object
     context=context,
     properties=properties
 )
 ```
 
+#### Errors in the Docs
+[TikTok's documentation](https://ads.tiktok.com/marketing_api/docs?id=1741601162187777) says that content_type should be a parameter of the Properties object, but it actually is a parameter of the Content object.
+
 ### Sending an event
 ``` python
 response = api.post_event(
     event=event,
     auth=auth
 )
 ```
```

### Comparing `pytt_events_api-0.1.4/pytt_events/context.py` & `pytt_events_api-0.1.5/pytt_events/context.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/pytt_events/event.py` & `pytt_events_api-0.1.5/pytt_events/event.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/pytt_events/properties.py` & `pytt_events_api-0.1.5/pytt_events/properties.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
 class Content(BaseModel):
     content_id: constr(strip_whitespace=True, min_length=1)
     quantity: PositiveInt
     price: PositiveFloat
     content_category: constr(min_length=1)
     content_name: constr(min_length=1)
+    content_type: ContentType
 
 class Properties(BaseModel):
     currency: Optional[constr(strip_whitespace=True, min_length=3, max_length=3)]
     value: Optional[PositiveFloat]
-    content_type: ContentType
     description: Optional[constr(min_length=1)]
     query: Optional[constr(min_length=1)]
     status: Optional[constr(min_length=1)]
     contents: Optional[conlist(
         item_type=Content, unique_items=True, min_items=1
     )]
```

### Comparing `pytt_events_api-0.1.4/pytt_events/supported_events.py` & `pytt_events_api-0.1.5/pytt_events/supported_events.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/pytt_events/tests/conftest.py` & `pytt_events_api-0.1.5/pytt_events/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/pytt_events/tests/test_event.py` & `pytt_events_api-0.1.5/pytt_events/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/pytt_events/tests/test_tiktok_post_events.py` & `pytt_events_api-0.1.5/pytt_events/tests/test_tiktok_post_events.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/pytt_events/tiktok_events_api.py` & `pytt_events_api-0.1.5/pytt_events/tiktok_events_api.py`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/pytt_events_api.egg-info/PKG-INFO` & `pytt_events_api-0.1.5/pytt_events_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytt-events-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python wrapper for the TikTok Events API
 Author: Victor Valar
 Author-email: <valar@victorvalar.me>
 License: LICENSE.txt
 Keywords: python,tiktok,events,api,tiktok ads,tiktok events api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -102,14 +102,17 @@
     event_id='123456789',
     timestamp='2023-02-01T00:00:00-03:00', # str or datetime object
     context=context,
     properties=properties
 )
 ```
 
+#### Errors in the Docs
+[TikTok's documentation](https://ads.tiktok.com/marketing_api/docs?id=1741601162187777) says that content_type should be a parameter of the Properties object, but it actually is a parameter of the Content object.
+
 ### Sending an event
 ``` python
 response = api.post_event(
     event=event,
     auth=auth
 )
 ```
```

### Comparing `pytt_events_api-0.1.4/pytt_events_api.egg-info/SOURCES.txt` & `pytt_events_api-0.1.5/pytt_events_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytt_events_api-0.1.4/setup.py` & `pytt_events_api-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 with open(requirements_filename) as f:
     # INSTALL_REQUIRES = [str(line[:-1]) for line in f]
     INSTALL_REQUIRES = ['requests', 'pytest', 'pydantic', 'phonenumbers', 'email-validator', 'ipaddress', 'pydantic[dotenv]']
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Python wrapper for the TikTok Events API'
 LONG_DESCRIPTION = long_description
 PACKAGE_LICENSE = 'LICENSE.txt'
 
 # Setting up
 setup(
     name="pytt_events_api",
```

