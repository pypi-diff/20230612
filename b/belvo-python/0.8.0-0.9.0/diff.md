# Comparing `tmp/belvo-python-0.8.0.tar.gz` & `tmp/belvo-python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/belvo-python-0.8.0.tar", last modified: Mon Feb 17 15:56:43 2020, max compression
+gzip compressed data, was "dist/belvo-python-0.9.0.tar", last modified: Mon Feb 24 12:34:58 2020, max compression
```

## Comparing `belvo-python-0.8.0.tar` & `belvo-python-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 menecio   (1000) menecio   (1000)        0 2020-02-17 15:56:43.000000 belvo-python-0.8.0/
--rw-r--r--   0 menecio   (1000) menecio   (1000)     1058 2020-01-20 15:59:17.000000 belvo-python-0.8.0/LICENSE
--rw-r--r--   0 menecio   (1000) menecio   (1000)      342 2020-01-20 15:59:17.000000 belvo-python-0.8.0/MANIFEST.in
--rw-rw-r--   0 menecio   (1000) menecio   (1000)     3118 2020-02-17 15:56:43.000000 belvo-python-0.8.0/PKG-INFO
--rw-rw-r--   0 menecio   (1000) menecio   (1000)     1733 2020-02-17 15:46:01.000000 belvo-python-0.8.0/README.md
-drwxrwxr-x   0 menecio   (1000) menecio   (1000)        0 2020-02-17 15:56:43.000000 belvo-python-0.8.0/belvo/
--rw-rw-r--   0 menecio   (1000) menecio   (1000)       22 2020-02-17 15:55:09.000000 belvo-python-0.8.0/belvo/__init__.py
--rw-r--r--   0 menecio   (1000) menecio   (1000)     1453 2020-01-20 15:59:17.000000 belvo-python-0.8.0/belvo/client.py
--rw-rw-r--   0 menecio   (1000) menecio   (1000)      233 2020-02-17 15:46:01.000000 belvo-python-0.8.0/belvo/exceptions.py
--rw-rw-r--   0 menecio   (1000) menecio   (1000)     3688 2020-02-17 15:46:01.000000 belvo-python-0.8.0/belvo/http.py
--rw-rw-r--   0 menecio   (1000) menecio   (1000)     7001 2020-02-17 15:46:01.000000 belvo-python-0.8.0/belvo/resources.py
-drwxrwxr-x   0 menecio   (1000) menecio   (1000)        0 2020-02-17 15:56:43.000000 belvo-python-0.8.0/belvo_python.egg-info/
--rw-rw-r--   0 menecio   (1000) menecio   (1000)     3118 2020-02-17 15:56:42.000000 belvo-python-0.8.0/belvo_python.egg-info/PKG-INFO
--rw-rw-r--   0 menecio   (1000) menecio   (1000)      442 2020-02-17 15:56:42.000000 belvo-python-0.8.0/belvo_python.egg-info/SOURCES.txt
--rw-rw-r--   0 menecio   (1000) menecio   (1000)        1 2020-02-17 15:56:42.000000 belvo-python-0.8.0/belvo_python.egg-info/dependency_links.txt
--rw-rw-r--   0 menecio   (1000) menecio   (1000)        1 2020-01-20 17:10:24.000000 belvo-python-0.8.0/belvo_python.egg-info/not-zip-safe
--rw-rw-r--   0 menecio   (1000) menecio   (1000)       15 2020-02-17 15:56:42.000000 belvo-python-0.8.0/belvo_python.egg-info/requires.txt
--rw-rw-r--   0 menecio   (1000) menecio   (1000)        6 2020-02-17 15:56:42.000000 belvo-python-0.8.0/belvo_python.egg-info/top_level.txt
-drwxrwxr-x   0 menecio   (1000) menecio   (1000)        0 2020-02-17 15:56:43.000000 belvo-python-0.8.0/requirements/
--rw-r--r--   0 menecio   (1000) menecio   (1000)       15 2020-01-20 15:59:17.000000 belvo-python-0.8.0/requirements/base.txt
--rw-r--r--   0 menecio   (1000) menecio   (1000)       57 2020-01-20 15:59:17.000000 belvo-python-0.8.0/requirements/documentation.txt
--rw-r--r--   0 menecio   (1000) menecio   (1000)       49 2020-01-20 15:59:17.000000 belvo-python-0.8.0/requirements/linting.txt
--rw-r--r--   0 menecio   (1000) menecio   (1000)      121 2020-01-20 15:59:17.000000 belvo-python-0.8.0/requirements/testing.txt
--rw-rw-r--   0 menecio   (1000) menecio   (1000)       38 2020-02-17 15:56:43.000000 belvo-python-0.8.0/setup.cfg
--rw-r--r--   0 menecio   (1000) menecio   (1000)      574 2020-01-20 15:59:17.000000 belvo-python-0.8.0/setup.py
+drwxr-xr-x   0 jordi     (1001) jordi     (1001)        0 2020-02-24 12:34:58.764541 belvo-python-0.9.0/
+-rw-r--r--   0 jordi     (1001) jordi     (1001)     1058 2020-02-24 08:17:32.000000 belvo-python-0.9.0/LICENSE
+-rw-r--r--   0 jordi     (1001) jordi     (1001)      342 2020-02-24 08:17:32.000000 belvo-python-0.9.0/MANIFEST.in
+-rw-r--r--   0 jordi     (1001) jordi     (1001)     3118 2020-02-24 12:34:58.764541 belvo-python-0.9.0/PKG-INFO
+-rw-r--r--   0 jordi     (1001) jordi     (1001)     1733 2020-02-24 08:17:32.000000 belvo-python-0.9.0/README.md
+drwxr-xr-x   0 jordi     (1001) jordi     (1001)        0 2020-02-24 12:34:58.764541 belvo-python-0.9.0/belvo/
+-rw-r--r--   0 jordi     (1001) jordi     (1001)       22 2020-02-24 10:49:24.000000 belvo-python-0.9.0/belvo/__init__.py
+-rw-r--r--   0 jordi     (1001) jordi     (1001)     1617 2020-02-24 10:49:24.000000 belvo-python-0.9.0/belvo/client.py
+-rw-r--r--   0 jordi     (1001) jordi     (1001)      233 2020-02-24 08:17:32.000000 belvo-python-0.9.0/belvo/exceptions.py
+-rw-r--r--   0 jordi     (1001) jordi     (1001)     3688 2020-02-24 08:17:32.000000 belvo-python-0.9.0/belvo/http.py
+-rw-r--r--   0 jordi     (1001) jordi     (1001)     7894 2020-02-24 10:49:24.000000 belvo-python-0.9.0/belvo/resources.py
+drwxr-xr-x   0 jordi     (1001) jordi     (1001)        0 2020-02-24 12:34:58.764541 belvo-python-0.9.0/belvo_python.egg-info/
+-rw-r--r--   0 jordi     (1001) jordi     (1001)     3118 2020-02-24 12:34:58.000000 belvo-python-0.9.0/belvo_python.egg-info/PKG-INFO
+-rw-r--r--   0 jordi     (1001) jordi     (1001)      442 2020-02-24 12:34:58.000000 belvo-python-0.9.0/belvo_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jordi     (1001) jordi     (1001)        1 2020-02-24 12:34:58.000000 belvo-python-0.9.0/belvo_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jordi     (1001) jordi     (1001)        1 2020-02-24 08:19:02.000000 belvo-python-0.9.0/belvo_python.egg-info/not-zip-safe
+-rw-r--r--   0 jordi     (1001) jordi     (1001)       15 2020-02-24 12:34:58.000000 belvo-python-0.9.0/belvo_python.egg-info/requires.txt
+-rw-r--r--   0 jordi     (1001) jordi     (1001)        6 2020-02-24 12:34:58.000000 belvo-python-0.9.0/belvo_python.egg-info/top_level.txt
+drwxr-xr-x   0 jordi     (1001) jordi     (1001)        0 2020-02-24 12:34:58.764541 belvo-python-0.9.0/requirements/
+-rw-r--r--   0 jordi     (1001) jordi     (1001)       15 2020-02-24 08:17:32.000000 belvo-python-0.9.0/requirements/base.txt
+-rw-r--r--   0 jordi     (1001) jordi     (1001)       57 2020-02-24 08:17:32.000000 belvo-python-0.9.0/requirements/documentation.txt
+-rw-r--r--   0 jordi     (1001) jordi     (1001)       49 2020-02-24 08:17:32.000000 belvo-python-0.9.0/requirements/linting.txt
+-rw-r--r--   0 jordi     (1001) jordi     (1001)      121 2020-02-24 08:17:32.000000 belvo-python-0.9.0/requirements/testing.txt
+-rw-r--r--   0 jordi     (1001) jordi     (1001)       38 2020-02-24 12:34:58.764541 belvo-python-0.9.0/setup.cfg
+-rw-r--r--   0 jordi     (1001) jordi     (1001)      574 2020-02-24 08:17:32.000000 belvo-python-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `belvo-python-0.8.0/LICENSE` & `belvo-python-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `belvo-python-0.8.0/PKG-INFO` & `belvo-python-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvo-python
-Version: 0.8.0
+Version: 0.9.0
 Summary: Belvo Python SDK
 Home-page: https://github.com/belvo-finance/belvo-python
 Author: Belvo Finance, S.L.
 Author-email: hello@belvo.co
 License: UNKNOWN
 Download-URL: https://github.com/belvo-finance/belvo-python/tarball/master
 Description: <h1 align="center">Belvo Python SDK</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: belvo-python Version: 0.8.0 Summary: Belvo Python
