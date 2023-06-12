# Comparing `tmp/petstore-sdk-2.3.8.tar.gz` & `tmp/petstore-sdk-6.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petstore-sdk-2.3.8.tar", last modified: Wed May 24 13:46:19 2023, max compression
+gzip compressed data, was "petstore-sdk-6.6.6.tar", last modified: Mon Jun 12 07:14:25 2023, max compression
```

## Comparing `petstore-sdk-2.3.8.tar` & `petstore-sdk-6.6.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.819970 petstore-sdk-2.3.8/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-24 13:46:19.820971 petstore-sdk-2.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2642 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.786970 petstore-sdk-2.3.8/petstore_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-24 13:46:19.000000 petstore-sdk-2.3.8/petstore_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1384 2023-05-24 13:46:19.000000 petstore-sdk-2.3.8/petstore_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 13:46:19.000000 petstore-sdk-2.3.8/petstore_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      181 2023-05-24 13:46:19.000000 petstore-sdk-2.3.8/petstore_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-24 13:46:19.000000 petstore-sdk-2.3.8/petstore_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      639 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-24 13:46:19.821971 petstore-sdk-2.3.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.789970 petstore-sdk-2.3.8/swaggerpetstore/
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4322 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.792970 petstore-sdk-2.3.8/swaggerpetstore/controllers/
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    12585 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/controllers/pet_controller.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/controllers/store_controller.py
--rw-r--r--   0 root         (0) root         (0)    10595 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.795970 petstore-sdk-2.3.8/swaggerpetstore/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.801970 petstore-sdk-2.3.8/swaggerpetstore/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.803970 petstore-sdk-2.3.8/swaggerpetstore/http/auth/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/http/auth/custom_authentication.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.815971 petstore-sdk-2.3.8/swaggerpetstore/models/
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2232 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/api_response.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/category.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/order.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/pet.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/status_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/status_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     4034 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/models/user.py
--rw-r--r--   0 root         (0) root         (0)     3216 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/swaggerpetstore_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 13:46:19.818971 petstore-sdk-2.3.8/swaggerpetstore/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-24 13:45:47.000000 petstore-sdk-2.3.8/swaggerpetstore/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.612955 petstore-sdk-6.6.6/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-12 07:14:25.612955 petstore-sdk-6.6.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.590955 petstore-sdk-6.6.6/petstore_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-12 07:14:25.000000 petstore-sdk-6.6.6/petstore_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-06-12 07:14:25.000000 petstore-sdk-6.6.6/petstore_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 07:14:25.000000 petstore-sdk-6.6.6/petstore_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-12 07:14:25.000000 petstore-sdk-6.6.6/petstore_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-12 07:14:25.000000 petstore-sdk-6.6.6/petstore_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-12 07:14:25.613955 petstore-sdk-6.6.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.592955 petstore-sdk-6.6.6/swaggerpetstore/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4322 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.594955 petstore-sdk-6.6.6/swaggerpetstore/controllers/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/controllers/pet_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/controllers/store_controller.py
+-rw-r--r--   0 root         (0) root         (0)    10595 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.594955 petstore-sdk-6.6.6/swaggerpetstore/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.597955 petstore-sdk-6.6.6/swaggerpetstore/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.601955 petstore-sdk-6.6.6/swaggerpetstore/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/http/auth/custom_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.610955 petstore-sdk-6.6.6/swaggerpetstore/models/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/api_response.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/pet.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/status_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/status_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4034 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/swaggerpetstore_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 07:14:25.611955 petstore-sdk-6.6.6/swaggerpetstore/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-12 07:13:57.000000 petstore-sdk-6.6.6/swaggerpetstore/utilities/file_wrapper.py
```

### Comparing `petstore-sdk-2.3.8/LICENSE` & `petstore-sdk-6.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/README.md` & `petstore-sdk-6.6.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,79 @@
-
-# Getting Started with Swagger Petstore
-
-## Introduction
-
-This is a sample server Petstore server.  You can find out more about Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).  For this sample, you can use the api key `special-key` to test the authorization filters.
-
-Find out more about Swagger: [http://swagger.io](http://swagger.io)
-
-## Install the Package
-
+Metadata-Version: 2.1
+Name: petstore-sdk
+Version: 6.6.6
+Summary: this is pet description.
+Author-email: Subtain <subtainshah2113@gmail.com>
+Project-URL: Documentation, https://youtube.com
+Keywords: this,is,testing
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: testutils
+License-File: LICENSE
+
+
+# Getting Started with Swagger Petstore
+
+## Introduction
+
+This is a sample server Petstore server.  You can find out more about Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).  For this sample, you can use the api key `special-key` to test the authorization filters.
+
+Find out more about Swagger: [http://swagger.io](http://swagger.io)
+
+## Install the Package
+
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
-Install the package from PyPi using the following pip command:
-
-```python
-pip install petstore-sdk==2.3.8
-```
-
+Install the package from PyPi using the following pip command:
+
+```python
+pip install petstore-sdk==6.6.6
+```
+
 You can also view the package at:
-https://pypi.python.org/pypi/petstore-sdk/2.3.8
-
-## Initialize the API Client
-
-**_Note:_** Documentation for the client can be found [here.](doc/client.md)
-
-The following parameters are configurable for the API Client:
-
-| Parameter | Type | Description |
-|  --- | --- | --- |
-| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
-| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
-| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
-| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
-| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
-| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
-| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
-| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
-| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
-| `password` | `string` |  |
-
-The API client can be initialized as follows:
-
-```python
-from swaggerpetstore.swaggerpetstore_client import SwaggerpetstoreClient
+https://pypi.python.org/pypi/petstore-sdk/6.6.6
+
+## Initialize the API Client
+
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/SYed-Subrta/test/tree/6.6.6/doc/client.md)
+
+The following parameters are configurable for the API Client:
+
+| Parameter | Type | Description |
+|  --- | --- | --- |
+| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
+| `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
+| `override_http_client_configuration` | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
+| `http_call_back` | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
+| `timeout` | `float` | The value to use for connection timeout. <br> **Default: 60** |
+| `max_retries` | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
+| `backoff_factor` | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
+| `retry_statuses` | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
+| `retry_methods` | `Array of string` | The http methods on which retry is to be done. <br> **Default: ['GET', 'PUT']** |
+| `password` | `string` |  |
+
+The API client can be initialized as follows:
+
+```python
+from swaggerpetstore.swaggerpetstore_client import SwaggerpetstoreClient
 from swaggerpetstore.configuration import Environment
-
+
 client = SwaggerpetstoreClient(
     password='Password'
-)
-```
-
-## Authorization
-
-This API uses `Custom Authentication`.
-
-## List of APIs
-
-* [Pet](doc/controllers/pet.md)
-* [Store](doc/controllers/store.md)
-* [User](doc/controllers/user.md)
-
-## Classes Documentation
-
-* [Utility Classes](doc/utility-classes.md)
-* [HttpResponse](doc/http-response.md)
-* [HttpRequest](doc/http-request.md)
-
+)
+```
+
+## Authorization
+
+This API uses `Custom Authentication`.
+
+## List of APIs
+
+* [Pet](https://www.github.com/SYed-Subrta/test/tree/6.6.6/doc/controllers/pet.md)
+* [Store](https://www.github.com/SYed-Subrta/test/tree/6.6.6/doc/controllers/store.md)
+* [User](https://www.github.com/SYed-Subrta/test/tree/6.6.6/doc/controllers/user.md)
+
+## Classes Documentation
+
+* [Utility Classes](https://www.github.com/SYed-Subrta/test/tree/6.6.6/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/SYed-Subrta/test/tree/6.6.6/doc/http-response.md)
+* [HttpRequest](https://www.github.com/SYed-Subrta/test/tree/6.6.6/doc/http-request.md)
+
```

