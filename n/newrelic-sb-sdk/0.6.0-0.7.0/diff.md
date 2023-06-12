# Comparing `tmp/newrelic_sb_sdk-0.6.0.tar.gz` & `tmp/newrelic_sb_sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic_sb_sdk-0.6.0.tar", max compression
+gzip compressed data, was "newrelic_sb_sdk-0.7.0.tar", max compression
```

## Comparing `newrelic_sb_sdk-0.6.0.tar` & `newrelic_sb_sdk-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1002 2023-06-10 11:01:12.829926 newrelic_sb_sdk-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1619 2023-04-16 17:39:52.127412 newrelic_sb_sdk-0.6.0/README.md
--rw-r--r--   0        0        0     2511 2023-06-10 11:01:12.825926 newrelic_sb_sdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-10 11:01:18.981947 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/__init__.py
--rw-r--r--   0        0        0   385992 2023-06-10 10:08:43.124672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/_modidx.py
--rw-r--r--   0        0        0     4902 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-10 10:08:43.124672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/enums.py
--rw-r--r--   0        0        0      769 2023-06-10 10:08:43.124672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/utils.py
--rw-r--r--   0        0        0     2060 2023-06-10 10:54:31.636620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/__init__.py
--rw-r--r--   0        0        0      372 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/base.py
--rw-r--r--   0        0        0      747 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/encoders.py
--rw-r--r--   0        0        0     2235 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/mixins.py
--rw-r--r--   0        0        0     1175 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/__init__.py
--rw-r--r--   0        0        0     1095 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/enums.py
--rw-r--r--   0        0        0     1006 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/pages.py
--rw-r--r--   0        0        0      593 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/utils.py
--rw-r--r--   0        0        0     3583 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/widgets.py
--rw-r--r--   0        0        0      200 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/__init__.py
--rw-r--r--   0        0        0    58585 2023-06-10 10:54:31.640620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/enums.py
--rw-r--r--   0        0        0   358452 2023-06-10 10:54:31.636620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/input_objects.py
--rw-r--r--   0        0        0   751350 2023-06-10 10:54:31.644620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/objects.py
--rw-r--r--   0        0        0     3054 2023-06-10 10:54:31.644620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/scalars.py
--rw-r--r--   0        0        0        0 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/__init__.py
--rw-r--r--   0        0        0      367 2023-06-10 10:54:31.636620 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/query.py
--rw-r--r--   0        0        0      787 2023-06-10 10:08:43.120672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/response.py
--rw-r--r--   0        0        0     1901 2023-06-10 10:08:43.116672 newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/text.py
--rw-r--r--   0        0        0     3132 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1379 2023-06-12 17:54:32.162562 newrelic_sb_sdk-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-03-04 19:28:34.334390 newrelic_sb_sdk-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     2761 2023-06-12 17:52:06.862280 newrelic_sb_sdk-0.7.0/README.md
+-rw-r--r--   0        0        0     2788 2023-06-12 17:54:32.154562 newrelic_sb_sdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-12 17:54:40.318579 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/__init__.py
+-rw-r--r--   0        0        0   385992 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/_modidx.py
+-rw-r--r--   0        0        0     4902 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/enums.py
+-rw-r--r--   0        0        0      769 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/utils.py
+-rw-r--r--   0        0        0     2024 2023-06-12 17:51:48.142247 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/base.py
+-rw-r--r--   0        0        0      747 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/encoders.py
+-rw-r--r--   0        0        0     2235 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/mixins.py
+-rw-r--r--   0        0        0     1175 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/__init__.py
+-rw-r--r--   0        0        0     1095 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/enums.py
+-rw-r--r--   0        0        0     1006 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/pages.py
+-rw-r--r--   0        0        0      593 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/utils.py
+-rw-r--r--   0        0        0     3583 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/widgets.py
+-rw-r--r--   0        0        0      200 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/__init__.py
+-rw-r--r--   0        0        0    58585 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/enums.py
+-rw-r--r--   0        0        0   358452 2023-06-12 17:47:57.221961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/input_objects.py
+-rw-r--r--   0        0        0   751350 2023-06-12 17:47:57.225961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/objects.py
+-rw-r--r--   0        0        0     3054 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/scalars.py
+-rw-r--r--   0        0        0        0 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      329 2023-06-12 17:51:48.142247 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/query.py
+-rw-r--r--   0        0        0      787 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/response.py
+-rw-r--r--   0        0        0     1901 2023-06-12 17:47:57.217961 newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/text.py
+-rw-r--r--   0        0        0     4600 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.7.0/PKG-INFO
```

### Comparing `newrelic_sb_sdk-0.6.0/LICENSE.txt` & `newrelic_sb_sdk-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/README.md` & `newrelic_sb_sdk-0.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk)
 ![PyPI - Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/newrelic-sb-sdk)
 ![PyPI - MIT License](https://img.shields.io/pypi/l/newrelic-sb-sdk)
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/newrelic-sb-sdk/dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![pipeline status](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/badges/master/pipeline.svg)](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/commits/master)
+
 
 # New Relic SB SDK
 
 New Relic SDK built by SoftButterfly to automate common New Relic One observability platform tasks
 
 ## Requirements
 