+Metadata-Version: 2.1 Name: belvo-python Version: 0.9.0 Summary: Belvo Python
 SDK Home-page: https://github.com/belvo-finance/belvo-python Author: Belvo
 Finance, S.L. Author-email: hello@belvo.co License: UNKNOWN Download-URL:
 https://github.com/belvo-finance/belvo-python/tarball/master Description:
                         ****** Belvo Python SDK ******
          [PyPI] [PyPI_-_Downloads] [Travis_(.com)] [Coveralls_github]
                        Developers_portal | Documentation
 ## ð Requirements * Python 3.6+ ## ð Getting started Install using `pip`:
```

### Comparing `belvo-python-0.8.0/README.md` & `belvo-python-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `belvo-python-0.8.0/belvo/client.py` & `belvo-python-0.9.0/belvo/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import os
 
 from .exceptions import BelvoAPIException
 from .http import APISession
-from .resources import Accounts, Institutions, Invoices, Links, Owners, TaxReturns, Transactions
+from .resources import (
+    Accounts,
+    Balances,
+    Institutions,
+    Invoices,
+    Links,
+    Owners,
+    TaxReturns,
+    Transactions,
+)
 
 
 class Client:
     def __init__(self, secret_key_id: str, secret_key_password: str, url: str = None) -> None:
         if url is None:
             url = os.getenv("BELVO_API_URL")
 
@@ -17,14 +26,15 @@
 
         if not self.session.login(secret_key_id, secret_key_password):
             raise BelvoAPIException("Login failed.")
 
         self._links = Links(self.session)
         self._accounts = Accounts(self.session)
         self._transactions = Transactions(self.session)
+        self._balances = Balances(self.session)
         self._institutions = Institutions(self.session)
         self._owners = Owners(self.session)
         self._invoices = Invoices(self.session)
         self._tax_returns = TaxReturns(self.session)
 
     @property
     def Links(self):
@@ -35,14 +45,18 @@
         return self._accounts
 
     @property
     def Transactions(self):
         return self._transactions
 
     @property
+    def Balances(self):
+        return self._balances
+
+    @property
     def Institutions(self):
         return self._institutions
 
     @property
     def Owners(self):
         return self._owners
```

