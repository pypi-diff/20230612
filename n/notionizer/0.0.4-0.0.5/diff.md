# Comparing `tmp/notionizer-0.0.4.tar.gz` & `tmp/notionizer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notionizer-0.0.4.tar", last modified: Tue Apr 18 09:33:34 2023, max compression
+gzip compressed data, was "notionizer-0.0.5.tar", last modified: Sun Jun 11 23:57:40 2023, max compression
```

## Comparing `notionizer-0.0.4.tar` & `notionizer-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.236627 notionizer-0.0.4/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-04-18 09:33:34.236627 notionizer-0.0.4/PKG-INFO
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      368 2022-06-22 11:05:47.000000 notionizer-0.0.4/README.md
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.232627 notionizer-0.0.4/notionizer/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      732 2023-02-17 11:30:57.000000 notionizer-0.0.4/notionizer/__init__.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2153 2023-02-09 05:51:58.000000 notionizer-0.0.4/notionizer/enum.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      316 2023-02-20 04:58:37.000000 notionizer-0.0.4/notionizer/exception.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1780 2023-02-21 08:17:05.000000 notionizer-0.0.4/notionizer/functions.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2535 2023-02-27 08:37:50.000000 notionizer-0.0.4/notionizer/http_request.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3977 2023-02-27 08:22:48.000000 notionizer-0.0.4/notionizer/notion.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     9289 2023-02-15 01:34:21.000000 notionizer-0.0.4/notionizer/object_adt.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     7170 2023-02-17 07:10:08.000000 notionizer-0.0.4/notionizer/object_basic.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2380 2023-02-27 08:22:48.000000 notionizer-0.0.4/notionizer/object_block.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    16955 2023-02-21 09:11:19.000000 notionizer-0.0.4/notionizer/object_database.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4950 2023-02-20 05:16:22.000000 notionizer-0.0.4/notionizer/object_page.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1587 2023-02-13 07:50:42.000000 notionizer-0.0.4/notionizer/object_user.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     6254 2023-02-22 07:23:08.000000 notionizer-0.0.4/notionizer/properties_basic.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3950 2023-02-21 10:19:28.000000 notionizer-0.0.4/notionizer/properties_db.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4924 2023-02-22 07:21:57.000000 notionizer-0.0.4/notionizer/properties_page.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4513 2023-02-21 08:37:01.000000 notionizer-0.0.4/notionizer/properties_property.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    42566 2023-02-21 09:16:09.000000 notionizer-0.0.4/notionizer/query.py
--rw-r--r--   0 sungyo    (1000) sungyo    (1000)      126 2023-02-27 08:38:48.000000 notionizer-0.0.4/notionizer/settings.py
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.236627 notionizer-0.0.4/notionizer.egg-info/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/PKG-INFO
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      855 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/SOURCES.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        1 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/dependency_links.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        9 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/requires.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       16 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/top_level.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       38 2023-04-18 09:33:34.236627 notionizer-0.0.4/setup.cfg
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      993 2023-04-18 09:33:03.000000 notionizer-0.0.4/setup.py
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.236627 notionizer-0.0.4/test/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        0 2022-06-14 09:15:51.000000 notionizer-0.0.4/test/__init__.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1986 2023-02-21 05:40:06.000000 notionizer-0.0.4/test/test_block.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      638 2023-02-21 12:44:32.000000 notionizer-0.0.4/test/test_notion.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4912 2023-02-09 07:32:20.000000 notionizer-0.0.4/test/test_notion1.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      398 2023-02-21 12:44:32.000000 notionizer-0.0.4/test/test_notion_getdatabase.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2647 2023-02-21 07:46:13.000000 notionizer-0.0.4/test/test_object_database.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2596 2023-02-27 08:22:48.000000 notionizer-0.0.4/test/test_object_page.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      169 2023-02-15 02:03:42.000000 notionizer-0.0.4/test/test_objects.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    14244 2023-02-13 05:30:10.000000 notionizer-0.0.4/test/test_query.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-06-11 23:57:40.371324 notionizer-0.0.5/PKG-INFO
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      368 2022-06-22 11:05:47.000000 notionizer-0.0.5/README.md
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/notionizer/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      732 2023-02-17 11:30:57.000000 notionizer-0.0.5/notionizer/__init__.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2153 2023-02-09 05:51:58.000000 notionizer-0.0.5/notionizer/enum.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      371 2023-05-16 10:10:19.000000 notionizer-0.0.5/notionizer/exception.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1799 2023-05-22 15:08:10.000000 notionizer-0.0.5/notionizer/functions.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3901 2023-05-22 22:50:26.000000 notionizer-0.0.5/notionizer/http_request.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4034 2023-05-15 08:29:49.000000 notionizer-0.0.5/notionizer/notion.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     9289 2023-02-15 01:34:21.000000 notionizer-0.0.5/notionizer/object_adt.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     7654 2023-05-22 10:04:46.000000 notionizer-0.0.5/notionizer/object_basic.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2380 2023-02-27 08:22:48.000000 notionizer-0.0.5/notionizer/object_block.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    17656 2023-05-22 21:42:21.000000 notionizer-0.0.5/notionizer/object_database.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     5048 2023-05-24 03:33:53.000000 notionizer-0.0.5/notionizer/object_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1643 2023-05-24 03:34:20.000000 notionizer-0.0.5/notionizer/object_user.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     6805 2023-05-22 23:24:23.000000 notionizer-0.0.5/notionizer/properties_basic.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4155 2023-05-22 11:31:36.000000 notionizer-0.0.5/notionizer/properties_db.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     5144 2023-05-22 23:23:28.000000 notionizer-0.0.5/notionizer/properties_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4530 2023-05-22 09:59:24.000000 notionizer-0.0.5/notionizer/properties_property.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    42595 2023-04-24 07:29:16.000000 notionizer-0.0.5/notionizer/query.py
+-rw-r--r--   0 sungyo    (1000) sungyo    (1000)      126 2023-02-27 08:38:48.000000 notionizer-0.0.5/notionizer/settings.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/notionizer.egg-info/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/PKG-INFO
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      855 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        1 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        9 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/requires.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       16 2023-06-11 23:57:40.000000 notionizer-0.0.5/notionizer.egg-info/top_level.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       38 2023-06-11 23:57:40.371324 notionizer-0.0.5/setup.cfg
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      993 2023-06-11 23:57:32.000000 notionizer-0.0.5/setup.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-06-11 23:57:40.371324 notionizer-0.0.5/test/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        0 2022-06-14 09:15:51.000000 notionizer-0.0.5/test/__init__.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1986 2023-02-21 05:40:06.000000 notionizer-0.0.5/test/test_block.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      639 2023-04-21 11:11:36.000000 notionizer-0.0.5/test/test_notion.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4912 2023-02-09 07:32:20.000000 notionizer-0.0.5/test/test_notion1.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      398 2023-02-21 12:44:32.000000 notionizer-0.0.5/test/test_notion_getdatabase.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2647 2023-02-21 07:46:13.000000 notionizer-0.0.5/test/test_object_database.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2596 2023-02-27 08:22:48.000000 notionizer-0.0.5/test/test_object_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      169 2023-02-15 02:03:42.000000 notionizer-0.0.5/test/test_objects.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    14244 2023-02-13 05:30:10.000000 notionizer-0.0.5/test/test_query.py
```

### Comparing `notionizer-0.0.4/PKG-INFO` & `notionizer-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionizer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python wrapper for Notion API
 Home-page: https://github.com/kimsg1984/notionizer
 Author: SeonGyo Kim
 Author-email: kimsg1984@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `notionizer-0.0.4/notionizer/__init__.py` & `notionizer-0.0.5/notionizer/__init__.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/notionizer/enum.py` & `notionizer-0.0.5/notionizer/enum.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/notionizer/functions.py` & `notionizer-0.0.5/notionizer/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     attr_list = dir(obj)
     if level == 'hide':
         attr_list = [a for a in attr_list if a[:2] != '__']
     elif level == 'public':
         attr_list = [a for a in attr_list if a[0] != '_']
     return attr_list
 
-
 def from_rich_text_array_to_plain_text(array: List[Dict[str, Any]]) -> str:
-    return ' '.join([e['plain_text'].replace(u'\xa0', u' ') for e in array])
+    result = ' '.join([e['plain_text'].replace(u'\xa0', u' ') for e in array])
+    return result
 
 
 def parse_date_object(date_obj: Dict[str, Any]) -> str:
     """
     parse date object to string format.
 
     :param date_obj:
```

