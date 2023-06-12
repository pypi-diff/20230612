# Comparing `tmp/pyfusion-1.0.8.tar.gz` & `tmp/pyfusion-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfusion-1.0.8.tar", max compression
+gzip compressed data, was "pyfusion-1.0.9.tar", max compression
```

## Comparing `pyfusion-1.0.8.tar` & `pyfusion-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      575 2023-01-20 04:07:27.174304 pyfusion-1.0.8/LICENSE
--rw-r--r--   0        0        0      897 2023-01-20 04:07:27.174304 pyfusion-1.0.8/README.md
--rw-r--r--   0        0        0      188 2023-01-20 04:07:27.174304 pyfusion-1.0.8/fusion/__init__.py
--rw-r--r--   0        0        0    18033 2023-01-20 04:07:27.174304 pyfusion-1.0.8/fusion/authentication.py
--rw-r--r--   0        0        0      960 2023-01-20 04:07:27.174304 pyfusion-1.0.8/fusion/exceptions.py
--rw-r--r--   0        0        0     9469 2023-01-20 04:07:27.178305 pyfusion-1.0.8/fusion/fs_sync.py
--rwxr-xr-x   0        0        0    31041 2023-01-20 04:07:27.178305 pyfusion-1.0.8/fusion/fusion.py
--rw-r--r--   0        0        0    13598 2023-01-20 04:07:27.178305 pyfusion-1.0.8/fusion/fusion_filesystem.py
--rw-r--r--   0        0        0    18153 2023-01-20 04:07:27.178305 pyfusion-1.0.8/fusion/utils.py
--rw-r--r--   0        0        0     3678 2023-01-20 04:07:27.178305 pyfusion-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       36 2023-01-20 04:07:27.178305 pyfusion-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0     3675 2023-01-20 04:07:27.178305 pyfusion-1.0.8/tests/conftest.py
--rw-r--r--   0        0        0     4622 2023-01-20 04:07:27.178305 pyfusion-1.0.8/tests/test_fusion.py
--rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 pyfusion-1.0.8/setup.py
--rw-r--r--   0        0        0     3947 1970-01-01 00:00:00.000000 pyfusion-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      575 2023-01-25 12:50:19.599452 pyfusion-1.0.9/LICENSE
+-rw-r--r--   0        0        0      897 2023-01-25 12:50:19.599452 pyfusion-1.0.9/README.md
+-rw-r--r--   0        0        0      188 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/__init__.py
+-rw-r--r--   0        0        0    18351 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/authentication.py
+-rw-r--r--   0        0        0      960 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/exceptions.py
+-rw-r--r--   0        0        0    10005 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/fs_sync.py
+-rwxr-xr-x   0        0        0    32117 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/fusion.py
+-rw-r--r--   0        0        0    13986 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/fusion_filesystem.py
+-rw-r--r--   0        0        0    18532 2023-01-25 12:50:19.603452 pyfusion-1.0.9/fusion/utils.py
+-rw-r--r--   0        0        0     3473 2023-01-25 12:50:19.603452 pyfusion-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-01-25 12:50:19.603452 pyfusion-1.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3675 2023-01-25 12:50:19.603452 pyfusion-1.0.9/tests/conftest.py
+-rw-r--r--   0        0        0     4793 2023-01-25 12:50:19.603452 pyfusion-1.0.9/tests/test_fusion.py
+-rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 pyfusion-1.0.9/setup.py
+-rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 pyfusion-1.0.9/PKG-INFO
```

### Comparing `pyfusion-1.0.8/LICENSE` & `pyfusion-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfusion-1.0.8/README.md` & `pyfusion-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyfusion-1.0.8/fusion/authentication.py` & `pyfusion-1.0.9/fusion/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """Fusion authentication module."""
 
 import datetime
 import json
 import logging
+import os
 from datetime import timedelta
 from pathlib import Path
 from typing import Dict, Union
 from urllib.parse import urlparse
+
 import fsspec
-import os
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from .exceptions import CredentialError
 
 logger = logging.getLogger(__name__)
 VERBOSE_LVL = 25
 
 
-def _res_plural(ref_int: int, pluraliser: str = 's') -> str:
+def _res_plural(ref_int: int, pluraliser: str = "s") -> str:
     """Private function to return the plural form when the number is more than one.
 
     Args:
         ref_int (int): The reference integer that determines whether to return a plural suffix.
         pluraliser (str, optional): The plural suffix. Defaults to "s".
 
     Returns:
         str: The plural suffix to append to a string.
     """
-    return '' if abs(ref_int) == 1 else pluraliser
+    return "" if abs(ref_int) == 1 else pluraliser
 
 
 def _is_json(data: str) -> bool:
     """Test whether the content of a string is a JSON object.
 
     Args:
         data (str): The content to evaluate.
@@ -66,19 +67,21 @@
 
 def get_default_fs():
     """Retrieve default filesystem.
 
     Returns: filesystem
 
     """
-    protocol = "file" if "FS_PROTOCOL" not in os.environ.keys() else os.environ["FS_PROTOCOL"]
+    protocol = (
+        "file" if "FS_PROTOCOL" not in os.environ.keys() else os.environ["FS_PROTOCOL"]
+    )
     if (
-            "S3_ENDPOINT" in os.environ.keys()
-            and "AWS_ACCESS_KEY_ID" in os.environ.keys()
-            and "AWS_SECRET_ACCESS_KEY" in os.environ.keys()
+        "S3_ENDPOINT" in os.environ.keys()
+        and "AWS_ACCESS_KEY_ID" in os.environ.keys()
+        and "AWS_SECRET_ACCESS_KEY" in os.environ.keys()
     ):
         endpoint = os.environ["S3_ENDPOINT"]
         fs = fsspec.filesystem(
             "s3",
             client_kwargs={"endpoint_url": f"https://{endpoint}"},
             key=os.environ["AWS_ACCESS_KEY_ID"],
             secret=os.environ["AWS_SECRET_ACCESS_KEY"],
@@ -88,23 +91,23 @@
     return fs
 
 
 class FusionCredentials:
     """Utility functions to manage credentials."""
 
     def __init__(
-            self,
-            client_id: str = None,
-            client_secret: str = None,
-            username: str = None,
-            password: str = None,
-            resource: str = None,
-            auth_url: str = None,
-            proxies={},
-            grant_type: str = 'client_credentials',
+        self,
+        client_id: str = None,
+        client_secret: str = None,
+        username: str = None,
+        password: str = None,
+        resource: str = None,
+        auth_url: str = None,
+        proxies={},
+        grant_type: str = "client_credentials",
     ) -> None:
         """Constructor for the FusionCredentials authentication management class.
 
         Args:
             client_id (str, optional): A valid OAuth client identifier. Defaults to None.
             client_secret (str, optional): A valid OAuth client secret. Defaults to None.
             username (str, optional): A valid username. Defaults to None.
@@ -122,15 +125,17 @@
         self.resource = resource
         self.auth_url = auth_url
         self.proxies = proxies
         self.grant_type = grant_type
 
     @staticmethod
     def add_proxies(
-            http_proxy: str, https_proxy: str = None, credentials_file: str = 'config/client_credentials.json'
+        http_proxy: str,
+        https_proxy: str = None,
+        credentials_file: str = "config/client_credentials.json",
     ) -> None:
         """A function to add proxies to an existing credentials files.
         This function can be called to add proxy addresses to a credential file downloaded from the Fusion website.
 
         Args:
             http_proxy (str): The HTTP proxy address.
             https_proxy (str): The HTTPS proxy address. If not specified then this will be the
@@ -140,43 +145,43 @@
                 Defaults to 'config/client_credentials.json'.
 
         Returns:
             None
         """
 
         credentials = FusionCredentials.from_file(credentials_file)
-        credentials.proxies['http'] = http_proxy
+        credentials.proxies["http"] = http_proxy
         if https_proxy is None:
             https_proxy = http_proxy
 
-        credentials.proxies['https'] = https_proxy
+        credentials.proxies["https"] = https_proxy
 
         data: Dict[str, Union[str, dict]] = dict(
             {
-                'client_id': credentials.client_id,
-                'client_secret': credentials.client_secret,
-                'resource': credentials.resource,
-                'auth_url': credentials.auth_url,
-                'proxies': credentials.proxies,
+                "client_id": credentials.client_id,
+                "client_secret": credentials.client_secret,
+                "resource": credentials.resource,
+                "auth_url": credentials.auth_url,
+                "proxies": credentials.proxies,
             }
         )
         json_data = json.dumps(data, indent=4)
-        with open(credentials_file, 'w') as credentialsfile:
+        with open(credentials_file, "w") as credentialsfile:
             credentialsfile.write(json_data)
 
         return
 
     @staticmethod
     def generate_credentials_file(
-            credentials_file: str = 'config/client_credentials.json',
-            client_id: str = None,
-            client_secret: str = None,
-            resource: str = "JPMC:URI:RS-93742-Fusion-PROD",
-            auth_url: str = "https://authe.jpmorgan.com/as/token.oauth2",
-            proxies: Union[str, dict] = None,
+        credentials_file: str = "config/client_credentials.json",
+        client_id: str = None,
+        client_secret: str = None,
+        resource: str = "JPMC:URI:RS-93742-Fusion-PROD",
+        auth_url: str = "https://authe.jpmorgan.com/as/token.oauth2",
+        proxies: Union[str, dict] = None,
     ):
         """Utility function to generate credentials file that can be used for authentication.
 
         Args:
             credentials_file (str, optional): The path and filename to store the credentials under.
                 Path may be absolute or relative to current working directory.
                 Defaults to 'config/client_credentials.json'.
@@ -191,55 +196,64 @@
         Raises:
             CredentialError: Exception to handle missing values required for authentication.
 
         Returns:
            FusionCredentials: a credentials object that can be used for authentication.
         """
         if not client_id:
-            raise CredentialError('A valid client_id is required')
+            raise CredentialError("A valid client_id is required")
         if not client_secret:
-            raise CredentialError('A valid client secret is required')
+            raise CredentialError("A valid client secret is required")
 
         data: Dict[str, Union[str, dict]] = dict(
-            {'client_id': client_id, 'client_secret': client_secret, 'resource': resource, 'auth_url': auth_url}
+            {
+                "client_id": client_id,
+                "client_secret": client_secret,
+                "resource": resource,
+                "auth_url": auth_url,
+            }
         )
 
         proxies_resolved = {}
         if proxies:
             if isinstance(proxies, dict):
                 raw_proxies_dict = proxies
             elif isinstance(proxies, str):
                 if _is_url(proxies):
-                    raw_proxies_dict = {'http': proxies, 'https': proxies}
+                    raw_proxies_dict = {"http": proxies, "https": proxies}
                 elif _is_json(proxies):
                     raw_proxies_dict = json.loads(proxies)
             else:
-                raise CredentialError(f'A valid proxies param is required, [{proxies}] is not supported.')
+                raise CredentialError(
+                    f"A valid proxies param is required, [{proxies}] is not supported."
+                )
 
             # Now validate and conform proxies dict
-            valid_pxy_keys = ['http', 'https', 'http_proxy', 'https_proxy']
+            valid_pxy_keys = ["http", "https", "http_proxy", "https_proxy"]
             pxy_key_map = {
-                'http': 'http',
-                'https': 'https',
-                'http_proxy': 'http',
-                'https_proxy': 'https',
+                "http": "http",
+                "https": "https",
+                "http_proxy": "http",
+                "https_proxy": "https",
             }
             lcase_dict = {k.lower(): v for k, v in raw_proxies_dict.items()}
 
