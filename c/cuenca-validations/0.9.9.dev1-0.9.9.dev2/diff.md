# Comparing `tmp/cuenca_validations-0.9.9.dev1.tar.gz` & `tmp/cuenca_validations-0.9.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuenca_validations-0.9.9.dev1.tar", last modified: Fri Jul 16 17:56:15 2021, max compression
+gzip compressed data, was "cuenca_validations-0.9.9.dev2.tar", last modified: Mon Jul 19 17:21:01 2021, max compression
```

## Comparing `cuenca_validations-0.9.9.dev1.tar` & `cuenca_validations-0.9.9.dev2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 17:56:15.354328 cuenca_validations-0.9.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-07-16 17:56:15.354328 cuenca_validations-0.9.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 17:56:15.354328 cuenca_validations-0.9.9.dev1/cuenca_validations/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/card_bins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 17:56:15.354328 cuenca_validations-0.9.9.dev1/cuenca_validations/types/
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/types/card.py
--rw-r--r--   0 runner    (1001) docker     (121)     4114 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/types/general.py
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/types/queries.py
--rw-r--r--   0 runner    (1001) docker     (121)     5206 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/cuenca_validations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 17:56:15.354328 cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-07-16 17:56:14.000000 cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-07-16 17:56:15.000000 cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-16 17:56:14.000000 cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-07-16 17:56:14.000000 cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-07-16 17:56:14.000000 cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      429 2021-07-16 17:56:15.354328 cuenca_validations-0.9.9.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 17:56:15.354328 cuenca_validations-0.9.9.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/tests/test_card.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/tests/test_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2021-07-16 17:56:05.000000 cuenca_validations-0.9.9.dev1/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 17:21:01.177493 cuenca_validations-0.9.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-07-19 17:21:01.177493 cuenca_validations-0.9.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 17:21:01.173493 cuenca_validations-0.9.9.dev2/cuenca_validations/
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/card_bins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 17:21:01.177493 cuenca_validations-0.9.9.dev2/cuenca_validations/types/
+-rw-r--r--   0 runner    (1001) docker     (121)     2145 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/types/card.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4227 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1390 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/types/general.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3006 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/types/queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5605 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/cuenca_validations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 17:21:01.173493 cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-07-19 17:21:00.000000 cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-07-19 17:21:01.000000 cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-19 17:21:00.000000 cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-07-19 17:21:00.000000 cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-07-19 17:21:00.000000 cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2021-07-19 17:21:01.177493 cuenca_validations-0.9.9.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 17:21:01.177493 cuenca_validations-0.9.9.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/tests/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/tests/test_statement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6185 2021-07-19 17:20:52.000000 cuenca_validations-0.9.9.dev2/tests/test_types.py
```

### Comparing `cuenca_validations-0.9.9.dev1/LICENSE` & `cuenca_validations-0.9.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/PKG-INFO` & `cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cuenca_validations
-Version: 0.9.9.dev1
+Name: cuenca-validations
+Version: 0.9.9.dev2
 Summary: Cuenca common validations
 Home-page: https://github.com/cuenca-mx/cuenca-validations
 Author: Cuenca
 Author-email: dev@cuenca.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/card_bins.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/card_bins.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/errors.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/errors.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/types/__init__.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     'IssuerNetwork',
     'JSONEncoder',
     'PageSize',
     'PaymentCardNumber',
     'PosCapability',
     'QueryParams',
     'SantizedDict',
+    'SavingCategory',
     'SavingRequest',
     'ServiceProviderCategory',
     'StatementQuery',
     'StrictPaymentCardNumber',
     'StrictPositiveInt',
     'StrictPositiveFloat',
     'StrictTransferRequest',
@@ -60,14 +61,15 @@
     CommissionType,
     Currency,
     DepositNetwork,
     EntryType,
     FileFormat,
     IssuerNetwork,
     PosCapability,
+    SavingCategory,
     ServiceProviderCategory,
     TrackDataMethod,
     TransactionStatus,
     TransferNetwork,
     UserCardNotification,
     WalletType,
 )