### Comparing `notionizer-0.0.4/notionizer/http_request.py` & `notionizer-0.0.5/notionizer/http_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 """
 HTTP REQUEST
 
 managing request
 
 """
+import time
 
 import requests  # type: ignore
 import json
 import logging
 
 from notionizer import settings
 
 from typing import Dict, Any, Tuple, TypeVar
 
 _logger = logging.getLogger(__name__)
 
 
 class HttpRequestError(Exception):
-    pass
+    def __init__(self, status, code, message, header, payload, request_url):
+        self.status = status
+        self.code = code
+        self.message = message
+        self.header = header
+        self.payload = payload
+        self.request_url = request_url
+        super().__init__(f'[{status}] {code}: {message}, header: {header} body: {payload} from: {request_url}')
 
 
 T_HttpRequest = TypeVar('T_HttpRequest', bound='HttpRequest')
 
 
 class HttpRequest:
 
-    def __init__(self, secret_key: str, timeout: int = 15):
+    def __init__(self, secret_key: str, timeout: int = 15, time_out_try=3, time_out_wait=30):
         self.base_url = settings.BASE_URL
         self.__headers = {
             'Authorization': 'Bearer ' + secret_key,
             'Content-Type': 'application/json',
             'Notion-Version': settings.NOTION_VERSION
         }
         self.timeout = timeout
+        self.time_out_try = time_out_try
+        self.time_out_wait = time_out_wait
+
 
     def post(self: T_HttpRequest, url: str, payload: Dict[str, Any]) -> Tuple[T_HttpRequest, Dict[str, Any]]:
         return self._request('POST', url, payload)
 
     def get(self: T_HttpRequest, url: str) -> Tuple[T_HttpRequest, Dict[str, Any]]:
         return self._request('GET', url, {})
 
@@ -51,25 +62,46 @@
         """
 
         :param request_type: 'POST' or 'GET'
         :param url: fully assembled url
         :param payload:
         :return: python data type object(dictionay and list)
         """
-        _logger.debug( f'[{request_type}] url[{self.base_url + url}] payload: {payload}')
+        _logger.debug(f'[{request_type}] url[{self.base_url + url}] payload: {payload}')
         # _logger.debug('payload:' + str(payload))
         payload_json = ''
         if payload:
             payload_json = json.dumps(payload)
         request_url: str = self.base_url + url
-        result_json: str = requests.request(request_type, request_url, headers=self.__headers,
+        for i in range(self.time_out_try):
+            try:
+                result_json: str = requests.request(request_type, request_url, headers=self.__headers,
                                             data=payload_json, timeout=self.timeout).text
 
-        result: Dict[str, Any] = json.loads(result_json)
-        _logger.debug(f"result: {result}")
-        if result['object'] == 'error':
-            status = result['status']
-            code = result['code']
-            message = result['message']
-            raise HttpRequestError(f'[{status}] {code}: {message}, header: {self.__headers} body: {payload} from: {request_url}')
+                result: Dict[str, Any] = json.loads(result_json)
+                _logger.debug(f"result: {result}")
+                if result['object'] == 'error':
+                    status = result['status']
+                    code = result['code']
+                    message = result['message']
+                    raise HttpRequestError(status, code, message, self.__headers, payload, request_url)
+                break
+            except requests.exceptions.ReadTimeout as e:
+                if i + 1 == self.time_out_try:
+                    raise e
+                _logger.info(f'time out:{i}')
+                time.sleep(self.time_out_wait)
+            except json.decoder.JSONDecodeError as e:
+                if i + 1 == self.time_out_try:
+                    raise e
+                _logger.info(f'time out:{i}')
+                time.sleep(self.time_out_wait)
+            except HttpRequestError as e:
+                if e.status == 500:
+                    if i + 1 == self.time_out_try:
+                        raise e
+                    _logger.info(f':{e.code}:{i}')
+                    time.sleep(self.time_out_wait)
+                else:
+                    raise e
 
         return self, result
```

### Comparing `notionizer-0.0.4/notionizer/notion.py` & `notionizer-0.0.5/notionizer/notion.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 class Notion:
     f"""
     Notion
 
     'Notion' is basic object of 'notionizer' module.
     """
 
-    def __init__(self, secret_key: str):
+    def __init__(self, secret_key: str, timeout=15):
         """
         Initializes an instance of the HttpRequest class with the specified secret key.
 
         Args:
             secret_key (str): A string containing the secret key used to authenticate requests.
         """
         self.__secret_key = secret_key
-        self._request: HttpRequest = HttpRequest(secret_key)
+        self._request: HttpRequest = HttpRequest(secret_key, timeout=timeout)
 
     def get_database(self, database_id: str) -> Database:
         f"""
         get 'Database' Object by 'database_id'
 
         https://www.notion.so/myworkspace/{{database_id}}?v=...
         
