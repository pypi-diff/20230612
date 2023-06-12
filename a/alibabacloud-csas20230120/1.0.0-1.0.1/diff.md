# Comparing `tmp/alibabacloud_csas20230120-1.0.0.tar.gz` & `tmp/alibabacloud_csas20230120-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_csas20230120-1.0.0.tar", last modified: Fri Mar 24 01:59:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_csas20230120-1.0.1.tar", last modified: Mon Jun 12 05:58:50 2023, max compression
```

## Comparing `alibabacloud_csas20230120-1.0.0.tar` & `alibabacloud_csas20230120-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 01:59:23.000000 alibabacloud_csas20230120-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-24 01:59:23.000000 alibabacloud_csas20230120-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 01:59:23.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)   106630 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120/client.py
--rw-r--r--   0 root         (0) root         (0)   217456 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 01:59:23.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-24 01:59:23.000000 alibabacloud_csas20230120-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2615 2023-03-24 01:59:22.000000 alibabacloud_csas20230120-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97118 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120/client.py
+-rw-r--r--   0 root         (0) root         (0)   202398 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-06-12 05:58:50.000000 alibabacloud_csas20230120-1.0.1/setup.py
```

### Comparing `alibabacloud_csas20230120-1.0.0/LICENSE` & `alibabacloud_csas20230120-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.0.0/PKG-INFO` & `alibabacloud_csas20230120-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_csas20230120
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120-1.0.0/README-CN.md` & `alibabacloud_csas20230120-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.0.0/README.md` & `alibabacloud_csas20230120-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120/client.py` & `alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -435,29 +435,28 @@
         request: csas_20230120_models.CreatePrivateAccessTagRequest,
     ) -> csas_20230120_models.CreatePrivateAccessTagResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_private_access_tag_with_options_async(request, runtime)
 
     def create_user_group_with_options(
         self,
-        tmp_req: csas_20230120_models.CreateUserGroupRequest,
+        request: csas_20230120_models.CreateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateUserGroupResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.CreateUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.attributes):
-            request.attributes_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.attributes, 'Attributes', 'json')
+        UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.attributes_shrink):
-            body['Attributes'] = request.attributes_shrink
+        body_flat = {}
+        if not UtilClient.is_unset(request.attributes):
+            body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
+        body = TeaCore.merge(body,
+            OpenApiUtilClient.query(body_flat))
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateUserGroup',
             version='2023-01-20',
             protocol='HTTPS',
@@ -471,29 +470,28 @@
         return TeaCore.from_map(
             csas_20230120_models.CreateUserGroupResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def create_user_group_with_options_async(
         self,
-        tmp_req: csas_20230120_models.CreateUserGroupRequest,
+        request: csas_20230120_models.CreateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateUserGroupResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.CreateUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.attributes):
-            request.attributes_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.attributes, 'Attributes', 'json')
+        UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.attributes_shrink):
-            body['Attributes'] = request.attributes_shrink
+        body_flat = {}
+        if not UtilClient.is_unset(request.attributes):
+            body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
+        body = TeaCore.merge(body,
+            OpenApiUtilClient.query(body_flat))
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='CreateUserGroup',
             version='2023-01-20',
             protocol='HTTPS',