-            if set(lcase_dict.keys()).intersection(set(valid_pxy_keys)) != set(lcase_dict.keys()):
+            if set(lcase_dict.keys()).intersection(set(valid_pxy_keys)) != set(
+                lcase_dict.keys()
+            ):
                 raise CredentialError(
-                    f'Invalid proxies keys in dict {raw_proxies_dict.keys()}.'
-                    f'Only {pxy_key_map.keys()} are accepted and will be mapped as necessary.'
+                    f"Invalid proxies keys in dict {raw_proxies_dict.keys()}."
+                    f"Only {pxy_key_map.keys()} are accepted and will be mapped as necessary."
                 )
             proxies_resolved = {pxy_key_map[k]: v for k, v in lcase_dict.items()}
 
-        data['proxies'] = proxies_resolved
+        data["proxies"] = proxies_resolved
         json_data = json.dumps(data, indent=4)
         Path(credentials_file).parent.mkdir(parents=True, exist_ok=True)
-        with open(credentials_file, 'w') as credentialsfile:
+        with open(credentials_file, "w") as credentialsfile:
             credentialsfile.write(json_data)
 
         credentials = FusionCredentials.from_file(file_path=credentials_file)
         return credentials
 
     @staticmethod
     def from_dict(credentials: dict):
@@ -251,41 +265,50 @@
         Args:
             credentials (dict): A dictionary containing the requried keys: client_id, client_secret,
                 resource, auth_url, and optionally proxies and an OAuth grant type.
 
         Returns:
             FusionCredentials: a credentials object that can be used for authentication.
         """
-        if 'grant_type' in credentials:
-            grant_type = credentials['grant_type']
+        if "grant_type" in credentials:
+            grant_type = credentials["grant_type"]
         else:
-            grant_type = 'client_credentials'
+            grant_type = "client_credentials"
 
-        client_id = credentials['client_id']
-        if grant_type == 'client_credentials':
-            client_secret = credentials['client_secret']
+        client_id = credentials["client_id"]
+        if grant_type == "client_credentials":
+            client_secret = credentials["client_secret"]
             username = None
             password = None
-        elif grant_type == 'password':
+        elif grant_type == "password":
             client_secret = None
-            username = credentials['username']
-            password = credentials['password']
+            username = credentials["username"]
+            password = credentials["password"]
         else:
-            raise CredentialError(f'Unrecognised grant type {grant_type}')
+            raise CredentialError(f"Unrecognised grant type {grant_type}")
 
-        resource = credentials['resource']
-        auth_url = credentials['auth_url']
-        proxies = credentials.get('proxies')
+        resource = credentials["resource"]
+        auth_url = credentials["auth_url"]
+        proxies = credentials.get("proxies")
         creds = FusionCredentials(
-            client_id, client_secret, username, password, resource, auth_url, proxies, grant_type=grant_type
+            client_id,
+            client_secret,
+            username,
+            password,
+            resource,
+            auth_url,
+            proxies,
+            grant_type=grant_type,
         )
         return creds
 
     @staticmethod
-    def from_file(file_path: str = 'config/client.credentials.json', fs=None, walk_up_dirs=True):
+    def from_file(
+        file_path: str = "config/client.credentials.json", fs=None, walk_up_dirs=True
+    ):
         """Create a credentials object from a file.
 
         Args:
             file_path (str, optional): Path (absolute or relative) and filename
                 to load credentials from. Defaults to 'config/client.credentials.json'.
             fs (fsspec.filesystem): Filesystem to use.
             walk_up_dirs (bool): if true it walks up the directories in search of a config folder