@@ -44,15 +44,16 @@
             database id -> a8aec43384f447ed84390e6e32c2e089
         
         :param database_id:
         :return: Database
         """
 
         result = self._request.get('v1/databases/' + database_id)
-        db_object: Database = Database(*result)
+        database = Database(*result)
+        db_object: Database = database
         return db_object
 
     def get_page(self, page_id: str) -> Page:
         """
         get 'Page' object by 'page id'
         :param page_id:
         :return: Page
```

### Comparing `notionizer-0.0.4/notionizer/object_adt.py` & `notionizer-0.0.5/notionizer/object_adt.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/notionizer/object_basic.py` & `notionizer-0.0.5/notionizer/object_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from notionizer.object_adt import DictionaryObject, ListObject, ImmutableProperty
+from notionizer.object_adt import DictionaryObject, ListObject, ImmutableProperty, MutableProperty
 from notionizer.exception import NotionApiPropertyException
 from notionizer.http_request import HttpRequest
 from typing import Any
 from typing import Optional
 from typing import Dict
 from typing import Tuple
 from typing import List
@@ -135,18 +135,33 @@
     def __set__(self, owner: Any, value: List[Any]) -> None:
 
         obj = ListObject(self.public_name, owner, value, mutable=self.mutable)
 
         super().__set__(owner, obj)
 
 
+class ArrayPropertyMutable(MutableProperty):
+    """
+    ArrayProperty which inherits 'MutableProperty'.
+    """
+
+    def __init__(self, owner: Any=None, name: Optional[str] = '', mutable: bool=False):
+        self.mutable = mutable
+        super().__init__(owner=owner, name=str(name))
+
+    def __set__(self, owner: Any, value: List[Any]) -> None:
+
+        obj = ListObject(self.public_name, owner, value, mutable=self.mutable)
+
+        super().__set__(owner, obj)
+
+
 class RichTextProperty(ArrayProperty):
     pass
 
-
 def set_proper_descriptor(cls: Any, key: str, value: Any) -> None:
     """
     check the value type and assign property with proper descriptor.
     (only descriptor, not value)
 
     :param cls: object
     :param key: str
```

### Comparing `notionizer-0.0.4/notionizer/object_block.py` & `notionizer-0.0.5/notionizer/object_block.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/notionizer/object_database.py` & `notionizer-0.0.5/notionizer/object_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 
         Usage:
             queried = db.query(filter=filter_base)
             for page in queried:
                 ...
 
         """
-
         self._request: HttpRequest = request
         self._url: str = url
         self._payload: Dict[str, Any] = dict(payload)
 
         request_post: HttpRequest
         result_data: Dict[str, Any]
         request_post, result_data = request.post(url, payload)
@@ -265,24 +264,25 @@
         if columns_select:
             keys = tuple(columns_select)
         else:
             keys = (*self.properties.keys(),)
 
         for page in queried_page_iterator:
             values = page.get_properties()
-            result.append(tuple([values[k] for k in keys]))
+            result.append(tuple([values.get(k, None) for k in keys]))
         if not result:
             return tuple()
 
         if header:
             result = [keys] + result
 
         return tuple(result)
 
     def get_as_dictionaries(self, queried_page_iterator: QueriedPageIterator, columns_select: list=[]):
+
         """
         change QueriedPageIterator as simple values.
         :param queried_page_iterator: QueriedPageIterator()
         :param columns_select: ('column_name1', 'column_name2'...)
         :return: dict(('key1': 'value1', 'key2': 'value2'...), ... )
 
         Usage:
@@ -292,50 +292,68 @@
         """
         result = list()
 
         if columns_select:
             keys = tuple(columns_select)
         else:
             keys = (*self.properties.keys(),)
+
         for page in queried_page_iterator:
             values = page.get_properties()
-            result.append({k: values[k] for k in keys})
+            result.append({k: values.get(k, None) for k in keys})
         if not result:
             return tuple()
 
         return tuple(result)
 
     def create_page(self, properties: dict = {}):
         """
         Create 'new page' in the database.
 
         :param properties: receive 'dictionay' type for database property.
         :return: 'Page' object.
         """
-
+        _log.debug('call()')
         url = 'v1/pages/'
 
         payload = dict()
         payload['parent'] = {'database_id': self.id}
-        payload['properties'] = dict(properties)
 
         if properties:
-            for key, value in properties.items():
-
-                assert key in self.properties, f"'{key}' property not in the database '{self.title}'."
-                db_property: DbPropertyObject = self.properties[key]
-                assert db_property._mutable is True, f"{db_property}('{key}') property is 'Immutable Property'"
-                assert type(value) in db_property._input_validation, f"type of '{value}' is '{type(value)}'. " \
-                    f"{db_property}('{key}') property has type {db_property._input_validation}"
-
-                value_converted = db_property._convert_to_update(value)
-                payload['properties'][key] = value_converted
+            payload['properties'] = self._convert_to_payload(properties)
 
         return Page(*self._request.post(url, payload))
 
