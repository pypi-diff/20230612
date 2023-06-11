# Comparing `tmp/payok.io-1.0.4.tar.gz` & `tmp/payok.io-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payok.io-1.0.4.tar", last modified: Sun Jun 11 22:29:10 2023, max compression
+gzip compressed data, was "payok.io-1.0.5.tar", last modified: Sun Jun 11 23:07:37 2023, max compression
```

## Comparing `payok.io-1.0.4.tar` & `payok.io-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 22:29:10.539602 payok.io-1.0.4/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.4/LICENSE
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-06-11 22:29:10.539602 payok.io-1.0.4/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1518 2023-05-17 15:09:15.000000 payok.io-1.0.4/README.md
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 22:29:10.535602 payok.io-1.0.4/payok/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      494 2023-05-17 14:50:33.000000 payok.io-1.0.4/payok/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     7300 2023-06-11 22:23:20.000000 payok.io-1.0.4/payok/api.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 22:29:10.539602 payok.io-1.0.4/payok/enums/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      362 2023-05-17 13:37:52.000000 payok.io-1.0.4/payok/enums/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.4/payok/enums/base.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.4/payok/enums/comission_type.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.4/payok/enums/currency.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.4/payok/enums/pay_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.4/payok/enums/payment_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.4/payok/enums/payout_method.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.4/payok/enums/webhook_status.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      272 2023-05-17 14:06:53.000000 payok.io-1.0.4/payok/exceptions.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 22:29:10.539602 payok.io-1.0.4/payok/models/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.4/payok/models/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.4/payok/models/balance.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      196 2023-05-17 14:49:19.000000 payok.io-1.0.4/payok/models/new_payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      898 2023-05-17 14:55:52.000000 payok.io-1.0.4/payok/models/payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1021 2023-06-11 22:24:05.000000 payok.io-1.0.4/payok/models/transaction.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 22:29:10.535602 payok.io-1.0.4/payok.io.egg-info/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-06-11 22:29:10.000000 payok.io-1.0.4/payok.io.egg-info/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      576 2023-06-11 22:29:10.000000 payok.io-1.0.4/payok.io.egg-info/SOURCES.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-06-11 22:29:10.000000 payok.io-1.0.4/payok.io.egg-info/dependency_links.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       17 2023-06-11 22:29:10.000000 payok.io-1.0.4/payok.io.egg-info/requires.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        6 2023-06-11 22:29:10.000000 payok.io-1.0.4/payok.io.egg-info/top_level.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-06-11 22:29:10.539602 payok.io-1.0.4/setup.cfg
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1269 2023-06-11 22:28:57.000000 payok.io-1.0.4/setup.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1063 2023-05-17 13:59:37.000000 payok.io-1.0.5/LICENSE
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-06-11 23:07:37.327316 payok.io-1.0.5/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1518 2023-05-17 15:09:15.000000 payok.io-1.0.5/README.md
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.323316 payok.io-1.0.5/payok/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      494 2023-05-17 14:50:33.000000 payok.io-1.0.5/payok/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     7284 2023-06-11 23:05:53.000000 payok.io-1.0.5/payok/api.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/payok/enums/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      362 2023-05-17 13:37:52.000000 payok.io-1.0.5/payok/enums/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      162 2023-05-17 14:34:42.000000 payok.io-1.0.5/payok/enums/base.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      114 2023-05-17 14:34:58.000000 payok.io-1.0.5/payok/enums/comission_type.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      138 2023-05-17 14:35:37.000000 payok.io-1.0.5/payok/enums/currency.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       99 2023-05-17 14:38:46.000000 payok.io-1.0.5/payok/enums/pay_status.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      293 2023-05-17 14:35:18.000000 payok.io-1.0.5/payok/enums/payment_method.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      455 2023-05-17 14:35:26.000000 payok.io-1.0.5/payok/enums/payout_method.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      103 2023-05-17 14:20:25.000000 payok.io-1.0.5/payok/enums/webhook_status.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      272 2023-05-17 14:06:53.000000 payok.io-1.0.5/payok/exceptions.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/payok/models/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      208 2023-05-17 14:49:34.000000 payok.io-1.0.5/payok/models/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      139 2023-05-16 21:14:21.000000 payok.io-1.0.5/payok/models/balance.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      196 2023-05-17 14:49:19.000000 payok.io-1.0.5/payok/models/new_payout.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      898 2023-06-11 23:05:12.000000 payok.io-1.0.5/payok/models/payout.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1021 2023-06-11 23:05:07.000000 payok.io-1.0.5/payok/models/transaction.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-06-11 23:07:37.327316 payok.io-1.0.5/payok.io.egg-info/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2309 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      576 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/SOURCES.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/dependency_links.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       17 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/requires.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        6 2023-06-11 23:07:37.000000 payok.io-1.0.5/payok.io.egg-info/top_level.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-06-11 23:07:37.327316 payok.io-1.0.5/setup.cfg
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1269 2023-06-11 23:06:14.000000 payok.io-1.0.5/setup.py
```

### Comparing `payok.io-1.0.4/LICENSE` & `payok.io-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.4/PKG-INFO` & `payok.io-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.4
+Version: 1.0.5
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
```

### Comparing `payok.io-1.0.4/README.md` & `payok.io-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.4/payok/api.py` & `payok.io-1.0.5/payok/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     Currency,
     ComissionType,
     PaymentMethod,
     PayoutMethod,
 )
 from .exceptions import PayOKError
 