### Comparing `petstore-sdk-2.3.8/petstore_sdk.egg-info/SOURCES.txt` & `petstore-sdk-6.6.6/petstore_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/pyproject.toml` & `petstore-sdk-6.6.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "petstore-sdk"
 description = "this is pet description."
-version = "2.3.8"
+version = "6.6.6"
+readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["this", "is", "testing"]
 authors = [{name = "Subtain", email = "subtainshah2113@gmail.com"}]
 urls = {Documentation = "https://youtube.com"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10", "deprecation~=2.1"]
 classifiers = []
 [project.optional-dependencies]
```

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/api_helper.py` & `petstore-sdk-6.6.6/swaggerpetstore/api_helper.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/configuration.py` & `petstore-sdk-6.6.6/swaggerpetstore/configuration.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/controllers/base_controller.py` & `petstore-sdk-6.6.6/swaggerpetstore/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/controllers/pet_controller.py` & `petstore-sdk-6.6.6/swaggerpetstore/controllers/pet_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,47 @@
 
 class PetController(BaseController):
 
     """A Controller to access Endpoints in the swaggerpetstore API."""
     def __init__(self, config):
         super(PetController, self).__init__(config)
 
+    def inpet(self,
+              body):
+        """Does a POST request to /pet.
+
+        Add a new pet to the store
+
+        Args:
+            body (Pet): Pet object that needs to be added to the store
+
+        Returns:
+            void: Response from the API.
+
+        Raises:
+            APIException: When an error occurs while fetching the data from
+                the remote API. This exception includes the HTTP Response
+                code, an error message, and the HTTP body that was received in
+                the request.
+
+        """
+
+        return super().new_api_call_builder.request(
+            RequestBuilder().server(Server.SERVER1)
+            .path('/pet')
+            .http_method(HttpMethodEnum.POST)
+            .body_param(Parameter()
+                        .value(body))
+            .header_param(Parameter()
+                          .key('Content-Type')
+                          .value('application/json'))
+            .body_serializer(APIHelper.json_serialize)
+            .auth(Single('global'))
+        ).execute()
+
     def upload_file(self,
                     pet_id,
                     additional_metadata=None,
                     file=None):
         """Does a POST request to /pet/{petId}/uploadImage.
 
         uploads an image
@@ -76,47 +109,14 @@
             .auth(Single('global'))
         ).response(
             ResponseHandler()
             .deserializer(APIHelper.json_deserialize)
             .deserialize_into(ApiResponse.from_dictionary)
         ).execute()
 
-    def inpet(self,
-              body):
-        """Does a POST request to /pet.
-
-        Add a new pet to the store
-
-        Args:
-            body (Pet): Pet object that needs to be added to the store
-
-        Returns:
-            void: Response from the API.
-
-        Raises:
-            APIException: When an error occurs while fetching the data from
-                the remote API. This exception includes the HTTP Response
-                code, an error message, and the HTTP body that was received in
-                the request.
-
-        """
-
-        return super().new_api_call_builder.request(
-            RequestBuilder().server(Server.SERVER1)
-            .path('/pet')
-            .http_method(HttpMethodEnum.POST)
-            .body_param(Parameter()
-                        .value(body))
-            .header_param(Parameter()
-                          .key('Content-Type')
-                          .value('application/json'))
-            .body_serializer(APIHelper.json_serialize)
-            .auth(Single('global'))
-        ).execute()
-
     def update_an_pet(self,
                       body):
         """Does a PUT request to /pet.
 
         Update an existing pet
 
         Args:
@@ -261,26 +261,24 @@
             ResponseHandler()
             .deserializer(APIHelper.json_deserialize)
             .deserialize_into(Pet.from_dictionary)
             .local_error('400', 'Invalid ID supplied', APIException)
             .local_error('404', 'Pet not found', APIException)
         ).execute()
 
-    def update_pet_with_form(self,
-                             pet_id,
-                             name=None,
-                             status=None):
-        """Does a POST request to /pet/{petId}.
+    def delete_pet(self,
+                   pet_id,
+                   api_key=None):
+        """Does a DELETE request to /pet/{petId}.
 
-        Updates a pet in the store with form data
+        Deletes a pet
 
         Args:
-            pet_id (long|int): ID of pet that needs to be updated
-            name (string, optional): Updated name of the pet
-            status (string, optional): Updated status of the pet
+            pet_id (long|int): Pet id to delete
+            api_key (string, optional): TODO: type description here.
 
         Returns:
             void: Response from the API.
 
         Raises:
             APIException: When an error occurs while fetching the data from
                 the remote API. This exception includes the HTTP Response
@@ -288,41 +286,37 @@
                 the request.
 
         """
 
         return super().new_api_call_builder.request(
             RequestBuilder().server(Server.SERVER1)
             .path('/pet/{petId}')
-            .http_method(HttpMethodEnum.POST)
+            .http_method(HttpMethodEnum.DELETE)
             .template_param(Parameter()
                             .key('petId')
                             .value(pet_id)
                             .should_encode(True))
-            .form_param(Parameter()
-                        .key('name')
-                        .value(name))
-            .form_param(Parameter()
-                        .key('status')
-                        .value(status))
             .header_param(Parameter()
-                          .key('content-type')
-                          .value('application/x-www-form-urlencoded'))
+                          .key('api_key')
+                          .value(api_key))
             .auth(Single('global'))
         ).execute()
 
-    def delete_pet(self,
-                   pet_id,
-                   api_key=None):
-        """Does a DELETE request to /pet/{petId}.
+    def update_pet_with_form(self,
+                             pet_id,
+                             name=None,
+                             status=None):
+        """Does a POST request to /pet/{petId}.
 
-        Deletes a pet
+        Updates a pet in the store with form data
 
         Args:
-            pet_id (long|int): Pet id to delete
-            api_key (string, optional): TODO: type description here.
+            pet_id (long|int): ID of pet that needs to be updated
+            name (string, optional): Updated name of the pet
+            status (string, optional): Updated status of the pet
 
         Returns:
             void: Response from the API.
 
         Raises:
             APIException: When an error occurs while fetching the data from
                 the remote API. This exception includes the HTTP Response
@@ -330,17 +324,23 @@
                 the request.
 
         """
 
         return super().new_api_call_builder.request(
             RequestBuilder().server(Server.SERVER1)
             .path('/pet/{petId}')
-            .http_method(HttpMethodEnum.DELETE)
+            .http_method(HttpMethodEnum.POST)
             .template_param(Parameter()
                             .key('petId')
                             .value(pet_id)
                             .should_encode(True))
+            .form_param(Parameter()
+                        .key('name')
+                        .value(name))
+            .form_param(Parameter()
+                        .key('status')
+                        .value(status))
             .header_param(Parameter()
-                          .key('api_key')
-                          .value(api_key))
+                          .key('content-type')
+                          .value('application/x-www-form-urlencoded'))
             .auth(Single('global'))
         ).execute()
```

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/controllers/store_controller.py` & `petstore-sdk-6.6.6/swaggerpetstore/controllers/store_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,40 @@
         ).response(
             ResponseHandler()
             .deserializer(APIHelper.json_deserialize)
             .deserialize_into(Order.from_dictionary)
             .local_error('400', 'Invalid Order', APIException)
         ).execute()
 
