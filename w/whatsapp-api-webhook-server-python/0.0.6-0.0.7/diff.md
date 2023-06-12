# Comparing `tmp/whatsapp-api-webhook-server-python-0.0.6.tar.gz` & `tmp/whatsapp-api-webhook-server-python-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-api-webhook-server-python-0.0.6.tar", last modified: Mon May 29 11:40:42 2023, max compression
+gzip compressed data, was "whatsapp-api-webhook-server-python-0.0.7.tar", last modified: Mon Jun 12 14:57:23 2023, max compression
```

## Comparing `whatsapp-api-webhook-server-python-0.0.6.tar` & `whatsapp-api-webhook-server-python-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.287552 whatsapp-api-webhook-server-python-0.0.6/
--rw-rw-rw-   0        0        0    18829 2023-05-29 11:34:04.000000 whatsapp-api-webhook-server-python-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     7668 2023-05-29 11:40:42.287552 whatsapp-api-webhook-server-python-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-05-29 11:35:26.000000 whatsapp-api-webhook-server-python-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 11:40:42.287552 whatsapp-api-webhook-server-python-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1434 2023-05-29 11:34:04.000000 whatsapp-api-webhook-server-python-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.278537 whatsapp-api-webhook-server-python-0.0.6/tests/
--rw-rw-rw-   0        0        0      518 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/tests/test_main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.281536 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/
--rw-rw-rw-   0        0        0        0 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/__init__.py
--rw-rw-rw-   0        0        0      255 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/webhooks.py
--rw-rw-rw-   0        0        0     1643 2023-05-29 10:36:08.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/webhooksHandler.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:40:42.286550 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/
--rw-rw-rw-   0        0        0     7668 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2023-05-29 11:40:42.000000 whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.663206 whatsapp-api-webhook-server-python-0.0.7/
+-rw-rw-rw-   0        0        0    18829 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     7921 2023-06-12 14:57:23.663206 whatsapp-api-webhook-server-python-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6847 2023-06-12 14:52:42.000000 whatsapp-api-webhook-server-python-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:57:23.663206 whatsapp-api-webhook-server-python-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1434 2023-06-12 14:52:42.000000 whatsapp-api-webhook-server-python-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.656187 whatsapp-api-webhook-server-python-0.0.7/tests/
+-rw-rw-rw-   0        0        0      518 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/tests/test_main.py
+-rw-rw-rw-   0        0        0      204 2023-06-04 08:13:40.000000 whatsapp-api-webhook-server-python-0.0.7/tests/test_methods.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.658193 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/
+-rw-rw-rw-   0        0        0        0 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/webhooks.py
+-rw-rw-rw-   0        0        0     1643 2023-06-04 08:02:14.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/webhooksHandler.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:57:23.662203 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/
+-rw-rw-rw-   0        0        0     7921 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-06-12 14:57:23.000000 whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/top_level.txt
```

### Comparing `whatsapp-api-webhook-server-python-0.0.6/LICENSE` & `whatsapp-api-webhook-server-python-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-api-webhook-server-python-0.0.6/PKG-INFO` & `whatsapp-api-webhook-server-python-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-api-webhook-server-python
-Version: 0.0.6
+Version: 0.0.7
 Summary: This library helps you easily create a Python server endpoint to receive WhatsApp message webhooks.
 Home-page: https://github.com/green-api/whatsapp-api-webhook-server-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,18 +19,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # whatsapp-api-webhook-server-python
 
