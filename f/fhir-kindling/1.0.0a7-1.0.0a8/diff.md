# Comparing `tmp/fhir_kindling-1.0.0a7.tar.gz` & `tmp/fhir_kindling-1.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhir_kindling-1.0.0a7.tar", max compression
+gzip compressed data, was "fhir_kindling-1.0.0a8.tar", max compression
```

## Comparing `fhir_kindling-1.0.0a7.tar` & `fhir_kindling-1.0.0a8.tar`

### file list

```diff
@@ -1,46 +1,55 @@
--rw-r--r--   0        0        0     1071 2023-03-04 09:55:34.447847 fhir_kindling-1.0.0a7/LICENSE
--rw-r--r--   0        0        0     9975 2023-03-23 00:55:55.094618 fhir_kindling-1.0.0a7/README.md
--rw-r--r--   0        0        0      133 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a7/fhir_kindling/__init__.py
--rw-r--r--   0        0        0      268 2023-03-23 12:51:15.067324 fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/__init__.py
--rw-r--r--   0        0        0    13717 2023-03-23 12:51:14.967324 fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/base.py
--rw-r--r--   0        0        0     9968 2023-03-23 11:28:17.585436 fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_async.py
--rw-r--r--   0        0        0    10919 2023-03-23 00:16:03.459242 fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_parameters.py
--rw-r--r--   0        0        0     7939 2023-03-23 00:48:36.910237 fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_response.py
--rw-r--r--   0        0        0     9972 2023-03-23 12:51:14.937324 fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_sync.py
--rw-r--r--   0        0        0       36 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/__init__.py
--rw-r--r--   0        0        0     3936 2023-03-23 00:16:03.319242 fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/auth.py
--rw-r--r--   0        0        0    35574 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/fhir_server.py
--rw-r--r--   0        0        0     3736 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/server_responses.py
--rw-r--r--   0        0        0     2610 2023-03-09 17:53:02.501330 fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/summary.py
--rw-r--r--   0        0        0     5700 2023-03-05 09:03:52.925391 fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/transactions.py
--rw-r--r--   0        0        0     8379 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/transfer.py
--rw-r--r--   0        0        0       89 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a7/fhir_kindling/figures/__init__.py
--rw-r--r--   0        0        0     1240 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a7/fhir_kindling/figures/resource_plots.py
--rw-r--r--   0        0        0      759 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a7/fhir_kindling/figures/summary.py
--rw-r--r--   0        0        0      203 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a7/fhir_kindling/generators/__init__.py
--rw-r--r--   0        0        0     8763 2023-03-23 00:16:03.409242 fhir_kindling-1.0.0a7/fhir_kindling/generators/dataset.py
--rw-r--r--   0        0        0     1530 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a7/fhir_kindling/generators/field_generator.py
--rw-r--r--   0        0        0     4452 2023-03-23 08:11:43.527240 fhir_kindling-1.0.0a7/fhir_kindling/generators/patient.py
--rw-r--r--   0        0        0     7476 2023-03-23 00:16:03.389242 fhir_kindling-1.0.0a7/fhir_kindling/generators/resource_generator.py
--rw-r--r--   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/privacy/__init__.py
--rw-r--r--   0        0        0     3774 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/privacy/k_anonymity.py
--rw-r--r--   0        0        0       57 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/serde/__init__.py
--rw-r--r--   0        0        0     4128 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/serde/flatten.py
--rw-r--r--   0        0        0      404 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/serde/json.py
--rw-r--r--   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/tests/__init__.py
--rw-r--r--   0        0        0      588 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-05 13:00:06.671372 fhir_kindling-1.0.0a7/fhir_kindling/tests/server/__init__.py
--rw-r--r--   0        0        0     1078 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a7/fhir_kindling/tests/server/test_transfer.py
--rw-r--r--   0        0        0     1482 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_auth.py
--rw-r--r--   0        0        0    55630 2023-03-05 18:48:17.265068 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_fhir_query.py
--rw-r--r--   0        0        0    21796 2023-03-23 01:10:38.288455 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_fhir_server.py
--rw-r--r--   0        0        0     9128 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_generators.py
--rw-r--r--   0        0        0     1115 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_plots.py
--rw-r--r--   0        0        0     1024 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_privacy.py
--rw-r--r--   0        0        0     2082 2023-03-23 00:16:03.359242 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_serialization.py
--rw-r--r--   0        0        0     4459 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/tests/test_util.py
--rw-r--r--   0        0        0       43 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/util/__init__.py
--rw-r--r--   0        0        0     4466 2023-03-23 00:16:03.399242 fhir_kindling-1.0.0a7/fhir_kindling/util/references.py
--rw-r--r--   0        0        0     1876 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a7/fhir_kindling/util/resources.py
--rw-r--r--   0        0        0     2414 2023-03-23 15:10:18.379973 fhir_kindling-1.0.0a7/pyproject.toml
--rw-r--r--   0        0        0    11431 1970-01-01 00:00:00.000000 fhir_kindling-1.0.0a7/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2023-03-04 09:55:34.447847 fhir_kindling-1.0.0a8/LICENSE
+-rwxr-xr-x   0        0        0    10041 2023-04-15 20:16:55.060230 fhir_kindling-1.0.0a8/README.md
+-rwxr-xr-x   0        0        0      133 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/__init__.py
+-rw-r--r--   0        0        0     9251 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/bench.py
+-rw-r--r--   0        0        0     3435 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/constants.py
+-rw-r--r--   0        0        0     8695 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/data.py
+-rw-r--r--   0        0        0     3251 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/figures.py
+-rw-r--r--   0        0        0     1774 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/benchmark/results.py
+-rwxr-xr-x   0        0        0      268 2023-03-23 12:51:15.067324 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/__init__.py
+-rwxr-xr-x   0        0        0    13598 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/base.py
+-rwxr-xr-x   0        0        0     9968 2023-03-23 11:28:17.585436 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_async.py
+-rwxr-xr-x   0        0        0    10919 2023-03-23 00:16:03.459242 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_parameters.py
+-rwxr-xr-x   0        0        0     7939 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_response.py
+-rwxr-xr-x   0        0        0     9972 2023-03-23 12:51:14.937324 fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_sync.py
+-rwxr-xr-x   0        0        0       36 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/__init__.py
+-rwxr-xr-x   0        0        0     3936 2023-03-23 00:16:03.319242 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/auth.py
+-rwxr-xr-x   0        0        0    35574 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/fhir_server.py
+-rwxr-xr-x   0        0        0     3736 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/server_responses.py
+-rwxr-xr-x   0        0        0     2610 2023-03-09 17:53:02.501330 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/summary.py
+-rwxr-xr-x   0        0        0     5700 2023-03-05 09:03:52.925391 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transactions.py
+-rwxr-xr-x   0        0        0     8894 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transfer.py
+-rwxr-xr-x   0        0        0       89 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/figures/__init__.py
+-rwxr-xr-x   0        0        0     1240 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/figures/resource_plots.py
+-rwxr-xr-x   0        0        0      759 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/figures/summary.py
+-rwxr-xr-x   0        0        0      203 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/generators/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/base.py
+-rwxr-xr-x   0        0        0    20029 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/dataset.py
+-rwxr-xr-x   0        0        0     1530 2023-03-04 09:55:34.717848 fhir_kindling-1.0.0a8/fhir_kindling/generators/field_generator.py
+-rwxr-xr-x   0        0        0     4860 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/patient.py
+-rwxr-xr-x   0        0        0     8165 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/resource_generator.py
+-rw-r--r--   0        0        0     5924 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/generators/time_series_generator.py
+-rwxr-xr-x   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/privacy/__init__.py
+-rwxr-xr-x   0        0        0     3774 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/privacy/k_anonymity.py
+-rwxr-xr-x   0        0        0      103 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/serde/__init__.py
+-rwxr-xr-x   0        0        0     4128 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/serde/flatten.py
+-rwxr-xr-x   0        0        0      404 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/serde/json.py
+-rwxr-xr-x   0        0        0        0 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/__init__.py
+-rwxr-xr-x   0        0        0      588 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/conftest.py
+-rwxr-xr-x   0        0        0        0 2023-03-05 13:00:06.671372 fhir_kindling-1.0.0a8/fhir_kindling/tests/server/__init__.py
+-rwxr-xr-x   0        0        0     1078 2023-03-23 00:47:12.807135 fhir_kindling-1.0.0a8/fhir_kindling/tests/server/test_transfer.py
+-rwxr-xr-x   0        0        0     1482 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_auth.py
+-rw-r--r--   0        0        0      419 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_benchmark.py
+-rwxr-xr-x   0        0        0    55630 2023-03-05 18:48:17.265068 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_query.py
+-rwxr-xr-x   0        0        0    21796 2023-05-23 15:03:19.828369 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_server.py
+-rwxr-xr-x   0        0        0    10914 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_generators.py
+-rwxr-xr-x   0        0        0     1115 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_plots.py
+-rwxr-xr-x   0        0        0     1024 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_privacy.py
+-rwxr-xr-x   0        0        0     2082 2023-05-31 12:10:59.853995 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_serialization.py
+-rwxr-xr-x   0        0        0     4736 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/fhir_kindling/tests/test_util.py
+-rwxr-xr-x   0        0        0       43 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/util/__init__.py
+-rwxr-xr-x   0        0        0     4466 2023-03-23 00:16:03.399242 fhir_kindling-1.0.0a8/fhir_kindling/util/references.py
+-rwxr-xr-x   0        0        0     1876 2023-03-04 09:55:34.727848 fhir_kindling-1.0.0a8/fhir_kindling/util/resources.py
+-rwxr-xr-x   0        0        0     2716 2023-06-12 10:41:39.764673 fhir_kindling-1.0.0a8/pyproject.toml
+-rw-r--r--   0        0        0    11758 1970-01-01 00:00:00.000000 fhir_kindling-1.0.0a8/PKG-INFO
```

### Comparing `fhir_kindling-1.0.0a7/LICENSE` & `fhir_kindling-1.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/README.md` & `fhir_kindling-1.0.0a8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,42 +15,47 @@
 as well as resource transfer between servers.
 Datascience features include flattening of resources and bundles into tabular format (pandas dataframes) and plotting 
 methods for resources and bundles can optionally be included with the `ds` extra.
 
 Check out the [documentation](https://migraf.github.io/fhir-kindling/) for more information and a detailed user guide.
 
 
+Table of Contents
+=================
+
+- [Table of Contents](#table-of-contents)
+  - [Features](#features)
+  - [Installation](#installation)
+    - [Extras (optional)](#extras-optional)
+  - [Usage](#usage)
+    - [Connecting to a FHIR server](#connecting-to-a-fhir-server)
+    - [Query resources from the server](#query-resources-from-the-server)
+      - [Basic resource query](#basic-resource-query)
+      - [Query with filters](#query-with-filters)
+      - [Including related resources in the query](#including-related-resources-in-the-query)
+      - [Query resources by reference](#query-resources-by-reference)
+    - [Add resources to the server](#add-resources-to-the-server)
+    - [Deleting/Updating resources](#deletingupdating-resources)
+    - [Transfer resources between servers](#transfer-resources-between-servers)
+  - [Performance](#performance)
+  - [Contributing](#contributing)
+    - [Development](#development)
+    - [Tests](#tests)
+  - [Credits](#credits)
+
 ## Features
 
 - Create, Read, Update, Delete resources using a FHIR server's REST API
 - Transfer resources between servers while maintaining referential integrity using server-given IDs
 - Bundle creation, validation and data management on a FHIR server via the REST API
 - Supports Hapi, Blaze and IBM FHIR servers
 - CSV serialization of query results
 - Synthetic data generation and
 
-Table of Contents
-=================
 
-* [FHIR Kindling](#fire-fhir-kindling)
-   * [Features](#features)
-   * [Installation](#installation)
-      * [Extras (optional)](#extras-optional)
-   * [Performance](#performance)
-   * [Usage](#usage)
-      * [Connecting to a FHIR server](#connecting-to-a-fhir-server)
-      * [Query resources from the server](#query-resources-from-the-server)
-         * [Basic resource query](#basic-resource-query)
-         * [Query with filters](#query-with-filters)
-         * [Including related resources in the query](#including-related-resources-in-the-query)
-         * [Query resources by reference](#query-resources-by-reference)
-      * [Add resources to the server](#add-resources-to-the-server)
-      * [Deleting/Updating resources](#deletingupdating-resources)
-      * [Transfer resources between servers](#transfer-resources-between-servers)
-   * [Credits](#credits)
 
 <!-- Created by https://github.com/ekalinin/github-markdown-toc -->
 
 
 ## Installation
 
 Install the package using pip:
```

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/base.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,355 +1,361 @@
-from inspect import signature
-from typing import Any, Callable, List, TypeVar, Union
-
-import fhir.resources
-import httpx
-from fhir.resources import FHIRAbstractModel
-from fhir.resources.bundle import Bundle
-from fhir.resources.fhirresourcemodel import FHIRResourceModel
-
-from fhir_kindling.fhir_query.query_parameters import (
-    FhirQueryParameters,
-    FieldParameter,
-    IncludeParameter,
-    QueryOperators,
-    ReverseChainParameter,
-)
-from fhir_kindling.fhir_query.query_response import (
-    OutputFormats,
-)
-
-T = TypeVar("T", bound="FhirQueryBase")
-
-
-class FhirQueryBase:
-    def __init__(
-        self,
-        base_url: str,
-        resource: Union[
-            FHIRResourceModel, fhir.resources.FHIRAbstractModel, str
-        ] = None,
-        query_parameters: FhirQueryParameters = None,
-        auth: httpx.Auth = None,
-        headers: dict = None,
-        output_format: str = "json",
-    ):
-        self.base_url = base_url
-
-        # Set up the requests session with auth and headers
-        self.auth = auth
-        self.headers = headers
-
-        # initialize the resource and query parameters
-        if resource:
-            if isinstance(resource, str):
-                self.resource = fhir.resources.get_fhir_model_class(resource)
-            elif isinstance(resource, FHIRResourceModel) or isinstance(
-                resource, FHIRAbstractModel
-            ):
-                self.resource = resource
-            else:
-                raise ValueError(
-                    f"resource must be a FHIRResourceModel or a string, given {type(resource)}"
-                )
-            self.resource = self.resource.construct()
-            self.query_parameters = FhirQueryParameters(
-                resource=self.resource.resource_type
-            )
-
-        elif query_parameters:
-            self.query_parameters = query_parameters
-            self.resource = fhir.resources.get_fhir_model_class(
-                query_parameters.resource
-            )
-            self.resource = self.resource.construct()
-        else:
-            raise ValueError("Either resource or query_parameters must be set")
-
-        try:
-            self.output_format = OutputFormats(output_format)
-        except ValueError:
-            raise ValueError(
-                f"output_format must be one of {OutputFormats.__members__.keys()}"
-            )
-        self._includes = None
-        self._limit = None
-        self._count = None
-        self._query_response: Union[Bundle, str, None] = None
-
-    def where(
-        self: T,
-        field: str = None,
-        operator: Union[QueryOperators, str] = None,
-        value: Union[int, float, bool, str, list] = None,
-        field_param: Union[FieldParameter, dict] = None,
-    ) -> T:
-        """
-        Add search conditions regarding a specific field of the queried resource.
-        Conditions can be added via FieldParameter class instance, via a dictionary or specifying condition via this
-        method's parameter arguments (field, operator, value).
-        Args:
-            field_param: Instance of FieldParameter defining the field to filter for.
-            field: string specifier of the field to fileter for
-            operator: comparison operator either as string or QueryOperators
-            value: comparison value.
-
-        Returns:
-            FhirQuery object with the added filter
-
-        """
-
-        # evaluate arguments
-        if field_param and (field or operator or value):
-            raise ValueError("Cannot use both field_param and kv parameters")
-        if not field_param and not (field and operator and value):
-            raise ValueError("Either field_param or kv parameters must be set")
-
-        # create field parameters from the different argument options
-        if isinstance(field_param, FieldParameter):
-            added_query_param = field_param
-        elif isinstance(field_param, dict):
-            added_query_param = FieldParameter(**field_param)
-        else:
-            added_query_param = self._param_from_field(field, operator, value)
-
-        # add the field parameter to the query parameters
-        query_field_params = self.query_parameters.resource_parameters
-        if isinstance(query_field_params, list) and len(query_field_params) > 0:
-            query_field_params.append(added_query_param)
-        else:
-            query_field_params = [added_query_param]
-
-        self.query_parameters.resource_parameters = query_field_params
-
-        return self
-
-    @staticmethod
-    def _param_from_field(field, operator, value):
-        if not (operator or operator == "") and value:
-            kv_error_message = (
-                f"\n\tField: {field}\n\tOperator: {operator}\n\tValue: {value}"
-            )
-            raise ValueError(
-                f"Must provide operator and search value when using kv parameters.{kv_error_message}"
-            )
-        else:
-            if isinstance(operator, str):
-                operator = QueryOperators(operator)
-            else:
-                raise ValueError(
-                    f"Operator must be a string or QueryOperators. Got {operator}"
-                )
-            added_query_param = FieldParameter(
-                field=field, operator=operator, value=value
-            )
-        return added_query_param
-
-    def include(
-        self: T,
-        resource: str = None,
-        reference_param: str = None,
-        target: str = None,
-        reverse: bool = False,
-        include_dict: dict = None,
-        include_param: IncludeParameter = None,
-    ) -> T:
-        """
-        Specify resources related to the queried resource, which should be included in the query results.
-
-        Args:
-            resource: name of the resource from which to include related resources, has to match the main resource
-                of the query
-            reference_param: the reference parameter to search for
-            target: further specification of the reference parameter to search for
-            reverse: whether to consider reverse references
-            include_dict: dictionary container the include parameters
-            include_param: instance of IncludeParameter defining the include parameters
-
-        Returns:
-            Updated query instance with an added include parameter
-
-        """
-
-        if include_dict and include_param:
-            raise ValueError("Cannot use both include_dict and include_param")
-        elif include_dict and (resource or reference_param or target):
-            raise ValueError("Cannot use both include_dict and kv parameters")
-        elif include_param and (resource or reference_param or target):
-            raise ValueError("Cannot use both include_param and kv parameters")
-
-        if isinstance(include_dict, dict):
-            added_include_param = IncludeParameter(**include_dict)
-        elif isinstance(include_param, IncludeParameter):
-            added_include_param = include_param
-        elif resource and reference_param:
-            added_include_param = IncludeParameter(
-                resource=resource,
-                search_param=reference_param,
-                target=target,
-                reverse=reverse,
-            )
-        else:
-            raise ValueError(
-                "Must provide a valid instance of either include_dict or include_param or the kv parameters"
-            )
-
-        query_include_params = self.query_parameters.include_parameters
-        if isinstance(query_include_params, list) and len(query_include_params) > 0:
-            query_include_params.append(added_include_param)
-        else:
-            query_include_params = [added_include_param]
-
-        self.query_parameters.include_parameters = query_include_params
-
-        return self
-
-    def has(
-        self: T,
-        resource: str = None,
-        reference_param: str = None,
-        search_param: str = None,
-        operator: QueryOperators = None,
-        value: Union[int, float, bool, str, list] = None,
-        has_param: Union[ReverseChainParameter, dict] = None,
-    ) -> T:
-        """
-        Specify query parameters for other resources that are referenced by the queried, only the resources whose
-        referenced resources match the specified search criteria are included in the results.
-
-        Args:
-            resource: type of resource that references the selected resource
-            reference_param: name of the field of the related resource that defines the relation
-            search_param: field of the resource to compare with the given value using the given query operator
-            operator: comparison operator, one of QueryOperators
-            value: the value to compare the field to
-            has_param: instance of ReverseChainParameter object
-        Returns:
-            Updated query object with an added ReverseChainParameter
-
-        """
-
-        # validate method input
-        if has_param and (
-            resource or reference_param or search_param or operator or value
-        ):
-            raise ValueError("Cannot use both has_param and kv parameters")
-
-        if not has_param and not (
-            resource or reference_param or search_param or operator or value
-        ):
-            raise ValueError(
-                "Must provide either has_param or a valid set of kv parameters"
-            )
-
-        # parse ReverseChainParameter from method input
-        if isinstance(has_param, dict):
-            added_has_param = ReverseChainParameter(**has_param)
-        elif isinstance(has_param, ReverseChainParameter):
-            added_has_param = has_param
-        else:
-            added_has_param = ReverseChainParameter(
-                resource=resource,
-                reference_param=reference_param,
-                search_param=search_param,
-                operator=operator,
-                value=value,
-            )
-
-        query_has_params = self.query_parameters.has_parameters
-        if isinstance(query_has_params, list) and len(query_has_params) > 0:
-            query_has_params.append(added_has_param)
-        else:
-            query_has_params = [added_has_param]
-        self.query_parameters.has_parameters = query_has_params
-
-        return self
-
-    def _make_query_string(self) -> str:
-        query_string = self.base_url + self.query_parameters.to_query_string()
-
-        if not self._count:
-            self._count = 5000
-
-        if self._limit and self._limit < self._count:
-            query_string += f"&_count={self._limit}"
-        else:
-            query_string += f"&_count={self._count}"
-        query_string += f"&_format={self.output_format.value}"
-
-        return query_string
-
-    def set_query_string(self, raw_query_string: str):
-        """
-        Use a raw query string to set the query parameters.
-        e.g. /Patient?_id=123&_lastUpdated=gt2019-01-01
-
-        Args:
-            raw_query_string: Query string to set the query parameters
-
-        Returns:
-            Query object with the query parameters set based on the raw query string
-
-        """
-        query_parameters = FhirQueryParameters.from_query_string(raw_query_string)
-        self.query_parameters = query_parameters
-        return self
-
-    @property
-    def query_url(self) -> str:
-        """
-        Display the query URL that will be used to execute the query.
-
-        Returns:
-
-        """
-        return self._make_query_string()
-
-    @staticmethod
-    def _execute_callback(
-        entries: list,
-        callback: Union[
-            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
-        ] = None,
-    ):
-        if callback:
-            callback_signature = signature(callback)
-
-            if len(callback_signature.parameters) > 1:
-                raise ValueError(
-                    "The callback function should have either one or zero arguments"
-                )
-
-            elif len(callback_signature.parameters) == 1:
-                callback(entries)
-            else:
-                callback()
-
-    def __repr__(self):
-        resource = self.resource.resource_type
-        if self.query_parameters.include_parameters:
-            includes = []
-            rev_includes = []
-            for include_param in self.query_parameters.include_parameters:
-                if include_param.reverse:
-                    rev_string = (
-                        f"{include_param.resource}:{include_param.search_param}"
-                    )
-                    if include_param.target:
-                        rev_string += f":{include_param.target}"
-                    rev_includes.append(rev_string)
-                else:
-                    include_string = f"{include_param.search_param}"
-                    if include_param.target:
-                        include_string += f":{include_param.target}"
-                    includes.append(include_string)
-
-            include_repr = f", include={','.join(includes)}" if includes else ""
-            rev_include_repr = (
-                f", reverse_includes={','.join(rev_includes)}" if rev_includes else ""
-            )
-            includes_repr = include_repr + rev_include_repr
-            return f"<{self.__class__.__name__}(resource={resource}{includes_repr}, url={self.query_url}>"
-        else:
-            return (
-                f"<{self.__class__.__name__}(resource={resource}, url={self.query_url}>"
-            )
+from inspect import signature
+from typing import Any, Callable, List, TypeVar, Union
+
+import fhir.resources
+import httpx
+from fhir.resources import FHIRAbstractModel
+from fhir.resources.bundle import Bundle
+from fhir.resources.fhirresourcemodel import FHIRResourceModel
+
+from fhir_kindling.fhir_query.query_parameters import (
+    FhirQueryParameters,
+    FieldParameter,
+    IncludeParameter,
+    QueryOperators,
+    ReverseChainParameter,
+)
+from fhir_kindling.fhir_query.query_response import (
+    OutputFormats,
+)
+
+T = TypeVar("T", bound="FhirQueryBase")
+
+
+class FhirQueryBase:
+    def __init__(
+        self,
+        base_url: str,
+        resource: Union[
+            FHIRResourceModel, fhir.resources.FHIRAbstractModel, str
+        ] = None,
+        query_parameters: FhirQueryParameters = None,
+        auth: httpx.Auth = None,
+        headers: dict = None,
+        output_format: str = "json",
+    ):
+        self.base_url = base_url
+
+        # Set up the requests session with auth and headers
+        self.auth = auth
+        self.headers = headers
+
+        # initialize the resource and query parameters
+        if resource:
+            if isinstance(resource, str):
+                self.resource = fhir.resources.get_fhir_model_class(resource)
+            elif isinstance(resource, FHIRResourceModel) or isinstance(
+                resource, FHIRAbstractModel
+            ):
+                self.resource = resource
+            else:
+                raise ValueError(
+                    f"resource must be a FHIRResourceModel or a string, given {type(resource)}"
+                )
+            self.resource = self.resource.construct()
+            self.query_parameters = FhirQueryParameters(
+                resource=self.resource.resource_type
+            )
+
+        elif query_parameters:
+            self.query_parameters = query_parameters
+            self.resource = fhir.resources.get_fhir_model_class(
+                query_parameters.resource
+            )
+            self.resource = self.resource.construct()
+        else:
+            raise ValueError("Either resource or query_parameters must be set")
+
+        try:
+            self.output_format = OutputFormats(output_format)
+        except ValueError:
+            raise ValueError(
+                f"output_format must be one of {OutputFormats.__members__.keys()}"
+            )
+        self._includes = None
+        self._limit = None
+        self._count = None
+        self._query_response: Union[Bundle, str, None] = None
+
+    def where(
+        self: T,
+        field: str = None,
+        operator: Union[QueryOperators, str] = None,
+        value: Union[int, float, bool, str, list] = None,
+        field_param: Union[FieldParameter, dict] = None,
+    ) -> T:
+        """
+        Add search conditions regarding a specific field of the queried resource.
+        Conditions can be added via FieldParameter class instance, via a dictionary or specifying condition via this
+        method's parameter arguments (field, operator, value).
+        Args:
+            field_param: Instance of FieldParameter defining the field to filter for.
+            field: string specifier of the field to fileter for
+            operator: comparison operator either as string or QueryOperators
+            value: comparison value.
+
+        Returns:
+            FhirQuery object with the added filter
+
+        """
+
+        # evaluate arguments
+        if field_param and (field or operator or value):
+            raise ValueError("Cannot use both field_param and kv parameters")
+        if not field_param and not (field and operator and value):
+            raise ValueError("Either field_param or kv parameters must be set")
+
+        # create field parameters from the different argument options
+        if isinstance(field_param, FieldParameter):
+            added_query_param = field_param
+        elif isinstance(field_param, dict):
+            added_query_param = FieldParameter(**field_param)
+        else:
+            added_query_param = self._param_from_field(field, operator, value)
+
+        # add the field parameter to the query parameters
+        query_field_params = self.query_parameters.resource_parameters
+        if isinstance(query_field_params, list) and len(query_field_params) > 0:
+            query_field_params.append(added_query_param)
+        else:
+            query_field_params = [added_query_param]
+
+        self.query_parameters.resource_parameters = query_field_params
+
+        return self
+
+    @staticmethod
+    def _param_from_field(field, operator, value):
+        if not (operator or operator == "") and value:
+            kv_error_message = (
+                f"\n\tField: {field}\n\tOperator: {operator}\n\tValue: {value}"
+            )
+            raise ValueError(
+                f"Must provide operator and search value when using kv parameters.{kv_error_message}"
+            )
+        else:
+            if isinstance(operator, str):
+                operator = QueryOperators(operator)
+            else:
+                raise ValueError(
+                    f"Operator must be a string or QueryOperators. Got {operator}"
+                )
+            added_query_param = FieldParameter(
+                field=field, operator=operator, value=value
+            )
+        return added_query_param
+
+    def include(
+        self: T,
+        resource: str = None,
+        reference_param: str = None,
+        target: str = None,
+        reverse: bool = False,
+        include_dict: dict = None,
+        include_param: IncludeParameter = None,
+    ) -> T:
+        """
+        Specify resources related to the queried resource, which should be included in the query results.
+
+        Args:
+            resource: name of the resource from which to include related resources, has to match the main resource
+                of the query
+            reference_param: the reference parameter to search for
+            target: further specification of the reference parameter to search for
+            reverse: whether to consider reverse references
+            include_dict: dictionary container the include parameters
+            include_param: instance of IncludeParameter defining the include parameters
+
+        Returns:
+            Updated query instance with an added include parameter
+
+        """
+
+        if include_dict and include_param:
+            raise ValueError("Cannot use both include_dict and include_param")
+        elif include_dict and (resource or reference_param or target):
+            raise ValueError("Cannot use both include_dict and kv parameters")
+        elif include_param and (resource or reference_param or target):
+            raise ValueError("Cannot use both include_param and kv parameters")
+
+        if isinstance(include_dict, dict):
+            added_include_param = IncludeParameter(**include_dict)
+        elif isinstance(include_param, IncludeParameter):
+            added_include_param = include_param
+        elif resource and reference_param:
+            added_include_param = IncludeParameter(
+                resource=resource,
+                search_param=reference_param,
+                target=target,
+                reverse=reverse,
+            )
+        else:
+            raise ValueError(
+                "Must provide a valid instance of either include_dict or include_param or the kv parameters"
+            )
+
+        query_include_params = self.query_parameters.include_parameters
+        if isinstance(query_include_params, list) and len(query_include_params) > 0:
+            query_include_params.append(added_include_param)
+        else:
+            query_include_params = [added_include_param]
+
+        self.query_parameters.include_parameters = query_include_params
+
+        return self
+
+    def has(
+        self: T,
+        resource: str = None,
+        reference_param: str = None,
+        search_param: str = None,
+        operator: QueryOperators = None,
+        value: Union[int, float, bool, str, list] = None,
+        has_param: Union[ReverseChainParameter, dict] = None,
+    ) -> T:
+        """
+        Specify query parameters for other resources that are referenced by the queried, only the resources whose
+        referenced resources match the specified search criteria are included in the results.
+
+        Args:
+            resource: type of resource that references the selected resource
+            reference_param: name of the field of the related resource that defines the relation
+            search_param: field of the resource to compare with the given value using the given query operator
+            operator: comparison operator, one of QueryOperators
+            value: the value to compare the field to
+            has_param: instance of ReverseChainParameter object
+        Returns:
+            Updated query object with an added ReverseChainParameter
+
+        """
+
+        # validate method input
+        if has_param and (
+            resource or reference_param or search_param or operator or value
+        ):
+            raise ValueError("Cannot use both has_param and kv parameters")
+
+        if not has_param and not (
+            resource or reference_param or search_param or operator or value
+        ):
+            raise ValueError(
+                "Must provide either has_param or a valid set of kv parameters"
+            )
+
+        # parse ReverseChainParameter from method input
+        if isinstance(has_param, dict):
+            added_has_param = ReverseChainParameter(**has_param)
+        elif isinstance(has_param, ReverseChainParameter):
+            added_has_param = has_param
+        else:
+            added_has_param = ReverseChainParameter(
+                resource=resource,
+                reference_param=reference_param,
+                search_param=search_param,
+                operator=operator,
+                value=value,
+            )
+
+        query_has_params = self.query_parameters.has_parameters
+        if isinstance(query_has_params, list) and len(query_has_params) > 0:
+            query_has_params.append(added_has_param)
+        else:
+            query_has_params = [added_has_param]
+        self.query_parameters.has_parameters = query_has_params
+
+        return self
+
+    def _make_query_string(self) -> str:
+        query_string = self.base_url + self.query_parameters.to_query_string()
+
+        if not self._count:
+            self._count = 5000
+
+        if self._limit and self._limit < self._count:
+            if query_string[-1] == "?":
+                query_string += f"_count={self._limit}"
+            else:
+                query_string += f"&_count={self._limit}"
+        else:
+            if query_string[-1] == "?":
+                query_string += f"_count={self._count}"
+            else:
+                query_string += f"&_count={self._count}"
+        query_string += f"&_format={self.output_format.value}"
+
+        return query_string
+
+    def set_query_string(self, raw_query_string: str):
+        """
+        Use a raw query string to set the query parameters.
+        e.g. /Patient?_id=123&_lastUpdated=gt2019-01-01
+
+        Args:
+            raw_query_string: Query string to set the query parameters
+
+        Returns:
+            Query object with the query parameters set based on the raw query string
+
+        """
+        query_parameters = FhirQueryParameters.from_query_string(raw_query_string)
+        self.query_parameters = query_parameters
+        return self
+
+    @property
+    def query_url(self) -> str:
+        """
+        Display the query URL that will be used to execute the query.
+
+        Returns:
+
+        """
+        return self._make_query_string()
+
+    @staticmethod
+    def _execute_callback(
+        entries: list,
+        callback: Union[
+            Callable[[List[FHIRAbstractModel]], Any], Callable[[], Any], None
+        ] = None,
+    ):
+        if callback:
+            callback_signature = signature(callback)
+
+            if len(callback_signature.parameters) > 1:
+                raise ValueError(
+                    "The callback function should have either one or zero arguments"
+                )
+
+            elif len(callback_signature.parameters) == 1:
+                callback(entries)
+            else:
+                callback()
+
+    def __repr__(self):
+        resource = self.resource.resource_type
+        if self.query_parameters.include_parameters:
+            includes = []
+            rev_includes = []
+            for include_param in self.query_parameters.include_parameters:
+                if include_param.reverse:
+                    rev_string = (
+                        f"{include_param.resource}:{include_param.search_param}"
+                    )
+                    if include_param.target:
+                        rev_string += f":{include_param.target}"
+                    rev_includes.append(rev_string)
+                else:
+                    include_string = f"{include_param.search_param}"
+                    if include_param.target:
+                        include_string += f":{include_param.target}"
+                    includes.append(include_string)
+
+            include_repr = f", include={','.join(includes)}" if includes else ""
+            rev_include_repr = (
+                f", reverse_includes={','.join(rev_includes)}" if rev_includes else ""
+            )
+            includes_repr = include_repr + rev_include_repr
+            return f"<{self.__class__.__name__}(resource={resource}{includes_repr}, url={self.query_url}>"
+        else:
+            return (
+                f"<{self.__class__.__name__}(resource={resource}, url={self.query_url}>"
+            )
```

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_async.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_async.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_parameters.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_parameters.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_response.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_response.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_query/query_sync.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_query/query_sync.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/auth.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/auth.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/fhir_server.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/fhir_server.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/server_responses.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/server_responses.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/summary.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/summary.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/transactions.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transactions.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/fhir_server/transfer.py` & `fhir_kindling-1.0.0a8/fhir_kindling/fhir_server/transfer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,222 +1,246 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, List, OrderedDict, Tuple, Union
-
-import networkx as nx
-import orjson
-from fhir.resources import FHIRAbstractModel, construct_fhir_element
-from fhir.resources.resource import Resource
-
-from fhir_kindling.fhir_query import FhirQuerySync
-from fhir_kindling.fhir_server.server_responses import (
-    ResourceCreateResponse,
-    TransferResponse,
-)
-from fhir_kindling.util.references import check_missing_references, extract_references
-
-if TYPE_CHECKING:
-    from fhir_kindling.fhir_server import FhirServer
-
-
-def transfer(
-    source: "FhirServer",
-    target: "FhirServer",
-    resources: List[Union[Resource, FHIRAbstractModel]] = None,
-    query: FhirQuerySync = None,
-    get_missing: bool = True,
-    record_linkage: bool = True,
-    display: bool = True,
-) -> TransferResponse:
-    """
-    Transfer a list of resources from one server to another.
-
-    Args:
-        source: The server to transfer the resources from.
-        target: The server to transfer the resources to.
-        resources: A list of resources to transfer.
-        query: A FhirQuerySync object to use to query the source server.
-        get_missing: Whether to get missing resources from the source server.
-        record_linkage: Whether to record the linkage between the source and target resources.
-        display: Whether to display a progress bar.
-    """
-
-    # get the resources to transfer, including missing references
-    transfer_resources = _get_transfer_resources(source, resources, query, get_missing)
-    transfer_graph = reference_graph(transfer_resources)
-
-    # process the graph to create the resources on the target server
-    create_responses, linkage = _resolve_reference_graph(
-        transfer_graph, target, record_linkage, display
-    )
-
-    return TransferResponse(
-        origin_server=source.api_address,
-        destination_server=target.api_address,
-        create_responses=create_responses,
-        linkage=linkage,
-    )
-
-
-def reference_graph(resources: List[Union[Resource, FHIRAbstractModel]]) -> nx.DiGraph:
-    """
-    Creates a graph of the references in a list of resources.
-
-    Args:
-        resources: List of resource to create the graph from.
-
-    Returns:
-        A directed graph depicting the references in the resources.
-    """
-    dg = nx.DiGraph()
-    for resource in resources:
-        path = resource.relative_path()
-        if path in dg:
-            dg.nodes[path]["resource"] = resource
-        else:
-            dg.add_node(path, resource=resource)
-        for reference in extract_references(resource):
-            reference_path = f"{reference[1]}/{reference[2]}"
-            if reference_path not in dg:
-                dg.add_node(reference_path, resource=None)
-            dg.add_edge(
-                reference_path, path, field=reference[0], list_field=reference[3]
-            )
-    return dg
-
-
-def _resolve_reference_graph(
-    graph: nx.DiGraph,
-    target: "FhirServer",
-    record_linkage: bool,
-    display: bool,
-) -> Tuple[List[ResourceCreateResponse], dict]:
-    nodes = list(graph.nodes)
-
-    linkage = {}
-    create_responses = []
-    # iterate over the graph and update the references off all successors node to match the newly created resources
-    # on the target server
-    while len(nodes) > 0:
-        top_nodes = [node for node in nodes if len(list(graph.predecessors(node))) == 0]
-        if display:
-            print(f"Transferring - {len(top_nodes)} resources: {top_nodes}")
-
-        # get the resources from the graph
-        resources = [_resource_from_graph_node(graph, node) for node in top_nodes]
-        # insert the resources into the target server
-        create_response = target.add_all(resources=resources)
-
-        # iterate through the top nodes and update the successors with the references from the target server
-        for node, reference in zip(top_nodes, create_response.references):
-            if record_linkage:
-                hash_origin = hash(node)
-                linkage[hash_origin] = reference.reference
-            _update_successors(graph, node, reference.reference)
-
-        # add the create response to the list of responses
-        create_responses.extend(create_response.create_responses)
-
-        # remove the processed top nodes from the graph
-        graph.remove_nodes_from(top_nodes)
-        nodes = list(graph.nodes)
-
-    return create_responses, linkage
-
-
-def _update_successors(graph: nx.DiGraph, node: str, reference: str):
-    """
-    Update the successors of a node in a graph with the updated reference from the new server.
-
-    Args:
-        graph: The graph to update.
-        node: The node to update.
-        reference: The reference to update the node with.
-    """
-    for successor in graph.successors(node):
-        field = graph[node][successor]["field"]
-        list_field = graph[node][successor]["list_field"]
-        resource = graph.nodes[successor]["resource"]
-
-        if list_field:
-            # Find the item that references the node
-            reference_list = graph.nodes[successor]["resource"].dict()[field]
-            reference_item = next(
-                (item for item in reference_list if item.get("reference") == str(node)),
-                None,
-            )
-            if reference_item:
-                # update the resource with the new reference
-                index = reference_list.index(reference_item)
-                resource = orjson.loads(resource.json())
-                resource[field][index] = {"reference": reference}
-                graph.nodes[successor]["resource"] = resource
-            else:
-                print("Reference item not found")
-        else:
-            if not isinstance(graph.nodes[successor]["resource"], dict):
-                resource = orjson.loads(resource.json())
-                resource[field] = {"reference": reference}
-                graph.nodes[successor]["resource"] = resource
-            else:
-                graph.nodes[successor]["resource"][field] = reference
-
-
-def _resource_from_graph_node(graph: nx.DiGraph, node: str) -> FHIRAbstractModel:
-    """
-    Get a resource from a graph node.
-
-    Args:
-        graph: The graph to get the resource from.
-        node: The node to get the resource from.
-
-    Returns:
-        The resource at the node.
-    """
-    resource = graph.nodes[node]["resource"]
-    if resource:
-        if isinstance(resource, OrderedDict) or isinstance(resource, dict):
-            resource_dict = dict(resource)
-            resource_type = resource_dict.get(
-                "resourceType", resource_dict.get("resource_type")
-            )
-            resource_json = orjson.dumps(resource_dict)
-            resource = construct_fhir_element(resource_type, resource_json)
-        elif isinstance(resource, FHIRAbstractModel):
-            pass
-        else:
-            raise ValueError(f"Unknown resource type: {type(resource)}")
-        return resource
-    else:
-        raise ValueError(f"Resource not found for node {node}")
-
-
-def _get_transfer_resources(
-    source: "FhirServer",
-    resources: List[Union[Resource, FHIRAbstractModel]] = None,
-    query: FhirQuerySync = None,
-    get_missing: bool = True,
-) -> List[FHIRAbstractModel]:
-    if query and resources:
-        raise ValueError("Cannot specify both query and resources")
-    if not query and not resources:
-        raise ValueError(
-            f"Must specify either query or resources. Query: {query}, Resources: {resources}"
-        )
-    # if query parameters are given execute the query against the server
-    if query:
-        resources = query.all().resource_list
-    # find missing references
-    missing_references = check_missing_references(resources)
-
-    # get missing references
-    if missing_references:
-        if get_missing:
-            missing = source.get_many(missing_references)
-            resources.extend(missing)
-        else:
-            raise ValueError(
-                f"Related resources of the resources to be transferred are missing:\n{missing_references} \n\n"
-                f"To get these resources, set get_missing=True."
-            )
-
-    return resources
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, List, OrderedDict, Tuple, Union
+
+import networkx as nx
+import orjson
+from fhir.resources import FHIRAbstractModel, construct_fhir_element
+from fhir.resources.resource import Resource
+from pydantic import ValidationError
+from tqdm.autonotebook import tqdm
+
+from fhir_kindling.fhir_query import FhirQuerySync
+from fhir_kindling.fhir_server.server_responses import (
+    ResourceCreateResponse,
+    TransferResponse,
+)
+from fhir_kindling.util.references import check_missing_references, extract_references
+
+if TYPE_CHECKING:
+    from fhir_kindling.fhir_server import FhirServer
+
+
+def transfer(
+    source: "FhirServer",
+    target: "FhirServer",
+    resources: List[Union[Resource, FHIRAbstractModel]] = None,
+    query: FhirQuerySync = None,
+    get_missing: bool = True,
+    record_linkage: bool = True,
+    display: bool = True,
+) -> TransferResponse:
+    """
+    Transfer a list of resources from one server to another.
+
+    Args:
+        source: The server to transfer the resources from.
+        target: The server to transfer the resources to.
+        resources: A list of resources to transfer.
+        query: A FhirQuerySync object to use to query the source server.
+        get_missing: Whether to get missing resources from the source server.
+        record_linkage: Whether to record the linkage between the source and target resources.
+        display: Whether to display a progress bar.
+    """
+
+    # get the resources to transfer, including missing references
+    transfer_resources = _get_transfer_resources(source, resources, query, get_missing)
+    transfer_graph = reference_graph(transfer_resources)
+
+    # process the graph to create the resources on the target server
+    create_responses, linkage = resolve_reference_graph(
+        transfer_graph, target, record_linkage, display
+    )
+
+    return TransferResponse(
+        origin_server=source.api_address,
+        destination_server=target.api_address,
+        create_responses=create_responses,
+        linkage=linkage,
+    )
+
+
+def reference_graph(resources: List[Union[Resource, FHIRAbstractModel]]) -> nx.DiGraph:
+    """
+    Creates a graph of the references in a list of resources.
+
+    Args:
+        resources: List of resource to create the graph from.
+
+    Returns:
+        A directed graph depicting the references in the resources.
+    """
+    dg = nx.DiGraph()
+    for resource in resources:
+        path = resource.relative_path()
+        if path in dg:
+            dg.nodes[path]["resource"] = resource
+        else:
+            dg.add_node(path, resource=resource)
+        for reference in extract_references(resource):
+            reference_path = f"{reference[1]}/{reference[2]}"
+            if reference_path not in dg:
+                dg.add_node(reference_path, resource=None)
+            dg.add_edge(
+                reference_path, path, field=reference[0], list_field=reference[3]
+            )
+    return dg
+
+
+def resolve_reference_graph(
+    graph: nx.DiGraph,
+    target: "FhirServer",
+    record_linkage: bool,
+    display: bool,
+) -> Tuple[List[ResourceCreateResponse], dict]:
+    nodes = list(graph.nodes)
+
+    linkage = {}
+    create_responses = []
+    # iterate over the graph and update the references off all successors node to match the newly created resources
+    # on the target server
+
+    with tqdm(total=len(nodes), disable=not display) as pbar:
+        while len(nodes) > 0:
+            top_nodes = [
+                node for node in nodes if len(list(graph.predecessors(node))) == 0
+            ]
+
+            # get the resources from the graph
+
+            resources = []
+
+            for node in top_nodes:
+                try:
+                    resources.append(_resource_from_graph_node(graph, node))
+                except Exception as e:
+                    print(e)
+                    print(node)
+                    raise e
+            # insert the resources into the target server
+            create_response = target.add_all(resources=resources)
+
+            # iterate through the top nodes and update the successors with the references from the target server
+            for node, reference in zip(top_nodes, create_response.references):
+                if record_linkage:
+                    hash_origin = hash(node)
+                    linkage[hash_origin] = reference.reference
+                _update_successors(graph, node, reference.reference)
+
+            # add the create response to the list of responses
+            create_responses.extend(create_response.create_responses)
+
+            # remove the processed top nodes from the graph
+            graph.remove_nodes_from(top_nodes)
+            nodes = list(graph.nodes)
+            pbar.update(len(top_nodes))
+
+    return create_responses, linkage
+
+
+def _update_successors(graph: nx.DiGraph, node: str, reference: str):
+    """
+    Update the successors of a node in a graph with the updated reference from the new server.
+
+    Args:
+        graph: The graph to update.
+        node: The node to update.
+        reference: The reference to update the node with.
+    """
+    for successor in graph.successors(node):
+        field = graph[node][successor]["field"]
+        list_field = graph[node][successor]["list_field"]
+        resource = graph.nodes[successor]["resource"]
+
+        if list_field:
+            # Find the item that references the node
+            reference_list = graph.nodes[successor]["resource"].dict()[field]
+            reference_item = next(
+                (item for item in reference_list if item.get("reference") == str(node)),
+                None,
+            )
+            if reference_item:
+                # update the resource with the new reference
+                index = reference_list.index(reference_item)
+                resource = orjson.loads(resource.json())
+                resource[field][index] = {"reference": reference}
+                graph.nodes[successor]["resource"] = resource
+            else:
+                print("Reference item not found")
+        else:
+            if not isinstance(graph.nodes[successor]["resource"], dict):
+                resource = orjson.loads(resource.json())
+                resource[field] = {"reference": reference}
+                graph.nodes[successor]["resource"] = resource
+            else:
+                graph.nodes[successor]["resource"][field] = reference
+
+
+def _resource_from_graph_node(graph: nx.DiGraph, node: str) -> FHIRAbstractModel:
+    """
+    Get a resource from a graph node.
+
+    Args:
+        graph: The graph to get the resource from.
+        node: The node to get the resource from.
+
+    Returns:
+        The resource at the node.
+    """
+    resource = graph.nodes[node]["resource"]
+
+    if resource:
+        if isinstance(resource, OrderedDict) or isinstance(resource, dict):
+            resource_dict = dict(resource)
+            resource_type = resource_dict.get(
+                "resourceType", resource_dict.get("resource_type")
+            )
+            resource_json = orjson.dumps(resource_dict)
+            try:
+                resource = construct_fhir_element(resource_type, resource_json)
+            except ValidationError as e:
+                print(f"Error creating resource: {e}")
+                print(f"Resource: {resource_dict}")
+                raise e
+            except Exception as e:
+                print(f"Error creating resource: {e}")
+                print(f"Resource: {resource_dict}")
+                raise e
+        elif isinstance(resource, FHIRAbstractModel):
+            pass
+        else:
+            raise ValueError(f"Unknown resource type: {type(resource)}")
+        return resource
+    else:
+        raise ValueError(f"Resource not found for node {node}")
+
+
+def _get_transfer_resources(
+    source: "FhirServer",
+    resources: List[Union[Resource, FHIRAbstractModel]] = None,
+    query: FhirQuerySync = None,
+    get_missing: bool = True,
+) -> List[FHIRAbstractModel]:
+    if query and resources:
+        raise ValueError("Cannot specify both query and resources")
+    if not query and not resources:
+        raise ValueError(
+            f"Must specify either query or resources. Query: {query}, Resources: {resources}"
+        )
+    # if query parameters are given execute the query against the server
+    if query:
+        resources = query.all().resource_list
+    # find missing references
+    missing_references = check_missing_references(resources)
+
+    # get missing references
+    if missing_references:
+        if get_missing:
+            missing = source.get_many(missing_references)
+            resources.extend(missing)
+        else:
+            raise ValueError(
+                f"Related resources of the resources to be transferred are missing:\n{missing_references} \n\n"
+                f"To get these resources, set get_missing=True."
+            )
+
+    return resources
```

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/figures/resource_plots.py` & `fhir_kindling-1.0.0a8/fhir_kindling/figures/resource_plots.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/figures/summary.py` & `fhir_kindling-1.0.0a8/fhir_kindling/figures/summary.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/generators/field_generator.py` & `fhir_kindling-1.0.0a8/fhir_kindling/generators/field_generator.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/generators/patient.py` & `fhir_kindling-1.0.0a8/fhir_kindling/generators/patient.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,41 +5,56 @@
 import pandas as pd
 import pendulum
 from faker import Faker
 from fhir.resources.humanname import HumanName
 from fhir.resources.patient import Patient
 from fhir.resources.reference import Reference
 
+from fhir_kindling.generators.base import BaseGenerator
+from fhir_kindling.serde.json import json_dict
 
-class PatientGenerator:
+
+class PatientGenerator(BaseGenerator):
     def __init__(
         self,
         n: int,
         age_range: Tuple[int, int] = None,
         gender_distribution: Tuple[float, float, float, float] = None,
         organisation: Reference = None,
         generate_ids: bool = False,
     ):
-        self.resource_type = Patient
+        self.resource = Patient
         self.n = n
         self.age_range = age_range
         self.gender_distribution = gender_distribution
         self._birthdate_range = None
         self.organisation = organisation
         self.generate_ids = generate_ids
         self.resources = None
 
-    def generate(self, references: bool = False):
+    def generate(
+        self,
+        references: bool = False,
+        generate_ids: bool = False,
+        as_dict: bool = False,
+    ):
         patients = self._generate()
         self.resources = patients
 
+        if as_dict:
+            resources = [json_dict(patient) for patient in patients]
+        if self.n == 1:
+            if references:
+                return resources[0], self._generate_references()[0]
+            return resources[0]
+
         if references and not self.generate_ids:
             raise ValueError("Cannot generate references without generating ids")
         elif references:
-            return patients, self._generate_references()
+            return resources, self._generate_references()
 
         return patients
 
     def _generate(self):
         patients = []
         names = self._generate_patient_names(self.n)
         for name in names:
@@ -60,17 +75,16 @@
         name = HumanName(**{"family": last_name, "given": [first_name]})
 
         birthdate = self._generate_birthdate()
         patient_dict = {"gender": gender, "name": [name], "birthDate": birthdate}
         if self.organisation:
             patient_dict["managingOrganization"] = self.organisation
 
-        if self.generate_ids:
-            patient_id = str(uuid4())
-            patient_dict["id"] = patient_id
+        patient_id = str(uuid4())
+        patient_dict["id"] = patient_id
 
         return Patient(**patient_dict)
 
     @staticmethod
     def _generate_patient_names(n: int):
         fake = Faker()
```

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/generators/resource_generator.py` & `fhir_kindling-1.0.0a8/fhir_kindling/generators/resource_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 from uuid import uuid4
 
 from fhir.resources import get_fhir_model_class
 from fhir.resources.fhirresourcemodel import FHIRResourceModel
 from fhir.resources.resource import Resource
 from pydantic import BaseModel
 
+from fhir_kindling.generators.base import BaseGenerator
 from fhir_kindling.generators.field_generator import FieldGenerator
 
 
 class FieldValue(BaseModel):
     field: str
     value: Union[Any, List[Any]]
+    list_field: bool = False
 
 
 class GeneratorParameters(BaseModel):
     count: Optional[int] = None
     field_generators: Optional[List[FieldGenerator]] = None
     field_values: Optional[List[FieldValue]] = None
 
     # todo count and list in field values of same length
 
 
-class ResourceGenerator:
+class ResourceGenerator(BaseGenerator):
     def __init__(
         self,
         resource: Union[str, Any],
         n: int = None,
         field_values: dict = None,
         disable_validation: bool = False,
         generator_parameters: GeneratorParameters = None,
@@ -46,90 +48,97 @@
         if self.field_values and not disable_validation:
             self._check_required_fields()
         self.disable_validation = disable_validation
         self.n = n
         self._value_iterators = {}
         # list to store the field names of all fields being generated
         self._generated_fields = set()
+        self._validated = False
 
     def required_fields(self) -> List[str]:
         required_fields = []
         for field_name, field in self.resource.__fields__.items():
             if field.required:
                 required_fields.append(field_name)
         return required_fields
 
     def fields(self):
         return self.resource.__fields__
 
     def generate(
-        self, disable_validation: bool = False, generate_ids: bool = False
+        self,
+        disable_validation: bool = False,
+        generate_ids: bool = False,
+        as_dict: bool = False,
     ) -> Union[Resource, List[Resource]]:
         self.disable_validation = disable_validation
         # if field values are given parse them into parameters
         if self.n and not self.params:
             self.params = GeneratorParameters(count=self.n)
 
         if self.field_values and self.n:
             self._parse_field_values()
         if not self.disable_validation:
             self._validate_params()
-        resources = self._generate_resources(generate_ids)
+        resources = self._generate_resources(generate_ids=generate_ids, as_dict=as_dict)
         return resources
 
-    def _generate_resources(self, generate_ids: bool):
-        resources = []
+    def _generate_resources(self, generate_ids: bool, as_dict: bool = False):
         if self.params.count:
-            for i in range(self.params.count):
-                resource = self._generate_resource(generate_ids)
+            resources = []
+            for _ in range(self.params.count):
+                resource = self._generate_resource(generate_ids, as_dict=as_dict)
                 resources.append(resource)
             return resources
         else:
-            return self._generate_resource(generate_ids)
+            return self._generate_resource(generate_ids, as_dict=as_dict)
 
-    def _generate_resource(self, generate_id: bool) -> FHIRResourceModel:
+    def _generate_resource(
+        self, generate_id: bool, as_dict: bool = False
+    ) -> Union[FHIRResourceModel, dict]:
         # construct a resource object to hold the generated fields
         resource = self.resource.construct()
+        resource_data = {}
         # disable assignment validation
         resource.Config.validate_assignment = False
         if self.params.field_values:
             for field_value in self.params.field_values:
                 # update resource with field value
-                self._update_with_field_value(resource, field_value)
+                self._update_with_field_value(resource_data, field_value)
 
         if self.params.field_generators:
             for generator in self.params.field_generators:
                 # update resource with generated field value
-                self._update_with_field_generator(resource, generator)
+                self._update_with_field_generator(resource_data, generator)
         if generate_id:
-            resource.id = str(uuid4())
+            resource_data["id"] = str(uuid4())
 
         # validate resource when validation is enabled
-        if not self.disable_validation:
-            resource = self.resource(**resource.dict(exclude_none=True))
-
+        # if not self.disable_validation:
+        #     resource = self.resource(**resource.dict(exclude_none=True))
+        if as_dict:
+            return resource_data
+        resource = self.resource(**resource_data)
         return resource
 
-    def _update_with_field_value(
-        self, resource: FHIRResourceModel, field_value: FieldValue
-    ):
-        if isinstance(field_value.value, list):
+    def _update_with_field_value(self, resource_data: dict, field_value: FieldValue):
+        if isinstance(field_value.value, list) and not field_value.list_field:
             iterator = self._value_iterators.get(field_value.field)
             if not iterator:
                 iterator = iter(field_value.value)
                 self._value_iterators[field_value.field] = iterator
-            resource.__setattr__(field_value.field, next(iterator))
+            resource_data[field_value.field] = next(iterator)
         else:
-            resource.__setattr__(field_value.field, field_value.value)
+            resource_data[field_value.field] = field_value.value
 
     def _update_with_field_generator(
-        self, resource: FHIRResourceModel, field_generator: FieldGenerator
+        self, resource_data: dict, field_generator: FieldGenerator
     ):
         value = field_generator.generate()
-        resource.__setattr__(field_generator.field, value)
+        resource_data[field_generator.field] = value
 
     def _check_required_fields(self):
         """
         Check if all required fields are being generated by the field generators or are given as field values
 
         Returns:
 
@@ -145,24 +154,29 @@
         params = GeneratorParameters(count=self.n)
 
         # todo: add support for field_values as a list of dicts
 
         self.params = params
 
     def _validate_params(self):
+        # skip validation if it has been previously validated
+        if self._validated:
+            return
         # validate field values
         if self.params.field_values:
             self._validate_field_values()
 
         # validate field generators
         if self.params.field_generators:
             self._validate_field_generators()
 
         # check that the required fields are being generated
-        self._check_required_fields()
+        # self._check_required_fields()
+
+        self._validated = True
 
     def _validate_field_values(self):
         field_values = self.params.field_values
         resource_count = self.params.count
 
         for field_value in field_values:
             # check for duplicates in generated fields
@@ -170,15 +184,18 @@
                 raise ValueError(
                     f"Field value {field_value.value} is already generated"
                 )
             self._generated_fields.add(field_value.field)
 
             # check that the list length matches the resource count
             if isinstance(field_value.value, list):
-                if len(field_value.value) != resource_count:
+                if (
+                    len(field_value.value) != resource_count
+                    and not field_value.list_field
+                ):
                     raise ValueError(
                         f"Field value list length does not match resource count: {field_value.field}"
                         f"Items in field value list: {len(field_value.value)},"
                         f" resource count: {resource_count}"
                     )
             # todo check that the type of the item fits into the selected field
```

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/privacy/k_anonymity.py` & `fhir_kindling-1.0.0a8/fhir_kindling/privacy/k_anonymity.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/serde/flatten.py` & `fhir_kindling-1.0.0a8/fhir_kindling/serde/flatten.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/conftest.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/server/test_transfer.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/server/test_transfer.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_auth.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_fhir_query.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_query.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_fhir_server.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_fhir_server.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_generators.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_generators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import random
+from datetime import datetime
 
 import pendulum
 import pytest
 from dotenv import find_dotenv, load_dotenv
 from fhir.resources.codeableconcept import CodeableConcept
 from fhir.resources.coding import Coding
 from fhir.resources.patient import Patient
@@ -14,14 +16,15 @@
 from fhir_kindling.generators.field_generator import FieldGenerator
 from fhir_kindling.generators.patient import PatientGenerator
 from fhir_kindling.generators.resource_generator import (
     FieldValue,
     GeneratorParameters,
     ResourceGenerator,
 )
+from fhir_kindling.generators.time_series_generator import TimeSeriesGenerator
 
 
 @pytest.fixture
 def api_url():
     """
     Base api url and env vars
     """
@@ -95,14 +98,15 @@
 
 
 def test_patient_generator():
     patient_generator = PatientGenerator(n=100)
     patients = patient_generator.generate()
     assert len(patients) == 100
     assert isinstance(patients[0], Patient)
+    print(patients[0].id)
 
     generator = PatientGenerator(n=10, age_range=(18, 60))
     patients = generator.generate()
 
     with pytest.raises(ValueError):
         generator = PatientGenerator(n=10, age_range=("hello", "world"))
         generator.generate()
@@ -277,15 +281,15 @@
         field_values=[
             FieldValue(field="code", value=covid_code),
         ]
     )
 
     covid_generator = ResourceGenerator("Condition", generator_parameters=covid_params)
     # add covid conditions to patients
-    dataset_generator.add_resource(covid_generator, name="covid")
+    dataset_generator.add_resource_generator(covid_generator, name="covid")
 
     patients, patient_ids = PatientGenerator(n=count, generate_ids=True).generate(
         references=True
     )
 
     vaccination_date_generator = FieldGenerator(
         field="occurrenceDateTime",
@@ -299,16 +303,74 @@
         ],
         field_generators=[vaccination_date_generator],
     )
     vaccination_generator = ResourceGenerator(
         "Immunization", generator_parameters=first_vax_params
     )
     print(vaccination_generator)
-    dataset_generator.add_resource(
+    dataset_generator.add_resource_generator(
         vaccination_generator, name="first_vaccination", likelihood=0.8
     )
 
     dataset = dataset_generator.generate(ids=True)
     print(dataset)
     # pprint(result.dict(exclude_none=True))
 
     dataset.upload(server)
+
+
+def test_time_series_generator():
+    body_temp_code = CodeableConcept(
+        coding=[
+            Coding(
+                system="http://loinc.org",
+                code="99836-5",
+                display="Body temperature",
+            )
+        ]
+    )
+
+    body_temp_params = GeneratorParameters(
+        field_values=[
+            FieldValue(field="code", value=body_temp_code),
+            FieldValue(field="status", value="final"),
+        ],
+        field_generators=[
+            FieldGenerator(
+                field="valueQuantity",
+                generator_function=lambda: {
+                    "value": random.randint(36, 40) + random.random(),
+                    "unit": "C",
+                    "system": "http://unitsofmeasure.org",
+                },
+            ),
+        ],
+    )
+
+    body_temp_generator = ResourceGenerator(
+        "Observation", generator_parameters=body_temp_params
+    )
+
+    body_temp_ts_generator = TimeSeriesGenerator(
+        resource_generator=body_temp_generator,
+        time_field="effectiveDateTime",
+        start=datetime(2021, 1, 1),
+        freq="daily",
+        n=20,
+    )
+
+    result = body_temp_ts_generator.generate()
+    print("Result generate n \n\n")
+    print(result)
+    assert len(result) == 20
+
+    body_temp_range_generator = TimeSeriesGenerator(
+        resource_generator=body_temp_generator,
+        time_field="effectiveDateTime",
+        start=datetime(2021, 1, 1),
+        end=datetime(2021, 3, 1),
+        freq="daily",
+    )
+    result = body_temp_range_generator.generate()
+
+    print("Result generate range \n\n")
+    print(result)
```

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_plots.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_privacy.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_privacy.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_serialization.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/tests/test_util.py` & `fhir_kindling-1.0.0a8/fhir_kindling/tests/test_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from fhir.resources.observation import Observation
 from fhir.resources.organization import Organization
 from fhir.resources.patient import Patient
 
 from fhir_kindling import FhirServer
 from fhir_kindling.fhir_server.transfer import reference_graph
 from fhir_kindling.generators import PatientGenerator
+from fhir_kindling.util.benchmark import ServerBenchmark
 from fhir_kindling.util.references import (
     _resource_ids_from_query_response,
     check_missing_references,
     extract_references,
 )
 from fhir_kindling.util.resources import (
     check_resource_contains_field,
@@ -135,7 +136,14 @@
     assert len(list(graph.predecessors(conditions[0].relative_path()))) == 2
 
 
 def test_resource_contains_field(server):
     check_resource_contains_field("Patient", "birthDate")
     with pytest.raises(ValueError):
         check_resource_contains_field("Patient", "foo")
+
+
+def test_benchmark(server):
+    transfer_server = FhirServer(api_address=os.getenv("TRANSFER_API_URL"))
+    benchmark = ServerBenchmark(servers=[server, transfer_server])
+    benchmark.run_suite()
+    benchmark.plot()
```

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/util/references.py` & `fhir_kindling-1.0.0a8/fhir_kindling/util/references.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/fhir_kindling/util/resources.py` & `fhir_kindling-1.0.0a8/fhir_kindling/util/resources.py`

 * *Files identical despite different names*

### Comparing `fhir_kindling-1.0.0a7/PKG-INFO` & `fhir_kindling-1.0.0a8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fhir-kindling
-Version: 1.0.0a7
+Version: 1.0.0a8
 Summary: Python library to simplify working with FHIR servers and resources.
 Home-page: https://migraf.github.io/fhir-kindling/
 License: MIT
 Keywords: python,fhir,hl7,client,medical records,healthcare,data
 Author: Michael Graf
 Author-email: michael.graf3110@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,24 +17,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: demo
 Provides-Extra: ds
+Requires-Dist: RISE ; extra == "demo"
 Requires-Dist: authlib
-Requires-Dist: faker (>=18.3.0,<19.0.0) ; extra == "ds"
-Requires-Dist: fhir.resources
+Requires-Dist: faker ; extra == "ds" or extra == "demo"
+Requires-Dist: fhir.resources (>=6.0.0,<7.0.0)
 Requires-Dist: httpx
+Requires-Dist: ipywidgets ; extra == "demo"
+Requires-Dist: matplotlib ; extra == "ds" or extra == "demo"
 Requires-Dist: networkx
+Requires-Dist: notebook ; extra == "demo"
 Requires-Dist: orjson
-Requires-Dist: pandas ; extra == "ds"
+Requires-Dist: pandas ; extra == "ds" or extra == "demo"
 Requires-Dist: pendulum
-Requires-Dist: plotly ; extra == "ds"
+Requires-Dist: plotly ; extra == "ds" or extra == "demo"
 Requires-Dist: pydantic
 Requires-Dist: tqdm
 Requires-Dist: xmltodict
 Project-URL: Repository, https://github.com/migraf/fhir-kindling
 Description-Content-Type: text/markdown
 
 ![Header](./docs/logo/kindling_header.png)
@@ -54,42 +59,47 @@
 as well as resource transfer between servers.
 Datascience features include flattening of resources and bundles into tabular format (pandas dataframes) and plotting 
 methods for resources and bundles can optionally be included with the `ds` extra.
 
 Check out the [documentation](https://migraf.github.io/fhir-kindling/) for more information and a detailed user guide.
 
 
+Table of Contents
+=================
+
+- [Table of Contents](#table-of-contents)
+  - [Features](#features)
+  - [Installation](#installation)
+    - [Extras (optional)](#extras-optional)
+  - [Usage](#usage)
+    - [Connecting to a FHIR server](#connecting-to-a-fhir-server)
+    - [Query resources from the server](#query-resources-from-the-server)
+      - [Basic resource query](#basic-resource-query)
+      - [Query with filters](#query-with-filters)
+      - [Including related resources in the query](#including-related-resources-in-the-query)
+      - [Query resources by reference](#query-resources-by-reference)
+    - [Add resources to the server](#add-resources-to-the-server)
+    - [Deleting/Updating resources](#deletingupdating-resources)
+    - [Transfer resources between servers](#transfer-resources-between-servers)
+  - [Performance](#performance)
+  - [Contributing](#contributing)
+    - [Development](#development)
+    - [Tests](#tests)
+  - [Credits](#credits)
+
 ## Features
 
 - Create, Read, Update, Delete resources using a FHIR server's REST API
 - Transfer resources between servers while maintaining referential integrity using server-given IDs
 - Bundle creation, validation and data management on a FHIR server via the REST API
 - Supports Hapi, Blaze and IBM FHIR servers
 - CSV serialization of query results
 - Synthetic data generation and
 
-Table of Contents
-=================
 
-* [FHIR Kindling](#fire-fhir-kindling)
-   * [Features](#features)
-   * [Installation](#installation)
-      * [Extras (optional)](#extras-optional)
-   * [Performance](#performance)
-   * [Usage](#usage)
-      * [Connecting to a FHIR server](#connecting-to-a-fhir-server)
-      * [Query resources from the server](#query-resources-from-the-server)
-         * [Basic resource query](#basic-resource-query)
-         * [Query with filters](#query-with-filters)
-         * [Including related resources in the query](#including-related-resources-in-the-query)
-         * [Query resources by reference](#query-resources-by-reference)
-      * [Add resources to the server](#add-resources-to-the-server)
-      * [Deleting/Updating resources](#deletingupdating-resources)
-      * [Transfer resources between servers](#transfer-resources-between-servers)
-   * [Credits](#credits)
 
 <!-- Created by https://github.com/ekalinin/github-markdown-toc -->
 
 
 ## Installation
 
 Install the package using pip:
```

