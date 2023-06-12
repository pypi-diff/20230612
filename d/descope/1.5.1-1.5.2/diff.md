# Comparing `tmp/descope-1.5.1.tar.gz` & `tmp/descope-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descope-1.5.1.tar", max compression
+gzip compressed data, was "descope-1.5.2.tar", max compression
```

## Comparing `descope-1.5.1.tar` & `descope-1.5.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1064 2023-05-15 15:16:00.107712 descope-1.5.1/LICENSE
--rw-r--r--   0        0        0    31005 2023-05-15 15:16:00.107712 descope-1.5.1/README.md
--rw-r--r--   0        0        0      531 2023-05-15 15:16:00.107712 descope-1.5.1/descope/__init__.py
--rw-r--r--   0        0        0      211 2023-05-15 15:16:00.107712 descope-1.5.1/descope/_auth_base.py
--rw-r--r--   0        0        0    21437 2023-05-15 15:16:00.107712 descope-1.5.1/descope/auth.py
--rw-r--r--   0        0        0        0 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/__init__.py
--rw-r--r--   0        0        0     5319 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/enchantedlink.py
--rw-r--r--   0        0        0     6200 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/magiclink.py
--rw-r--r--   0        0        0     1528 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/oauth.py
--rw-r--r--   0        0        0    11067 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/otp.py
--rw-r--r--   0        0        0     8146 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/password.py
--rw-r--r--   0        0        0     1481 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/saml.py
--rw-r--r--   0        0        0     5128 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/totp.py
--rw-r--r--   0        0        0     6705 2023-05-15 15:16:00.107712 descope-1.5.1/descope/authmethod/webauthn.py
--rw-r--r--   0        0        0     4296 2023-05-15 15:16:00.107712 descope-1.5.1/descope/common.py
--rw-r--r--   0        0        0    11583 2023-05-15 15:16:00.107712 descope-1.5.1/descope/descope_client.py
--rw-r--r--   0        0        0     1420 2023-05-15 15:16:00.107712 descope-1.5.1/descope/exceptions.py
--rw-r--r--   0        0        0     5798 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/access_key.py
--rw-r--r--   0        0        0     3933 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/common.py
--rw-r--r--   0        0        0     3394 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/flow.py
--rw-r--r--   0        0        0     3971 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/group.py
--rw-r--r--   0        0        0      959 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/jwt.py
--rw-r--r--   0        0        0     2531 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/permission.py
--rw-r--r--   0        0        0     3094 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/role.py
--rw-r--r--   0        0        0     5895 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/sso_settings.py
--rw-r--r--   0        0        0     3685 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/tenant.py
--rw-r--r--   0        0        0    29070 2023-05-15 15:16:00.107712 descope-1.5.1/descope/management/user.py
--rw-r--r--   0        0        0     1556 2023-05-15 15:16:00.107712 descope-1.5.1/descope/mgmt.py
--rw-r--r--   0        0        0     1220 2023-05-15 15:16:27.592050 descope-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    32073 1970-01-01 00:00:00.000000 descope-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-12 17:44:27.190722 descope-1.5.2/LICENSE
+-rw-r--r--   0        0        0    31590 2023-06-12 17:44:27.190722 descope-1.5.2/README.md
+-rw-r--r--   0        0        0      531 2023-06-12 17:44:27.190722 descope-1.5.2/descope/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-12 17:44:27.190722 descope-1.5.2/descope/_auth_base.py
+-rw-r--r--   0        0        0    20602 2023-06-12 17:44:27.190722 descope-1.5.2/descope/auth.py
+-rw-r--r--   0        0        0        0 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/__init__.py
+-rw-r--r--   0        0        0     5352 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/enchantedlink.py
+-rw-r--r--   0        0        0     6211 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/magiclink.py
+-rw-r--r--   0        0        0     1528 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/oauth.py
+-rw-r--r--   0        0        0    11078 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/otp.py
+-rw-r--r--   0        0        0     8150 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/password.py
+-rw-r--r--   0        0        0     1481 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/saml.py
+-rw-r--r--   0        0        0     5128 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/totp.py
+-rw-r--r--   0        0        0     6705 2023-06-12 17:44:27.190722 descope-1.5.2/descope/authmethod/webauthn.py
+-rw-r--r--   0        0        0     4266 2023-06-12 17:44:27.190722 descope-1.5.2/descope/common.py
+-rw-r--r--   0        0        0    11637 2023-06-12 17:44:27.190722 descope-1.5.2/descope/descope_client.py
+-rw-r--r--   0        0        0     1420 2023-06-12 17:44:27.190722 descope-1.5.2/descope/exceptions.py
+-rw-r--r--   0        0        0     5809 2023-06-12 17:44:27.190722 descope-1.5.2/descope/management/access_key.py
+-rw-r--r--   0        0        0     4604 2023-06-12 17:44:27.190722 descope-1.5.2/descope/management/audit.py
+-rw-r--r--   0        0        0     4050 2023-06-12 17:44:27.190722 descope-1.5.2/descope/management/common.py
+-rw-r--r--   0        0        0     3394 2023-06-12 17:44:27.190722 descope-1.5.2/descope/management/flow.py
+-rw-r--r--   0        0        0     3971 2023-06-12 17:44:27.190722 descope-1.5.2/descope/management/group.py
+-rw-r--r--   0        0        0      959 2023-06-12 17:44:27.190722 descope-1.5.2/descope/management/jwt.py
+-rw-r--r--   0        0        0     2535 2023-06-12 17:44:27.194722 descope-1.5.2/descope/management/permission.py
+-rw-r--r--   0        0        0     3098 2023-06-12 17:44:27.194722 descope-1.5.2/descope/management/role.py
+-rw-r--r--   0        0        0     6386 2023-06-12 17:44:27.194722 descope-1.5.2/descope/management/sso_settings.py
+-rw-r--r--   0        0        0     3689 2023-06-12 17:44:27.194722 descope-1.5.2/descope/management/tenant.py
+-rw-r--r--   0        0        0    30085 2023-06-12 17:44:27.194722 descope-1.5.2/descope/management/user.py
+-rw-r--r--   0        0        0     1710 2023-06-12 17:44:27.194722 descope-1.5.2/descope/mgmt.py
+-rw-r--r--   0        0        0     1220 2023-06-12 17:44:59.792024 descope-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    32610 1970-01-01 00:00:00.000000 descope-1.5.2/PKG-INFO
```

### Comparing `descope-1.5.1/LICENSE` & `descope-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/README.md` & `descope-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 3. [Manage Access Keys](#manage-access-keys)
 4. [Manage SSO Setting](#manage-sso-setting)
 5. [Manage Permissions](#manage-permissions)
 6. [Manage Roles](#manage-roles)
 7. [Query SSO Groups](#query-sso-groups)
 8. [Manage Flows](#manage-flows)
 9. [Manage JWTs](#manage-jwts)
+10. [Search Audit](#search-audit)
 
 If you wish to run any of our code samples and play with them, check out our [Code Examples](#code-examples) section.
 
 If you're performing end-to-end testing, check out the [Utils for your end to end (e2e) tests and integration tests](#utils-for-your-end-to-end-e2e-tests-and-integration-tests) section. You will need to use the `DescopeClient` object created under [Setup](#setup-1) guide.
 
 For rate limiting information, please confer to the [API Rate Limits](#api-rate-limits) section.
 
@@ -308,25 +309,25 @@
 
 In the [password authentication method](https://app.descope.com/settings/authentication/password) in the Descope console, it is possible to define which alternative authentication method can be used in order to authenticate the user, in order to reset and update their password.
 
 ```python
 # Start the reset process by sending a password reset prompt. In this example we'll assume
 # that magic link is configured as the reset method. The optional redirect URL is used in the
 # same way as in regular magic link authentication.
-login_id := "desmond@descope.com"
-redirect_url := "https://myapp.com/password-reset"
+login_id = "desmond@descope.com"
+redirect_url = "https://myapp.com/password-reset"
 descope_client.password.send_reset(login_id, redirect_url)
 ```
 
 The magic link, in this case, must then be verified like any other magic link (see the [magic link section](#magic-link) for more details). However, after verifying the user, it is expected
 to allow them to provide a new password instead of the old one. Since the user is now authenticated, this is possible via:
 
 ```python
 # The refresh token is required to make sure the user is authenticated.
-err := descope_client.password.update(login_id, new_password, token)
+err = descope_client.password.update(login_id, new_password, token)
 ```
 
 `update` can always be called when the user is authenticated and has a valid session.
 
 Alternatively, it is also possible to replace an existing active password with a new one.
 
 ```python
@@ -761,22 +762,37 @@
 
 ### Manage JWTs
 
 You can add custom claims to a valid JWT.
 
 ```python
 updated_jwt = descope_client.mgmt.jwt.update_jwt(
-    jwt: "original-jwt",
-    custom_claims: {
+    jwt="original-jwt",
+    custom_claims={
         "custom-key1": "custom-value1",
         "custom-key2": "custom-value2"
     },
 )
 ```
 
+### Search Audit
+
+You can perform an audit search for either specific values or full-text across the fields. Audit search is limited to the last 30 days.
+Below are some examples. For a full list of available search criteria options, see the function documentation.
+
+```python
+# Full text search on last 10 days
+audits = descope_client.mgmt.audit.search(
+    text="some-text",
+    from_ts=datetime.now(timezone.utc)-timedelta(days=10)
+)
+# Search successful logins in the last 30 days
+audits = descope_client.mgmt.audit.search(actions=["LoginSucceed"])
+```
+
 ### Utils for your end to end (e2e) tests and integration tests
 
 To ease your e2e tests, we exposed dedicated management methods,
 that way, you don't need to use 3rd party messaging services in order to receive sign-in/up Emails or SMS, and avoid the need of parsing the code and token from them.
 
 ```Python
 # User for test can be created, this user will be able to generate code/link without
```

### Comparing `descope-1.5.1/descope/__init__.py` & `descope-1.5.2/descope/__init__.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/auth.py` & `descope-1.5.2/descope/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import json
 import os
 import platform
 import re
+from http import HTTPStatus
 from threading import Lock
 from typing import Tuple
 
 import jwt
 import pkg_resources
 import requests
 from email_validator import EmailNotValidError, validate_email
@@ -30,64 +31,62 @@
     ERROR_TYPE_INVALID_PUBLIC_KEY,
     ERROR_TYPE_INVALID_TOKEN,
     ERROR_TYPE_SERVER_ERROR,
     AuthException,
     RateLimitException,
 )
 
+_default_headers = {
+    "Content-Type": "application/json",
+    "x-descope-sdk-name": "python",
+}
+
 
 class Auth:
     ALGORITHM_KEY = "alg"
 
     def __init__(
         self,
         project_id: str = None,
         public_key: str = None,
         skip_verify: bool = False,
         management_key: str = None,
         timeout_seconds: float = DEFAULT_TIMEOUT_SECONDS,
     ):
         self.lock_public_keys = Lock()
         # validate project id
+        project_id = project_id or os.getenv("DESCOPE_PROJECT_ID")
         if not project_id:
-            # try get the project_id from env
-            project_id = os.getenv("DESCOPE_PROJECT_ID", "")
-            if project_id == "":
-                raise AuthException(
-                    400,
-                    ERROR_TYPE_INVALID_ARGUMENT,
-                    "Unable to init Auth object because project_id cannot be empty. Set environment variable DESCOPE_PROJECT_ID or pass your Project ID to the init function.",
-                )
+            raise AuthException(
+                400,
+                ERROR_TYPE_INVALID_ARGUMENT,
+                (
+                    "Unable to init Auth object because project_id cannot be empty. "
+                    "Set environment variable DESCOPE_PROJECT_ID or pass your Project ID to the init function."
+                ),
+            )
         self.project_id = project_id
+        self.secure = not skip_verify
 
-        self.secure = True
-        if skip_verify:
-            self.secure = False
-
-        self.base_url = os.getenv("DESCOPE_BASE_URI", None) or DEFAULT_BASE_URL
+        self.base_url = os.getenv("DESCOPE_BASE_URI") or DEFAULT_BASE_URL
         self.timeout_seconds = timeout_seconds
+        self.management_key = management_key or os.getenv("DESCOPE_MANAGEMENT_KEY")
 
-        if not management_key:
-            management_key = os.getenv("DESCOPE_MANAGEMENT_KEY", None)
-        self.management_key = management_key
-
-        if not public_key:
-            public_key = os.getenv("DESCOPE_PUBLIC_KEY", None)
-
+        public_key = public_key or os.getenv("DESCOPE_PUBLIC_KEY")
         with self.lock_public_keys:
             if not public_key:
                 self.public_keys = {}
             else:
                 kid, pub_key, alg = self._validate_and_load_public_key(public_key)
                 self.public_keys = {kid: (pub_key, alg)}
 
     def _raise_rate_limit_exception(self, response):
         resp = response.json()
         raise RateLimitException(
-            resp.get("errorCode", "429"),
+            resp.get("errorCode", HTTPStatus.TOO_MANY_REQUESTS),
             ERROR_TYPE_API_RATE_LIMIT,
             resp.get("errorDescription", ""),
             resp.get("errorMessage", ""),
             rate_limit_parameters={
                 API_RATE_LIMIT_RETRY_AFTER_HEADER: int(
                     response.headers.get(API_RATE_LIMIT_RETRY_AFTER_HEADER, 0)
                 )
@@ -105,78 +104,62 @@
             f"{self.base_url}{uri}",
             headers=self._get_default_headers(pswd),
             params=params,
             allow_redirects=allow_redirects,
             verify=self.secure,
             timeout=self.timeout_seconds,
         )
-        if not response.ok:
-            if response.status_code == 429:
-                self._raise_rate_limit_exception(response)  # Raise RateLimitException
-            raise AuthException(
-                response.status_code, ERROR_TYPE_SERVER_ERROR, response.text
-            )
+        self._raise_from_response(response)
         return response
 
     def do_post(
         self, uri: str, body: dict, params=None, pswd: str = None
     ) -> requests.Response:
         response = requests.post(
             f"{self.base_url}{uri}",
             headers=self._get_default_headers(pswd),
-            data=json.dumps(body),
+            json=body,
             allow_redirects=False,
             verify=self.secure,
             params=params,
             timeout=self.timeout_seconds,
         )
-        if not response.ok:
-            if response.status_code == 429:
-                self._raise_rate_limit_exception(response)  # Raise RateLimitException
-
-            raise AuthException(
-                response.status_code, ERROR_TYPE_SERVER_ERROR, response.text
-            )
+        self._raise_from_response(response)
         return response
 
-    def do_delete(self, uri: str, pswd: str = None) -> requests.Response:
+    def do_delete(self, uri: str, params=None, pswd: str = None) -> requests.Response:
         response = requests.delete(
             f"{self.base_url}{uri}",
+            params=params,
             headers=self._get_default_headers(pswd),
             allow_redirects=False,
             verify=self.secure,
             timeout=self.timeout_seconds,
         )
-        if not response.ok:
-            if response.status_code == 429:
-                self._raise_rate_limit_exception(response)  # Raise RateLimitException
-
-            raise AuthException(
-                response.status_code, ERROR_TYPE_SERVER_ERROR, response.text
-            )
+        self._raise_from_response(response)
         return response
 
     def exchange_token(self, uri, code: str) -> dict:
         if not code:
             raise AuthException(
                 400,
                 ERROR_TYPE_INVALID_ARGUMENT,
                 "exchange code is empty",
             )
 
         body = Auth._compose_exchange_body(code)
-        response = self.do_post(uri, body, None)
+        response = self.do_post(uri=uri, body=body, params=None)
         resp = response.json()
         jwt_response = self.generate_jwt_response(
-            resp, response.cookies.get(REFRESH_SESSION_COOKIE_NAME, None)
+            resp, response.cookies.get(REFRESH_SESSION_COOKIE_NAME)
         )
         return jwt_response
 
     @staticmethod
-    def verify_delivery_method(
+    def adjust_and_verify_delivery_method(
         method: DeliveryMethod, login_id: str, user: dict
     ) -> bool:
         if not login_id:
             return False
 
         if not isinstance(user, dict):
             return False
@@ -202,57 +185,57 @@
         else:
             return False
 
         return True
 
     @staticmethod
     def compose_url(base: str, method: DeliveryMethod) -> str:
-        suffix = ""
-        if method is DeliveryMethod.EMAIL:
-            suffix = "email"
-        elif method is DeliveryMethod.SMS:
-            suffix = "sms"
-        elif method is DeliveryMethod.WHATSAPP:
-            suffix = "whatsapp"
-        else:
+        suffix = {
+            DeliveryMethod.EMAIL: "email",
+            DeliveryMethod.SMS: "sms",
+            DeliveryMethod.WHATSAPP: "whatsapp",
+        }.get(method)
+
+        if not suffix:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, f"Unknown delivery method: {method}"
             )
 
         return f"{base}/{suffix}"
 
     @staticmethod
     def get_login_id_by_method(method: DeliveryMethod, user: dict) -> Tuple[str, str]:
-        if method is DeliveryMethod.EMAIL:
-            email = user.get("email", "")
-            return "email", email
-        elif method is DeliveryMethod.SMS:
-            phone = user.get("phone", "")
-            return "phone", phone
-        elif method is DeliveryMethod.WHATSAPP:
-            whatsapp = user.get("phone", "")
-            return ("whatsapp", whatsapp)
-        else:
+        login_id = {
+            DeliveryMethod.EMAIL: ("email", user.get("email", "")),
+            DeliveryMethod.SMS: ("phone", user.get("phone", "")),
+            DeliveryMethod.WHATSAPP: ("whatsapp", user.get("phone", "")),
+        }.get(method)
+
+        if not login_id:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, f"Unknown delivery method: {method}"
             )
 
+        return login_id
+
     @staticmethod
     def get_method_string(method: DeliveryMethod) -> str:
-        if method is DeliveryMethod.EMAIL:
-            return "email"
-        elif method is DeliveryMethod.SMS:
-            return "sms"
-        elif method is DeliveryMethod.WHATSAPP:
-            return "whatsapp"
-        else:
+        name = {
+            DeliveryMethod.EMAIL: "email",
+            DeliveryMethod.SMS: "sms",
+            DeliveryMethod.WHATSAPP: "whatsapp",
+        }.get(method)
+
+        if not name:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, f"Unknown delivery method: {method}"
             )
 
+        return name
+
     @staticmethod
     def validate_email(email: str):
         if email == "":
             raise AuthException(
                 400,
                 ERROR_TYPE_INVALID_ARGUMENT,
                 "email address argument cannot be empty",
@@ -282,41 +265,43 @@
         if method != DeliveryMethod.SMS and method != DeliveryMethod.WHATSAPP:
             raise AuthException(
                 400, ERROR_TYPE_INVALID_ARGUMENT, "Invalid delivery method"
             )
 
     def exchange_access_key(self, access_key: str) -> dict:
         uri = EndpointsV1.exchange_auth_access_key_path
-        server_response = self.do_post(uri, {}, None, access_key)
+        server_response = self.do_post(uri=uri, body={}, params=None, pswd=access_key)
         json = server_response.json()
-        return self._generate_auth_info(json, None, False)
+        return self._generate_auth_info(
+            response_body=json, refresh_token=None, user_jwt=False
+        )
 
     @staticmethod
     def _compose_exchange_body(code: str) -> dict:
         return {"code": code}
 
     @staticmethod
     def _validate_and_load_public_key(public_key) -> Tuple[str, jwt.PyJWK, str]:
+        if not isinstance(public_key, (str, dict)):
+            raise AuthException(
+                500,
+                ERROR_TYPE_INVALID_PUBLIC_KEY,
+                "Unable to load public key. Invalid public key error: (unknown type)",
+            )
+
         if isinstance(public_key, str):
             try:
                 public_key = json.loads(public_key)
             except Exception as e:
                 raise AuthException(
                     500,
                     ERROR_TYPE_INVALID_PUBLIC_KEY,
                     f"Unable to load public key. error: {e}",
                 )
 
-        if not isinstance(public_key, dict):
-            raise AuthException(
-                500,
-                ERROR_TYPE_INVALID_PUBLIC_KEY,
-                "Unable to load public key. Invalid public key error: (unknown type)",
-            )
-
         alg = public_key.get(Auth.ALGORITHM_KEY, None)
         if alg is None:
             raise AuthException(
                 500,
                 ERROR_TYPE_INVALID_PUBLIC_KEY,
                 "Unable to load public key. Missing property: alg",
             )
@@ -327,44 +312,44 @@
                 500,
                 ERROR_TYPE_INVALID_PUBLIC_KEY,
                 "Unable to load public key. Missing property: kid",
             )
         try:
             # Load and validate public key
             return (kid, jwt.PyJWK(public_key), alg)
-        except jwt.InvalidKeyError as e:
-            raise AuthException(
-                500,
-                ERROR_TYPE_INVALID_PUBLIC_KEY,
-                f"Unable to load public key. Error: {e}",
-            )
-        except jwt.PyJWKError as e:
+        except (jwt.PyJWKError, jwt.InvalidKeyError) as e:
             raise AuthException(
                 500,
                 ERROR_TYPE_INVALID_PUBLIC_KEY,
                 f"Unable to load public key {e}",
             )
 
+    def _raise_from_response(self, response):
+        """Raise appropriate exception from response, does nothing if response.ok is True."""
+        if response.ok:
+            return
+
+        if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
+            self._raise_rate_limit_exception(response)  # Raise RateLimitException
+
+        raise AuthException(
+            response.status_code,
+            ERROR_TYPE_SERVER_ERROR,
+            f"Error: {response.reason}",
+        )
+
     def _fetch_public_keys(self) -> None:
         # This function called under mutex protection so no need to acquire it once again
         response = requests.get(
             f"{self.base_url}{EndpointsV2.public_key_path}/{self.project_id}",
             headers=self._get_default_headers(),
             verify=self.secure,
             timeout=self.timeout_seconds,
         )
-
-        if not response.ok:
-            if response.status_code == 429:
-                self._raise_rate_limit_exception(response)  # Raise RateLimitException
-            raise AuthException(
-                response.status_code,
-                ERROR_TYPE_SERVER_ERROR,
-                f"Error: {response.reason}",
-            )
+        self._raise_from_response(response)
 
         jwks_data = response.text
         try:
             jwkeys_wrapper = json.loads(jwks_data)
             jwkeys = jwkeys_wrapper["keys"]
         except Exception as e:
             raise AuthException(
@@ -379,25 +364,25 @@
                 self.public_keys[loaded_kid] = (pub_key, alg)
             except Exception:
                 # just continue to the next key
                 pass
 
     def adjust_properties(self, jwt_response: dict, user_jwt: bool):
         # Save permissions, roles and tenants info from Session token or from refresh token on the json top level
-        if jwt_response.get(SESSION_TOKEN_NAME, None):
+        if SESSION_TOKEN_NAME in jwt_response:
             jwt_response["permissions"] = jwt_response.get(SESSION_TOKEN_NAME).get(
                 "permissions", []
             )
             jwt_response["roles"] = jwt_response.get(SESSION_TOKEN_NAME).get(
                 "roles", []
             )
             jwt_response["tenants"] = jwt_response.get(SESSION_TOKEN_NAME).get(
                 "tenants", {}
             )
-        elif jwt_response.get(REFRESH_SESSION_TOKEN_NAME, None):
+        elif REFRESH_SESSION_TOKEN_NAME in jwt_response:
             jwt_response["permissions"] = jwt_response.get(
                 REFRESH_SESSION_TOKEN_NAME
             ).get("permissions", [])
             jwt_response["roles"] = jwt_response.get(REFRESH_SESSION_TOKEN_NAME).get(
                 "roles", []
             )
             jwt_response["tenants"] = jwt_response.get(REFRESH_SESSION_TOKEN_NAME).get(
@@ -463,19 +448,15 @@
         jwt_response = self._generate_auth_info(response_body, refresh_cookie, True)
 
         jwt_response["user"] = response_body.get("user", {})
         jwt_response["firstSeen"] = response_body.get("firstSeen", True)
         return jwt_response
 
     def _get_default_headers(self, pswd: str = None):
-        headers = {}
-        headers["Content-Type"] = "application/json"
-
-        headers["x-descope-sdk-name"] = "python"
-
+        headers = _default_headers.copy()
         try:
             headers["x-descope-sdk-python-version"] = platform.python_version()
             headers["x-descope-sdk-version"] = pkg_resources.get_distribution(
                 "descope"
             ).version
         except Exception:
             pass
@@ -577,15 +558,15 @@
         except Exception as e:
             # Refresh is invalid
             raise AuthException(
                 401, ERROR_TYPE_INVALID_TOKEN, f"Invalid refresh token: {e}"
             )
 
         uri = EndpointsV1.refresh_token_path
-        response = self.do_post(uri, {}, None, refresh_token)
+        response = self.do_post(uri=uri, body={}, params=None, pswd=refresh_token)
 
         resp = response.json()
         return self.generate_jwt_response(resp, refresh_token)
 
     def validate_and_refresh_session(
         self, session_token: str = None, refresh_token: str = None
     ) -> dict:
```

### Comparing `descope-1.5.1/descope/authmethod/enchantedlink.py` & `descope-1.5.2/descope/authmethod/enchantedlink.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,17 @@
         response = self._auth.do_post(uri, body, None, refresh_token)
         return EnchantedLink._get_pending_ref_from_response(response)
 
     def sign_up(self, login_id: str, uri: str, user: dict = None) -> dict:
         if not user:
             user = {}
 
-        if not self._auth.verify_delivery_method(DeliveryMethod.EMAIL, login_id, user):
+        if not self._auth.adjust_and_verify_delivery_method(
+            DeliveryMethod.EMAIL, login_id, user
+        ):
             raise AuthException(
                 400,
                 ERROR_TYPE_INVALID_ARGUMENT,
                 f"Login ID {login_id} is not valid for email",
             )
 
         body = EnchantedLink._compose_signup_body(login_id, uri, user)
```

### Comparing `descope-1.5.1/descope/authmethod/magiclink.py` & `descope-1.5.2/descope/authmethod/magiclink.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def sign_up(
         self, method: DeliveryMethod, login_id: str, uri: str, user: dict = None
     ) -> str:
         if not user:
             user = {}
 
-        if not self._auth.verify_delivery_method(method, login_id, user):
+        if not self._auth.adjust_and_verify_delivery_method(method, login_id, user):
             raise AuthException(
                 400,
                 ERROR_TYPE_INVALID_ARGUMENT,
                 f"Login ID {login_id} is not valid by delivery method {method}",
             )
 
         body = MagicLink._compose_signup_body(method, login_id, uri, user)
```

### Comparing `descope-1.5.1/descope/authmethod/oauth.py` & `descope-1.5.2/descope/authmethod/oauth.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/authmethod/otp.py` & `descope-1.5.2/descope/authmethod/otp.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         Raise:
         AuthException: raised if sign-up operation fails
         """
 
         if not user:
             user = {}
 
-        if not self._auth.verify_delivery_method(method, login_id, user):
+        if not self._auth.adjust_and_verify_delivery_method(method, login_id, user):
             raise AuthException(
                 400,
                 ERROR_TYPE_INVALID_ARGUMENT,
                 f"Login ID {login_id} is not valid by delivery method {method}",
             )
 
         uri = OTP._compose_signup_url(method)
```

### Comparing `descope-1.5.1/descope/authmethod/password.py` & `descope-1.5.2/descope/authmethod/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             number - the password required at least one number character
             nonAlphanumeric - the password required at least one non alphanumeric character
 
         Raise:
         AuthException: raised if get policy operation fails
         """
 
-        response = self._auth.do_get(EndpointsV1.password_policy_path)
+        response = self._auth.do_get(uri=EndpointsV1.password_policy_path)
         return response.json()
 
     @staticmethod
     def _compose_signup_body(login_id: str, password: str, user: dict) -> dict:
         body = {"loginId": login_id, "password": password}
         if user is not None:
             body["user"] = user
```

### Comparing `descope-1.5.1/descope/authmethod/saml.py` & `descope-1.5.2/descope/authmethod/saml.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/authmethod/totp.py` & `descope-1.5.2/descope/authmethod/totp.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/authmethod/webauthn.py` & `descope-1.5.2/descope/authmethod/webauthn.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/common.py` & `descope-1.5.2/descope/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
 DEFAULT_BASE_URL = "https://api.descope.com"  # pragma: no cover
 DEFAULT_TIMEOUT_SECONDS = 60
 
-PHONE_REGEX = """^(?:(?:\\(?(?:00|\\+)([1-4]\\d\\d|[1-9]\\d?)\\)?)?[\\-\\.\\ \\\\/]?)?((?:\\(?\\d{1,}\\)?[\\-\\.\\ \\\\/]?){0,})(?:[\\-\\.\\ \\\\/]?(?:#|ext\\.?|extension|x)[\\-\\.\\ \\\\/]?(\\d+))?$"""
+PHONE_REGEX = r"""^(?:(?:\(?(?:00|\+)([1-4]\d\d|[1-9]\d?)\)?)?[\-\.\ \\/]?)?((?:\(?\d{1,}\)?[\-\.\ \\/]?){0,})(?:[\-\.\ \\/]?(?:#|ext\.?|extension|x)[\-\.\ \\/]?(\d+))?$"""
 
 SESSION_COOKIE_NAME = "DS"
 REFRESH_SESSION_COOKIE_NAME = "DSR"
 
 SESSION_TOKEN_NAME = "sessionToken"
 REFRESH_SESSION_TOKEN_NAME = "refreshSessionToken"
 COOKIE_DATA_NAME = "cookieData"
```

### Comparing `descope-1.5.1/descope/descope_client.py` & `descope-1.5.2/descope/descope_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,17 @@
             raise AuthException(
                 400,
                 ERROR_TYPE_INVALID_ARGUMENT,
                 f"signed refresh token {refresh_token} is empty",
             )
 
         uri = EndpointsV1.me_path
-        response = self._auth.do_get(uri, None, None, refresh_token)
+        response = self._auth.do_get(
+            uri=uri, params=None, allow_redirects=None, pswd=refresh_token
+        )
         return response.json()
 
     def exchange_access_key(self, access_key: str) -> dict:
         """
         Return a new session token for the given access key
 
         Args:
```

### Comparing `descope-1.5.1/descope/exceptions.py` & `descope-1.5.2/descope/exceptions.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/management/access_key.py` & `descope-1.5.2/descope/management/access_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,16 @@
              {"key": {}}
         Containing the loaded access key information.
 
         Raise:
         AuthException: raised if load operation fails
         """
         response = self._auth.do_get(
-            MgmtV1.access_key_load_path,
-            {"id": id},
+            uri=MgmtV1.access_key_load_path,
+            params={"id": id},
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def search_all_access_keys(
         self,
         tenant_ids: List[str] = None,
```

### Comparing `descope-1.5.1/descope/management/common.py` & `descope-1.5.2/descope/management/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     # user
     user_create_path = "/v1/mgmt/user/create"
     user_update_path = "/v1/mgmt/user/update"
     user_delete_path = "/v1/mgmt/user/delete"
     user_delete_all_test_users_path = "/v1/mgmt/user/test/delete/all"
     user_load_path = "/v1/mgmt/user"
     users_search_path = "/v1/mgmt/user/search"
+    user_get_provider_token = "/v1/mgmt/user/provider/token"
     user_update_status_path = "/v1/mgmt/user/update/status"
     user_update_email_path = "/v1/mgmt/user/update/email"
     user_update_phone_path = "/v1/mgmt/user/update/phone"
     user_update_name_path = "/v1/mgmt/user/update/name"
     user_update_picture_path = "/v1/mgmt/user/update/picture"
     user_update_custom_attribute_path = "/v1/mgmt/user/update/customAttribute"
     user_add_role_path = "/v1/mgmt/user/update/role/add"
@@ -69,14 +70,17 @@
     theme_export_path = "/v1/mgmt/theme/export"
 
     # group
     group_load_all_path = "/v1/mgmt/group/all"
     group_load_all_for_member_path = "/v1/mgmt/group/member/all"
     group_load_all_group_members_path = "/v1/mgmt/group/members"
 
+    # Audit
+    audit_search = "/v1/mgmt/audit/search"
+
 
 class AssociatedTenant:
     """
     Represents a tenant association for a User or Access Key. The tenant_id is required to denote
     which tenant the user or access key belongs to. The role_names array is an optional list of
     roles for the user or access key in this specific tenant.
     """
```

### Comparing `descope-1.5.1/descope/management/flow.py` & `descope-1.5.2/descope/management/flow.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/management/group.py` & `descope-1.5.2/descope/management/group.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/management/jwt.py` & `descope-1.5.2/descope/management/jwt.py`

 * *Files identical despite different names*

### Comparing `descope-1.5.1/descope/management/permission.py` & `descope-1.5.2/descope/management/permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,11 +78,11 @@
              {"permissions": [{"name": <name>, "description": <description>, "systemDefault":<True/False>}]}
         Containing the loaded permission information.
 
         Raise:
         AuthException: raised if load operation fails
         """
         response = self._auth.do_get(
-            MgmtV1.permission_load_all_path,
+            uri=MgmtV1.permission_load_all_path,
             pswd=self._auth.management_key,
         )
         return response.json()
```

### Comparing `descope-1.5.1/descope/management/role.py` & `descope-1.5.2/descope/management/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,11 +96,11 @@
              {"roles": [{"name": <name>, "description": <description>, "permissionNames":[]}] }
         Containing the loaded role information.
 
         Raise:
         AuthException: raised if load operation fails
         """
         response = self._auth.do_get(
-            MgmtV1.role_load_all_path,
+            uri=MgmtV1.role_load_all_path,
             pswd=self._auth.management_key,
         )
         return response.json()
```

### Comparing `descope-1.5.1/descope/management/sso_settings.py` & `descope-1.5.2/descope/management/sso_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,38 @@
         Return value (dict):
         Containing the loaded SSO settings information.
 
         Raise:
         AuthException: raised if configuration operation fails
         """
         response = self._auth.do_get(
+            uri=MgmtV1.sso_settings_path,
+            params={"tenantId": tenant_id},
+            pswd=self._auth.management_key,
+        )
+        return response.json()
+
+    def delete_settings(
+        self,
+        tenant_id: str,
+    ):
+        """
+        Delete SSO setting for the provided tenant_id.
+
+        Args:
+        tenant_id (str): The tenant ID of the desired SSO Settings to delete
+
+        Raise:
+        AuthException: raised if configuration operation fails
+        """
+        self._auth.do_delete(
             MgmtV1.sso_settings_path,
             {"tenantId": tenant_id},
             pswd=self._auth.management_key,
         )
-        return response.json()
 
     def configure(
         self,
         tenant_id: str,
         idp_url: str,
         entity_id: str,
         idp_cert: str,
```

### Comparing `descope-1.5.1/descope/management/tenant.py` & `descope-1.5.2/descope/management/tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
              {"tenants": [{"id": <id>, "name": <name>, "selfProvisioningDomains": []}]}
         Containing the loaded tenant information.
 
         Raise:
         AuthException: raised if load operation fails
         """
         response = self._auth.do_get(
-            MgmtV1.tenant_load_all_path,
+            uri=MgmtV1.tenant_load_all_path,
             pswd=self._auth.management_key,
         )
         return response.json()
 
     @staticmethod
     def _compose_create_update_body(
         name: str, id: str, self_provisioning_domains: List[str]
```

### Comparing `descope-1.5.1/descope/management/user.py` & `descope-1.5.2/descope/management/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -264,16 +264,16 @@
              {"user": {}}
         Containing the loaded user information.
 
         Raise:
         AuthException: raised if load operation fails
         """
         response = self._auth.do_get(
-            MgmtV1.user_load_path,
-            {"loginId": login_id},
+            uri=MgmtV1.user_load_path,
+            params={"loginId": login_id},
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def load_by_user_id(
         self,
         user_id: str,
@@ -290,16 +290,16 @@
              {"user": {}}
         Containing the loaded user information.
 
         Raise:
         AuthException: raised if load operation fails
         """
         response = self._auth.do_get(
-            MgmtV1.user_load_path,
-            {"userId": user_id},
+            uri=MgmtV1.user_load_path,
+            params={"userId": user_id},
             pswd=self._auth.management_key,
         )
         return response.json()
 
     def search_all(
         self,
         tenant_ids: List[str] = None,
@@ -355,14 +355,43 @@
         response = self._auth.do_post(
             MgmtV1.users_search_path,
             body=body,
             pswd=self._auth.management_key,
         )
         return response.json()
 
+    def get_provider_token(
+        self,
+        login_id: str,
+        provider: str,
+    ) -> dict:
+        """
+        Get the provider token for the given login ID.
+        Only users that sign-in using social providers will have token.
+        Note: The 'Manage tokens from provider' setting must be enabled.
+
+        Args:
+        login_id (str): The login ID of the user.
+        provider (str): The provider name (google, facebook, etc').
+
+        Return value (dict):
+        Return dict in the format
+             {"provider": "", "providerUserId": "", "accessToken": "", "expiration": "", "scopes": "[]"}
+        Containing the provider token of the given user and provider.
+
+        Raise:
+        AuthException: raised if the operation fails
+        """
+        response = self._auth.do_get(
+            MgmtV1.user_get_provider_token,
+            {"loginId": login_id, "provider": provider},
+            pswd=self._auth.management_key,
+        )
+        return response.json()
+
     def activate(
         self,
         login_id: str,
     ) -> dict:
         """
         Activate an existing user.
```

### Comparing `descope-1.5.1/descope/mgmt.py` & `descope-1.5.2/descope/mgmt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from descope.auth import Auth
 from descope.management.access_key import AccessKey  # noqa: F401
+from descope.management.audit import Audit  # noqa: F401
 from descope.management.flow import Flow  # noqa: F401
 from descope.management.group import Group  # noqa: F401
 from descope.management.jwt import JWT  # noqa: F401
 from descope.management.permission import Permission  # noqa: F401
 from descope.management.role import Role  # noqa: F401
 from descope.management.sso_settings import SSOSettings  # noqa: F401
 from descope.management.tenant import Tenant  # noqa: F401
@@ -20,14 +21,15 @@
         self._access_key = AccessKey(auth)
         self._sso = SSOSettings(auth)
         self._jwt = JWT(auth)
         self._permission = Permission(auth)
         self._role = Role(auth)
         self._group = Group(auth)
         self._flow = Flow(auth)
+        self._audit = Audit(auth)
 
     @property
     def tenant(self):
         return self._tenant
 
     @property
     def user(self):
@@ -56,7 +58,11 @@
     @property
     def group(self):
         return self._group
 
     @property
     def flow(self):
         return self._flow
+
+    @property
+    def audit(self):
+        return self._audit
```

### Comparing `descope-1.5.1/pyproject.toml` & `descope-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descope"
-version = "1.5.1"
+version = "1.5.2"
 description = "Descope Python SDK"
 authors = ["Descope <info@descope.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://descope.com/"
 repository = "https://github.com/descope/python-sdk"
 documentation = "https://docs.descope.com"
@@ -21,27 +21,27 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/descope/python-sdk/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-requests = "2.30.0" # First support for python 3.10
+requests = "2.31.0" # First support for python 3.10
 PyJWT = {version = "2.7.0", extras = ["crypto"]} # Latest secrutiy update
 email-validator = "==2.0.0.post2"
 
 [tool.poetry.group.dev.dependencies]
 mock = "5.0.2"
 pre-commit = "2.21.0"
 Flask = "2.2.5"
 flake8 = "5.0.4"
 flake8-bugbear = "22.12.6"
 pytest-cov = "4.0.0"
 pytest = "7.3.1"
 black = "23.3.0"
-liccheck = "0.9.0"
+liccheck = "0.9.1"
 isort = "5.11.4"
 pep8-naming = "0.13.3"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `descope-1.5.1/PKG-INFO` & `descope-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: descope
-Version: 1.5.1
+Version: 1.5.2
 Summary: Descope Python SDK
 Home-page: https://descope.com/
 License: MIT
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyJWT[crypto] (==2.7.0)
 Requires-Dist: email-validator (==2.0.0.post2)
-Requires-Dist: requests (==2.30.0)
+Requires-Dist: requests (==2.31.0)
 Project-URL: Bug Tracker, https://github.com/descope/python-sdk/issues
 Project-URL: Documentation, https://docs.descope.com
 Project-URL: Repository, https://github.com/descope/python-sdk
 Description-Content-Type: text/markdown
 
 # Descope SDK for Python
 
@@ -81,14 +80,15 @@
 3. [Manage Access Keys](#manage-access-keys)
 4. [Manage SSO Setting](#manage-sso-setting)
 5. [Manage Permissions](#manage-permissions)
 6. [Manage Roles](#manage-roles)
 7. [Query SSO Groups](#query-sso-groups)
 8. [Manage Flows](#manage-flows)
 9. [Manage JWTs](#manage-jwts)
+10. [Search Audit](#search-audit)
 
 If you wish to run any of our code samples and play with them, check out our [Code Examples](#code-examples) section.
 
 If you're performing end-to-end testing, check out the [Utils for your end to end (e2e) tests and integration tests](#utils-for-your-end-to-end-e2e-tests-and-integration-tests) section. You will need to use the `DescopeClient` object created under [Setup](#setup-1) guide.
 
 For rate limiting information, please confer to the [API Rate Limits](#api-rate-limits) section.
 
@@ -335,25 +335,25 @@
 
 In the [password authentication method](https://app.descope.com/settings/authentication/password) in the Descope console, it is possible to define which alternative authentication method can be used in order to authenticate the user, in order to reset and update their password.
 
 ```python
 # Start the reset process by sending a password reset prompt. In this example we'll assume
 # that magic link is configured as the reset method. The optional redirect URL is used in the
 # same way as in regular magic link authentication.
-login_id := "desmond@descope.com"
-redirect_url := "https://myapp.com/password-reset"
+login_id = "desmond@descope.com"
+redirect_url = "https://myapp.com/password-reset"
 descope_client.password.send_reset(login_id, redirect_url)
 ```
 
 The magic link, in this case, must then be verified like any other magic link (see the [magic link section](#magic-link) for more details). However, after verifying the user, it is expected
 to allow them to provide a new password instead of the old one. Since the user is now authenticated, this is possible via:
 
 ```python
 # The refresh token is required to make sure the user is authenticated.
-err := descope_client.password.update(login_id, new_password, token)
+err = descope_client.password.update(login_id, new_password, token)
 ```
 
 `update` can always be called when the user is authenticated and has a valid session.
 
 Alternatively, it is also possible to replace an existing active password with a new one.
 
 ```python
@@ -788,22 +788,37 @@
 
 ### Manage JWTs
 
 You can add custom claims to a valid JWT.
 
 ```python
 updated_jwt = descope_client.mgmt.jwt.update_jwt(
-    jwt: "original-jwt",
-    custom_claims: {
+    jwt="original-jwt",
+    custom_claims={
         "custom-key1": "custom-value1",
         "custom-key2": "custom-value2"
     },
 )
 ```
 
+### Search Audit
+
+You can perform an audit search for either specific values or full-text across the fields. Audit search is limited to the last 30 days.
+Below are some examples. For a full list of available search criteria options, see the function documentation.
+
+```python
+# Full text search on last 10 days
+audits = descope_client.mgmt.audit.search(
+    text="some-text",
+    from_ts=datetime.now(timezone.utc)-timedelta(days=10)
+)
+# Search successful logins in the last 30 days
+audits = descope_client.mgmt.audit.search(actions=["LoginSucceed"])
+```
+
 ### Utils for your end to end (e2e) tests and integration tests
 
 To ease your e2e tests, we exposed dedicated management methods,
 that way, you don't need to use 3rd party messaging services in order to receive sign-in/up Emails or SMS, and avoid the need of parsing the code and token from them.
 
 ```Python
 # User for test can be created, this user will be able to generate code/link without
```

