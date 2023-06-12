# Comparing `tmp/pyntelope-0.8.5.tar.gz` & `tmp/pyntelope-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntelope-0.8.5.tar", max compression
+gzip compressed data, was "pyntelope-0.8.6.tar", max compression
```

## Comparing `pyntelope-0.8.5.tar` & `pyntelope-0.8.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-01-09 20:18:32.312701 pyntelope-0.8.5/LICENSE
--rw-r--r--   0        0        0     4618 2023-01-09 20:18:32.328702 pyntelope-0.8.5/README.md
--rw-r--r--   0        0        0      133 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/__init__.py
--rw-r--r--   0        0        0      115 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/_version.py
--rw-r--r--   0        0        0      484 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/exc.py
--rw-r--r--   0        0        0    10575 2023-05-30 02:49:12.304752 pyntelope-0.8.5/pyntelope/net.py
--rw-r--r--   0        0        0    10203 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/transaction.py
--rw-r--r--   0        0        0      933 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/__init__.py
--rw-r--r--   0        0        0      875 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/base.py
--rw-r--r--   0        0        0    11680 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/compostes.py
--rw-r--r--   0        0        0    17252 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/primitives.py
--rw-r--r--   0        0        0     8414 2023-03-27 18:18:22.970029 pyntelope-0.8.5/pyntelope/utils.py
--rw-r--r--   0        0        0      934 2023-05-30 02:51:18.085364 pyntelope-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     5287 1970-01-01 00:00:00.000000 pyntelope-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-09 20:18:32.312701 pyntelope-0.8.6/LICENSE
+-rw-r--r--   0        0        0     4736 2023-06-10 20:22:25.219806 pyntelope-0.8.6/README.md
+-rw-r--r--   0        0        0      133 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/__init__.py
+-rw-r--r--   0        0        0      115 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/_version.py
+-rw-r--r--   0        0        0      484 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/exc.py
+-rw-r--r--   0        0        0    12272 2023-06-11 21:32:07.421558 pyntelope-0.8.6/pyntelope/net.py
+-rw-r--r--   0        0        0    10203 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/transaction.py
+-rw-r--r--   0        0        0      933 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/types/__init__.py
+-rw-r--r--   0        0        0      875 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/types/base.py
+-rw-r--r--   0        0        0    11680 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/types/compostes.py
+-rw-r--r--   0        0        0    17252 2023-01-09 20:18:32.316702 pyntelope-0.8.6/pyntelope/types/primitives.py
+-rw-r--r--   0        0        0     8414 2023-03-27 18:18:22.970029 pyntelope-0.8.6/pyntelope/utils.py
+-rw-r--r--   0        0        0      978 2023-06-12 00:51:08.955347 pyntelope-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     5405 1970-01-01 00:00:00.000000 pyntelope-0.8.6/PKG-INFO
```

### Comparing `pyntelope-0.8.5/LICENSE` & `pyntelope-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.5/README.md` & `pyntelope-0.8.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -124,10 +124,15 @@
 #### Run tests
 The tests are run against a local network.  
 Before running the tests you'll need to `docker-compose up` to create the local network, users and contracts used in the tests.  
 When ready, just:
 ```
 pytest
 ```
+Some tests are marked as "slow".  
+You can skip them and run the test suite faster with:
+```
+pytest -m "not slow"
+```
```

### Comparing `pyntelope-0.8.5/pyntelope/net.py` & `pyntelope-0.8.6/pyntelope/net.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 Nodeos api reference:
 https://developers.eos.io/manuals/eos/latest/nodeos/plugins/chain_api_plugin/api-reference/index
 """
 
 import base64
 import logging
-import typing
+import types
+from typing import Optional, Type, Union
 from urllib.parse import urljoin
 
 import httpx
 import pydantic
 
 from pyntelope import exc
 from pyntelope._version import __version__
@@ -22,39 +23,86 @@
     "The abi_bin_to_json and abi_json_to_bin conversion APIs are "
     "both deprecated as of the Leap v3.1 release. "
     "(https://eosnetwork.com/blog/leap-v3-1-release-features/)"
     "They will also be removed from pyntelope in a future version."
 )
 
 
-class Net(pydantic.BaseModel):
+class Net:
     """
-    The net hold the connection information with the blockchain network api.
-    """  # NOQA: D200
+    A Net is an interface to the blockchain network api.
 
-    host: pydantic.AnyHttpUrl
-    headers: dict = {}
+    It holds the connection information and methods for some of its endpoints
+    host: any http url
+        the address of the host you're connecting to
+    headers: dict
+        optional if you want to send a custom header in the request
+    auth: tuple
+        optional if your host requires basic http authentication
+    """
+
+    def __init__(
+        self,
+        *,
+        host: str,
+        headers: dict = dict(),
+        auth: Optional[tuple] = None,
+        client: Optional[Union[httpx.Client, httpx.AsyncClient]] = None,
+    ):
+        pydantic.parse_obj_as(pydantic.AnyHttpUrl, host)
+        self.host = host
+        self.headers = headers
+        self.auth = auth
+        self.client = client
+
+    def __new__(cls, *args, **kwargs):
+        if hasattr(cls, "default_host"):
+
+            def __init__(
+                self,
+                *,
+                host: str = cls.default_host,
+                headers: dict = dict(),
+                auth: Optional[tuple] = None,
+                client: Optional[
+                    Union[httpx.Client, httpx.AsyncClient]
+                ] = None,
+            ):
+                pydantic.parse_obj_as(pydantic.AnyHttpUrl, host)
+                self.host = host
+                self.headers = headers
+                self.auth = auth
+                self.client = client
+
+            cls.__init__ = __init__
+
+        return super().__new__(cls)
 
     def _request(
         self,
         *,
         endpoint: str,
-        payload: typing.Optional[dict] = dict(),
-        verb: str = "POST",
+        payload: Optional[dict] = dict(),
     ):
         url = urljoin(self.host, endpoint)
 
         headers = {
             "user-agent": f"pyntelope/{__version__}",
             "content-type": "application/json",
         }
         headers.update(self.headers)
 