@@ -1081,22 +1079,18 @@
         request: csas_20230120_models.GetUserGroupRequest,
     ) -> csas_20230120_models.GetUserGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_user_group_with_options_async(request, runtime)
 
     def list_applications_for_private_access_policy_with_options(
         self,
-        tmp_req: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
+        request: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListApplicationsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -1111,22 +1105,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_applications_for_private_access_policy_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
+        request: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListApplicationsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -1155,22 +1145,18 @@
         request: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_applications_for_private_access_policy_with_options_async(request, runtime)
 
     def list_applications_for_private_access_tag_with_options(
         self,
-        tmp_req: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
+        request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListApplicationsForPrivateAccessTagShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessTag',
             version='2023-01-20',
@@ -1185,22 +1171,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListApplicationsForPrivateAccessTagResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_applications_for_private_access_tag_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
+        request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListApplicationsForPrivateAccessTagShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessTag',
             version='2023-01-20',
@@ -1229,22 +1211,18 @@
         request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_applications_for_private_access_tag_with_options_async(request, runtime)
 
     def list_connectors_with_options(
         self,
-        tmp_req: csas_20230120_models.ListConnectorsRequest,
+        request: csas_20230120_models.ListConnectorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListConnectorsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListConnectorsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.connector_ids):
-            request.connector_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.connector_ids, 'ConnectorIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListConnectors',
             version='2023-01-20',
@@ -1259,22 +1237,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListConnectorsResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_connectors_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListConnectorsRequest,
+        request: csas_20230120_models.ListConnectorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListConnectorsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListConnectorsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.connector_ids):
-            request.connector_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.connector_ids, 'ConnectorIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListConnectors',
             version='2023-01-20',
@@ -1303,22 +1277,18 @@
         request: csas_20230120_models.ListConnectorsRequest,
     ) -> csas_20230120_models.ListConnectorsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_connectors_with_options_async(request, runtime)
 
     def list_polices_for_private_access_application_with_options(
         self,
-        tmp_req: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
+        request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForPrivateAccessApplicationShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessApplication',
             version='2023-01-20',
@@ -1333,22 +1303,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_polices_for_private_access_application_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
+        request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForPrivateAccessApplicationShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessApplication',
             version='2023-01-20',
@@ -1377,22 +1343,18 @@
         request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_polices_for_private_access_application_with_options_async(request, runtime)
 
     def list_polices_for_private_access_tag_with_options(
         self,
-        tmp_req: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
+        request: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessTagResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForPrivateAccessTagShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessTag',
             version='2023-01-20',
@@ -1407,22 +1369,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListPolicesForPrivateAccessTagResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_polices_for_private_access_tag_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
+        request: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessTagResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForPrivateAccessTagShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessTag',
             version='2023-01-20',
@@ -1451,22 +1409,18 @@
         request: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessTagResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_polices_for_private_access_tag_with_options_async(request, runtime)
 
     def list_polices_for_user_group_with_options(
         self,
-        tmp_req: csas_20230120_models.ListPolicesForUserGroupRequest,
+        request: csas_20230120_models.ListPolicesForUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_group_ids):
-            request.user_group_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_group_ids, 'UserGroupIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForUserGroup',
             version='2023-01-20',
@@ -1481,22 +1435,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListPolicesForUserGroupResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_polices_for_user_group_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListPolicesForUserGroupRequest,
+        request: csas_20230120_models.ListPolicesForUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_group_ids):
-            request.user_group_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_group_ids, 'UserGroupIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForUserGroup',
             version='2023-01-20',
@@ -1525,22 +1475,18 @@
         request: csas_20230120_models.ListPolicesForUserGroupRequest,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_polices_for_user_group_with_options_async(request, runtime)
 
     def list_private_access_applications_with_options(
         self,
-        tmp_req: csas_20230120_models.ListPrivateAccessApplicationsRequest,
+        request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessApplicationsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessApplications',
             version='2023-01-20',
@@ -1555,22 +1501,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListPrivateAccessApplicationsResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_private_access_applications_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListPrivateAccessApplicationsRequest,
+        request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessApplicationsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessApplications',
             version='2023-01-20',
@@ -1599,22 +1541,18 @@
         request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_applications_with_options_async(request, runtime)
 
     def list_private_access_polices_with_options(
         self,
-        tmp_req: csas_20230120_models.ListPrivateAccessPolicesRequest,
+        request: csas_20230120_models.ListPrivateAccessPolicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessPolicesResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessPolicesShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessPolices',
             version='2023-01-20',
@@ -1629,22 +1567,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListPrivateAccessPolicesResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_private_access_polices_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListPrivateAccessPolicesRequest,
+        request: csas_20230120_models.ListPrivateAccessPolicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessPolicesResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessPolicesShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessPolices',
             version='2023-01-20',
@@ -1673,22 +1607,18 @@
         request: csas_20230120_models.ListPrivateAccessPolicesRequest,
     ) -> csas_20230120_models.ListPrivateAccessPolicesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_polices_with_options_async(request, runtime)
 
     def list_private_access_tags_with_options(
         self,
-        tmp_req: csas_20230120_models.ListPrivateAccessTagsRequest,
+        request: csas_20230120_models.ListPrivateAccessTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessTagsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessTagsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessTags',
             version='2023-01-20',
@@ -1703,22 +1633,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListPrivateAccessTagsResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_private_access_tags_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListPrivateAccessTagsRequest,
+        request: csas_20230120_models.ListPrivateAccessTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessTagsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessTagsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessTags',
             version='2023-01-20',
@@ -1747,22 +1673,18 @@
         request: csas_20230120_models.ListPrivateAccessTagsRequest,
     ) -> csas_20230120_models.ListPrivateAccessTagsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_tags_with_options_async(request, runtime)
 
     def list_tags_for_private_access_application_with_options(
         self,
-        tmp_req: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
+        request: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessApplicationResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListTagsForPrivateAccessApplicationShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessApplication',
             version='2023-01-20',
@@ -1777,22 +1699,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListTagsForPrivateAccessApplicationResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_tags_for_private_access_application_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
+        request: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessApplicationResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListTagsForPrivateAccessApplicationShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessApplication',
             version='2023-01-20',
@@ -1821,22 +1739,18 @@
         request: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.ListTagsForPrivateAccessApplicationResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_tags_for_private_access_application_with_options_async(request, runtime)
 
     def list_tags_for_private_access_policy_with_options(
         self,
-        tmp_req: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
+        request: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessPolicyResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListTagsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -1851,22 +1765,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListTagsForPrivateAccessPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_tags_for_private_access_policy_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
+        request: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessPolicyResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListTagsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -1895,22 +1805,18 @@
         request: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListTagsForPrivateAccessPolicyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_tags_for_private_access_policy_with_options_async(request, runtime)
 
     def list_user_groups_with_options(
         self,
-        tmp_req: csas_20230120_models.ListUserGroupsRequest,
+        request: csas_20230120_models.ListUserGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListUserGroupsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_group_ids):
-            request.user_group_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_group_ids, 'UserGroupIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroups',
             version='2023-01-20',
@@ -1925,22 +1831,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListUserGroupsResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_user_groups_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListUserGroupsRequest,
+        request: csas_20230120_models.ListUserGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListUserGroupsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_group_ids):
-            request.user_group_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_group_ids, 'UserGroupIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroups',
             version='2023-01-20',
@@ -1969,22 +1871,18 @@
         request: csas_20230120_models.ListUserGroupsRequest,
     ) -> csas_20230120_models.ListUserGroupsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_user_groups_with_options_async(request, runtime)
 
     def list_user_groups_for_private_access_policy_with_options(
         self,
-        tmp_req: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
+        request: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsForPrivateAccessPolicyResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListUserGroupsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroupsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -1999,22 +1897,18 @@
         return TeaCore.from_map(
             csas_20230120_models.ListUserGroupsForPrivateAccessPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_user_groups_for_private_access_policy_with_options_async(
         self,
-        tmp_req: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
+        request: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsForPrivateAccessPolicyResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListUserGroupsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroupsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -2291,31 +2185,30 @@
         request: csas_20230120_models.UpdatePrivateAccessPolicyRequest,
     ) -> csas_20230120_models.UpdatePrivateAccessPolicyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.update_private_access_policy_with_options_async(request, runtime)
 
     def update_user_group_with_options(
         self,
-        tmp_req: csas_20230120_models.UpdateUserGroupRequest,
+        request: csas_20230120_models.UpdateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserGroupResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.UpdateUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.attributes):
-            request.attributes_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.attributes, 'Attributes', 'json')
+        UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.attributes_shrink):
-            body['Attributes'] = request.attributes_shrink
+        body_flat = {}
+        if not UtilClient.is_unset(request.attributes):
+            body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.modify_type):
             body['ModifyType'] = request.modify_type
         if not UtilClient.is_unset(request.user_group_id):
             body['UserGroupId'] = request.user_group_id
+        body = TeaCore.merge(body,
+            OpenApiUtilClient.query(body_flat))
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateUserGroup',
             version='2023-01-20',
             protocol='HTTPS',
@@ -2329,31 +2222,30 @@
         return TeaCore.from_map(
             csas_20230120_models.UpdateUserGroupResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def update_user_group_with_options_async(
         self,
-        tmp_req: csas_20230120_models.UpdateUserGroupRequest,
+        request: csas_20230120_models.UpdateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserGroupResponse:
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.UpdateUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.attributes):
-            request.attributes_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.attributes, 'Attributes', 'json')
+        UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.attributes_shrink):
-            body['Attributes'] = request.attributes_shrink
+        body_flat = {}
+        if not UtilClient.is_unset(request.attributes):
+            body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.modify_type):
             body['ModifyType'] = request.modify_type
         if not UtilClient.is_unset(request.user_group_id):
             body['UserGroupId'] = request.user_group_id
