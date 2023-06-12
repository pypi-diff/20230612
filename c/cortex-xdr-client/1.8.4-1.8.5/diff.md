# Comparing `tmp/cortex_xdr_client-1.8.4.tar.gz` & `tmp/cortex_xdr_client-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_xdr_client-1.8.4.tar", max compression
+gzip compressed data, was "cortex_xdr_client-1.8.5.tar", max compression
```

## Comparing `cortex_xdr_client-1.8.4.tar` & `cortex_xdr_client-1.8.5.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/LICENSE
--rw-r--r--   0        0        0     3617 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/README.rst
--rw-r--r--   0        0        0       61 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/__init__.py
--rw-r--r--   0        0        0     2059 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/actions_api.py
--rw-r--r--   0        0        0     3387 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/alerts_api.py
--rw-r--r--   0        0        0     1544 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/authentication.py
--rw-r--r--   0        0        0     2376 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/base_api.py
--rw-r--r--   0        0        0     1037 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/download_api.py
--rw-r--r--   0        0        0    15639 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/endpoints_api.py
--rw-r--r--   0        0        0     5261 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/incidents_api.py
--rw-r--r--   0        0        0        0 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/__init__.py
--rw-r--r--   0        0        0      357 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/action_status.py
--rw-r--r--   0        0        0     5902 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/alerts.py
--rw-r--r--   0        0        0     2721 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/endpoints.py
--rw-r--r--   0        0        0      692 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/exceptions.py
--rw-r--r--   0        0        0     2835 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/filters.py
--rw-r--r--   0        0        0     7770 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/incidents.py
--rw-r--r--   0        0        0     2392 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/scripts.py
--rw-r--r--   0        0        0    12326 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/scripts_api.py
--rw-r--r--   0        0        0     5414 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/api/xql_api.py
--rw-r--r--   0        0        0     2341 2023-02-24 16:20:38.053518 cortex_xdr_client-1.8.4/cortex_xdr_client/client.py
--rw-r--r--   0        0        0      646 2023-02-24 16:20:57.360738 cortex_xdr_client-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.4/setup.py
--rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/LICENSE
+-rw-r--r--   0        0        0     3617 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/README.rst
+-rw-r--r--   0        0        0       61 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/__init__.py
+-rw-r--r--   0        0        0     2059 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/actions_api.py
+-rw-r--r--   0        0        0     3387 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/alerts_api.py
+-rw-r--r--   0        0        0     1544 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/authentication.py
+-rw-r--r--   0        0        0     2376 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/base_api.py
+-rw-r--r--   0        0        0     1037 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/download_api.py
+-rw-r--r--   0        0        0    15639 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/endpoints_api.py
+-rw-r--r--   0        0        0     5261 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/incidents_api.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/__init__.py
+-rw-r--r--   0        0        0      390 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/action_status.py
+-rw-r--r--   0        0        0     5902 2023-06-12 08:48:06.179484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/alerts.py
+-rw-r--r--   0        0        0     2721 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/endpoints.py
+-rw-r--r--   0        0        0      692 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/exceptions.py
+-rw-r--r--   0        0        0     2835 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/filters.py
+-rw-r--r--   0        0        0     7770 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/incidents.py
+-rw-r--r--   0        0        0     2392 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/scripts.py
+-rw-r--r--   0        0        0    12326 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/scripts_api.py
+-rw-r--r--   0        0        0     5414 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/api/xql_api.py
+-rw-r--r--   0        0        0     2341 2023-06-12 08:48:06.183484 cortex_xdr_client-1.8.5/cortex_xdr_client/client.py
+-rw-r--r--   0        0        0      646 2023-06-12 08:48:31.307594 cortex_xdr_client-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.5/PKG-INFO
```

### Comparing `cortex_xdr_client-1.8.4/LICENSE` & `cortex_xdr_client-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/README.rst` & `cortex_xdr_client-1.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/actions_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/alerts_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/authentication.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/authentication.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/base_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/base_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/download_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/download_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/endpoints_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/endpoints_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/incidents_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/incidents_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/alerts.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/alerts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/endpoints.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/exceptions.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/filters.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/filters.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/incidents.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/incidents.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/models/scripts.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/models/scripts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/scripts_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/scripts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/api/xql_api.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/api/xql_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/cortex_xdr_client/client.py` & `cortex_xdr_client-1.8.5/cortex_xdr_client/client.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.4/pyproject.toml` & `cortex_xdr_client-1.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "cortex-xdr-client"
 packages= [
     { include = "cortex_xdr_client", from="." },
 ]