+        client = self.client
+        if client is None:
+            client = httpx.Client()
+
         try:
-            resp = httpx.post(url, json=payload, headers=headers)
+            resp = client.post(
+                url, json=payload, headers=headers, auth=self.auth
+            )
         except (
             httpx.TimeoutException,
             httpx.NetworkError,
             httpx.WriteError,
         ) as e:
             raise exc.ConnectionError(
                 response=None, url=url, payload=payload, error=e
@@ -278,65 +326,78 @@
             compression=compression,
             packed_context_free_data=packed_context_free_data,
             packed_trx=transaction.pack(),
         )
         data = self._request(endpoint=endpoint, payload=payload)
         return data
 
+    def __enter__(self):
+        if self.client is None:
+            self.client = httpx.Client()
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]] = None,
+        exc_value: Optional[BaseException] = None,
+        traceback: Optional[types.TracebackType] = None,
+    ) -> None:
+        self.client.__exit__(exc_type, exc_value, traceback)
+
 
 class WaxTestnet(Net):
-    host: pydantic.HttpUrl = "https://testnet.wax.detroitledger.tech"
+    default_host = "https://testnet.wax.detroitledger.tech"
 
 
 class WaxMainnet(Net):
-    host: pydantic.HttpUrl = "https://api.wax.detroitledger.tech"
+    default_host = "https://api.wax.detroitledger.tech"
 
 
 class EosMainnet(Net):
-    host: pydantic.HttpUrl = "https://api.eos.detroitledger.tech"
+    default_host = "https://api.eos.detroitledger.tech"
 
 
 class KylinTestnet(Net):
-    host: pydantic.HttpUrl = "https://kylin.eossweden.org"
+    default_host = "https://kylin.eossweden.org"
 
 
 class Jungle3Testnet(Net):
-    host: pydantic.HttpUrl = "https://jungle3.eossweden.org"
+    default_host = "https://jungle3.eossweden.org"
 
 
 class Jungle4Testnet(Net):
-    host: pydantic.HttpUrl = "https://jungle4.api.eosnation.io"
+    default_host = "https://jungle4.api.eosnation.io"
 
 
 class TelosMainnet(Net):
-    host: pydantic.HttpUrl = "https://telos.caleos.io/"
+    default_host = "https://telos.caleos.io/"
 
 
 class TelosTestnet(Net):
-    host: pydantic.HttpUrl = "https://testnet.telos.detroitledger.tech"
+    default_host = "https://testnet.telos.detroitledger.tech"
 
 
 class ProtonMainnet(Net):
-    host: pydantic.HttpUrl = "https://proton.cryptolions.io"
+    default_host = "https://proton.cryptolions.io"
 
 
 class ProtonTestnet(Net):
-    host: pydantic.HttpUrl = "https://testnet.protonchain.com"
+    default_host = "https://testnet.protonchain.com"
 
 
 class UosMainnet(Net):
-    host: pydantic.HttpUrl = "https://uos.eosusa.news"
+    default_host = "https://uos.eosusa.news"
 
 
 class FioMainnet(Net):
-    host: pydantic.HttpUrl = "https://fio.cryptolions.io"
+    default_host = "https://fio.cryptolions.io"
 
 
 class Local(Net):
-    host: pydantic.HttpUrl = "http://127.0.0.1:8888"
+    default_host = "http://127.0.0.1:8888"
 
 
 __all__ = [
     "Net",
     "EosMainnet",
     "KylinTestnet",
     "Jungle3Testnet",
```

### Comparing `pyntelope-0.8.5/pyntelope/transaction.py` & `pyntelope-0.8.6/pyntelope/transaction.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.5/pyntelope/types/__init__.py` & `pyntelope-0.8.6/pyntelope/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.5/pyntelope/types/base.py` & `pyntelope-0.8.6/pyntelope/types/base.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.5/pyntelope/types/compostes.py` & `pyntelope-0.8.6/pyntelope/types/compostes.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.5/pyntelope/types/primitives.py` & `pyntelope-0.8.6/pyntelope/types/primitives.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.5/pyntelope/utils.py` & `pyntelope-0.8.6/pyntelope/utils.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.5/pyproject.toml` & `pyntelope-0.8.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyntelope"
-version = "0.8.5"
+version = "0.8.6"
 description = "Interact with Antelope blockchains"
 authors = ["Team <pyntelope@facings.io>"]
 homepage = "https://github.com/FACINGS/pyntelope"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -30,13 +30,14 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-vvv --cov-report=term-missing --cov=pyntelope"
 testpaths = ["tests/unit"]
 log_level = "DEBUG"
+markers = "slow: these tests are very slow"
 
 [tool.black]
 line-length = 79
 
 [tool.pydocstyle]
 match_dir = '^(?!tests)[^\.].+$'
```

### Comparing `pyntelope-0.8.5/PKG-INFO` & `pyntelope-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntelope
-Version: 0.8.5
+Version: 0.8.6
 Summary: Interact with Antelope blockchains
 Home-page: https://github.com/FACINGS/pyntelope
 Author: Team
 Author-email: pyntelope@facings.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -143,11 +143,16 @@
 #### Run tests
 The tests are run against a local network.  
 Before running the tests you'll need to `docker-compose up` to create the local network, users and contracts used in the tests.  
 When ready, just:
 ```
 pytest
 ```
+Some tests are marked as "slow".  
+You can skip them and run the test suite faster with:
+```
+pytest -m "not slow"
+```
```