```

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/types/card.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/types/card.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/types/enums.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/types/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     succeeded = 'succeeded'
     failed = 'failed'
 
 
 class TransferNetwork(str, Enum):
     internal = 'internal'
     spei = 'spei'
+    wallet = 'wallet'
 
 
 class CommissionType(str, Enum):
     card_request = 'card_request'
     cash_deposit = 'cash_deposit'
 
 
@@ -170,9 +171,15 @@
     btc = 'btc'
     cuenca = 'cuenca'
 
 
 class WalletType(str, Enum):
     saving = 'saving'
     crypto = 'crypto'
-    foreign_currency = 'foreign_currency'
-    cuenca = 'cuenca'
+
+
+class SavingCategory(str, Enum):
+    vehicle = 'vehicle'
+    property = 'property'
+    education = 'education'
+    travel = 'travel'
+    other = 'other'
```

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/types/general.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/types/general.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/types/queries.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/types/queries.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/types/requests.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/types/requests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
+from datetime import datetime
 from typing import Optional, Union
 
 from clabe import Clabe
 from pydantic import (
     BaseModel,
     Extra,
     Field,
     StrictStr,
     conint,
     constr,
     root_validator,
 )
+from pydantic.class_validators import validator
 
 from ..types.enums import (
     AuthorizerTransaction,
     CardDesign,
     CardFundingType,
     CardIssuer,
     CardPackaging,
     CardStatus,
     CardType,
     Currency,
     IssuerNetwork,
     PosCapability,
+    SavingCategory,
     TrackDataMethod,
     UserCardNotification,
 )
 from ..typing import DictStrAny
 from .card import PaymentCardNumber, StrictPaymentCardNumber
 from .general import StrictPositiveInt
 
@@ -187,12 +190,20 @@
 
 
 class UserCardNotificationRequest(CardTransactionRequest):
     type: UserCardNotification
 
 
 class SavingRequest(BaseRequest):
+    '''Request for oaxaca to create a saving object'''
+
     name: str
-    category: str
-    goal: int
-    end_goal: int
+    category: SavingCategory
+    amount: StrictPositiveInt
+    end_date: datetime
     currency: Currency
+
+    @validator('end_date')
+    def validate_end_date(cls, v: datetime) -> datetime:
+        if v <= datetime.now():
+            raise ValueError('The end_date always need to be higher than now')
+        return v
```

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations/validators.py` & `cuenca_validations-0.9.9.dev2/cuenca_validations/validators.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/PKG-INFO` & `cuenca_validations-0.9.9.dev2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cuenca-validations
-Version: 0.9.9.dev1
+Name: cuenca_validations
+Version: 0.9.9.dev2
 Summary: Cuenca common validations
 Home-page: https://github.com/cuenca-mx/cuenca-validations
 Author: Cuenca
 Author-email: dev@cuenca.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cuenca_validations-0.9.9.dev1/cuenca_validations.egg-info/SOURCES.txt` & `cuenca_validations-0.9.9.dev2/cuenca_validations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/setup.py` & `cuenca_validations-0.9.9.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/tests/test_card.py` & `cuenca_validations-0.9.9.dev2/tests/test_card.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/tests/test_statement.py` & `cuenca_validations-0.9.9.dev2/tests/test_statement.py`

 * *Files identical despite different names*

### Comparing `cuenca_validations-0.9.9.dev1/tests/test_types.py` & `cuenca_validations-0.9.9.dev2/tests/test_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     SantizedDict,
     TransactionStatus,
     digits,
 )
 from cuenca_validations.types.requests import (
     ApiKeyUpdateRequest,
     ChargeRequest,
+    SavingRequest,
     UserCardNotificationRequest,
     UserCredentialUpdateRequest,
 )
 
 today = dt.date.today()
 now = dt.datetime.now()
 utcnow = now.astimezone(dt.timezone.utc)
@@ -219,7 +220,28 @@
     # invalid fields
     data['atm_fee'] = -1
     with pytest.raises(ValidationError):
         ChargeRequest(**data)
     data['amount'] = -1
     with pytest.raises(ValidationError):
         UserCardNotificationRequest(**data)
+
+
+def test_saving_request():
+    dt_now = dt.datetime.now()
+    data = dict(
+        name='Mi depa',
+        category='vehicle',
+        currency='mxn',
+        amount=66600,
+        end_date=dt_now + dt.timedelta(days=1),
+    )
+    SavingRequest(**data)
+
+    data['amount'] = -1000
+    with pytest.raises(ValidationError):
+        SavingRequest(**data)
+
+    data['amount'] = 66600
+    data['end_date'] = dt_now
+    with pytest.raises(ValidationError):
+        SavingRequest(**data)
```