+    def get_inventory(self):
+        """Does a GET request to /store/inventory.
+
+        Returns a map of status codes to quantities
+
+        Returns:
+            dict: Response from the API. successful operation
+
+        Raises:
+            APIException: When an error occurs while fetching the data from
+                the remote API. This exception includes the HTTP Response
+                code, an error message, and the HTTP body that was received in
+                the request.
+
+        """
+
+        return super().new_api_call_builder.request(
+            RequestBuilder().server(Server.SERVER1)
+            .path('/store/inventory')
+            .http_method(HttpMethodEnum.GET)
+            .auth(Single('global'))
+        ).response(
+            ResponseHandler()
+            .deserializer(APIHelper.json_deserialize)
+        ).execute()
+
     def get_order_by_id(self,
                         order_id):
         """Does a GET request to /store/order/{orderId}.
 
         For valid response try integer IDs with value >= 1 and <= 10. Other
         values will generated exceptions
 
@@ -136,33 +162,7 @@
             .http_method(HttpMethodEnum.DELETE)
             .template_param(Parameter()
                             .key('orderId')
                             .value(order_id)
                             .should_encode(True))
             .auth(Single('global'))
         ).execute()
-
-    def get_inventory(self):
-        """Does a GET request to /store/inventory.
-
-        Returns a map of status codes to quantities
-
-        Returns:
-            dict: Response from the API. successful operation
-
-        Raises:
-            APIException: When an error occurs while fetching the data from
-                the remote API. This exception includes the HTTP Response
-                code, an error message, and the HTTP body that was received in
-                the request.
-
-        """
-
-        return super().new_api_call_builder.request(
-            RequestBuilder().server(Server.SERVER1)
-            .path('/store/inventory')
-            .http_method(HttpMethodEnum.GET)
-            .auth(Single('global'))
-        ).response(
-            ResponseHandler()
-            .deserializer(APIHelper.json_deserialize)
-        ).execute()
```

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/controllers/user_controller.py` & `petstore-sdk-6.6.6/swaggerpetstore/controllers/user_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,47 +56,14 @@
             .header_param(Parameter()
                           .key('Content-Type')
                           .value('application/json'))
             .body_serializer(APIHelper.json_serialize)
             .auth(Single('global'))
         ).execute()
 
-    def create_users_with_list_input(self,
-                                     body):
-        """Does a POST request to /user/createWithList.
-
-        Creates list of users with given input array
-
-        Args:
-            body (list of User): List of user object
-
-        Returns:
-            void: Response from the API.
-
-        Raises:
-            APIException: When an error occurs while fetching the data from
-                the remote API. This exception includes the HTTP Response
-                code, an error message, and the HTTP body that was received in
-                the request.
-
-        """
-
-        return super().new_api_call_builder.request(
-            RequestBuilder().server(Server.SERVER1)
-            .path('/user/createWithList')
-            .http_method(HttpMethodEnum.POST)
-            .body_param(Parameter()
-                        .value(body))
-            .header_param(Parameter()
-                          .key('Content-Type')
-                          .value('application/json'))
-            .body_serializer(APIHelper.json_serialize)
-            .auth(Single('global'))
-        ).execute()
-
     def get_user_by_name(self,
                          username):
         """Does a GET request to /user/{username}.
 
         Get user by user name
 
         Args:
@@ -130,53 +97,14 @@
             ResponseHandler()
             .deserializer(APIHelper.json_deserialize)
             .deserialize_into(User.from_dictionary)
             .local_error('400', 'Invalid username supplied', APIException)
             .local_error('404', 'User not found', APIException)
         ).execute()
 
-    def update_user(self,
-                    username,
-                    body):
-        """Does a PUT request to /user/{username}.
-
-        This can only be done by the logged in user.
-
-        Args:
-            username (string): name that need to be updated
-            body (User): Updated user object
-
-        Returns:
-            void: Response from the API.
-
-        Raises:
-            APIException: When an error occurs while fetching the data from
-                the remote API. This exception includes the HTTP Response
-                code, an error message, and the HTTP body that was received in
-                the request.
-
-        """
-
-        return super().new_api_call_builder.request(
-            RequestBuilder().server(Server.SERVER1)
-            .path('/user/{username}')
-            .http_method(HttpMethodEnum.PUT)
-            .template_param(Parameter()
-                            .key('username')
-                            .value(username)
-                            .should_encode(True))
-            .body_param(Parameter()
-                        .value(body))
-            .header_param(Parameter()
-                          .key('Content-Type')
-                          .value('application/json'))
-            .body_serializer(APIHelper.json_serialize)
-            .auth(Single('global'))
-        ).execute()
-
     def delete_user(self,
                     username):
         """Does a DELETE request to /user/{username}.
 
         This can only be done by the logged in user.
 
         Args:
@@ -239,14 +167,86 @@
             .auth(Single('global'))
         ).response(
             ResponseHandler()
             .deserializer(APIHelper.json_deserialize)
             .local_error('400', 'Invalid username/password supplied', APIException)
         ).execute()
 
+    def create_users_with_list_input(self,
+                                     body):
+        """Does a POST request to /user/createWithList.
+
+        Creates list of users with given input array
+
+        Args:
+            body (list of User): List of user object
+
+        Returns:
+            void: Response from the API.
+
+        Raises:
+            APIException: When an error occurs while fetching the data from
+                the remote API. This exception includes the HTTP Response
+                code, an error message, and the HTTP body that was received in
+                the request.
+
+        """
+
+        return super().new_api_call_builder.request(
+            RequestBuilder().server(Server.SERVER1)
+            .path('/user/createWithList')
+            .http_method(HttpMethodEnum.POST)
+            .body_param(Parameter()
+                        .value(body))
+            .header_param(Parameter()
+                          .key('Content-Type')
+                          .value('application/json'))
+            .body_serializer(APIHelper.json_serialize)
+            .auth(Single('global'))
+        ).execute()
+
+    def update_user(self,
+                    username,
+                    body):
+        """Does a PUT request to /user/{username}.
+
+        This can only be done by the logged in user.
+
+        Args:
+            username (string): name that need to be updated
+            body (User): Updated user object
+
+        Returns:
+            void: Response from the API.
+
+        Raises:
+            APIException: When an error occurs while fetching the data from
+                the remote API. This exception includes the HTTP Response
+                code, an error message, and the HTTP body that was received in
+                the request.
+
+        """
+
+        return super().new_api_call_builder.request(
+            RequestBuilder().server(Server.SERVER1)
+            .path('/user/{username}')
+            .http_method(HttpMethodEnum.PUT)
+            .template_param(Parameter()
+                            .key('username')
+                            .value(username)
+                            .should_encode(True))
+            .body_param(Parameter()
+                        .value(body))
+            .header_param(Parameter()
+                          .key('Content-Type')
+                          .value('application/json'))
+            .body_serializer(APIHelper.json_serialize)
+            .auth(Single('global'))
+        ).execute()
+
     def logout_user(self):
         """Does a GET request to /user/logout.
 
         Logs out current logged in user session
 
         Returns:
             void: Response from the API.