### Comparing `belvo-python-0.8.0/belvo/http.py` & `belvo-python-0.9.0/belvo/http.py`

 * *Files identical despite different names*

### Comparing `belvo-python-0.8.0/belvo/resources.py` & `belvo-python-0.9.0/belvo/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,14 +150,48 @@
             data.update(encryption_key=encryption_key)
 
         return self.session.post(
             self.endpoint, data=data, raise_exception=raise_exception, **kwargs
         )
 
 
+class Balances(Resource):
+    endpoint = "/api/balances/"
+
+    def create(
+        self,
+        link: str,
+        date_from: str,
+        *,
+        date_to: str = None,
+        account: str = None,
+        token: str = None,
+        encryption_key: str = None,
+        save_data: bool = True,
+        raise_exception: bool = False,
+        **kwargs: str,
+    ) -> Union[List[Dict], Dict]:
+
+        if date_to is None:
+            date_to = date.today().isoformat()
+
+        data = {"link": link, "date_from": date_from, "date_to": date_to, "save_data": save_data}
+
+        if account:
+            data.update(account=account)
+        if token:
+            data.update(token=token)
+        if encryption_key:
+            data.update(encryption_key=encryption_key)
+
+        return self.session.post(
+            self.endpoint, data=data, raise_exception=raise_exception, **kwargs
+        )
+
+
 class Institutions(Resource):
     endpoint = "/api/institutions/"
 
     def delete(self, id: str) -> bool:
         raise NotImplementedError()
 
     def resume(
```

### Comparing `belvo-python-0.8.0/belvo_python.egg-info/PKG-INFO` & `belvo-python-0.9.0/belvo_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: belvo-python
-Version: 0.8.0
+Version: 0.9.0
 Summary: Belvo Python SDK
 Home-page: https://github.com/belvo-finance/belvo-python
 Author: Belvo Finance, S.L.
 Author-email: hello@belvo.co
 License: UNKNOWN
 Download-URL: https://github.com/belvo-finance/belvo-python/tarball/master
 Description: <h1 align="center">Belvo Python SDK</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: belvo-python Version: 0.8.0 Summary: Belvo Python
+Metadata-Version: 2.1 Name: belvo-python Version: 0.9.0 Summary: Belvo Python
 SDK Home-page: https://github.com/belvo-finance/belvo-python Author: Belvo
 Finance, S.L. Author-email: hello@belvo.co License: UNKNOWN Download-URL:
 https://github.com/belvo-finance/belvo-python/tarball/master Description:
                         ****** Belvo Python SDK ******
          [PyPI] [PyPI_-_Downloads] [Travis_(.com)] [Coveralls_github]
                        Developers_portal | Documentation
 ## ð Requirements * Python 3.6+ ## ð Getting started Install using `pip`:
```

### Comparing `belvo-python-0.8.0/setup.py` & `belvo-python-0.9.0/setup.py`

 * *Files identical despite different names*

