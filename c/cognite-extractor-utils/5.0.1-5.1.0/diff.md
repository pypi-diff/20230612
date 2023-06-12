# Comparing `tmp/cognite_extractor_utils-5.0.1.tar.gz` & `tmp/cognite_extractor_utils-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-5.0.1.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-5.1.0.tar", max compression
```

## Comparing `cognite_extractor_utils-5.0.1.tar` & `cognite_extractor_utils-5.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10173 2023-05-31 10:34:47.101698 cognite_extractor_utils-5.0.1/LICENSE
--rw-r--r--   0        0        0     4091 2023-05-31 10:34:47.101698 cognite_extractor_utils-5.0.1/README.md
--rw-r--r--   0        0        0      739 2023-05-31 10:34:47.101698 cognite_extractor_utils-5.0.1/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-31 10:34:47.101698 cognite_extractor_utils-5.0.1/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    15990 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     2861 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4294 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    18506 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0     9188 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1061 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    14604 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0     1005 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/middleware.py
--rw-r--r--   0        0        0        0 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    17449 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3054 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     5240 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3865 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     5292 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    11351 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     6888 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    25071 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7404 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1146 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    13352 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     1650 2023-05-31 10:34:47.105698 cognite_extractor_utils-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/LICENSE
+-rw-r--r--   0        0        0     4091 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/README.md
+-rw-r--r--   0        0        0      739 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    15990 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     2861 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4294 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    19616 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0     9188 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1061 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    14604 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0     1005 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-12 12:33:44.287061 cognite_extractor_utils-5.1.0/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    17449 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3054 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5240 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3865 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5292 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    11351 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6888 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    25071 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7404 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1146 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    13352 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     1650 2023-06-12 12:33:44.291061 cognite_extractor_utils-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.1.0/PKG-INFO
```

### Comparing `cognite_extractor_utils-5.0.1/LICENSE` & `cognite_extractor_utils-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/README.md` & `cognite_extractor_utils-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "5.0.1"
+__version__ = "5.1.0"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/base.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,30 @@
     audience: Optional[str] = None
     authority: str = "https://login.microsoftonline.com/"
     min_ttl: float = 30  # minimum time to live: refresh token ahead of expiration
     certificate: Optional[CertificateConfig] = None
 
 
 @dataclass
+class ConnectionConfig:
+    """
+    Configuration parameters for the global_config python SDK settings
+    """
+
+    disable_gzip: bool = False
+    status_forcelist: List[int] = field(default_factory=lambda: [429, 502, 503, 504])
+    max_retries: int = 10
+    max_retries_connect: int = 3
+    max_retry_backoff: int = 30
+    max_connection_pool_size: int = 50
+    disable_ssl: bool = False
+    proxies: Dict[str, str] = field(default_factory=dict)
+
+
+@dataclass
 class EitherIdConfig:
     id: Optional[int]
     external_id: Optional[str]
 
     @property
     def either_id(self) -> EitherId:
         return EitherId(id=self.id, external_id=self.external_id)
@@ -216,23 +232,32 @@
     project: str
     idp_authentication: AuthenticatorConfig
     data_set: Optional[EitherIdConfig]
     data_set_id: Optional[int]
     data_set_external_id: Optional[str]
     extraction_pipeline: Optional[EitherIdConfig]
     timeout: TimeIntervalConfig = TimeIntervalConfig("30s")
+    connection: ConnectionConfig = field(default_factory=ConnectionConfig)
     external_id_prefix: str = ""
     host: str = "https://api.cognitedata.com"
 
     def get_cognite_client(
         self, client_name: str, token_custom_args: Optional[Dict[str, str]] = None, use_experimental_sdk=False
     ) -> CogniteClient:
         from cognite.client.config import global_config
 
         global_config.disable_pypi_version_check = True
+        global_config.disable_gzip = self.connection.disable_gzip
+        global_config.status_forcelist = set(self.connection.status_forcelist)
+        global_config.max_retries = self.connection.max_retries
+        global_config.max_retries_connect = self.connection.max_retries_connect
+        global_config.max_retry_backoff = self.connection.max_retry_backoff
+        global_config.max_connection_pool_size = self.connection.max_connection_pool_size
+        global_config.disable_ssl = self.connection.disable_ssl
+        global_config.proxies = self.connection.proxies
 
         if self.idp_authentication.certificate:
             if self.idp_authentication.certificate.authority_url:
                 authority_url = self.idp_authentication.certificate.authority_url
             elif self.idp_authentication.tenant:
                 authority_url = urljoin(self.idp_authentication.authority, self.idp_authentication.tenant)
             else:
```

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/middleware.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/middleware.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/statestore.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/_metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/events.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/files.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/cognite/extractorutils/util.py` & `cognite_extractor_utils-5.1.0/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.0.1/pyproject.toml` & `cognite_extractor_utils-5.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "5.0.1"
+version = "5.1.0"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
```

### Comparing `cognite_extractor_utils-5.0.1/PKG-INFO` & `cognite_extractor_utils-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 5.0.1
+Version: 5.1.0
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.0.1 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.1.0 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