@@ -294,26 +317,30 @@
         """
         fs = fs if fs else get_default_fs()
         to_use_file_path = None
 
         if fs.exists(file_path):  # absolute path case
             logger.log(VERBOSE_LVL, f"Found credentials file at {file_path}")
             to_use_file_path = file_path
-        elif fs.exists(os.path.join(fs.info("")["name"], file_path)):  # relative path case
+        elif fs.exists(
+            os.path.join(fs.info("")["name"], file_path)
+        ):  # relative path case
             to_use_file_path = os.path.join(fs.info("")["name"], file_path)
             logger.log(VERBOSE_LVL, f"Found credentials file at {to_use_file_path}")
         else:
             for p in [s.__str__() for s in Path(fs.info("")["name"]).parents]:
                 if fs.exists(os.path.join(p, file_path)):
                     to_use_file_path = os.path.join(p, file_path)
-                    logger.log(VERBOSE_LVL, f"Found credentials file at {to_use_file_path}")
+                    logger.log(
+                        VERBOSE_LVL, f"Found credentials file at {to_use_file_path}"
+                    )
                     break
         if fs.size(to_use_file_path) > 0:
             try:
-                with fs.open(to_use_file_path, 'r') as credentials:
+                with fs.open(to_use_file_path, "r") as credentials:
                     data = json.load(credentials)
                     credentials = FusionCredentials.from_dict(data)
                     return credentials
             except Exception as e:
                 print(e)
                 logger.error(e)
                 raise Exception(e)
@@ -340,28 +367,30 @@
             return FusionCredentials.from_dict(credentials_source)
         elif isinstance(credentials_source, str):
             if _is_json(credentials_source):
                 return FusionCredentials.from_dict(json.loads(credentials_source))
             else:
                 return FusionCredentials.from_file(credentials_source)
 
-        raise CredentialError(f'Could not resolve the credentials provided: {credentials_source}')
+        raise CredentialError(
+            f"Could not resolve the credentials provided: {credentials_source}"
+        )
 
 
 class FusionOAuthAdapter(HTTPAdapter):
     """An OAuth adapter to manage authentication and session tokens."""
 
     def __init__(
-            self,
-            credentials: Union[FusionCredentials, Union[str, dict]],
-            proxies: dict = {},
-            refresh_within_seconds: int = 5,
-            auth_retries: Union[int, Retry] = None,
-            *args,
-            **kwargs,
+        self,
+        credentials: Union[FusionCredentials, Union[str, dict]],
+        proxies: dict = {},
+        refresh_within_seconds: int = 5,
+        auth_retries: Union[int, Retry] = None,
+        *args,
+        **kwargs,
     ) -> None:
         """Class constructor to create a FusionOAuthAdapter object.
 
         Args:
             credentials (Union[FusionCredentials, Union[str, dict]): Valid user credentials to authenticate.
             proxies (dict, optional): Specify a proxy if required to access the authentication server.
                 Defaults to {}.
@@ -407,45 +436,49 @@
             payload = (
                 {
                     "grant_type": "client_credentials",
                     "client_id": self.credentials.client_id,
                     "client_secret": self.credentials.client_secret,
                     "aud": self.credentials.resource,
                 }
-                if self.credentials.grant_type == 'client_credentials'
+                if self.credentials.grant_type == "client_credentials"
                 else {
                     "grant_type": "password",
                     "client_id": self.credentials.client_id,
                     "username": self.credentials.username,
                     "password": self.credentials.password,
                     "resource": self.credentials.resource,
                 }
             )
 
             try:
                 s = requests.Session()
                 if self.proxies:
                     # mypy does note recognise session.proxies as a dict so fails this line, we'll ignore this chk
                     s.proxies.update(self.proxies)  # type:ignore
-                s.mount('http://', HTTPAdapter(max_retries=self.auth_retries))
+                s.mount("http://", HTTPAdapter(max_retries=self.auth_retries))
                 response = s.post(self.credentials.auth_url, data=payload)
                 response_data = response.json()
                 access_token = response_data["access_token"]
                 expiry = response_data["expires_in"]
                 return access_token, expiry
             except Exception as ex:
-                raise Exception(f'Failed to authenticate against OAuth server {ex}')
+                raise Exception(f"Failed to authenticate against OAuth server {ex}")
 
-        token_expires_in = (self.bearer_token_expiry - datetime.datetime.now()).total_seconds()
+        token_expires_in = (
+            self.bearer_token_expiry - datetime.datetime.now()
+        ).total_seconds()
         if token_expires_in < self.refresh_within_seconds:
             token, expiry = _refresh_token_data()
             self.token = token
-            self.bearer_token_expiry = datetime.datetime.now() + timedelta(seconds=int(expiry))
+            self.bearer_token_expiry = datetime.datetime.now() + timedelta(
+                seconds=int(expiry)
+            )
             self.number_token_refreshes += 1
             logger.log(
                 VERBOSE_LVL,
-                f'Refreshed token {self.number_token_refreshes} time{_res_plural(self.number_token_refreshes)}',
+                f"Refreshed token {self.number_token_refreshes} time{_res_plural(self.number_token_refreshes)}",
             )
 
-        request.headers.update({'Authorization': f'Bearer {self.token}'})
+        request.headers.update({"Authorization": f"Bearer {self.token}"})
         response = super(FusionOAuthAdapter, self).send(request, **kwargs)
         return response
```

### Comparing `pyfusion-1.0.8/fusion/exceptions.py` & `pyfusion-1.0.9/fusion/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfusion-1.0.8/fusion/fs_sync.py` & `pyfusion-1.0.9/fusion/fs_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 """Fusion fsync."""
 
-import time
-import sys
+import base64
+import hashlib
+import json
+import logging
 import os
+import sys
+import time
 from os.path import relpath
-import json
 from pathlib import Path
-import hashlib
-import base64
-import logging
-from tqdm.auto import tqdm
-from joblib import Parallel, delayed
+
 import fsspec
 import pandas as pd
-from .utils import distribution_to_filename, path_to_url, validate_file_names, upload_files, \
-    cpu_count
+from joblib import Parallel, delayed
+from tqdm.auto import tqdm
+
+from .utils import (
+    cpu_count,
+    distribution_to_filename,
+    path_to_url,
+    upload_files,
+    validate_file_names,
+)
 
 logger = logging.getLogger(__name__)
 VERBOSE_LVL = 25
-DEFAULT_CHUNK_SIZE = 2 ** 16
+DEFAULT_CHUNK_SIZE = 2**16
 
 
 def _get_loop(df, show_progress):
     if show_progress:
         loop = tqdm(df.iterrows(), total=len(df))
     else:
         loop = df.iterrows()
     return loop
 
 
 def _url_to_path(x):
-    file_name = distribution_to_filename("", x.split('/')[2], x.split('/')[4], x.split('/')[6], x.split("/")[0])
+    file_name = distribution_to_filename(
+        "", x.split("/")[2], x.split("/")[4], x.split("/")[6], x.split("/")[0]
+    )
     return f"{x.split('/')[0]}/{x.split('/')[2]}/{x.split('/')[4]}/{file_name}"
 
 
 def _download(fs_fusion, fs_local, df, n_par, show_progress=True):
     def _download_files(row):
         p_path = row["path_fusion"]
         if not fs_local.exists(p_path):
@@ -44,34 +53,38 @@
                 logger.info(f"Path {p_path} exists already", ex)
         try:
             fs_fusion.get(row["url"], p_path, chunk_size=DEFAULT_CHUNK_SIZE)
             return True, p_path, None
         except Exception as ex:
             logger.log(
                 VERBOSE_LVL,
-                f'Failed to write to {p_path}. ex - {ex}',
+                f"Failed to write to {p_path}. ex - {ex}",
             )
             msg = str(ex)
 
             return False, p_path, msg
 
     loop = _get_loop(df, show_progress)
     if len(df) > 1:
-        res = Parallel(n_jobs=n_par)(delayed(_download_files)(row) for index, row in loop)
+        res = Parallel(n_jobs=n_par)(
+            delayed(_download_files)(row) for index, row in loop
+        )
     else:
         res = [_download_files(row) for index, row in loop]
 
     return res
 
 
 def _upload(fs_fusion, fs_local, df, n_par, show_progress=True):
     df.rename(columns={"path_local": "path"}, inplace=True)
     loop = _get_loop(df, show_progress)
     parallel = True if len(df) > 1 else False
-    res = upload_files(fs_fusion, fs_local, loop, parallel=parallel, n_par=n_par, multipart=True)
+    res = upload_files(
+        fs_fusion, fs_local, loop, parallel=parallel, n_par=n_par, multipart=True
+    )
 
     return res
 
 
 def _generate_md5_token(path, fs):
     hash_md5 = hashlib.md5()
     with fs.open(path, "rb") as file:
@@ -79,24 +92,32 @@
             hash_md5_chunk = hashlib.md5()
             hash_md5_chunk.update(chunk)
             hash_md5.update(chunk)
 
     return base64.b64encode(hash_md5.digest()).decode()
 
 
-def _get_fusion_df(fs_fusion, datasets_lst, catalog, flatten=False, dataset_format=None):
+def _get_fusion_df(
+    fs_fusion, datasets_lst, catalog, flatten=False, dataset_format=None
+):
     df_lst = []
     for dataset in datasets_lst:
         changes = fs_fusion.info(f"{catalog}/datasets/{dataset}")["changes"]["datasets"]
         if len(changes) > 0:
             changes = changes[0]["distributions"]
-            urls = [catalog + "/datasets/" + "/".join(i["key"].split(".")) for i in changes]
+            urls = [
+                catalog + "/datasets/" + "/".join(i["key"].split(".")) for i in changes
+            ]
             urls = [i.replace("distribution", "distributions") for i in urls]
-            urls = ["/".join(i.split("/")[:3] + ["datasetseries"] + i.split("/")[3:]) if "datasetseries" not in i else i
-                    for i in urls]
+            urls = [
+                "/".join(i.split("/")[:3] + ["datasetseries"] + i.split("/")[3:])
+                if "datasetseries" not in i
+                else i
+                for i in urls
+            ]
             # ts = [pd.Timestamp(i["values"][0]).timestamp() for i in changes]
             sz = [int(i["values"][1]) for i in changes]
             md = [i["values"][2].split("md5=")[-1] for i in changes]
             keys = [_url_to_path(i) for i in urls]
 
             if flatten:
                 keys = ["/".join(k.split("/")[:2] + k.split("/")[-1:]) for k in keys]
@@ -111,70 +132,91 @@
 
     return pd.concat(df_lst)
 
 
 def _get_local_state(fs_local, fs_fusion, datasets, catalog, dataset_format=None):
     local_files = []
     local_files_rel = []
-    local_dirs = [f"{catalog}/{i}" for i in datasets] if len(datasets) > 0 else [catalog]
+    local_dirs = (
+        [f"{catalog}/{i}" for i in datasets] if len(datasets) > 0 else [catalog]
+    )
 
     for local_dir in local_dirs:
         if not fs_local.exists(local_dir):
             fs_local.mkdir(local_dir, exist_ok=True, create_parents=True)
 
         local_files = fs_local.find(local_dir)
-        local_rel_path = [i[i.find(local_dir):] for i in local_files]
+        local_rel_path = [i[i.find(local_dir) :] for i in local_files]
         local_file_validation = validate_file_names(local_rel_path, fs_fusion)
-        local_files += [f for flag, f in zip(local_file_validation, local_files) if flag]
-        local_files_rel += [os.path.join(local_dir, relpath(i, local_dir)).replace("\\", "/") for i in local_files]
+        local_files += [
+            f for flag, f in zip(local_file_validation, local_files) if flag
+        ]
+        local_files_rel += [
+            os.path.join(local_dir, relpath(i, local_dir)).replace("\\", "/")
+            for i in local_files
+        ]
 
     # local_mtime = [fs_local.info(x)["mtime"] for x in local_files]
     local_md5 = [_generate_md5_token(x, fs_local) for x in local_files]
     local_url_eqiv = [path_to_url(i) for i in local_files]
     df_local = pd.DataFrame([local_files_rel, local_url_eqiv, local_md5]).T
     df_local.columns = ["path", "url", "md5"]
 
     if dataset_format and len(df_local) > 0:
         df_local = df_local[df_local.url.str.split("/").str[-1] == dataset_format]
 
     df_local = df_local.sort_values("path").drop_duplicates()
     return df_local
 
 
-def _synchronize(fs_fusion: fsspec.filesystem, fs_local: fsspec.filesystem, df_local: pd.DataFrame,
-                 df_fusion: pd.DataFrame, direction: str = "upload", n_par: int = None, show_progress: bool = True):
+def _synchronize(
+    fs_fusion: fsspec.filesystem,
+    fs_local: fsspec.filesystem,
+    df_local: pd.DataFrame,
+    df_fusion: pd.DataFrame,
+    direction: str = "upload",
+    n_par: int = None,
+    show_progress: bool = True,
+):
     """Synchronize two filesystems."""
 
     n_par = cpu_count(n_par)
     if direction == "upload":
-        join_df = df_local.merge(df_fusion, on="url", suffixes=("_local", "_fusion"), how="left")
+        join_df = df_local.merge(
+            df_fusion, on="url", suffixes=("_local", "_fusion"), how="left"
+        )
         join_df = join_df[join_df["md5_local"] != join_df["md5_fusion"]]
         res = _upload(fs_fusion, fs_local, join_df, n_par, show_progress=show_progress)
     elif direction == "download":
-        join_df = df_local.merge(df_fusion, on="url", suffixes=("_local", "_fusion"), how="right")
+        join_df = df_local.merge(
+            df_fusion, on="url", suffixes=("_local", "_fusion"), how="right"
+        )
         join_df = join_df[join_df["md5_local"] != join_df["md5_fusion"]]
-        res = _download(fs_fusion, fs_local, join_df, n_par, show_progress=show_progress)
+        res = _download(
+            fs_fusion, fs_local, join_df, n_par, show_progress=show_progress
+        )
     else:
         raise ValueError("Unknown direction of operation.")
     return res
 
 
-def fsync(fs_fusion: fsspec.filesystem,
-          fs_local: fsspec.filesystem,
-          products: list = None,
-          datasets: list = None,
-          catalog: str= None,
-          direction: str = "upload",
-          flatten=False,
-          dataset_format=None,
-          n_par=None,
-          show_progress=True,
-          log_level=logging.ERROR,
-          log_path: str = "."
-          ):
+def fsync(
+    fs_fusion: fsspec.filesystem,
+    fs_local: fsspec.filesystem,
+    products: list = None,
+    datasets: list = None,
+    catalog: str = None,
+    direction: str = "upload",
+    flatten=False,
+    dataset_format=None,
+    n_par=None,
+    show_progress=True,
+    log_level=logging.ERROR,
+    log_path: str = ".",
+):
     """Synchronisation between the local filesystem and Fusion.
 
     Args:
         fs_fusion (fsspec.filesystem): Fusion filesystem.
         fs_local (fsspec.filesystem): Local filesystem.
         datasets (list): List of products.
         datasets (list): List of datasets.
@@ -189,52 +231,72 @@
 
     Returns:
 
     """
 
     if logger.hasHandlers():
         logger.handlers.clear()
-    file_handler = logging.FileHandler(filename="{0}/{1}".format(log_path, "fusion_fsync.log"))
+    file_handler = logging.FileHandler(
+        filename="{0}/{1}".format(log_path, "fusion_fsync.log")
+    )
     logging.addLevelName(VERBOSE_LVL, "VERBOSE")
     stdout_handler = logging.StreamHandler(sys.stdout)
     formatter = logging.Formatter(
-        "%(asctime)s.%(msecs)03d %(name)s:%(levelname)s %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
+        "%(asctime)s.%(msecs)03d %(name)s:%(levelname)s %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
     )
     stdout_handler.setFormatter(formatter)
     logger.addHandler(stdout_handler)
     logger.addHandler(file_handler)
     logger.setLevel(log_level)
 
     catalog = "common" if not catalog else catalog
     datasets = [] if not datasets else datasets
     products = [] if not products else products
 
-    assert len(products) > 0 or len(datasets) > 0, "At least one list products or datasets should be non-empty."
-    assert direction in ["upload", "download"], "The direction must be either upload or download."
+    assert (
+        len(products) > 0 or len(datasets) > 0
+    ), "At least one list products or datasets should be non-empty."
+    assert direction in [
+        "upload",
+        "download",
+    ], "The direction must be either upload or download."
 
     for product in products:
         res = json.loads(fs_fusion.cat(f"common/products/{product}").decode())
         datasets += [r["identifier"] for r in res["resources"]]
 
     assert len(datasets) > 0, "The supplied products did not contain any datasets."
 
     local_state = pd.DataFrame()
     while True:
         try:
-            local_state_temp = _get_local_state(fs_local, fs_fusion, datasets, catalog, dataset_format)
+            local_state_temp = _get_local_state(
+                fs_local, fs_fusion, datasets, catalog, dataset_format
+            )
             if not local_state_temp.equals(local_state):
-                fusion_state = _get_fusion_df(fs_fusion, datasets, catalog, flatten, dataset_format)
-                res = _synchronize(fs_fusion, fs_local, local_state_temp, fusion_state, direction, n_par, show_progress)
+                fusion_state = _get_fusion_df(
+                    fs_fusion, datasets, catalog, flatten, dataset_format
+                )
+                res = _synchronize(
+                    fs_fusion,
+                    fs_local,
+                    local_state_temp,
+                    fusion_state,
+                    direction,
+                    n_par,
+                    show_progress,
+                )
                 if len(res) == 0 or all((i[0] for i in res)):
                     local_state = local_state_temp
             else:
                 logger.info("All synced, sleeping")
                 time.sleep(10)
 
         except KeyboardInterrupt:
             if input("Type exit to exit: ") != "exit":
                 continue
             break
 
         except Exception as ex:
-            logger.error('%s Issue occurred: %s', type(ex), ex)
+            logger.error("%s Issue occurred: %s", type(ex), ex)
             continue
```

### Comparing `pyfusion-1.0.8/fusion/fusion.py` & `pyfusion-1.0.9/fusion/fusion.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     cpu_count,
     distribution_to_filename,
     distribution_to_url,
     get_session,
     normalise_dt_param_str,
     path_to_url,
     read_csv,
-    read_parquet,
     read_json,
+    read_parquet,
     stream_single_file_new_session,
     upload_files,
     validate_file_names,
 )
 
 logger = logging.getLogger(__name__)
 VERBOSE_LVL = 25
@@ -47,21 +47,21 @@
             session (requests.Session): Specify a proxy if required to access the authentication server. Defaults to {}.
 
         Returns:
             pandas.DataFrame: a dataframe containing the requested data.
         """
         response = session.get(url)
         response.raise_for_status()
-        table = response.json()['resources']
+        table = response.json()["resources"]
         df = pd.DataFrame(table).reset_index(drop=True)
         return df
 
     def __init__(
         self,
-        credentials: Union[str, dict] = 'config/client_credentials.json',
+        credentials: Union[str, dict] = "config/client_credentials.json",
         root_url: str = "https://fusion-api.jpmorgan.com/fusion/v1/",
         download_folder: str = "downloads",
         log_level: int = logging.ERROR,
         fs=None,
         log_path: str = ".",
     ) -> None:
         """Constructor to instantiate a new Fusion object.