@@ -24,18 +26,58 @@
 
 Install from PyPI
 
 ```bash
 pip install newrelic-sb-sdk
 ```
 
+## Usage
+
+There is an example on how to use this module to make a simple requesto to New Relic GraphQL API.
+
+```python
+from newrelic_sb_sdk.client import NewRelicGqlClient
+from newrelic_sb_sdk.utils.response import print_response
+from newrelic_sb_sdk.graphql import nerdgraph
+from newrelic_sb_sdk.graphql.objects import RootQueryType, RootMutationType
+
+from sgqlc.operation import Operation
+
+nerdgraph.query_type = RootQueryType
+nerdgraph.mutation_type = RootMutationType
+
+newrelic = NewRelicGqlClient(new_relic_user_key=YOUR_NEW_RELIC_USER_KEY)
+
+operation = Operation(nerdgraph.query_type)
+operation.actor.user()
+
+operation = operation.__to_graphql__()
+
+response = newrelic.execute(operation)
+
+print_response(response)
+
+# Output
+# {
+#     "data": {
+#         "actor": {
+#             "user": {
+#                 "email": "admin@example.com",
+#                 "id": 1234567890,
+#                 "name": "Admin User",
+#             }
+#         }
+#     }
+# }
+```
+
 ## Docs
 
-* [Ejemplos](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/wikis)
-* [Wiki](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/wikis)
+* [Ejemplos](https://gitlab.com/softbutterfly/open-source/newrelic-playground)
+* [Wiki](https://softbutterfly.gitlab.io/open-source/newrelic-sb-sdk/)
 
 ## Changelog
 
 All changes to versions of this library are listed in the [change history](./CHANGELOG.md).
 
 ## Development
```

#### html2text {}

```diff
@@ -4,19 +4,33 @@
 pyversions/newrelic-sb-sdk) ![PyPI - Package version](https://img.shields.io/
 pypi/v/newrelic-sb-sdk) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
 newrelic-sb-sdk) ![PyPI - MIT License](https://img.shields.io/pypi/l/newrelic-
 sb-sdk) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/
 1c25dec51e1c4a719be4c2d4ebe7eef6)](https://app.codacy.com/gl/softbutterfly/
 newrelic-sb-sdk/
 dashboard?utm_source=gl&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-# New Relic SB SDK New Relic SDK built by SoftButterfly to automate common New
-Relic One observability platform tasks ## Requirements * Python 3.8.1 or higher
-* `enforce-typing` * `python-dotenv` * `requests` * `semver` * `sgqlc` ##
-Install Install from PyPI ```bash pip install newrelic-sb-sdk ``` ## Docs *
-[Ejemplos](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/
-wikis) * [Wiki](https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/
-wikis) ## Changelog All changes to versions of this library are listed in the
-[change history](./CHANGELOG.md). ## Development Check out our [contribution
-guide](./CONTRIBUTING.md). ## Contributors See the list of contributors [here]
-(https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/graphs/
-develop). ## License This project is licensed under the terms of the MIT
-license. See the LICENSE file.
+[![pipeline status](https://gitlab.com/softbutterfly/open-source/newrelic-sb-
+sdk/badges/master/pipeline.svg)](https://gitlab.com/softbutterfly/open-source/
+newrelic-sb-sdk/-/commits/master) # New Relic SB SDK New Relic SDK built by
+SoftButterfly to automate common New Relic One observability platform tasks ##
+Requirements * Python 3.8.1 or higher * `enforce-typing` * `python-dotenv` *
+`requests` * `semver` * `sgqlc` ## Install Install from PyPI ```bash pip
+install newrelic-sb-sdk ``` ## Usage There is an example on how to use this
+module to make a simple requesto to New Relic GraphQL API. ```python from
+newrelic_sb_sdk.client import NewRelicGqlClient from
+newrelic_sb_sdk.utils.response import print_response from
+newrelic_sb_sdk.graphql import nerdgraph from newrelic_sb_sdk.graphql.objects
+import RootQueryType, RootMutationType from sgqlc.operation import Operation
+nerdgraph.query_type = RootQueryType nerdgraph.mutation_type = RootMutationType
+newrelic = NewRelicGqlClient(new_relic_user_key=YOUR_NEW_RELIC_USER_KEY)
+operation = Operation(nerdgraph.query_type) operation.actor.user() operation =
+operation.__to_graphql__() response = newrelic.execute(operation)
+print_response(response) # Output # { # "data": { # "actor": { # "user": { #
+"email": "admin@example.com", # "id": 1234567890, # "name": "Admin User", # } #
+} # } # } ``` ## Docs * [Ejemplos](https://gitlab.com/softbutterfly/open-
+source/newrelic-playground) * [Wiki](https://softbutterfly.gitlab.io/open-
+source/newrelic-sb-sdk/) ## Changelog All changes to versions of this library
+are listed in the [change history](./CHANGELOG.md). ## Development Check out
+our [contribution guide](./CONTRIBUTING.md). ## Contributors See the list of
+contributors [here](https://gitlab.com/softbutterfly/open-source/newrelic-sb-
+sdk/-/graphs/develop). ## License This project is licensed under the terms of
+the MIT license. See the LICENSE file.
```

### Comparing `newrelic_sb_sdk-0.6.0/pyproject.toml` & `newrelic_sb_sdk-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 [tool.poetry]
 name = "newrelic-sb-sdk"