+        body = TeaCore.merge(body,
+            OpenApiUtilClient.query(body_flat))
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='UpdateUserGroup',
             version='2023-01-20',
             protocol='HTTPS',
```

### Comparing `alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120/models.py` & `alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,16 +451,20 @@
         self.application_type = application_type
         self.custom_user_attributes = custom_user_attributes
         self.description = description
         self.name = name
         self.policy_action = policy_action
         self.priority = priority
         self.status = status
+        # 内网访问标签ID集合。最多可输入100个内网访问标签ID。当**ApplicationType**为**Tag时**，必填。和**ApplicationIds**互斥。
         self.tag_ids = tag_ids
         self.user_group_ids = user_group_ids
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode
 
     def validate(self):
         if self.custom_user_attributes:
             for k in self.custom_user_attributes:
                 if k:
                     k.validate()
@@ -546,16 +550,20 @@
         self.application_type = application_type
         self.custom_user_attributes_shrink = custom_user_attributes_shrink
         self.description = description
         self.name = name
         self.policy_action = policy_action
         self.priority = priority
         self.status = status
+        # 内网访问标签ID集合。最多可输入100个内网访问标签ID。当**ApplicationType**为**Tag时**，必填。和**ApplicationIds**互斥。
         self.tag_ids_shrink = tag_ids_shrink
         self.user_group_ids_shrink = user_group_ids_shrink
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -889,53 +897,14 @@
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
-class CreateUserGroupShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        attributes_shrink: str = None,
-        description: str = None,
-        name: str = None,
-    ):
-        self.attributes_shrink = attributes_shrink
-        self.description = description
-        self.name = name
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.attributes_shrink is not None:
-            result['Attributes'] = self.attributes_shrink
-        if self.description is not None:
-            result['Description'] = self.description
-        if self.name is not None:
-            result['Name'] = self.name
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Attributes') is not None:
-            self.attributes_shrink = m.get('Attributes')
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        return self
-
-
 class CreateUserGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         user_group_id: str = None,
     ):
         self.request_id = request_id