+    def _convert_to_payload(self, properties_dict):
+        """
+        convert dictionary to payload form, to input request parameter.
+        :param properties_dict:
+        :return:
+        """
+        _log.debug('call()')
+        properties_payload = {}
+        for key, value in properties_dict.items():
+            assert key in self.properties, f"'{key}' property not in the database '{self.title}'."
+            db_property: DbPropertyObject = self.properties[key]
+            assert db_property._mutable is True, f"{db_property}('{key}') property is 'Immutable Property'"
+            # print(value, db_property)
+            assert type(value) in db_property._input_validation, f"type of '{value}' is '{type(value)}'. " \
+                                                                 f"{db_property}('{key}') property has type {db_property._input_validation}"
+
+            value_converted = db_property._convert_to_update(value)
+            properties_payload[key] = value_converted
+        return properties_payload
+
+    def update_row_properties(self, page_id, properties_dict):
+        _log.debug('call()')
+        url = f'v1/pages/{page_id}'
+        payload = dict()
+        payload['properties'] = self._convert_to_payload(properties_dict)
+        return self._request.patch(url, payload)
+
     # Implement MutableMapping method
     def __getitem__(self, key):
         raise NotImplementedError
 
     # def __iter__(self):
     #     raise NotImplementedError
     #
```

### Comparing `notionizer-0.0.4/notionizer/object_page.py` & `notionizer-0.0.5/notionizer/object_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 
 
 NotionUpdateObject = notionizer.object_basic.NotionUpdateObject
 UserProperty = notionizer.object_user.UserProperty
 # Database = notionizer.objects.Database
 PropertiesProperty = notionizer.properties_property.PropertiesProperty
 ImmutableProperty = notionizer.object_user.ImmutableProperty
+MutableProperty = notionizer.object_user.MutableProperty
 notion_object_init_handler = notionizer.functions.notion_object_init_handler
 HttpRequest = notionizer.http_request.HttpRequest
 from_plain_text_to_rich_text_array = notionizer.functions.from_plain_text_to_rich_text_array
 
 
 class Page(NotionUpdateObject):
     """
     Page Object
     """
     properties = PropertiesProperty(object_type='page')
     id = ImmutableProperty()
     created_by = UserProperty()
     last_edited_by = UserProperty()
+    archived = MutableProperty()
 
     _api_url = 'v1/pages/'
 
     @notion_object_init_handler
     def __init__(self, request: HttpRequest, data: Dict[str, Any]):
 
         """
@@ -141,9 +143,9 @@
                 if opt == 'options':
                     data['properties'][p.name][p.prop_type]['options'] = []
                     for name, color in p.arguments[opt].items():
                         data['properties'][p.name][p.prop_type]['options'].append({'name': name, 'color': color})
                 else:
                     data['properties'][p.name][p.prop_type][opt] = p.arguments[opt]
 
-        db_object: 'Database' = __import__('notionizer').objects.Database(*self._request.post('v1/databases/', data))
+        db_object: 'Database' = __import__('notionizer').object_database.Database(*self._request.post('v1/databases/', data))
         return db_object
```

### Comparing `notionizer-0.0.4/notionizer/object_user.py` & `notionizer-0.0.5/notionizer/object_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import notionizer.object_adt
 import notionizer.object_basic
 import notionizer.functions
 import notionizer.http_request
 
 ImmutableProperty = notionizer.object_adt.ImmutableProperty
+MutableProperty = notionizer.object_adt.MutableProperty
 NotionUpdateObject = notionizer.object_basic.NotionUpdateObject
 UserBaseObject = notionizer.object_basic.UserBaseObject
 notion_object_init_handler = notionizer.functions.notion_object_init_handler
 HttpRequest = notionizer.http_request.HttpRequest
```

### Comparing `notionizer-0.0.4/notionizer/properties_basic.py` & `notionizer-0.0.5/notionizer/properties_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,38 @@
 from typing import Any
 from typing import Callable
 
 from urllib import parse
 _log = __import__('logging').getLogger(__name__)
 
 
-class TitleProperty(MutableProperty):
+class RichTextProperty(MutableProperty):
+    """
+    Specific object for richtext property.
+
+    :: USAGE
+
+    [1] print(db.title)
+    'some title'
+
+    [2] db.title = 'fixed title'
+    ...
+
+    """
+
+    def __get__(self, obj, objtype=None):
+        return getattr(obj, self.private_name)
+
+    def __set__(self, obj, value):
+        if type(value) == str:
+            value = from_plain_text_to_rich_text_array(value)
+        super().__set__(obj, value)
+
+
+class TitleProperty(RichTextProperty):
     """
     Specific object for title of database.
 
     :: USAGE
 
     [1] print(db.title)
     'some title'
@@ -31,15 +54,14 @@
 
     def __set__(self, obj, value):
         if type(value) == str:
             value = from_plain_text_to_rich_text_array(value)
 
         super().__set__(obj, value)
 
-
 class IdProperty(ImmutableProperty):
     """
     Property for id of properties with decoding 'url'.
     """
 
     def __set__(self, obj: Any, value: Any) -> None:
         """
@@ -75,14 +97,15 @@
         """
         self._parent: 'PropertiesProperty' = parent  # type: ignore
         self._parent_type = parent_type
         # dictionary for filter
         self._filter_body: Dict[str, Any] = dict()
         # page properties don't have 'name' property. This method assign '_name' property manually.
         self._name = name
+        # self.name = name
         super().__init__(data)
 
 
 class PagePropertyObject(PropertyBaseObject):
     """
     Basic Object for Data and Page Properties.
     """
@@ -90,15 +113,16 @@
     # to figure out which object is 'proper', uses '_type_defined' while assigning event.
     _type_defined = ''
 
     def __repr__(self) -> str:
         return f"<'{self.__class__.__name__}: {self._name}' at {hex(id(self))}>"
 
     def _update(self, property_name: str, data: Dict[str, Any]) -> None:
-        self._parent._update(self.name, {property_name: data})
+        self._parent._update(self._name, {property_name: data})
+        # self._parent._update(self.name, {property_name: data})
 
     def get_value(self):
 
         value = getattr(self, self.type)
 
         if hasattr(value, 'keys'):
             if 'name' in value:
@@ -119,15 +143,15 @@
                     result.append(e['id'])
                 elif hasattr(e, 'name'):
                     result.append(e.name.replace(u'\xa0', u' '))
                 else:
                     result.append(e)
             return tuple(result)
         else:
-            _log.info(f"{self}, {self.type}, {value}")
+            # _log.info(f"{self}, {self.type}, {value}")
             return value
 
 
 class DbPropertyObject(PropertyBaseObject):
     """
     Basic Object for Data and Page Properties.
     """
```

### Comparing `notionizer-0.0.4/notionizer/properties_db.py` & `notionizer-0.0.5/notionizer/properties_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,194 +2,200 @@
 from notionizer.properties_basic import TitleProperty
 from notionizer.object_adt import DictionaryObject
 from notionizer.functions import from_plain_text_to_rich_text_array
 from typing import Any
 from typing import Dict
 
 
-class DbPropertyLastEditedTime(DbPropertyObject):
-    """
-    'DbPropertyLastEditedTime'
-    """
-    _type_defined = 'last_edited_time'
-    _mutable = False
-
-
 class DbPropertyCreatedBy(DbPropertyObject):
     """
     'DbPropertyCreatedBy'
     """
     _type_defined = 'created_by'
     _mutable = False
 
 
-class DbPropertyCreatedTime(DbPropertyObject):
-    """
-    'DbPropertyCreatedTime'
-    """
-    _type_defined = 'created_time'
-    _mutable = False
-
-
-class DbPropertyLastEditedBy(DbPropertyObject):
+class DbPropertyPhoneNumber(DbPropertyObject):
     """
-    'DbPropertyLastEditedBy'
+    'DbPropertyPhoneNumber'
     """
-    _type_defined = 'last_edited_by'
-    _mutable = False
+    _type_defined = 'phone_number'
+    _mutable = True
+    _input_validation = (str, )
 
 
-class DbPropertyRollup(DbPropertyObject):
+class DbPropertyEmail(DbPropertyObject):
     """
-    'DbPropertyRollup'
+    'DbPropertyEmail'
     """
-    _type_defined = 'rollup'
-    _mutable = False
+    _type_defined = 'email'
+    _mutable = True
+    _input_validation = (str, )
 
 
 class DbPropertyPeople(DbPropertyObject):
     """
     'DbPropertyPeople'
     """
     _type_defined = 'people'
     _mutable = True
     _input_validation = (list, )
 
 
-class DbPropertyCheckbox(DbPropertyObject):
+class DbPropertyTitle(DbPropertyObject):
     """
-    'DbPropertyCheckbox'
+    'DbPropertyTitle'
     """
-    _type_defined = 'checkbox'
+    _type_defined = 'title'
     _mutable = True
-    _input_validation = (bool, )
+    _input_validation = (str, list)
+    title = TitleProperty()
 
+    def _convert_to_update(self, value: str) -> Dict[str, Any]:
+        """
+        convert value to 'title' update from.
 
-class DbPropertyRelation(DbPropertyObject):
+        :param value: str
+        :return: dictionary
+        """
+        return {'title': from_plain_text_to_rich_text_array(value)}
+
+
+class DbPropertyText(DbPropertyObject):
     """
-    'DbPropertyRelation'
+    'DbPropertyText'
     """
-    _type_defined = 'relation'
-    _mutable = False
-    relation: DictionaryObject
+    _type_defined = 'text'
+    _mutable = True
+    _input_validation = (str, list)
 
+    def _convert_to_update(self, value: Any) -> Any:
+        """
+        convert value to 'text' update from.
 
-class DbPropertyFormula(DbPropertyObject):
+        :param value: str or list
+        :return: dictionary
+        """
+        if type(value) is str:
+            return {'rich_text': from_plain_text_to_rich_text_array(value)}
+        elif type(value) is list:
+            return value
+
+
+class DbPropertyFiles(DbPropertyObject):
     """
-    'DbPropertyFormula'
+    'DbPropertyFiles'
     """
-    _type_defined = 'formula'
-    _mutable = False
+    _type_defined = 'files'
+    _mutable = True
+    _input_validation = (list, )
 
 
-class DbPropertyUrl(DbPropertyObject):
+class DbPropertyCreatedTime(DbPropertyObject):
     """
-    'DbPropertyUrl'
+    'DbPropertyCreatedTime'
     """
-    _type_defined = 'url'
-    _mutable = True
-    _input_validation = (str, )
+    _type_defined = 'created_time'
+    _mutable = False
 
 
-class DbPropertyEmail(DbPropertyObject):
+class DbPropertyNumber(DbPropertyObject):
     """
-    'DbPropertyEmail'
+    'DbPropertyNumber'
     """
-    _type_defined = 'email'
+    _type_defined = 'number'
     _mutable = True
-    _input_validation = (str, )
+    _input_validation = (int, float)
 
 
-class DbPropertyPhoneNumber(DbPropertyObject):
+class DbPropertyRollup(DbPropertyObject):
     """
-    'DbPropertyPhoneNumber'
+    'DbPropertyRollup'
     """
-    _type_defined = 'phone_number'
-    _mutable = True
-    _input_validation = (str, )
+    _type_defined = 'rollup'
+    _mutable = False
 
 
-class DbPropertyFiles(DbPropertyObject):
+class DbPropertyRelation(DbPropertyObject):
     """
-    'DbPropertyFiles'
+    'DbPropertyRelation'
     """
-    _type_defined = 'files'
-    _mutable = True
-    _input_validation = (list, )
+    _type_defined = 'relation'
+    _mutable = False
+    relation: DictionaryObject
 
 
-class DbPropertyDate(DbPropertyObject):
+class DbPropertyCheckbox(DbPropertyObject):
     """
-    'DbPropertyDate'
+    'DbPropertyCheckbox'
     """
-    _type_defined = 'date'
+    _type_defined = 'checkbox'
     _mutable = True