@@ -82,19 +82,22 @@
 
         self.root_url = root_url
         self.download_folder = download_folder
         Path(download_folder).mkdir(parents=True, exist_ok=True)
 
         if logger.hasHandlers():
             logger.handlers.clear()
-        file_handler = logging.FileHandler(filename="{0}/{1}".format(log_path, "fusion_sdk.log"))
+        file_handler = logging.FileHandler(
+            filename="{0}/{1}".format(log_path, "fusion_sdk.log")
+        )
         logging.addLevelName(VERBOSE_LVL, "VERBOSE")
         stdout_handler = logging.StreamHandler(sys.stdout)
         formatter = logging.Formatter(
-            "%(asctime)s.%(msecs)03d %(name)s:%(levelname)s %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
+            "%(asctime)s.%(msecs)03d %(name)s:%(levelname)s %(message)s",
+            datefmt="%Y-%m-%d %H:%M:%S",
         )
         stdout_handler.setFormatter(formatter)
         logger.addHandler(stdout_handler)
         logger.addHandler(file_handler)
         logger.setLevel(log_level)
 
         if isinstance(credentials, FusionCredentials):
@@ -109,17 +112,22 @@
         """Object representation to list all available methods."""
         return "Fusion object \nAvailable methods:\n" + tabulate(
             pd.DataFrame(
                 [
                     [
                         method_name
                         for method_name in dir(Fusion)
-                        if callable(getattr(Fusion, method_name)) and not method_name.startswith("_")
+                        if callable(getattr(Fusion, method_name))
+                        and not method_name.startswith("_")
+                    ]
+                    + [
+                        p
+                        for p in dir(Fusion)
+                        if isinstance(getattr(Fusion, p), property)
                     ]
-                    + [p for p in dir(Fusion) if isinstance(getattr(Fusion, p), property)]
                 ]
             ).T.set_index(0),
             tablefmt="psql",
         )
 
     @property
     def default_catalog(self) -> str:
@@ -158,46 +166,50 @@
 
     def get_fusion_filesystem(self):
         """Creates Fusion Filesystem.
 
         Returns: Fusion Filesystem
 
         """
-        return FusionHTTPFileSystem(client_kwargs={"root_url": self.root_url, "credentials": self.credentials})
+        return FusionHTTPFileSystem(
+            client_kwargs={"root_url": self.root_url, "credentials": self.credentials}
+        )
 
     def list_catalogs(self, output: bool = False) -> pd.DataFrame:
         """Lists the catalogs available to the API account.
 
         Args:
             output (bool, optional): If True then print the dataframe. Defaults to False.
 
         Returns:
             class:`pandas.DataFrame`: A dataframe with a row for each catalog
         """
-        url = f'{self.root_url}catalogs/'
+        url = f"{self.root_url}catalogs/"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql"))
 
         return df
 
-    def catalog_resources(self, catalog: str = None, output: bool = False) -> pd.DataFrame:
+    def catalog_resources(
+        self, catalog: str = None, output: bool = False
+    ) -> pd.DataFrame:
         """List the resources contained within the catalog, for example products and datasets.
 
         Args:
             catalog (str, optional): A catalog identifier. Defaults to 'common'.
             output (bool, optional): If True then print the dataframe. Defaults to False.
 
         Returns:
            class:`pandas.DataFrame`: A dataframe with a row for each resource within the catalog
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}'
+        url = f"{self.root_url}catalogs/{catalog}"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
 
         return df
 
@@ -226,32 +238,34 @@
                 otherwise only the key columns are displayed
 
         Returns:
             class:`pandas.DataFrame`: a dataframe with a row for each product
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}/products'
+        url = f"{self.root_url}catalogs/{catalog}/products"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if contains:
             if isinstance(contains, list):
-                contains = "|".join(f'{s}' for s in contains)
+                contains = "|".join(f"{s}" for s in contains)
             if id_contains:
-                df = df[df['identifier'].str.contains(contains, case=False)]
+                df = df[df["identifier"].str.contains(contains, case=False)]
             else:
                 df = df[
-                    df['identifier'].str.contains(contains, case=False)
-                    | df['description'].str.contains(contains, case=False)
+                    df["identifier"].str.contains(contains, case=False)
+                    | df["description"].str.contains(contains, case=False)
                 ]
 
         df["category"] = df.category.str.join(", ")
         df["region"] = df.region.str.join(", ")
         if not display_all_columns:
-            df = df[["identifier", "title", "region", "category", "status", "description"]]
+            df = df[
+                ["identifier", "title", "region", "category", "status", "description"]
+            ]
 
         if max_results > -1:
             df = df[0:max_results]
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
 
@@ -282,66 +296,80 @@
                 otherwise only the key columns are displayed
 
         Returns:
             class:`pandas.DataFrame`: a dataframe with a row for each dataset.
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}/datasets'
+        url = f"{self.root_url}catalogs/{catalog}/datasets"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if contains:
             if isinstance(contains, list):
-                contains = "|".join(f'{s}' for s in contains)
+                contains = "|".join(f"{s}" for s in contains)
             if id_contains:
-                df = df[df['identifier'].str.contains(contains, case=False)]
+                df = df[df["identifier"].str.contains(contains, case=False)]
             else:
                 df = df[
-                    df['identifier'].str.contains(contains, case=False)
-                    | df['description'].str.contains(contains, case=False)
+                    df["identifier"].str.contains(contains, case=False)
+                    | df["description"].str.contains(contains, case=False)
                 ]
 
         if max_results > -1:
             df = df[0:max_results]
 
         df["category"] = df.category.str.join(", ")
         df["region"] = df.region.str.join(", ")
         if not display_all_columns:
             df = df[
-                ["identifier", "title", "region", "category", "coverageStartDate", "coverageEndDate", "description"]
+                [
+                    "identifier",
+                    "title",
+                    "region",
+                    "category",
+                    "coverageStartDate",
+                    "coverageEndDate",
+                    "description",
+                ]
             ]
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
 
         return df
 
-    def dataset_resources(self, dataset: str, catalog: str = None, output: bool = False) -> pd.DataFrame:
+    def dataset_resources(
+        self, dataset: str, catalog: str = None, output: bool = False
+    ) -> pd.DataFrame:
         """List the resources available for a dataset, currently this will always be a datasetseries.
 
         Args:
             dataset (str): A dataset identifier
             catalog (str, optional): A catalog identifier. Defaults to 'common'.
             output (bool, optional): If True then print the dataframe. Defaults to False.
 
         Returns:
             class:`pandas.DataFrame`: A dataframe with a row for each resource
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}/datasets/{dataset}'
+        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql"))
 
         return df
 
     def list_dataset_attributes(
-        self, dataset: str, catalog: str = None, output: bool = False, display_all_columns: bool = False
+        self,
+        dataset: str,
+        catalog: str = None,
+        output: bool = False,
+        display_all_columns: bool = False,
     ) -> pd.DataFrame:
         """Returns the list of attributes that are in the dataset.
 
         Args:
             dataset (str): A dataset identifier
             catalog (str, optional): A catalog identifier. Defaults to 'common'.
             output (bool, optional): If True then print the dataframe. Defaults to False.
@@ -349,27 +377,35 @@
                 otherwise only the key columns are displayed
 
         Returns:
             class:`pandas.DataFrame`: A dataframe with a row for each attribute
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}/datasets/{dataset}/attributes'
-        df = Fusion._call_for_dataframe(url, self.session).sort_values(by="index").reset_index(drop=True)
+        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/attributes"
+        df = (
+            Fusion._call_for_dataframe(url, self.session)
+            .sort_values(by="index")
+            .reset_index(drop=True)
+        )
 
         if not display_all_columns:
             df = df[["identifier", "dataType", "isDatasetKey", "description"]]
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql", maxcolwidths=30))
 
         return df
 
     def list_datasetmembers(
-        self, dataset: str, catalog: str = None, output: bool = False, max_results: int = -1
+        self,
+        dataset: str,
+        catalog: str = None,
+        output: bool = False,
+        max_results: int = -1,
     ) -> pd.DataFrame:
         """List the available members in the dataset series.
 
         Args:
             dataset (str): A dataset identifier
             catalog (str, optional): A catalog identifier. Defaults to 'common'.
             output (bool, optional): If True then print the dataframe. Defaults to False.
@@ -377,15 +413,15 @@
                 Defaults to -1 which returns all results.
 
         Returns:
             class:`pandas.DataFrame`: a dataframe with a row for each dataset member.
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries'
+        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if max_results > -1:
             df = df[0:max_results]
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql"))
@@ -405,46 +441,52 @@
 
         Returns:
             class:`pandas.DataFrame`: A dataframe with a row for each datasetseries member resource.
                 Currently, this will always be distributions.
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/{series}'
+        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/{series}"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql"))
 
         return df
 
-    def list_distributions(self, dataset: str, series: str, catalog: str = None, output: bool = False) -> pd.DataFrame:
+    def list_distributions(
+        self, dataset: str, series: str, catalog: str = None, output: bool = False
+    ) -> pd.DataFrame:
         """List the available distributions (downloadable instances of the dataset with a format type).
 
         Args:
             dataset (str): A dataset identifier
             series (str): The datasetseries identifier
             catalog (str, optional): A catalog identifier. Defaults to 'common'.
             output (bool, optional): If True then print the dataframe. Defaults to False.
 
         Returns:
             class:`pandas.DataFrame`: A dataframe with a row for each distribution.
         """
         catalog = self.__use_catalog(catalog)
 
-        url = f'{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/{series}/distributions'
+        url = f"{self.root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/{series}/distributions"
         df = Fusion._call_for_dataframe(url, self.session)
 
         if output:
             print(tabulate(df, headers="keys", tablefmt="psql"))
 
         return df
 
     def _resolve_distro_tuples(
-        self, dataset: str, dt_str: str = 'latest', dataset_format: str = 'parquet', catalog: str = None
+        self,
+        dataset: str,
+        dt_str: str = "latest",
+        dataset_format: str = "parquet",
+        catalog: str = None,
     ):
         """Resolve distribution tuples given specification params.
 
         A private utility function to generate a list of distribution tuples.
         Each tuple is a distribution, identified by catalog, dataset id,
         datasetseries member id, and the file format.
 
@@ -461,41 +503,49 @@
         """
         catalog = self.__use_catalog(catalog)
 
         datasetseries_list = self.list_datasetmembers(dataset, catalog)
 
         if datasetseries_list.empty:
             raise APIResponseError(
-                f'No data available for dataset {dataset}. '
-                f'Check that a valid dataset identifier and date/date range has been set.'
+                f"No data available for dataset {dataset}. "
+                f"Check that a valid dataset identifier and date/date range has been set."
             )
 
-        if dt_str == 'latest':
-            dt_str = datasetseries_list.iloc[datasetseries_list['createdDate'].values.argmax()]['identifier']
+        if dt_str == "latest":
+            dt_str = datasetseries_list.iloc[
+                datasetseries_list["createdDate"].values.argmax()
+            ]["identifier"]
 
         parsed_dates = normalise_dt_param_str(dt_str)
         if len(parsed_dates) == 1:
             parsed_dates = (parsed_dates[0], parsed_dates[0])
 
         if parsed_dates[0]:
-            datasetseries_list = datasetseries_list[datasetseries_list['fromDate'] >= parsed_dates[0]]
+            datasetseries_list = datasetseries_list[
+                datasetseries_list["fromDate"] >= parsed_dates[0]
+            ]
 
         if parsed_dates[1]:
-            datasetseries_list = datasetseries_list[datasetseries_list['toDate'] <= parsed_dates[1]]
+            datasetseries_list = datasetseries_list[
+                datasetseries_list["toDate"] <= parsed_dates[1]
+            ]
 
-        required_series = list(datasetseries_list['@id'])
-        tups = [(catalog, dataset, series, dataset_format) for series in required_series]
+        required_series = list(datasetseries_list["@id"])
+        tups = [
+            (catalog, dataset, series, dataset_format) for series in required_series
+        ]
 
         return tups
 
     def download(
         self,
         dataset: str,
-        dt_str: str = 'latest',
-        dataset_format: str = 'parquet',
+        dt_str: str = "latest",
+        dataset_format: str = "parquet",
         catalog: str = None,
         n_par: int = None,
         show_progress: bool = True,
         force_download: bool = False,
         download_folder: str = None,
         return_paths: bool = False,
     ):
@@ -519,52 +569,60 @@
 
         Returns:
 
         """
         catalog = self.__use_catalog(catalog)
 
         n_par = cpu_count(n_par)
-        required_series = self._resolve_distro_tuples(dataset, dt_str, dataset_format, catalog)
+        required_series = self._resolve_distro_tuples(
+            dataset, dt_str, dataset_format, catalog
+        )
 
         if not download_folder:
             download_folder = self.download_folder
 
         if not self.fs.exists(download_folder):
             self.fs.mkdir(download_folder, create_parents=True)
         download_spec = [
             {
                 "credentials": self.credentials,
-                "url": distribution_to_url(self.root_url, series[1], series[2], series[3], series[0]),
-                "output_file": distribution_to_filename(download_folder, series[1], series[2], series[3], series[0]),
+                "url": distribution_to_url(
+                    self.root_url, series[1], series[2], series[3], series[0]
+                ),
+                "output_file": distribution_to_filename(
+                    download_folder, series[1], series[2], series[3], series[0]
+                ),
                 "overwrite": force_download,
                 "fs": self.fs,
             }
             for series in required_series
         ]
 
         if show_progress:
             loop = tqdm(download_spec)
         else:
             loop = download_spec
         logger.log(
             VERBOSE_LVL,
-            f'Beginning {len(loop)} downloads in batches of {n_par}',
+            f"Beginning {len(loop)} downloads in batches of {n_par}",
+        )
+        res = Parallel(n_jobs=n_par)(
+            delayed(stream_single_file_new_session)(**spec) for spec in loop
         )
-        res = Parallel(n_jobs=n_par)(delayed(stream_single_file_new_session)(**spec) for spec in loop)
         if (len(res) > 0) and (not all((r[0] for r in res))):
             for r in res:
                 if not r[0]:
                     warnings.warn(f"The download of {r[1]} was not successful")
         return res if return_paths else None
 
     def to_df(
         self,
         dataset: str,
-        dt_str: str = 'latest',
-        dataset_format: str = 'parquet',
+        dt_str: str = "latest",
+        dataset_format: str = "parquet",
         catalog: str = None,
         n_par: int = None,
         show_progress: bool = True,
         columns: List = None,
         filters: List = None,
         force_download: bool = False,
         download_folder: str = None,
@@ -622,45 +680,47 @@
                 f"Not all downloads were successfully completed. "
                 f"Re-run to collect missing files. The following failed:\n{failed_res}"
             )
 
         files = [res[1] for res in download_res]
 
         pd_read_fn_map = {
-            'csv': read_csv,
-            'parquet': read_parquet,
-            'parq': read_parquet,
-            'json': read_json,
-            'raw': read_csv,
+            "csv": read_csv,
+            "parquet": read_parquet,
+            "parq": read_parquet,
+            "json": read_json,
+            "raw": read_csv,
         }
 
         pd_read_default_kwargs: Dict[str, Dict[str, object]] = {
-            'csv': {'columns': columns, 'filters': filters, 'fs': self.fs},
-            'parquet': {'columns': columns, 'filters': filters, 'fs': self.fs},
-            'json': {'columns': columns, 'filters': filters, 'fs': self.fs},
-            'raw': {'columns': columns, 'filters': filters, 'fs': self.fs},
+            "csv": {"columns": columns, "filters": filters, "fs": self.fs},
+            "parquet": {"columns": columns, "filters": filters, "fs": self.fs},
+            "json": {"columns": columns, "filters": filters, "fs": self.fs},
+            "raw": {"columns": columns, "filters": filters, "fs": self.fs},
         }
 
-        pd_read_default_kwargs['parq'] = pd_read_default_kwargs['parquet']
+        pd_read_default_kwargs["parq"] = pd_read_default_kwargs["parquet"]
 
         pd_reader = pd_read_fn_map.get(dataset_format)
         pd_read_kwargs = pd_read_default_kwargs.get(dataset_format, {})
         if not pd_reader:
-            raise Exception(f'No pandas function to read file in format {dataset_format}')
+            raise Exception(
+                f"No pandas function to read file in format {dataset_format}"
+            )
 
         pd_read_kwargs.update(kwargs)
 
         if len(files) == 0:
             raise APIResponseError(
                 f"No series members for dataset: {dataset} "
                 f"in date or date range: {dt_str} and format: {dataset_format}"
             )
         if dataset_format in ["parquet", "parq"]:
             df = pd_reader(files, **pd_read_kwargs)  # type: ignore
-        elif dataset_format == 'raw':
+        elif dataset_format == "raw":
             dataframes = (
                 pd.concat(
                     [pd_reader(ZipFile(f).open(p), **pd_read_kwargs) for p in ZipFile(f).namelist()], ignore_index=True  # type: ignore
                 )  # type: ignore
                 for f in files
             )  # type: ignore
             df = pd.concat(dataframes, ignore_index=True)
@@ -670,15 +730,15 @@
 
         return df
 
     def upload(
         self,
         path: str,
         dataset: str = None,
-        dt_str: str = 'latest',
+        dt_str: str = "latest",
         catalog: str = None,
         n_par: int = None,
         show_progress: bool = True,
         return_paths: bool = False,
         multipart=True,
         chunk_size=5 * 2**20,
     ):
@@ -708,49 +768,65 @@
         if not self.fs.exists(path):
             raise RuntimeError("The provided path does not exist")
 
         fs_fusion = self.get_fusion_filesystem()
         if self.fs.info(path)["type"] == "directory":
             file_path_lst = self.fs.find(path)
             local_file_validation = validate_file_names(file_path_lst, fs_fusion)
-            file_path_lst = [f for flag, f in zip(local_file_validation, file_path_lst) if flag]
+            file_path_lst = [
+                f for flag, f in zip(local_file_validation, file_path_lst) if flag
+            ]
             local_url_eqiv = [path_to_url(i) for i in file_path_lst]
         else:
             file_path_lst = [path]
             if not catalog or not dataset:
                 local_file_validation = validate_file_names(file_path_lst, fs_fusion)
-                file_path_lst = [f for flag, f in zip(local_file_validation, file_path_lst) if flag]
+                file_path_lst = [
+                    f for flag, f in zip(local_file_validation, file_path_lst) if flag
+                ]
                 local_url_eqiv = [path_to_url(i) for i in file_path_lst]
             else:
                 file_format = path.split(".")[-1]
-                dt_str = dt_str if dt_str != "latest" else pd.Timestamp("today").date().strftime("%Y%m%d")
+                dt_str = (
+                    dt_str
+                    if dt_str != "latest"
+                    else pd.Timestamp("today").date().strftime("%Y%m%d")
+                )
                 dt_str = pd.Timestamp(dt_str).date().strftime("%Y%m%d")
-                if catalog not in fs_fusion.ls('') or dataset not in [
-                    i.split('/')[-1] for i in fs_fusion.ls(f"{catalog}/datasets")
+                if catalog not in fs_fusion.ls("") or dataset not in [
+                    i.split("/")[-1] for i in fs_fusion.ls(f"{catalog}/datasets")
                 ]:
                     msg = (
                         f"File file has not been uploaded, one of the catalog: {catalog} "
                         f"or dataset: {dataset} does not exit."
                     )
                     warnings.warn(msg)
                     return [(False, path, Exception(msg))]
-                local_url_eqiv = [path_to_url(f"{dataset}__{catalog}__{dt_str}.{file_format}")]
+                local_url_eqiv = [
+                    path_to_url(f"{dataset}__{catalog}__{dt_str}.{file_format}")
+                ]
 
         df = pd.DataFrame([file_path_lst, local_url_eqiv]).T
         df.columns = ["path", "url"]
 
         if show_progress:
             loop = tqdm(df.iterrows(), total=len(df))
         else:
             loop = df.iterrows()
 
         n_par = cpu_count(n_par)
         parallel = True if len(df) > 1 else False
         res = upload_files(
-            fs_fusion, self.fs, loop, parallel=parallel, n_par=n_par, multipart=multipart, chunk_size=chunk_size
+            fs_fusion,
+            self.fs,
+            loop,
+            parallel=parallel,
+            n_par=n_par,
+            multipart=multipart,
+            chunk_size=chunk_size,
         )
 
         if not all(r[0] for r in res):
             failed_res = [r for r in res if not r[0]]
             msg = f"Not all uploads were successfully completed. The following failed:\n{failed_res}"
             logger.warning(msg)
             warnings.warn(msg)
```

### Comparing `pyfusion-1.0.8/fusion/fusion_filesystem.py` & `pyfusion-1.0.9/fusion/fusion_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Fusion FileSystem."""
 
-import logging
-from urllib.parse import urljoin
-import hashlib
 import base64
-from copy import deepcopy
+import hashlib
 import io
-from fsspec.implementations.http import HTTPFileSystem, sync
+import logging
+from copy import deepcopy
+from urllib.parse import urljoin
+
+import pandas as pd
 from fsspec.callbacks import _DEFAULT_CALLBACK
+from fsspec.implementations.http import HTTPFileSystem, sync
 from fsspec.utils import nullcontext
-import pandas as pd
-from .utils import get_client
+
 from .authentication import FusionCredentials
+from .utils import get_client
 
 logger = logging.getLogger(__name__)
 VERBOSE_LVL = 25
 
 
 class FusionHTTPFileSystem(HTTPFileSystem):
-    """Fusion HTTP filesystem.
-    """
+    """Fusion HTTP filesystem."""
 
-    def __init__(self, credentials='config/client_credentials.json', *args, **kwargs):
+    def __init__(self, credentials="config/client_credentials.json", *args, **kwargs):
         """Same signature as the fsspec HTTPFileSystem.
 
         Args:
             credentials: Credentials.
             *args: Args.
             **kwargs: Kwargs.
         """
@@ -34,16 +35,18 @@
         if "get_client" not in kwargs:
             kwargs["get_client"] = get_client
         if "client_kwargs" not in kwargs:
             if isinstance(credentials, FusionCredentials):
                 self.credentials = credentials
             else:
                 self.credentials = FusionCredentials.from_object(credentials)