-version = "v1.8.4"
+version = "v1.8.5"
 description = "API client for Cortex XDR Prevent"
 authors = ["ebarti"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ebarti/cortex-xdr-client"
 repository = "https://github.com/ebarti/cortex-xdr-client"
```

### Comparing `cortex_xdr_client-1.8.4/setup.py` & `cortex_xdr_client-1.8.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,75 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cortex-xdr-client
+Version: 1.8.5
+Summary: API client for Cortex XDR Prevent
+Home-page: https://github.com/ebarti/cortex-xdr-client
+License: MIT
+Author: ebarti
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Project-URL: Repository, https://github.com/ebarti/cortex-xdr-client
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': '.'}
+About the cortex-xdr-client
+###########################
 
-packages = \
-['cortex_xdr_client', 'cortex_xdr_client.api', 'cortex_xdr_client.api.models']
+A python-based API client for `Cortex XDR
+API <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api>`__.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.8.2,<2.0.0', 'requests>=2.26.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'cortex-xdr-client',
-    'version': '1.8.4',
-    'description': 'API client for Cortex XDR Prevent',
-    'long_description': 'About the cortex-xdr-client\n###########################\n\nA python-based API client for `Cortex XDR\nAPI <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api>`__.\n\nCurrently, it supports the following Cortex XDR **Prevent & Pro** APIs:\n\n*Incidents API:*\n\n-  `Get Incidents <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/incident-management/get-incidents.html>`__\n-  `Get Extra Incident Data <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/incident-management/get-extra-incident-data.html>`__\n\n\n*Alerts API:*\n\n-  `Get Alerts <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/incident-management/get-alerts.html>`__\n\n\n*Endpoints API:*\n\n-  `Get All Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/endpoint-management/get-all-endpoints.html>`__\n-  `Get Endpoint <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/endpoint-management/get-endpoints.html>`__\n-  `Isolate Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/isolate-endpoints.html>`__\n-  `Unisolate Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/unisolate-endpoints.html>`__\n-  `Scan Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/scan-endpoints.html>`__\n-  `Retrieve File <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/retrieve-file.html>`__\n-  `Quarantine File <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/quarantine-file.html>`__\n\n\n*XQL API:*\n\n-  `Start XQL <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/xql-apis/start-xql-query.html>`__\n-  `Get XQL Results <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/xql-apis/get-xql-query-results.html>`__\n-  `Get XQL Result Stream <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/xql-apis/get-xql-query-exported-data.html>`__\n\n\n*Scripts API:*\n\n-  `Get Scripts <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-scripts.html>`__\n-  `Get Script Metadata <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-metadata.html>`__\n-  `Get Script Execution Status <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-execution-status.html>`__\n-  `Get Script Execution Results <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-execution-results.html>`__\n-  `Get Script Execution Result Files <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-execution-result-files.html>`__\n-  `Run Script <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/run-script.html>`__\n-  `Run Snippet Code Script <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/run-snippet-code-script.html>`__\n\n\n*Response Actions API:*\n\n-  `Get Action Status <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/get-action-status.html>`__\n\n*Contributing:*\n\nSee `CONTRIBUTING.md <./CONTRIBUTING.md>`__ for details.\n',
-    'author': 'ebarti',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ebarti/cortex-xdr-client',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+Currently, it supports the following Cortex XDR **Prevent & Pro** APIs:
 
+*Incidents API:*
+
+-  `Get Incidents <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/incident-management/get-incidents.html>`__
+-  `Get Extra Incident Data <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/incident-management/get-extra-incident-data.html>`__
+
+
+*Alerts API:*
+
+-  `Get Alerts <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/incident-management/get-alerts.html>`__
+
+
+*Endpoints API:*
+
+-  `Get All Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/endpoint-management/get-all-endpoints.html>`__
+-  `Get Endpoint <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/endpoint-management/get-endpoints.html>`__
+-  `Isolate Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/isolate-endpoints.html>`__
+-  `Unisolate Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/unisolate-endpoints.html>`__
+-  `Scan Endpoints <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/scan-endpoints.html>`__
+-  `Retrieve File <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/retrieve-file.html>`__
+-  `Quarantine File <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/quarantine-file.html>`__
+
+
+*XQL API:*
+
+-  `Start XQL <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/xql-apis/start-xql-query.html>`__
+-  `Get XQL Results <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/xql-apis/get-xql-query-results.html>`__
+-  `Get XQL Result Stream <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/xql-apis/get-xql-query-exported-data.html>`__
+
+
+*Scripts API:*
+
+-  `Get Scripts <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-scripts.html>`__
+-  `Get Script Metadata <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-metadata.html>`__
+-  `Get Script Execution Status <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-execution-status.html>`__
+-  `Get Script Execution Results <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-execution-results.html>`__
+-  `Get Script Execution Result Files <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/get-script-execution-result-files.html>`__
+-  `Run Script <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/run-script.html>`__
+-  `Run Snippet Code Script <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/script-execution/run-snippet-code-script.html>`__
+
+
+*Response Actions API:*
+
+-  `Get Action Status <https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/get-action-status.html>`__
+
+*Contributing:*
+
+See `CONTRIBUTING.md <./CONTRIBUTING.md>`__ for details.
 
-setup(**setup_kwargs)
```