-    _input_validation = (dict, )
+    _input_validation = (bool, )
 
 
-class DbPropertyMultiSelect(DbPropertyObject):
+class DbPropertyUrl(DbPropertyObject):
     """
-    'DbPropertyMultiSelect'
+    'DbPropertyUrl'
     """
-    _type_defined = 'multi_select'
+    _type_defined = 'url'
     _mutable = True
-    _input_validation = (list, )
+    _input_validation = (str, )
 
 
 class DbPropertySelect(DbPropertyObject):
     """
     'DbPropertySelect'
     """
     _type_defined = 'select'
     _mutable = True
     _input_validation = (dict, )
 
+    def set_select_list(self, select_list):
+        payload = {"options": []}
+        for s in select_list:
+            payload["options"].append({'name': s})
+        self._update('select', payload)
 
-class DbPropertyText(DbPropertyObject):
+
+class DbPropertyFormula(DbPropertyObject):
     """
-    'DbPropertyText'
+    'DbPropertyFormula'
     """
-    _type_defined = 'text'
-    _mutable = True
-    _input_validation = (str, list)
+    _type_defined = 'formula'
+    _mutable = False
 
-    def _convert_to_update(self, value: Any) -> Any:
-        """
-        convert value to 'text' update from.
 
-        :param value: str or list
-        :return: dictionary
-        """
-        if type(value) is str:
-            return {'rich_text': from_plain_text_to_rich_text_array(value)}
-        elif type(value) is list:
-            return value
+class DbPropertyLastEditedTime(DbPropertyObject):
+    """
+    'DbPropertyLastEditedTime'
+    """
+    _type_defined = 'last_edited_time'
+    _mutable = False
 
 
-class DbPropertyTitle(DbPropertyObject):
+class DbPropertyDate(DbPropertyObject):
     """
-    'DbPropertyTitle'
+    'DbPropertyDate'
     """
-    _type_defined = 'title'
+    _type_defined = 'date'
     _mutable = True
-    _input_validation = (str, list)
-    title = TitleProperty()
+    _input_validation = (dict, )
 
-    def _convert_to_update(self, value: str) -> Dict[str, Any]:
-        """
-        convert value to 'title' update from.
 
-        :param value: str
-        :return: dictionary
-        """
-        return {'title': from_plain_text_to_rich_text_array(value)}
+class DbPropertyMultiSelect(DbPropertyObject):
+    """
+    'DbPropertyMultiSelect'
+    """
+    _type_defined = 'multi_select'
+    _mutable = True
+    _input_validation = (list, )
 
 
-class DbPropertyNumber(DbPropertyObject):
+class DbPropertyLastEditedBy(DbPropertyObject):
     """
-    'DbPropertyNumber'
+    'DbPropertyLastEditedBy'
     """
-    _type_defined = 'number'
-    _mutable = True
-    _input_validation = (int, )
+    _type_defined = 'last_edited_by'
+    _mutable = False
```

### Comparing `notionizer-0.0.4/notionizer/properties_page.py` & `notionizer-0.0.5/notionizer/properties_page.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from notionizer.functions import from_rich_text_array_to_plain_text
+from notionizer.functions import from_rich_text_array_to_plain_text, from_plain_text_to_rich_text_array
 from notionizer.functions import parse_date_object
 from notionizer.object_adt import MutableProperty
-from notionizer.properties_basic import PagePropertyObject
+from notionizer.properties_basic import PagePropertyObject, TitleProperty,RichTextProperty
 from notionizer.object_basic import UserBaseObject
 from typing import Any, Dict, List
 
 
 def parse_value_object(obj: Any) -> Any:
     """
     parse value of 'formula' and 'rollup'. 
@@ -21,218 +21,212 @@
         return [parse_value_object(e) for e in value]
     
     # 'number', 'string', 'boolean'
     else:
         return value
 
 
-class PagePropertyPhoneNumber(PagePropertyObject):
+class PagePropertySelect(PagePropertyObject):
     """
-    'PagePropertyPhoneNumber'
+    'PagePropertySelect'
     """
-    _type_defined = 'phone_number'
-    phone_number = MutableProperty()
+    _type_defined = 'select'
 
 
-class PagePropertySelect(PagePropertyObject):
+class PagePropertyPhoneNumber(PagePropertyObject):
     """
-    'PagePropertySelect'
+    'PagePropertyPhoneNumber'
     """
-    _type_defined = 'select'
+    _type_defined = 'phone_number'
+    phone_number = MutableProperty()
 
 
-class PagePropertyCreatedTime(PagePropertyObject):
+class PagePropertyFiles(PagePropertyObject):
     """
-    'PagePropertyCreatedTime'
+    'PagePropertyFiles'
     """
-    _type_defined = 'created_time'
+    _type_defined = 'files'
 
 
-class PagePropertyCreatedBy(PagePropertyObject):
+class PagePropertyEmail(PagePropertyObject):
     """
-    'PagePropertyCreatedBy'
+    'PagePropertyEmail'
     """
-    _type_defined = 'created_by'
+    _type_defined = 'email'
+    email = MutableProperty()
 
 
-class PagePropertyRollup(PagePropertyObject):
+class PagePropertyRichText(PagePropertyObject):
     """
-    'PagePropertyRollup'
+    'PagePropertyRichText'
     """
-    _type_defined = 'rollup'
+    _type_defined = 'rich_text'
+    rich_text = RichTextProperty()
 
     def get_value(self) -> Any:
         """
-        parse 'rollup object'
+        parse 'rich_text' to plain 'string' and return
         """
-        return parse_value_object(self.rollup)
+        return from_rich_text_array_to_plain_text(self.rich_text)
+    
+    def _convert_to_update(self, value: str) -> Dict[str, Any]:
+        """
+        convert value to 'title' update from.
 
+        :param value: str
+        :return: dictionary
+        """
+        return {'rich_text': from_plain_text_to_rich_text_array(value)}
 
-class PagePropertyPeople(PagePropertyObject):
+
+class PagePropertyTitle(PagePropertyObject):
     """