@@ -2259,41 +2228,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         return self
 
 
-class ListApplicationsForPrivateAccessPolicyShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        policy_ids_shrink: str = None,
-    ):
-        self.policy_ids_shrink = policy_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.policy_ids_shrink is not None:
-            result['PolicyIds'] = self.policy_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('PolicyIds') is not None:
-            self.policy_ids_shrink = m.get('PolicyIds')
-        return self
-
-
 class ListApplicationsForPrivateAccessPolicyResponseBodyPolicesApplicationsPortRanges(TeaModel):
     def __init__(
         self,
         begin: int = None,
         end: int = None,
     ):
         self.begin = begin
@@ -2549,41 +2491,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('TagIds') is not None:
             self.tag_ids = m.get('TagIds')
         return self
 
 
-class ListApplicationsForPrivateAccessTagShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        tag_ids_shrink: str = None,
-    ):
-        self.tag_ids_shrink = tag_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.tag_ids_shrink is not None:
-            result['TagIds'] = self.tag_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('TagIds') is not None:
-            self.tag_ids_shrink = m.get('TagIds')
-        return self
-
-
 class ListApplicationsForPrivateAccessTagResponseBodyTagsApplicationsPortRanges(TeaModel):
     def __init__(
         self,
         begin: int = None,
         end: int = None,
     ):
         self.begin = begin
@@ -2623,14 +2538,15 @@
         name: str = None,
         port_ranges: List[ListApplicationsForPrivateAccessTagResponseBodyTagsApplicationsPortRanges] = None,
         protocol: str = None,
         status: str = None,
     ):
         self.addresses = addresses
         self.application_id = application_id
+        # 内网访问应用创建时间。
         self.create_time = create_time
         self.description = description
         self.name = name
         self.port_ranges = port_ranges
         self.protocol = protocol
         self.status = status
 
@@ -2819,19 +2735,23 @@
 class ListConnectorsRequest(TeaModel):
     def __init__(
         self,
         connector_ids: List[str] = None,
         current_page: int = None,
         name: str = None,
         page_size: int = None,
+        status: str = None,
+        switch_status: str = None,
     ):
         self.connector_ids = connector_ids
         self.current_page = current_page
         self.name = name
         self.page_size = page_size
+        self.status = status
+        self.switch_status = switch_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -2842,71 +2762,34 @@
             result['ConnectorIds'] = self.connector_ids
         if self.current_page is not None:
             result['CurrentPage'] = self.current_page
         if self.name is not None:
             result['Name'] = self.name
         if self.page_size is not None:
             result['PageSize'] = self.page_size
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.switch_status is not None:
+            result['SwitchStatus'] = self.switch_status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ConnectorIds') is not None:
             self.connector_ids = m.get('ConnectorIds')
         if m.get('CurrentPage') is not None:
             self.current_page = m.get('CurrentPage')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
