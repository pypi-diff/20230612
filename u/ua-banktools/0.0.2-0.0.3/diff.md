# Comparing `tmp/ua_banktools-0.0.2.tar.gz` & `tmp/ua_banktools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ua_banktools-0.0.2.tar", max compression
+gzip compressed data, was "ua_banktools-0.0.3.tar", max compression
```

## Comparing `ua_banktools-0.0.2.tar` & `ua_banktools-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1072 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/LICENSE
--rw-r--r--   0        0        0       90 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/README.md
--rw-r--r--   0        0        0      462 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       42 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/ua_banktools/banks/__init__.py
--rw-r--r--   0        0        0     1019 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/ua_banktools/banks/base.py
--rw-r--r--   0        0        0     2932 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/ua_banktools/banks/privatbank.py
--rw-r--r--   0        0        0     4070 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/ua_banktools/banks/privatbank_types.py
--rw-r--r--   0        0        0       21 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/ua_banktools/core/__init__.py
--rw-r--r--   0        0        0     2885 2022-11-25 22:32:54.721518 ua_banktools-0.0.2/ua_banktools/core/ipn.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 ua_banktools-0.0.2/setup.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 ua_banktools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-11-11 11:33:33.984279 ua_banktools-0.0.3/LICENSE
+-rw-r--r--   0        0        0       90 2022-11-11 11:33:33.984457 ua_banktools-0.0.3/README.md
+-rw-r--r--   0        0        0      499 2023-06-12 09:55:17.821690 ua_banktools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       42 2022-11-21 21:38:59.066607 ua_banktools-0.0.3/ua_banktools/banks/__init__.py
+-rw-r--r--   0        0        0     1019 2022-11-23 18:59:47.021031 ua_banktools-0.0.3/ua_banktools/banks/base.py
+-rw-r--r--   0        0        0     2932 2022-11-23 19:27:42.860885 ua_banktools-0.0.3/ua_banktools/banks/privatbank.py
+-rw-r--r--   0        0        0     4127 2023-06-12 09:53:55.077217 ua_banktools-0.0.3/ua_banktools/banks/privatbank_types.py
+-rw-r--r--   0        0        0       21 2022-11-22 19:06:44.631488 ua_banktools-0.0.3/ua_banktools/core/__init__.py
+-rw-r--r--   0        0        0     2885 2022-11-25 19:23:49.358596 ua_banktools-0.0.3/ua_banktools/core/ipn.py
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 ua_banktools-0.0.3/PKG-INFO
```

### Comparing `ua_banktools-0.0.2/LICENSE` & `ua_banktools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ua_banktools-0.0.2/ua_banktools/banks/base.py` & `ua_banktools-0.0.3/ua_banktools/banks/base.py`

 * *Files identical despite different names*

### Comparing `ua_banktools-0.0.2/ua_banktools/banks/privatbank.py` & `ua_banktools-0.0.3/ua_banktools/banks/privatbank.py`

 * *Files identical despite different names*

### Comparing `ua_banktools-0.0.2/ua_banktools/banks/privatbank_types.py` & `ua_banktools-0.0.3/ua_banktools/banks/privatbank_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import List, Optional, Dict
 
 from pydantic import BaseModel
 
+
 # Allow arbitrary types like IBAN in requests and responses
 class Config:
     arbitrary_types_allowed = True
 
 
 # Enums for the Privatbank Commercial API
 class Currency(Enum):
@@ -109,37 +110,40 @@
     recipient_nceo: str
     payment_naming: str
     payment_amount: float
     payment_destination: str
 
 
 class PaymentData(BaseModel):
-    tabs: List[str]
-    user_id: str
+    can_edit: str
+    can_copy: Optional[str]
+    document_number: str
+    document_type: str
+    id: str
+    internal_type: str
+    level_sign: Dict[str, str]
     payer_account: str
-    payer_nceo: str
+    payer_bank_name: str
     payer_name: str
-    recipient_account: str
-    recipient_nceo: str
-    payment_naming: str
-    document_type: str
-    document_number: str
-    payment_date: str  # date
-    payment_accept_date: str  # date
+    payer_nceo: str
     payment_amount: float
-    payment_destination: str
-    payment_status: str  # Enum?
     payment_ccy: Currency
     payment_date_unix: str  # Unix Timestamp
-    level_sign: Dict[str, str]
-    internal_type: str
+    payment_destination: str
+    payment_naming: str
+    payment_sign: List[str]
+    payment_status: str  # Enum?
+    payment_status_short: str
+    recipient_account: str
+    recipient_ifi_text: str
+    recipient_nceo: str
     service_update_utime: str
     source: str
-    can_edit: str
-    can_copy: Optional[str]
+    tabs: List[str]
+    user_id: str
 
 
 class PaymentCreateSuccessResponse(BaseModel):
     payment_data: PaymentData
     payment_pack_ref: str
     payment_ref: str
```

### Comparing `ua_banktools-0.0.2/ua_banktools/core/ipn.py` & `ua_banktools-0.0.3/ua_banktools/core/ipn.py`

 * *Files identical despite different names*

### Comparing `ua_banktools-0.0.2/PKG-INFO` & `ua_banktools-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ua-banktools
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Anton Shpigunov
 Author-email: shpigunov@gmail.com
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: schwifty (>=2022.9.0,<2023.0.0)
 Description-Content-Type: text/markdown
```