-from urllib.parse import urlencode
 from typing import Union, Optional, List
+from urllib.parse import urlencode
 
 from aiohttp import ClientSession
 
 
 class PayOK(object):
     """
     PayOK API Wrapper
@@ -230,15 +230,15 @@
             'currency': currency,
             'desc': description,
             'email': email,
             'success_url': success_url,
             'method': method,
             'lang': lang,
             'sign': sign.hexdigest(),
-            'custom': custom_params or None,
+            **custom_params,
         }
         url = 'https://payok.io/pay?' + urlencode(
             {
                 key: value
                 for key, value in params.items()
                 if value is not None
             },
```

### Comparing `payok.io-1.0.4/payok/models/payout.py` & `payok.io-1.0.5/payok/models/payout.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..enums import PayoutMethod, PayStatus
 
-from typing import Optional
 from datetime import datetime
+from typing import Optional
 
 from pydantic import BaseModel, validator
 from pydantic.fields import Field
 
 
 class Payout(BaseModel):
     """
```

### Comparing `payok.io-1.0.4/payok/models/transaction.py` & `payok.io-1.0.5/payok/models/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from ..enums import (
     Currency,
     PayStatus, 
     WebhookStatus, 
 )
 
-from typing import Optional
 from datetime import datetime
+from typing import Dict, Any
 
 from pydantic import BaseModel, validator
 from pydantic.fields import Field
 
 
 class Transaction(BaseModel):
     """
@@ -27,21 +27,21 @@
     comission_percent: float
     comission_fixed: float
     method: str
     transaction: int
     date: datetime
     pay_date: datetime = None
     status: PayStatus = Field(PayStatus.waiting, alias='transaction_status')
-    custom_fields: Optional[dict]
+    custom_fields: Dict[str, Any]
     webhook_status: WebhookStatus
     webhook_amount: int
 
     @property
     def is_paid(self) -> bool:
 
         return bool(self.status)
 
     @validator('custom_fields', pre=True)
     def validate_fields(raw_field: str) -> dict:
 
-        string = raw_field.replace('&quot;', '\"')
+        string = raw_field.replace('&quot;', '"')
         return json.loads(string)
```

### Comparing `payok.io-1.0.4/payok.io.egg-info/PKG-INFO` & `payok.io-1.0.5/payok.io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payok.io
-Version: 1.0.4
+Version: 1.0.5
 Summary: Asynchronous PayOK API wrapper
 Home-page: https://github.com/nikitalm8/payok
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/payok
 Project-URL: Bug Tracker, https://github.com/nikitalm8/payok/issues
 Project-URL: API Docs, https://payok.io/cabinet/documentation/doc_api_main
```

### Comparing `payok.io-1.0.4/payok.io.egg-info/SOURCES.txt` & `payok.io-1.0.5/payok.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payok.io-1.0.4/setup.py` & `payok.io-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import os
 import codecs
+import os
 
 from setuptools import setup, find_packages
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as file:
 
     long_description = "\n" + file.read()
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 DESCRIPTION = 'Asynchronous PayOK API wrapper'
 
 setup(
     name="payok.io",
     version=VERSION,
     author="Nikita Minaev",
     author_email="<nikita@minaev.su>",
```