-        return self
-
-
-class ListConnectorsShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        connector_ids_shrink: str = None,
-        current_page: int = None,
-        name: str = None,
-        page_size: int = None,
-    ):
-        self.connector_ids_shrink = connector_ids_shrink
-        self.current_page = current_page
-        self.name = name
-        self.page_size = page_size
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.connector_ids_shrink is not None:
-            result['ConnectorIds'] = self.connector_ids_shrink
-        if self.current_page is not None:
-            result['CurrentPage'] = self.current_page
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ConnectorIds') is not None:
-            self.connector_ids_shrink = m.get('ConnectorIds')
-        if m.get('CurrentPage') is not None:
-            self.current_page = m.get('CurrentPage')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('SwitchStatus') is not None:
+            self.switch_status = m.get('SwitchStatus')
         return self
 
 
 class ListConnectorsResponseBodyConnectorsApplications(TeaModel):
     def __init__(
         self,
         application_id: str = None,
@@ -3167,41 +3050,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApplicationIds') is not None:
             self.application_ids = m.get('ApplicationIds')
         return self
 
 
-class ListPolicesForPrivateAccessApplicationShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        application_ids_shrink: str = None,
-    ):
-        self.application_ids_shrink = application_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.application_ids_shrink is not None:
-            result['ApplicationIds'] = self.application_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ApplicationIds') is not None:
-            self.application_ids_shrink = m.get('ApplicationIds')
-        return self
-
-
 class ListPolicesForPrivateAccessApplicationResponseBodyApplicationsPoliciesCustomUserAttributes(TeaModel):
     def __init__(
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
@@ -3481,52 +3337,39 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('TagIds') is not None:
             self.tag_ids = m.get('TagIds')
         return self
 
 
-class ListPolicesForPrivateAccessTagShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        tag_ids_shrink: str = None,
-    ):
-        self.tag_ids_shrink = tag_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.tag_ids_shrink is not None:
-            result['TagIds'] = self.tag_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('TagIds') is not None:
-            self.tag_ids_shrink = m.get('TagIds')
-        return self
-
-
 class ListPolicesForPrivateAccessTagResponseBodyTagsPolicesCustomUserAttributes(TeaModel):
     def __init__(
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
     ):
+        # 用户组的身份源ID。当自定义用户组类型为**department**时，存在该值。
         self.idp_id = idp_id
+        # 用户组的关系。取值：
+        # - **Equal**：等于。
+        # - **Unequal**：不等于。
         self.relation = relation
+        # 用户组的类型。取值：
+        # - **username**：用户名。
+        # - **department**：部门。
+        # - **email**：邮箱。
+        # - **telephone**：手机。
         self.user_group_type = user_group_type
+        # 用户组属性的值。
+        # - 当用户组类型为**username**时，表示用户名的值。长度为1~128个字符，支持中文和大小写英文字母，可包含数字、半角句号（.）、下划线（_）和短划线（-）。
+        # - 当用户组类型为**department**时，表示部门的值。如：OU=部门1,OU=SASE钉钉。
+        # - 当用户组类型为**email**时，表示邮箱的值。如：username@example.com。
+        # - 当用户组类型为**telephone**时，表示手机的值。如：13900001234。
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3568,15 +3411,17 @@
         policy_action: str = None,
         policy_id: str = None,
         priority: int = None,
         status: str = None,
         user_group_type: str = None,
     ):
         self.application_type = application_type
+        # 内网访问策略创建时间。
         self.create_time = create_time
+        # 自定义用户组属性集合。多个自定义用户组属性之间是或的关系，按照合集生效。
         self.custom_user_attributes = custom_user_attributes
         self.description = description
         self.name = name
         self.policy_action = policy_action
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
@@ -3795,41 +3640,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('UserGroupIds') is not None:
             self.user_group_ids = m.get('UserGroupIds')
         return self
 
 
-class ListPolicesForUserGroupShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        user_group_ids_shrink: str = None,
-    ):
-        self.user_group_ids_shrink = user_group_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.user_group_ids_shrink is not None:
-            result['UserGroupIds'] = self.user_group_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('UserGroupIds') is not None:
-            self.user_group_ids_shrink = m.get('UserGroupIds')
-        return self
-
-
 class ListPolicesForUserGroupResponseBodyUserGroupsPolices(TeaModel):
     def __init__(
         self,
         name: str = None,
         policy_id: str = None,
         policy_type: str = None,
     ):