```

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/exceptions/api_exception.py` & `petstore-sdk-6.6.6/swaggerpetstore/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/http/auth/custom_authentication.py` & `petstore-sdk-6.6.6/swaggerpetstore/http/auth/custom_authentication.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/http/http_request.py` & `petstore-sdk-6.6.6/swaggerpetstore/http/http_request.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/http/http_response.py` & `petstore-sdk-6.6.6/swaggerpetstore/http/http_response.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/models/api_response.py` & `petstore-sdk-6.6.6/swaggerpetstore/models/api_response.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/models/category.py` & `petstore-sdk-6.6.6/swaggerpetstore/models/category.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/models/order.py` & `petstore-sdk-6.6.6/swaggerpetstore/models/order.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/models/pet.py` & `petstore-sdk-6.6.6/swaggerpetstore/models/pet.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/models/status_2_enum.py` & `petstore-sdk-6.6.6/swaggerpetstore/models/status_2_enum.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/models/tag.py` & `petstore-sdk-6.6.6/swaggerpetstore/models/tag.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/models/user.py` & `petstore-sdk-6.6.6/swaggerpetstore/models/user.py`

 * *Files identical despite different names*

### Comparing `petstore-sdk-2.3.8/swaggerpetstore/swaggerpetstore_client.py` & `petstore-sdk-6.6.6/swaggerpetstore/swaggerpetstore_client.py`

 * *Files identical despite different names*