-            kwargs["client_kwargs"] = {"credentials": self.credentials,
-                                       "root_url": "https://fusion-api.jpmorgan.com/fusion/v1/"}
+            kwargs["client_kwargs"] = {
+                "credentials": self.credentials,
+                "root_url": "https://fusion-api.jpmorgan.com/fusion/v1/",
+            }
         else:
             self.credentials = kwargs["client_kwargs"]["credentials"]
 
         if self.credentials.proxies:
             if "http" in self.credentials.proxies.keys():
                 kwargs["proxy"] = self.credentials.proxies["http"]
             elif "https" in self.credentials.proxies.keys():
@@ -51,19 +54,27 @@
 
         if "headers" not in kwargs:
             kwargs["headers"] = {"Accept-Encoding": "identity"}
 
         super().__init__(*args, **kwargs)
 
     async def _decorate_url_a(self, url):
-        url = urljoin(f'{self.client_kwargs["root_url"]}catalogs/', url) if "http" not in url else url
+        url = (
+            urljoin(f'{self.client_kwargs["root_url"]}catalogs/', url)
+            if "http" not in url
+            else url
+        )
         return url
 
     def _decorate_url(self, url):
-        url = urljoin(f'{self.client_kwargs["root_url"]}catalogs/', url) if "http" not in url else url
+        url = (
+            urljoin(f'{self.client_kwargs["root_url"]}catalogs/', url)
+            if "http" not in url
+            else url
+        )
         return url
 
     async def _isdir(self, path):
         path = self._decorate_url(path)
         try:
             ret = await self._info(path)
             return ret["type"] == "directory"