@@ -4056,83 +3874,14 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
         return self
 
 
-class ListPrivateAccessApplicationsShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        address: str = None,
-        application_ids_shrink: str = None,
-        current_page: int = None,
-        name: str = None,
-        page_size: int = None,
-        policy_id: str = None,
-        status: str = None,
-        tag_id: str = None,
-    ):
-        self.address = address
-        self.application_ids_shrink = application_ids_shrink
-        self.current_page = current_page
-        self.name = name
-        self.page_size = page_size
-        self.policy_id = policy_id
-        self.status = status
-        self.tag_id = tag_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.address is not None:
-            result['Address'] = self.address
-        if self.application_ids_shrink is not None:
-            result['ApplicationIds'] = self.application_ids_shrink
-        if self.current_page is not None:
-            result['CurrentPage'] = self.current_page
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.policy_id is not None:
-            result['PolicyId'] = self.policy_id
-        if self.status is not None:
-            result['Status'] = self.status
-        if self.tag_id is not None:
-            result['TagId'] = self.tag_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Address') is not None:
-            self.address = m.get('Address')
-        if m.get('ApplicationIds') is not None:
-            self.application_ids_shrink = m.get('ApplicationIds')
-        if m.get('CurrentPage') is not None:
-            self.current_page = m.get('CurrentPage')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('PolicyId') is not None:
-            self.policy_id = m.get('PolicyId')
-        if m.get('Status') is not None:
-            self.status = m.get('Status')
-        if m.get('TagId') is not None:
-            self.tag_id = m.get('TagId')
-        return self
-
-
 class ListPrivateAccessApplicationsResponseBodyApplicationsPortRanges(TeaModel):
     def __init__(
         self,
         begin: int = None,
         end: int = None,
     ):
         self.begin = begin
@@ -4359,14 +4108,17 @@
         self.current_page = current_page
         self.name = name
         self.page_size = page_size
         self.policy_action = policy_action
         self.policy_ids = policy_ids
         self.status = status
         self.tag_id = tag_id