-    'PagePropertyPeople'
+    'PagePropertyTitle'
     """
-    _type_defined = 'people'
+    _type_defined = 'title'
+    title = TitleProperty()
 
-    def __init__(self, parent: Any, data: Dict[str, Any], parent_type: str, name: str, force_new: bool = False):
+    def get_value(self) -> Any:
         """
-
-        :param parent: PropertiesProperty
-        :param data:
-        :param parent_type:
-        :param name:
-        :param force_new:
+        parse 'rich_text' to plain 'string' and return
         """
+        return self.title
+    
+    def _convert_to_update(self, value: str) -> Dict[str, Any]:
+        """
+        convert value to 'title' update from.
 
-        user_list: List[UserBaseObject] = list()
-        object_list: List[Dict[str, Any]] = data['people']
-        for e in object_list:
-            user_list.append(UserBaseObject(e))
-        data['people'] = user_list
-        super().__init__(parent, data, parent_type, name)
+        :param value: str
+        :return: dictionary
+        """
+        return {'title': from_plain_text_to_rich_text_array(value)}
 
 
 class PagePropertyMultiSelect(PagePropertyObject):
     """
     'PagePropertyMultiSelect'
     """
     _type_defined = 'multi_select'
 
 
-class PagePropertyNumber(PagePropertyObject):
+class PagePropertyLastEditedTime(PagePropertyObject):
     """
-    'PagePropertyNumber'
+    'PagePropertyLastEditedTime'
     """
-    _type_defined = 'number'
-    number = MutableProperty()
+    _type_defined = 'last_edited_time'
 
 
-class PagePropertyLastEditedBy(PagePropertyObject):
+class PagePropertyCreatedBy(PagePropertyObject):
     """
-    'PagePropertyLastEditedBy'
+    'PagePropertyCreatedBy'
     """
-    _type_defined = 'last_edited_by'
+    _type_defined = 'created_by'
+
+
+class PagePropertyDate(PagePropertyObject):
+    """
+    'PagePropertyDate'
+    """
+    _type_defined = 'date'
+
+    def get_value(self) -> Any:
+        """
+        parse 'date object'
+        """
+        return parse_date_object(self.date)
 
 
 class PagePropertyCheckbox(PagePropertyObject):
     """
     'PagePropertyCheckbox'
     """
     _type_defined = 'checkbox'
     checkbox = MutableProperty()
 
 
-class PagePropertyEmail(PagePropertyObject):
+class PagePropertyRelation(PagePropertyObject):
     """
-    'PagePropertyEmail'
+    'PagePropertyRelation'
     """
-    _type_defined = 'email'
-    email = MutableProperty()
+    _type_defined = 'relation'
 
 
-class PagePropertyRichText(PagePropertyObject):
+class PagePropertyPeople(PagePropertyObject):
     """
-    'PagePropertyRichText'
+    'PagePropertyPeople'
     """
-    _type_defined = 'rich_text'
+    _type_defined = 'people'
 
-    def get_value(self) -> Any:
-        """
-        parse 'rich_text' to plain 'string' and return
+    def __init__(self, parent: Any, data: Dict[str, Any], parent_type: str, name: str, force_new: bool = False):
         """
-        return from_rich_text_array_to_plain_text(self.rich_text)
-
-    def is_not_empty(self):
-        pass
-
-    def starts_with(self):
-        pass
 
-    def does_not_contain(self):
-        pass
-
-    def ends_with(self):
-        pass
+        :param parent: PropertiesProperty
+        :param data:
+        :param parent_type:
+        :param name:
+        :param force_new:
+        """
 
-    def does_not_equal(self):
-        pass
+        user_list: List[UserBaseObject] = list()
+        object_list: List[Dict[str, Any]] = data['people']
+        for e in object_list:
+            user_list.append(UserBaseObject(e))
+        data['people'] = user_list
+        super().__init__(parent, data, parent_type, name)
 
-    def is_empty(self):
-        pass
 
-    def equals(self, string: str):
-        self._body[self._type_defined]['equals'] = string
-        return self
+class PagePropertyLastEditedBy(PagePropertyObject):
+    """
+    'PagePropertyLastEditedBy'
+    """
+    _type_defined = 'last_edited_by'
 
-    def contains(self):
-        pass
 
+class PagePropertyCreatedTime(PagePropertyObject):
+    """
+    'PagePropertyCreatedTime'
+    """
+    _type_defined = 'created_time'
 
 
 class PagePropertyUrl(PagePropertyObject):
     """
     'PagePropertyUrl'
     """
     _type_defined = 'url'
     url = MutableProperty()
 
 
-class PagePropertyLastEditedTime(PagePropertyObject):
-    """
-    'PagePropertyLastEditedTime'
-    """
-    _type_defined = 'last_edited_time'
-
-
 class PagePropertyFormula(PagePropertyObject):
     """
     'PagePropertyFormula'
     """
     _type_defined = 'formula'
 
     def get_value(self) -> Any:
         """
         parse 'formula object'
         """
         return parse_value_object(self.formula)
 
 
-class PagePropertyRelation(PagePropertyObject):
-    """
-    'PagePropertyRelation'
-    """
-    _type_defined = 'relation'
-
-
-class PagePropertyDate(PagePropertyObject):
-    """
-    'PagePropertyDate'
-    """
-    _type_defined = 'date'
-
-    def get_value(self) -> Any:
-        """
-        parse 'date object'
-        """
-        return parse_date_object(self.date)
-
-
-class PagePropertyFiles(PagePropertyObject):
+class PagePropertyNumber(PagePropertyObject):
     """
-    'PagePropertyFiles'
+    'PagePropertyNumber'
     """
-    _type_defined = 'files'
+    _type_defined = 'number'
+    number = MutableProperty()
 
 
-class PagePropertyTitle(PagePropertyObject):
+class PagePropertyRollup(PagePropertyObject):
     """
-    'PagePropertyTitle'
+    'PagePropertyRollup'
     """
-    _type_defined = 'title'
+    _type_defined = 'rollup'
 
     def get_value(self) -> Any:
         """
-        parse 'rich_text' to plain 'string' and return
+        parse 'rollup object'
         """