-version = "0.6.0"
+version = "0.7.0"
 description = "New Relic SDK to interact with Nerdgraph API."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk"
 repository = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk"
-documentation = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/wikis"
+documentation = "https://softbutterfly.gitlab.io/open-source/newrelic-sb-sdk/"
 keywords = [
   "Softbutterfly",
   "New Relic",
   "SDK",
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
+  "Intended Audience :: System Administrators",
+  "Intended Audience :: Information Technology",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Topic :: Software Development",
+  "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: System",
+  "Topic :: System :: Monitoring",
+  "Topic :: System :: Networking :: Monitoring",
 ]
 packages = [
     { include = "newrelic_sb_sdk", from = "src" },
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.6.0/newrelic-sb-sdk-v0.6.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.7.0/newrelic-sb-sdk-v0.7.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 enforce-typing = "^1.0.0.post1"
 python-dotenv = "^1.0.0"
```

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/_modidx.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/_modidx.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/__init__.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/enums.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/alerts/utils.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/client/__init__.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/client/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,29 +41,29 @@
             {
                 "Content-Type": "application/json",
                 "API-Key": new_relic_user_key,
             }
         )
 
     def execute(
-        self, query: str, variables: Union[Dict[str, Any], None] = None, **kwargs
+        self, query: str, *, variables: Union[Dict[str, Any], None] = None, **kwargs
     ) -> Response:
         data = json.dumps(
             {
                 "query": query,
                 "variables": variables,
             },
         )
         return self.post(self.url, data=data, **kwargs)
 
     @staticmethod
     def build_query(
-        *, query_string: str, query_params: Union[Dict[str, Any], None] = None
+        template: str, *, params: Union[Dict[str, Any], None] = None
     ) -> str:
-        return build_query(query_string=query_string, query_params=query_params)
+        return build_query(template, params=params)
 
 
 class NewRelicRestClient(Session):
     """Client for New Relic Rest API."""
 
     url: str = "https://api.newrelic.com/v2/"
```

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/encoders.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/encoders.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/core/mixins.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/__init__.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/enums.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/pages.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/pages.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/utils.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/dashboards/widgets.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/dashboards/widgets.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/enums.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/input_objects.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/input_objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/objects.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/graphql/scalars.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/graphql/scalars.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/response.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/response.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.6.0/src/newrelic_sb_sdk/utils/text.py` & `newrelic_sb_sdk-0.7.0/src/newrelic_sb_sdk/utils/text.py`

 * *Files identical despite different names*