+        # 用户组ID。取值来源：
+        # - [ListUserGroups](~~ListUserGroups~~)：批量查询用户组。
+        # - [CreateUserGroup](~~CreateUserGroup~~)：创建用户组。
         self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4413,89 +4165,14 @@
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
 
 
-class ListPrivateAccessPolicesShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        application_id: str = None,
-        current_page: int = None,
-        name: str = None,
-        page_size: int = None,
-        policy_action: str = None,
-        policy_ids_shrink: str = None,
-        status: str = None,
-        tag_id: str = None,
-        user_group_id: str = None,
-    ):
-        self.application_id = application_id
-        self.current_page = current_page
-        self.name = name
-        self.page_size = page_size
-        self.policy_action = policy_action
-        self.policy_ids_shrink = policy_ids_shrink
-        self.status = status
-        self.tag_id = tag_id
-        self.user_group_id = user_group_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.application_id is not None:
-            result['ApplicationId'] = self.application_id
-        if self.current_page is not None:
-            result['CurrentPage'] = self.current_page
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.policy_action is not None:
-            result['PolicyAction'] = self.policy_action
-        if self.policy_ids_shrink is not None:
-            result['PolicyIds'] = self.policy_ids_shrink
-        if self.status is not None:
-            result['Status'] = self.status
-        if self.tag_id is not None:
-            result['TagId'] = self.tag_id
-        if self.user_group_id is not None:
-            result['UserGroupId'] = self.user_group_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ApplicationId') is not None:
-            self.application_id = m.get('ApplicationId')
-        if m.get('CurrentPage') is not None:
-            self.current_page = m.get('CurrentPage')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('PolicyAction') is not None:
-            self.policy_action = m.get('PolicyAction')
-        if m.get('PolicyIds') is not None:
-            self.policy_ids_shrink = m.get('PolicyIds')
-        if m.get('Status') is not None:
-            self.status = m.get('Status')
-        if m.get('TagId') is not None:
-            self.tag_id = m.get('TagId')
-        if m.get('UserGroupId') is not None:
-            self.user_group_id = m.get('UserGroupId')
-        return self
-
-
 class ListPrivateAccessPolicesResponseBodyPolicesCustomUserAttributes(TeaModel):
     def __init__(
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
@@ -4788,71 +4465,14 @@
         if m.get('PolicyId') is not None:
             self.policy_id = m.get('PolicyId')
         if m.get('TagIds') is not None:
             self.tag_ids = m.get('TagIds')
         return self
 
 
-class ListPrivateAccessTagsShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        application_id: str = None,
-        current_page: int = None,
-        name: str = None,
-        page_size: int = None,
-        policy_id: str = None,
-        tag_ids_shrink: str = None,
-    ):
-        self.application_id = application_id
-        self.current_page = current_page
-        self.name = name
-        self.page_size = page_size
-        self.policy_id = policy_id
-        self.tag_ids_shrink = tag_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.application_id is not None:
-            result['ApplicationId'] = self.application_id
-        if self.current_page is not None:
-            result['CurrentPage'] = self.current_page
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.policy_id is not None:
-            result['PolicyId'] = self.policy_id
-        if self.tag_ids_shrink is not None:
-            result['TagIds'] = self.tag_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ApplicationId') is not None:
-            self.application_id = m.get('ApplicationId')
-        if m.get('CurrentPage') is not None:
-            self.current_page = m.get('CurrentPage')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('PolicyId') is not None:
-            self.policy_id = m.get('PolicyId')
-        if m.get('TagIds') is not None:
-            self.tag_ids_shrink = m.get('TagIds')
-        return self
-
-
 class ListPrivateAccessTagsResponseBodyTags(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
         create_time: str = None,
         description: str = None,
         name: str = None,
@@ -5026,41 +4646,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApplicationIds') is not None:
             self.application_ids = m.get('ApplicationIds')
         return self
 
 
-class ListTagsForPrivateAccessApplicationShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        application_ids_shrink: str = None,
-    ):
-        self.application_ids_shrink = application_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.application_ids_shrink is not None:
-            result['ApplicationIds'] = self.application_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('ApplicationIds') is not None:
-            self.application_ids_shrink = m.get('ApplicationIds')
-        return self
-
-
 class ListTagsForPrivateAccessApplicationResponseBodyApplicationsTags(TeaModel):
     def __init__(
         self,
         create_time: str = None,
         description: str = None,
         name: str = None,
         tag_id: str = None,
@@ -5257,50 +4850,24 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         return self
 
 
-class ListTagsForPrivateAccessPolicyShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        policy_ids_shrink: str = None,
-    ):
-        self.policy_ids_shrink = policy_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.policy_ids_shrink is not None:
-            result['PolicyIds'] = self.policy_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('PolicyIds') is not None:
-            self.policy_ids_shrink = m.get('PolicyIds')
-        return self
-
-
 class ListTagsForPrivateAccessPolicyResponseBodyPolicesTags(TeaModel):
     def __init__(
         self,
         create_time: str = None,
         description: str = None,
         name: str = None,
         tag_id: str = None,
         tag_type: str = None,
     ):
+        # 内网访问标签创建时间。
         self.create_time = create_time
         self.description = description
         self.name = name
         self.tag_id = tag_id
         self.tag_type = tag_type
 
     def validate(self):
@@ -5473,14 +5040,15 @@
         name: str = None,
         papolicy_id: str = None,
         page_size: int = None,
         user_group_ids: List[str] = None,
     ):
         self.attribute_value = attribute_value
         self.current_page = current_page
+        # 用户组名称。长度为1~128个字符，支持中文和大小写英文字母，可包含数字、半角句号（.）、下划线（_）和短划线（-）。
         self.name = name
         self.papolicy_id = papolicy_id
         self.page_size = page_size
         self.user_group_ids = user_group_ids
 
     def validate(self):
         pass
@@ -5518,71 +5086,14 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('UserGroupIds') is not None:
             self.user_group_ids = m.get('UserGroupIds')
         return self
 
 