-        return from_rich_text_array_to_plain_text(self.title)
+        return parse_value_object(self.rollup)
```

### Comparing `notionizer-0.0.4/notionizer/properties_property.py` & `notionizer-0.0.5/notionizer/properties_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from notionizer.object_adt import DictionaryObject, ImmutableProperty
+from notionizer.object_adt import DictionaryObject, ImmutableProperty, MutableProperty
 from notionizer.properties_basic import PropertyBaseObject, PagePropertyObject, DbPropertyObject
 
 import notionizer.properties_page
 import notionizer.properties_db
 from typing import Any
 from typing import Dict
 from typing import Optional
```

### Comparing `notionizer-0.0.4/notionizer/query.py` & `notionizer-0.0.5/notionizer/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,14 +547,18 @@
         self._body[self._property_type]['does_not_contain'] = option
         return self
 
 
 class filter_date(FilterConditionEmpty):
     data_type = 'date'
 
+    TYPE_DATE = 'date'
+    TYPE_CREATED_TIME = 'created_time'
+    TYPE_LAST_EDITED_TIME = 'last_edited_time'
+
     def __init__(self, property_type: str, property_name: str, timezone: Optional[str] = ''):
         """
 
         date filter requires 'timezone'. You should tail after 'datetime' like "2021-10-15T12:00:00+09:00" to set the
         specific 'timezone' value. Module set the 'timezone' dynamically. So user doesn't need to set.  But if user want
         to set manually, use 'timezone' parameter or after generating 'filter_date' instance, assign value on 'timezone'
         property.
@@ -571,19 +575,15 @@
             or
 
             filter_dt = filter_date(filter_date.TYPE_DATE, 'PropertyName')
             filter_dt.timezone = '+09:00'
             filter_dt.equals("2021-05-10")
         """
 
-        TYPE_DATE = 'date'
-        TYPE_CREATED_TIME = 'created_time'
-        TYPE_LAST_EDITED_TIME = 'last_edited_time'
-
-        assert property_type in [TYPE_DATE, TYPE_CREATED_TIME, TYPE_LAST_EDITED_TIME], \
+        assert property_type in [self.TYPE_DATE, self.TYPE_CREATED_TIME, self.TYPE_LAST_EDITED_TIME], \
             f"'property_type' allows only 'date', 'created_time', and 'last_edited_time'"
 
         if not timezone:
             timezone = ''
             timezone_int = -int(time.timezone / 60 / 60)
             if timezone_int == 0:
                 timezone = '+00:00'
@@ -603,15 +603,15 @@
                 "timestamp": "created_time",
                 "created_time": {
                   "past_week": {}
                 }
              }
         }
         """
-        if property_type in [TYPE_CREATED_TIME, TYPE_LAST_EDITED_TIME]:
+        if property_type in [self.TYPE_CREATED_TIME, self.TYPE_LAST_EDITED_TIME]:
             self._body: Dict[str, Any] = {
                 'timestamp': property_type,
                 property_type: dict()
             }
             self._property_type: str = str(property_type)
 
         # 'date' property
@@ -969,15 +969,15 @@
 
 
 """
 SORTS
 """
 
 
-class sorts:
+class sorts(SortObject):
 
     ASCENDING = 'ascending'
     DESCENDING = 'descending'
     CREATED_TIME = 'created_time'
     LAST_EDITED_TIME = 'last_edited_time'
 
     def __init__(self) -> None:
@@ -985,26 +985,24 @@
 
         Args:
             compound: 'filter.OR' or 'filter.AND'
         """
         self._body: List[Any] = []
 
     def add(self, sort_obj: Type[SortObject]) -> 'sorts':
-        assert issubclass(sort_obj, SortObject)
+        assert issubclass(type(sort_obj), SortObject)
         self._body.append(dict(sort_obj._body))
-
         return self
 
 
 class sort_by_timestamp(SortObject):
 
     def __init__(self, time_property: str, direction: Optional[str] = sorts.ASCENDING):
         assert time_property in [sorts.CREATED_TIME, sorts.LAST_EDITED_TIME]
         assert direction in [sorts.ASCENDING, sorts.DESCENDING]
-
         self._body = {'timestamp': time_property, 'direction': direction}
 
 
 class sort_by_property(SortObject):
 
     def __init__(self, property_name: str, direction: Optional[str] = sorts.ASCENDING):
         assert direction in [sorts.ASCENDING, sorts.DESCENDING]
```

### Comparing `notionizer-0.0.4/notionizer.egg-info/PKG-INFO` & `notionizer-0.0.5/notionizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionizer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python wrapper for Notion API
 Home-page: https://github.com/kimsg1984/notionizer
 Author: SeonGyo Kim
 Author-email: kimsg1984@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `notionizer-0.0.4/notionizer.egg-info/SOURCES.txt` & `notionizer-0.0.5/notionizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/setup.py` & `notionizer-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 reqs = parse_requirements("requirements.txt", session=False)
 install_requires = [str(ir.requirement) for ir in reqs]
 
 setuptools.setup(
     name="notionizer",
-    version="0.0.4",
+    version="0.0.5",
     author="SeonGyo Kim",
     author_email="kimsg1984@gmail.com",
     description="Python wrapper for Notion API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimsg1984/notionizer",
     install_requires=install_requires,
```

### Comparing `notionizer-0.0.4/test/test_block.py` & `notionizer-0.0.5/test/test_block.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/test/test_notion.py` & `notionizer-0.0.5/test/test_notion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unittest import TestCase
+wfrom unittest import TestCase
 from setting import setting
 
 notion_api_key = setting.notion_api_key
 
 
 class TestNotion(TestCase):
     def test_get_user(self):
```

### Comparing `notionizer-0.0.4/test/test_notion1.py` & `notionizer-0.0.5/test/test_notion1.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/test/test_object_database.py` & `notionizer-0.0.5/test/test_object_database.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/test/test_object_page.py` & `notionizer-0.0.5/test/test_object_page.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.4/test/test_query.py` & `notionizer-0.0.5/test/test_query.py`

 * *Files identical despite different names*