-[![Python application](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-publish.yml)
+![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-api-webhook-server-python)
+![](https://img.shields.io/pypi/pyversions/whatsapp-api-webhook-server-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-webhook-server-python/python-app.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-api-webhook-server-python)
 
-- [Документация на русском языке](docs/README_RU.md).
+- [Документация на русском языке](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/docs/README_RU.md).
 
 whatsapp-api-webhook-server-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
 ## API
 
@@ -95,15 +98,17 @@
 
 Library installation:
 
 ```shell
 python3 -m pip install whatsapp-api-webhook-server-python
 ```
 
-As an example you can download and run [our script](examples/echo.py). The script sends all incoming notifications.
+As an example you can download and run [our script](
+https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/examples/echo.py
+). The script sends all incoming notifications.
 
 ```shell
 wget https://raw.githubusercontent.com/green-api/whatsapp-api-webhook-server-python/master/examples/echo.py
 ```
 
 ```shell
 python3 -m echo.py
@@ -197,24 +202,24 @@
 
 | Parameter       | Description                   |
 |-----------------|-------------------------------|
 | webhooksHandler | library class instance        |
 | typeWebhook     | type of incoming notification |
 | body            | notification body             |
 
-Example: [echo.py](examples/echo.py).
+Example: [echo.py](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/examples/echo.py).
 
 ## How to reroute incoming notifications to a web server
 
 To reroute incoming notifications, you need to set the notification sending address (URL)
 in [personal cabinet](https://console.green-api.com/).
 
 ## Service methods documentation
 
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
-Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
+Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 ](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](LICENSE).
+Please see file [LICENSE](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/LICENSE).
```

### Comparing `whatsapp-api-webhook-server-python-0.0.6/README.md` & `whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,39 @@
+Metadata-Version: 2.1
+Name: whatsapp-api-webhook-server-python
+Version: 0.0.7
+Summary: This library helps you easily create a Python server endpoint to receive WhatsApp message webhooks.
+Home-page: https://github.com/green-api/whatsapp-api-webhook-server-python
+Author: GREEN API
+Author-email: support@green-api.com
+License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # whatsapp-api-webhook-server-python
 
-[![Python application](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-publish.yml/badge.svg)](https://github.com/green-api/whatsapp-api-webhook-server-python/actions/workflows/python-publish.yml)
+![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
+![](https://img.shields.io/pypi/status/whatsapp-api-webhook-server-python)
+![](https://img.shields.io/pypi/pyversions/whatsapp-api-webhook-server-python)
+![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-api-webhook-server-python/python-app.yml)
+![](https://img.shields.io/pypi/dm/whatsapp-api-webhook-server-python)
 
-- [Документация на русском языке](docs/README_RU.md).
+- [Документация на русском языке](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/docs/README_RU.md).
 
 whatsapp-api-webhook-server-python is a library for integration with WhatsApp messenger using the API
 service [green-api.com](https://green-api.com/en/). You should get a registration token and an account ID in
 your [personal cabinet](https://console.green-api.com/) to use the library. There is a free developer account tariff.
 
 ## API
 
@@ -72,15 +98,17 @@
 
 Library installation:
 
 ```shell
 python3 -m pip install whatsapp-api-webhook-server-python
 ```
 
-As an example you can download and run [our script](examples/echo.py). The script sends all incoming notifications.
+As an example you can download and run [our script](
+https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/examples/echo.py
+). The script sends all incoming notifications.
 
 ```shell
 wget https://raw.githubusercontent.com/green-api/whatsapp-api-webhook-server-python/master/examples/echo.py
 ```
 
 ```shell
 python3 -m echo.py
@@ -174,24 +202,24 @@
 
 | Parameter       | Description                   |
 |-----------------|-------------------------------|
 | webhooksHandler | library class instance        |
 | typeWebhook     | type of incoming notification |
 | body            | notification body             |
 
-Example: [echo.py](examples/echo.py).
+Example: [echo.py](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/examples/echo.py).
 
 ## How to reroute incoming notifications to a web server
 
 To reroute incoming notifications, you need to set the notification sending address (URL)
 in [personal cabinet](https://console.green-api.com/).
 
 ## Service methods documentation
 
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
-Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
+Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 ](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](LICENSE).
+Please see file [LICENSE](https://github.com/green-api/whatsapp-api-webhook-server-python/blob/master/LICENSE).
```

### Comparing `whatsapp-api-webhook-server-python-0.0.6/setup.py` & `whatsapp-api-webhook-server-python-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-api-webhook-server-python",
-    version="0.0.6",
+    version="0.0.7",
     description=(
         "This library helps you easily create"
         " a Python server endpoint to receive WhatsApp message webhooks."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-api-webhook-server-python-0.0.6/tests/test_main.py` & `whatsapp-api-webhook-server-python-0.0.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `whatsapp-api-webhook-server-python-0.0.6/whatsapp_api_webhook_server_python/webhooksHandler.py` & `whatsapp-api-webhook-server-python-0.0.7/whatsapp_api_webhook_server_python/webhooksHandler.py`

 * *Files identical despite different names*