@@ -114,15 +125,17 @@
 
         if detail:
             if not is_file:
                 return [
                     {
                         "name": u,
                         "size": None,
-                        "type": "directory" if not (u.endswith("csv") or u.endswith("parquet")) else "file",
+                        "type": "directory"
+                        if not (u.endswith("csv") or u.endswith("parquet"))
+                        else "file",
                     }
                     for u in out
                 ]
             else:
                 return [
                     {
                         "name": out[0],
@@ -172,19 +185,24 @@
         """
         url = self._decorate_url(url)
         ret = super().ls(url, detail=detail, **kwargs)
         keep_protocol = kwargs.pop("keep_protocol", False)
         if detail:
             if not keep_protocol:
                 for k in ret:
-                    k["name"] = k["name"].split(f'{self.client_kwargs["root_url"]}catalogs/')[-1]
+                    k["name"] = k["name"].split(
+                        f'{self.client_kwargs["root_url"]}catalogs/'
+                    )[-1]
 
         else:
             if not keep_protocol:
-                return [x.split(f'{self.client_kwargs["root_url"]}catalogs/')[-1] for x in ret]
+                return [
+                    x.split(f'{self.client_kwargs["root_url"]}catalogs/')[-1]
+                    for x in ret
+                ]
 
         return ret
 
     def exists(self, url, detail=True, **kwargs):
         """Check existence.
 
         Args:
@@ -221,29 +239,33 @@
 
         Returns:
 
         """
         url = self._decorate_url(url)
         return super().cat(url, start=start, end=end, **kwargs)
 
-    def get(self, rpath, lpath, chunk_size=5 * 2 ** 20, callback=_DEFAULT_CALLBACK, **kwargs):
+    def get(
+        self, rpath, lpath, chunk_size=5 * 2**20, callback=_DEFAULT_CALLBACK, **kwargs
+    ):
         """Copy file(s) to local.
 
         Args:
             rpath: Rpath.
             lpath: Lpath.
             chunk_size: Chunk size.
             callback: Callback function.
             **kwargs: Kwargs.
 
         Returns:
 
         """
         rpath = self._decorate_url(rpath)
-        return super().get(rpath, lpath, chunk_size=chunk_size, callback=_DEFAULT_CALLBACK, **kwargs)
+        return super().get(
+            rpath, lpath, chunk_size=chunk_size, callback=_DEFAULT_CALLBACK, **kwargs
+        )
 
     async def _put_file(
         self,
         lpath,
         rpath,
         chunk_size=5 * 2**20,
         callback=_DEFAULT_CALLBACK,
@@ -268,15 +290,18 @@
                 else:
                     callback.set_size(getattr(f, "size", None))
 
                 chunk = f.read(chunk_size)
                 i = 0
                 while chunk:
                     kw = self.kwargs.copy()
-                    url = rpath + f"/operations/upload?operationId={operation_id}&partNumber={i+1}"
+                    url = (
+                        rpath
+                        + f"/operations/upload?operationId={operation_id}&partNumber={i+1}"
+                    )
                     kw.update({"headers": kwargs["chunk_headers_lst"][i]})
                     async with meth(url=url, data=chunk, **kw) as resp:
                         self._raise_not_found_for_status(resp, rpath)
                         yield await resp.json()
                     i += 1
                     callback.relative_update(len(chunk))
                     chunk = f.read(chunk_size)
@@ -304,57 +329,64 @@
 
             operation_id = operation_id["operationId"]
             resps = []
             async for resp in put_data():
                 resps.append(resp)
             kw = self.kwargs.copy()
             kw.update({"headers": headers})
-            async with session.post(url=rpath + f"/operations/upload?operationId={operation_id}",
-                                    json={"parts": resps}, **kw) as resp:
-                self._raise_not_found_for_status(resp,
-                                                 rpath + f"/operations/upload?operationId={operation_id}")
+            async with session.post(
+                url=rpath + f"/operations/upload?operationId={operation_id}",
+                json={"parts": resps},
+                **kw,
+            ) as resp:
+                self._raise_not_found_for_status(
+                    resp, rpath + f"/operations/upload?operationId={operation_id}"
+                )
 
     @staticmethod
-    def _construct_headers(file_local, dt_iso, chunk_size=5 * 2 ** 20, multipart=False):
+    def _construct_headers(file_local, dt_iso, chunk_size=5 * 2**20, multipart=False):
 
         headers = {
             "Content-Type": "application/octet-stream",
             "x-jpmc-distribution-created-date": dt_iso,
             "x-jpmc-distribution-from-date": dt_iso,
             "x-jpmc-distribution-to-date": dt_iso,
-            "Digest": ""
-        }
-        headers["Content-Type"] = "application/json" if multipart else headers["Content-Type"]
-        headers_chunks = {
-            "Content-Type": "application/octet-stream",
-            "Digest": ""
+            "Digest": "",
         }
+        headers["Content-Type"] = (
+            "application/json" if multipart else headers["Content-Type"]
+        )
+        headers_chunks = {"Content-Type": "application/octet-stream", "Digest": ""}
 
         headers_chunk_lst = []
         hash_md5 = hashlib.md5()
         for chunk in iter(lambda: file_local.read(chunk_size), b""):
             hash_md5_chunk = hashlib.md5()
             hash_md5_chunk.update(chunk)
             hash_md5.update(chunk)
             headers_chunks = deepcopy(headers_chunks)
-            headers_chunks["Digest"] = "md5=" + base64.b64encode(hash_md5_chunk.digest()).decode()
+            headers_chunks["Digest"] = (
+                "md5=" + base64.b64encode(hash_md5_chunk.digest()).decode()
+            )
             headers_chunk_lst.append(headers_chunks)
 
         file_local.seek(0)
         headers["Digest"] = "md5=" + base64.b64encode(hash_md5.digest()).decode()
         return headers, headers_chunk_lst
 
-    def put(self,
-            lpath,
-            rpath,
-            chunk_size=5 * 2 ** 20,
-            callback=_DEFAULT_CALLBACK,
-            method="put",
-            multipart=False,
-            **kwargs):
+    def put(
+        self,
+        lpath,
+        rpath,
+        chunk_size=5 * 2**20,
+        callback=_DEFAULT_CALLBACK,
+        method="put",
+        multipart=False,
+        **kwargs,
+    ):
         """Copy file(s) from local.
 
         Args:
             lpath: Lpath.
             rpath: Rpath.
             chunk_size: Chunk size.
             callback: Callback function.
@@ -363,15 +395,17 @@
             **kwargs: Kwargs.
 
         Returns:
 
         """
 
         dt_iso = pd.Timestamp(rpath.split("/")[-3]).strftime("%Y-%m-%d")
-        headers, chunk_headers_lst = self._construct_headers(lpath, dt_iso, chunk_size, multipart)
+        headers, chunk_headers_lst = self._construct_headers(
+            lpath, dt_iso, chunk_size, multipart
+        )
         rpath = self._decorate_url(rpath)
         kwargs.update({"headers": headers})
         if multipart:
             kwargs.update({"chunk_headers_lst": chunk_headers_lst})
             args = [lpath, rpath, chunk_size, callback, method, multipart]
         else:
             args = [lpath, rpath, None, callback, method, multipart]
@@ -402,19 +436,20 @@
 
         Returns:
 
         """
 
         return super().glob(path, **kwargs)
 
-    def open(self,
-             path,
-             mode="rb",
-             **kwargs,
-             ):
+    def open(
+        self,
+        path,
+        mode="rb",
+        **kwargs,
+    ):
         """Open.
 
         Args:
             path: Path.
             mode: Defaults to rb.
             **kwargs: Kwargs.
```

### Comparing `pyfusion-1.0.8/fusion/utils.py` & `pyfusion-1.0.9/fusion/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 import datetime
 import logging
 import os
 import re
 import sys
 from io import BytesIO
+from pathlib import Path
 from typing import Union
 from urllib.parse import urlparse, urlunparse
-from pathlib import Path
+
 import aiohttp
 import pandas as pd
 import pyarrow.parquet as pq
 import requests
 from joblib import Parallel, delayed
 from pyarrow import csv, json
 
@@ -117,37 +118,41 @@
     """
     try:
         try:
             tbl = _csv_to_table(path, fs)
         except Exception as err:
             logger.log(
                 VERBOSE_LVL,
-                f'Failed to read {path}, with comma delimiter. {err}',
+                f"Failed to read {path}, with comma delimiter. {err}",
             )
             raise Exception
 
         out = BytesIO()
         pq.write_table(tbl, out)
         del tbl
         res = pq.read_table(out, filters=filters, columns=columns).to_pandas()
     except Exception as err:
         logger.log(
             VERBOSE_LVL,
-            f"Could not parse {path} properly. " f"Trying with pandas csv reader. {err}",
+            f"Could not parse {path} properly. "
+            f"Trying with pandas csv reader. {err}",
         )
         try:
             with (fs.open(path) if fs else nullcontext(path)) as f:
                 res = pd.read_csv(f, usecols=columns, index_col=False)
         except Exception as err:
             logger.log(
                 VERBOSE_LVL,
-                f"Could not parse {path} properly. " f"Trying with pandas csv reader pandas engine. {err}",
+                f"Could not parse {path} properly. "
+                f"Trying with pandas csv reader pandas engine. {err}",
             )
             with (fs.open(path) if fs else nullcontext(path)) as f:
-                res = pd.read_table(f, usecols=columns, index_col=False, engine="python", delimiter=None)
+                res = pd.read_table(
+                    f, usecols=columns, index_col=False, engine="python", delimiter=None
+                )
     return res
 
 
 def read_json(path: str, columns: list = None, filters: list = None, fs=None):
     """Read json files(s) to pandas.
 
     Args:
@@ -162,54 +167,63 @@
 
     try:
         try:
             tbl = _json_to_table(path, fs)
         except Exception as err:
             logger.log(
                 VERBOSE_LVL,
-                f'Failed to read {path}, with arrow reader. {err}',
+                f"Failed to read {path}, with arrow reader. {err}",
             )
             raise Exception
 
         out = BytesIO()
         pq.write_table(tbl, out)
         del tbl
         res = pq.read_table(out, filters=filters, columns=columns).to_pandas()
     except Exception as err:
         logger.log(
             VERBOSE_LVL,
-            f"Could not parse {path} properly. " f"Trying with pandas json reader. {err}",
+            f"Could not parse {path} properly. "
+            f"Trying with pandas json reader. {err}",
         )
         try:
             with (fs.open(path) if fs else nullcontext(path)) as f:
                 res = pd.read_json(f)
         except Exception as err:
             logger.error(
                 VERBOSE_LVL,
                 f"Could not parse {path} properly. " f"{err}",
             )
             raise Exception(err)
     return res
 
 
-def read_parquet(path: Union[list, str], columns: list = None, filters: list = None, fs=None):
+def read_parquet(
+    path: Union[list, str], columns: list = None, filters: list = None, fs=None
+):
     """Read parquet files(s) to pandas.
 
     Args:
         path (Union[list, str]): path or a list of paths to parquet files.
         columns (list): list of selected fields.
         filters (list): filters.
         fs: filesystem object.
 
     Returns:
         pandas.DataFrame: a dataframe containing the data.
 
     """
     return (
-        pq.ParquetDataset(path, use_legacy_dataset=False, filters=filters, filesystem=fs, memory_map=True)
+        pq.ParquetDataset(
+            path,
+            use_legacy_dataset=False,
+            filters=filters,
+            filesystem=fs,
+            memory_map=True,
+        )
         .read_pandas(columns=columns)
         .to_pandas()
     )
 
 
 def _normalise_dt_param(dt: Union[str, int, datetime.datetime, datetime.date]) -> str:
     """Convert dates into a normalised string representation.
@@ -254,33 +268,39 @@
         tuple: A tuple of dates.
     """
     date_parts = dt.split(":")
 
     if not date_parts or len(date_parts) > 2:
         raise ValueError(f"Unable to parse {dt} as either a date or an interval")
 
-    return tuple((_normalise_dt_param(dt_part) if dt_part else dt_part for dt_part in date_parts))
+    return tuple(
+        (_normalise_dt_param(dt_part) if dt_part else dt_part for dt_part in date_parts)
+    )
 
 
 def distribution_to_filename(
-    root_folder: str, dataset: str, datasetseries: str, file_format: str, catalog: str = 'common'
+    root_folder: str,
+    dataset: str,
+    datasetseries: str,
+    file_format: str,
+    catalog: str = "common",
 ) -> str:
     """Returns a filename representing a dataset distribution.
 
     Args:
         root_folder (str): The root folder path.
         dataset (str): The dataset identifier.
         datasetseries (str): The datasetseries instance identifier.
         file_format (str): The file type, e.g. CSV or Parquet
         catalog (str, optional): The data catalog containing the dataset. Defaults to "common".
 
     Returns:
         str: FQ distro file name
     """
-    if datasetseries[-1] == '/' or datasetseries[-1] == '\\':
+    if datasetseries[-1] == "/" or datasetseries[-1] == "\\":
         datasetseries = datasetseries[0:-1]
     file_name = f"{dataset}__{catalog}__{datasetseries}.{file_format}"
 
     sep = "/"
     if "\\" in root_folder:
         sep = "\\"
     return f"{root_folder}{sep}{file_name}"
@@ -291,35 +311,39 @@
 
     Args:
         file_name (str): The filename to decompose.
 
     Returns:
         tuple: A tuple consisting of catalog id, dataset id, datasetseries instane id, and file format (e.g. CSV).
     """
-    dataset, catalog, series_format = Path(file_name).name.split('__')
-    datasetseries, file_format = series_format.split('.')
+    dataset, catalog, series_format = Path(file_name).name.split("__")
+    datasetseries, file_format = series_format.split(".")
     return catalog, dataset, datasetseries, file_format
 
 
 def distribution_to_url(
-    root_url: str, dataset: str, datasetseries: str, file_format: str, catalog: str = 'common'
+    root_url: str,
+    dataset: str,
+    datasetseries: str,
+    file_format: str,
+    catalog: str = "common",
 ) -> str:
     """Returns the API URL to download a dataset distribution.
 
     Args:
         root_url (str): The base url for the API.
         dataset (str): The dataset identifier.
         datasetseries (str): The datasetseries instance identifier.
         file_format (str): The file type, e.g. CSV or Parquet
         catalog (str, optional): The data catalog containing the dataset. Defaults to "common".
 
     Returns:
         str: A URL for the API distribution endpoint.
     """
-    if datasetseries[-1] == '/' or datasetseries[-1] == '\\':
+    if datasetseries[-1] == "/" or datasetseries[-1] == "\\":
         datasetseries = datasetseries[0:-1]
 
     return f"{root_url}catalogs/{catalog}/datasets/{dataset}/datasetseries/{datasetseries}/distributions/{file_format}"
 
 
 def _get_canonical_root_url(any_url: str) -> str:
     """Get the full URL for the API endpoint.
@@ -328,15 +352,15 @@
         any_url (str): A valid URL or URL part
 
     Returns:
         str: A complete root URL
 
     """
     url_parts = urlparse(any_url)
-    root_url = urlunparse((url_parts[0], url_parts[1], '', '', '', ''))
+    root_url = urlunparse((url_parts[0], url_parts[1], "", "", "", ""))
     return root_url
 
 
 async def get_client(credentials, **kwargs):
     """Gets session for async.
 
     Args:
@@ -351,32 +375,34 @@
         payload = (
             {
                 "grant_type": "client_credentials",
                 "client_id": credentials.client_id,
                 "client_secret": credentials.client_secret,
                 "aud": credentials.resource,
             }
-            if credentials.grant_type == 'client_credentials'
+            if credentials.grant_type == "client_credentials"
             else {
                 "grant_type": "password",
                 "client_id": credentials.client_id,
                 "username": credentials.username,
                 "password": credentials.password,
                 "resource": credentials.resource,
             }
         )
         async with aiohttp.ClientSession() as session:
             if credentials.proxies:
-                response = await session.post(credentials.auth_url, data=payload, proxy=http_proxy)
+                response = await session.post(
+                    credentials.auth_url, data=payload, proxy=http_proxy
+                )
             else:
                 response = await session.post(credentials.auth_url, data=payload)
             response_data = await response.json()
 
         access_token = response_data["access_token"]
-        params.headers.update({'Authorization': f'Bearer {access_token}'})
+        params.headers.update({"Authorization": f"Bearer {access_token}"})
 
     if credentials.proxies:
         if "http" in credentials.proxies.keys():
             http_proxy = credentials.proxies["http"]
         elif "https" in credentials.proxies.keys():
             http_proxy = credentials.proxies["https"]
 
@@ -395,15 +421,17 @@
         root_url (str): The URL to call.
 
     Returns:
         requests.Session(): A HTTP Session object
 
     """
     if not get_retries:
-        get_retries = Retry(total=5, backoff_factor=0.1, status_forcelist=[429, 500, 502, 503, 504])
+        get_retries = Retry(
+            total=5, backoff_factor=0.1, status_forcelist=[429, 500, 502, 503, 504]
+        )
     else:
         get_retries = Retry.from_int(get_retries)
     session = requests.Session()
     auth_handler = FusionOAuthAdapter(credentials, max_retries=get_retries)
     if credentials.proxies:
         # mypy does note recognise session.proxies as a dict so fails this line, we'll ignore this chk
         session.proxies.update(credentials.proxies)  # type:ignore
@@ -438,15 +466,15 @@
 def stream_single_file_new_session(
     credentials,
     url: str,
     output_file: str,
     overwrite: bool = True,
     block_size=DEFAULT_CHUNK_SIZE,
     dry_run: bool = False,
-    fs: fsspec.AbstractFileSystem = fsspec.filesystem('file'),
+    fs: fsspec.AbstractFileSystem = fsspec.filesystem("file"),
 ) -> tuple:
     """Function to stream a single file from the API to a file on disk.
 
     Args:
         credentials (FusionCredentials): Valid user credentials to provide an acces token
         url (str): The URL to call.
         output_file (str): The filename that the data will be saved into.
@@ -472,21 +500,21 @@
             byte_cnt = 0
             with fs.open(output_file, "wb") as outfile:
                 for chunk in r.iter_content(block_size):
                     byte_cnt += len(chunk)
                     outfile.write(chunk)
         logger.log(
             VERBOSE_LVL,
-            f'Wrote {byte_cnt:,} bytes to {output_file}',
+            f"Wrote {byte_cnt:,} bytes to {output_file}",
         )
         return (True, output_file, None)
     except Exception as ex:
         logger.log(
             VERBOSE_LVL,
-            f'Failed to write to {output_file}. ex - {ex}',
+            f"Failed to write to {output_file}. ex - {ex}",
         )
         return False, output_file, ex
 
 
 def validate_file_names(paths, fs_fusion):
     """Validate if the file name format adheres to the standard.
 
@@ -495,25 +523,27 @@
         fs_fusion: Fusion filesystem.
 
     Returns (list): List of booleans.
 
     """
     file_names = [i.split("/")[-1].split(".")[0] for i in paths]
     validation = []
-    all_catalogs = fs_fusion.ls('')
+    all_catalogs = fs_fusion.ls("")
     all_datasets = {}
     for f_n in file_names:
-        tmp = f_n.split('__')
+        tmp = f_n.split("__")
         if len(tmp) == 3:
             val = tmp[1] in all_catalogs
             if not val:
                 validation.append(False)
             else:
                 if tmp[1] not in all_datasets.keys():
-                    all_datasets[tmp[1]] = [i.split('/')[-1] for i in fs_fusion.ls(f"{tmp[1]}/datasets")]
+                    all_datasets[tmp[1]] = [
+                        i.split("/")[-1] for i in fs_fusion.ls(f"{tmp[1]}/datasets")
+                    ]
 
                 val = tmp[0] in all_datasets[tmp[1]]
                 validation.append(val)
         else:
             validation.append(False)
 
     if not all(validation):
@@ -535,15 +565,23 @@
     Returns (str): Fusion url string.
 
     """
     catalog, dataset, date, ext = _filename_to_distribution(x.split("/")[-1])
     return "/".join(distribution_to_url("", dataset, date, ext, catalog).split("/")[1:])
 
 
-def upload_files(fs_fusion, fs_local, loop, parallel=True, n_par=-1, multipart=True, chunk_size=5 * 2**20):
+def upload_files(
+    fs_fusion,
+    fs_local,
+    loop,
+    parallel=True,
+    n_par=-1,
+    multipart=True,
+    chunk_size=5 * 2**20,
+):
     """Upload file into Fusion.
 
     Args:
         fs_fusion: Fusion filesystem.
         fs_local: Local filesystem.
         loop (iterable): Loop of files to iterate through.
         parallel (bool): Is parallel mode enabled.
@@ -556,15 +594,17 @@
     """
 
     def _upload(row):
         p_url = row["url"]
         try:
             mp = multipart and fs_local.size(row["path"]) > chunk_size
             with fs_local.open(row["path"], "rb") as file_local:
-                fs_fusion.put(file_local, p_url, chunk_size=chunk_size, method="put", multipart=mp)
+                fs_fusion.put(
+                    file_local, p_url, chunk_size=chunk_size, method="put", multipart=mp
+                )
             return True, row["path"], None
         except Exception as ex:
             logger.log(
                 VERBOSE_LVL,
                 f'Failed to upload {row["path"]}. ex - {ex}',
             )
             return False, row["path"], ex
```

### Comparing `pyfusion-1.0.8/pyproject.toml` & `pyfusion-1.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "PyFusion"
-version = "1.0.8"
+version = "1.0.9"
 
 homepage = "https://github.com/jpmorganchase/fusion"
 description = "JPMC Fusion Developer Tools"
 authors = ["FusionDevs <fusion_developers@jpmorgan.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
@@ -99,34 +99,26 @@
     "mkdocs-include-markdown-plugin",
     "mkdocs-git-revision-date-plugin",
     "mkdocs-jupyter",
     "jupyter_contrib_nbextensions",
     "mike"
     ]
 
-# 
-[tool.black]
-line-length = 120
-skip-string-normalization = true
-target-version = ['py37', 'py38', 'py39', 'py310']
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-)/
-'''
+aws = [
+    "s3fs"
+]
+
+gcs = [
+    "gcsfs"
+]
+
+azr = [
+    "adlfs"
+]
+
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `pyfusion-1.0.8/tests/conftest.py` & `pyfusion-1.0.9/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,40 +19,40 @@
 @pytest.fixture
 def example_https_proxy():
     return "https://myproxy.com:8080"
 
 
 @pytest.fixture
 def example_proxy_http_dict(example_http_proxy):
-    return {'http': example_http_proxy}
+    return {"http": example_http_proxy}
 
 
 @pytest.fixture
 def example_proxy_https_dict(example_https_proxy):
-    return {'https': example_https_proxy}
+    return {"https": example_https_proxy}
 
 
 @pytest.fixture
 def example_proxy_both_dict(example_http_proxy, example_https_proxy):
-    return {'http': example_http_proxy, 'https': example_https_proxy}
+    return {"http": example_http_proxy, "https": example_https_proxy}
 
 
 @pytest.fixture
 def example_proxy_both_alt_dict(example_http_proxy, example_https_proxy):
-    return {'http_proxy': example_http_proxy, 'https_proxy': example_https_proxy}
+    return {"http_proxy": example_http_proxy, "https_proxy": example_https_proxy}
 
 
 @pytest.fixture
 def example_proxy_str1(example_http_proxy):
     return example_http_proxy
 
 
 @pytest.fixture
 def example_proxy_str_bad():
-    return 'not_a_proxy'
+    return "not_a_proxy"
 
 
 @pytest.fixture
 def example_creds_dict(example_client_id, example_client_secret):
     # Mocked creds info
     return {
         "client_id": example_client_id,
@@ -64,22 +64,22 @@
             "https": "http://myproxy.com:8081",
         },
     }
 
 
 @pytest.fixture
 def example_creds_dict_no_pxy(example_creds_dict):
-    example_creds_dict.pop('proxies')
+    example_creds_dict.pop("proxies")
     return example_creds_dict
 
 
 @pytest.fixture
 def example_creds_dict_empty_pxy(example_creds_dict):
-    example_creds_dict['proxies'].pop('http')
-    example_creds_dict['proxies'].pop('https')
+    example_creds_dict["proxies"].pop("http")
+    example_creds_dict["proxies"].pop("https")
     return example_creds_dict
 
 
 @pytest.fixture
 def good_json():
     return """{
         "client_id": "vf3tdjK0jdp7MdY3",
```

### Comparing `pyfusion-1.0.8/tests/test_fusion.py` & `pyfusion-1.0.9/tests/test_fusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,103 +23,133 @@
 
 def test_FusionCredentials_empty_pxy(example_creds_dict_empty_pxy):
     from fusion.fusion import FusionCredentials
 
     FusionCredentials.from_dict(example_creds_dict_empty_pxy)
 
 
-def test_FusionCredentials_from_empty(example_client_id, example_client_secret, example_http_proxy):
+def test_FusionCredentials_from_empty(
+    example_client_id, example_client_secret, example_http_proxy
+):
     from fusion.authentication import FusionCredentials
 
     creds = FusionCredentials.generate_credentials_file(
         client_id=example_client_id, client_secret=example_client_secret, proxies={}
     )
 
     assert creds.proxies == {}
 
 
-def test_FusionCredentials_from_str(example_client_id, example_client_secret, example_http_proxy):
+def test_FusionCredentials_from_str(
+    example_client_id, example_client_secret, example_http_proxy
+):
     from fusion.authentication import FusionCredentials
 
     creds = FusionCredentials.generate_credentials_file(
-        client_id=example_client_id, client_secret=example_client_secret, proxies=example_http_proxy
+        client_id=example_client_id,
+        client_secret=example_client_secret,
+        proxies=example_http_proxy,
     )
 
-    assert creds.proxies['http'] == example_http_proxy
+    assert creds.proxies["http"] == example_http_proxy
 
 
 def test_FusionCredentials_from_http_dict(
-    example_client_id, example_client_secret, example_proxy_http_dict, example_http_proxy
+    example_client_id,
+    example_client_secret,
+    example_proxy_http_dict,
+    example_http_proxy,
 ):
     from fusion.authentication import FusionCredentials
 
     creds = FusionCredentials.generate_credentials_file(
-        client_id=example_client_id, client_secret=example_client_secret, proxies=example_proxy_http_dict
+        client_id=example_client_id,
+        client_secret=example_client_secret,
+        proxies=example_proxy_http_dict,
     )
 
-    assert creds.proxies['http'] == example_http_proxy
+    assert creds.proxies["http"] == example_http_proxy
 
 
 def test_FusionCredentials_from_https_dict(
-    example_client_id, example_client_secret, example_proxy_https_dict, example_https_proxy
+    example_client_id,
+    example_client_secret,
+    example_proxy_https_dict,
+    example_https_proxy,
 ):
     from fusion.authentication import FusionCredentials
 
     creds = FusionCredentials.generate_credentials_file(
-        client_id=example_client_id, client_secret=example_client_secret, proxies=example_proxy_https_dict
+        client_id=example_client_id,
+        client_secret=example_client_secret,
+        proxies=example_proxy_https_dict,
     )
 
-    assert creds.proxies['https'] == example_https_proxy
+    assert creds.proxies["https"] == example_https_proxy
 
 
 def test_FusionCredentials_from_both_dict(
-    example_client_id, example_client_secret, example_proxy_both_dict, example_https_proxy, example_http_proxy
+    example_client_id,
+    example_client_secret,
+    example_proxy_both_dict,
+    example_https_proxy,
+    example_http_proxy,
 ):
     from fusion.authentication import FusionCredentials
 
     creds = FusionCredentials.generate_credentials_file(
-        client_id=example_client_id, client_secret=example_client_secret, proxies=example_proxy_both_dict
+        client_id=example_client_id,
+        client_secret=example_client_secret,
+        proxies=example_proxy_both_dict,
     )
 
-    assert creds.proxies['https'] == example_https_proxy
-    assert creds.proxies['http'] == example_http_proxy
+    assert creds.proxies["https"] == example_https_proxy
+    assert creds.proxies["http"] == example_http_proxy
 
 
 def test_FusionCredentials_from_both_alt_dict(
-    example_client_id, example_client_secret, example_proxy_both_alt_dict, example_https_proxy, example_http_proxy
+    example_client_id,
+    example_client_secret,
+    example_proxy_both_alt_dict,
+    example_https_proxy,
+    example_http_proxy,
 ):
     from fusion.authentication import FusionCredentials
 
     creds = FusionCredentials.generate_credentials_file(
-        client_id=example_client_id, client_secret=example_client_secret, proxies=example_proxy_both_alt_dict
+        client_id=example_client_id,
+        client_secret=example_client_secret,
+        proxies=example_proxy_both_alt_dict,
     )
 
-    assert creds.proxies['https'] == example_https_proxy
-    assert creds.proxies['http'] == example_http_proxy
+    assert creds.proxies["https"] == example_https_proxy
+    assert creds.proxies["http"] == example_http_proxy
 
 
 def test_date_parsing():
     import datetime
     from fusion.utils import _normalise_dt_param
 
-    assert '2020-12-12' == _normalise_dt_param(20201212)
-    assert '2020-12-12' == _normalise_dt_param('20201212')
-    assert '2020-12-12' == _normalise_dt_param('2020-12-12')
-    assert '2020-12-12' == _normalise_dt_param(datetime.date(2020, 12, 12))
-    assert '2020-12-12' == _normalise_dt_param(datetime.datetime(2020, 12, 12, 23, 55, 59, 342380))
+    assert "2020-12-12" == _normalise_dt_param(20201212)
+    assert "2020-12-12" == _normalise_dt_param("20201212")
+    assert "2020-12-12" == _normalise_dt_param("2020-12-12")
+    assert "2020-12-12" == _normalise_dt_param(datetime.date(2020, 12, 12))
+    assert "2020-12-12" == _normalise_dt_param(
+        datetime.datetime(2020, 12, 12, 23, 55, 59, 342380)
+    )
 
 
-@pytest.mark.parametrize('ref_int', [-1, 0, 1, 2])
-@pytest.mark.parametrize('pluraliser', [None, 's', 'es'])
+@pytest.mark.parametrize("ref_int", [-1, 0, 1, 2])
+@pytest.mark.parametrize("pluraliser", [None, "s", "es"])
 def test_res_plural(ref_int, pluraliser):
     from fusion.authentication import _res_plural
 
     res = _res_plural(ref_int, pluraliser)
     if abs(ref_int) == 1:
-        assert res == ''
+        assert res == ""
     else:
         assert res == pluraliser
 
 
 def test_is_json_positive(good_json):
     from fusion.authentication import _is_json
```

### Comparing `pyfusion-1.0.8/setup.py` & `pyfusion-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
           'flake8-docstrings>=1.6.0,<2.0.0',
           'mypy>=0.900,<0.901',
           'pytest>=6.2.4,<7.0.0',
           'pytest-cov>=2.12.0,<3.0.0']}
 
 setup_kwargs = {
     'name': 'pyfusion',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': 'JPMC Fusion Developer Tools',
     'long_description': "# PyFusion #\n\nPyFusion is the Python SDK for the Fusion platform API. \n\n## Installation\n\n```bash\npip install pyfusion\n```\n\nFusion by J.P. Morgan is a cloud-native data platform for institutional investors, providing end-to-end data management, analytics, and reporting solutions across the investment lifecycle. The platform allows clients to seamlessly integrate and combine data from multiple sources into a single data model that delivers the benefits and scale and reduces costs, along with the ability to more easily unlock timely analysis and insights. Fusion's open data architecture supports flexible distribution, including partnerships with cloud and data providers, all managed by J.P. Morgan data experts. \n\nFor more information, please visit [fusion.jpmorgan.com](https://fusion.jpmorgan.com)\n\nFor the SDK documentation, please visit [page](https://jpmorganchase.github.io/fusion)\n\n\n\n",
     'author': 'FusionDevs',
     'author_email': 'fusion_developers@jpmorgan.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jpmorganchase/fusion',
```

### Comparing `pyfusion-1.0.8/PKG-INFO` & `pyfusion-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfusion
-Version: 1.0.8
+Version: 1.0.9
 Summary: JPMC Fusion Developer Tools
 Home-page: https://github.com/jpmorganchase/fusion
 License: Apache-2.0
 Author: FusionDevs
 Author-email: fusion_developers@jpmorgan.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,16 +17,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: aws
+Provides-Extra: azr
 Provides-Extra: dev
 Provides-Extra: doc
+Provides-Extra: gcs
 Provides-Extra: test
 Requires-Dist: aiohttp (>=3.7.1)
 Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "test"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "test"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
 Requires-Dist: fsspec (>=2021.6.1)
```