-class ListUserGroupsShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        attribute_value: str = None,
-        current_page: int = None,
-        name: str = None,
-        papolicy_id: str = None,
-        page_size: int = None,
-        user_group_ids_shrink: str = None,
-    ):
-        self.attribute_value = attribute_value
-        self.current_page = current_page
-        self.name = name
-        self.papolicy_id = papolicy_id
-        self.page_size = page_size
-        self.user_group_ids_shrink = user_group_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.attribute_value is not None:
-            result['AttributeValue'] = self.attribute_value
-        if self.current_page is not None:
-            result['CurrentPage'] = self.current_page
-        if self.name is not None:
-            result['Name'] = self.name
-        if self.papolicy_id is not None:
-            result['PAPolicyId'] = self.papolicy_id
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.user_group_ids_shrink is not None:
-            result['UserGroupIds'] = self.user_group_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('AttributeValue') is not None:
-            self.attribute_value = m.get('AttributeValue')
-        if m.get('CurrentPage') is not None:
-            self.current_page = m.get('CurrentPage')
-        if m.get('Name') is not None:
-            self.name = m.get('Name')
-        if m.get('PAPolicyId') is not None:
-            self.papolicy_id = m.get('PAPolicyId')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('UserGroupIds') is not None:
-            self.user_group_ids_shrink = m.get('UserGroupIds')
-        return self
-
-
 class ListUserGroupsResponseBodyUserGroupsAttributes(TeaModel):
     def __init__(
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
@@ -5797,41 +5308,14 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         return self
 
 
-class ListUserGroupsForPrivateAccessPolicyShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        policy_ids_shrink: str = None,
-    ):
-        self.policy_ids_shrink = policy_ids_shrink
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.policy_ids_shrink is not None:
-            result['PolicyIds'] = self.policy_ids_shrink
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('PolicyIds') is not None:
-            self.policy_ids_shrink = m.get('PolicyIds')
-        return self
-
-
 class ListUserGroupsForPrivateAccessPolicyResponseBodyPolicesUserGroupsAttributes(TeaModel):
     def __init__(
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
@@ -5879,14 +5363,15 @@
         attributes: List[ListUserGroupsForPrivateAccessPolicyResponseBodyPolicesUserGroupsAttributes] = None,
         create_time: str = None,
         description: str = None,
         name: str = None,
         user_group_id: str = None,
     ):
         self.attributes = attributes
+        # 用户组创建时间。
         self.create_time = create_time
         self.description = description
         self.name = name
         self.user_group_id = user_group_id
 
     def validate(self):
         if self.attributes:
@@ -6374,16 +5859,20 @@
         self.custom_user_attributes = custom_user_attributes
         self.description = description
         self.modify_type = modify_type
         self.policy_action = policy_action
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
+        # 内网访问标签ID集合。一条策略最多支持100个内网访问标签ID。
         self.tag_ids = tag_ids
         self.user_group_ids = user_group_ids
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode
 
     def validate(self):
         if self.custom_user_attributes:
             for k in self.custom_user_attributes:
                 if k:
                     k.validate()
@@ -6475,16 +5964,20 @@
         self.custom_user_attributes_shrink = custom_user_attributes_shrink
         self.description = description
         self.modify_type = modify_type
         self.policy_action = policy_action
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
+        # 内网访问标签ID集合。一条策略最多支持100个内网访问标签ID。
         self.tag_ids_shrink = tag_ids_shrink
         self.user_group_ids_shrink = user_group_ids_shrink
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6710,59 +6203,14 @@
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('ModifyType') is not None:
             self.modify_type = m.get('ModifyType')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
-
-
-class UpdateUserGroupShrinkRequest(TeaModel):
-    def __init__(
-        self,
-        attributes_shrink: str = None,
-        description: str = None,
-        modify_type: str = None,
-        user_group_id: str = None,
-    ):
-        self.attributes_shrink = attributes_shrink
-        self.description = description
-        self.modify_type = modify_type
-        self.user_group_id = user_group_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.attributes_shrink is not None:
-            result['Attributes'] = self.attributes_shrink
-        if self.description is not None:
-            result['Description'] = self.description
-        if self.modify_type is not None:
-            result['ModifyType'] = self.modify_type
-        if self.user_group_id is not None:
-            result['UserGroupId'] = self.user_group_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Attributes') is not None:
-            self.attributes_shrink = m.get('Attributes')
-        if m.get('Description') is not None:
-            self.description = m.get('Description')
-        if m.get('ModifyType') is not None:
-            self.modify_type = m.get('ModifyType')
-        if m.get('UserGroupId') is not None:
-            self.user_group_id = m.get('UserGroupId')
-        return self
 
 
 class UpdateUserGroupResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
```

### Comparing `alibabacloud_csas20230120-1.0.0/alibabacloud_csas20230120.egg-info/PKG-INFO` & `alibabacloud_csas20230120-1.0.1/alibabacloud_csas20230120.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-csas20230120
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120-1.0.0/setup.py` & `alibabacloud_csas20230120-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_csas20230120.
 
-Created on 24/03/2023
+Created on 12/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_csas20230120"
 NAME = "alibabacloud_csas20230120" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud csas (20230120) SDK Library for Python"
```

