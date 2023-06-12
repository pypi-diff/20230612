# Comparing `tmp/alibabacloud_csas20230120_py2-1.0.0.tar.gz` & `tmp/alibabacloud_csas20230120_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_csas20230120_py2-1.0.0.tar", last modified: Fri Mar 24 01:58:50 2023, max compression
+gzip compressed data, was "dist/alibabacloud_csas20230120_py2-1.0.1.tar", last modified: Mon Jun 12 05:58:16 2023, max compression
```

## Comparing `alibabacloud_csas20230120_py2-1.0.0.tar` & `alibabacloud_csas20230120_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44274 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120/client.py
--rw-r--r--   0 root         (0) root         (0)   220488 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-03-24 01:58:50.000000 alibabacloud_csas20230120_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39518 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120/client.py
+-rw-r--r--   0 root         (0) root         (0)   205134 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-12 05:58:16.000000 alibabacloud_csas20230120_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_csas20230120_py2-1.0.0/LICENSE` & `alibabacloud_csas20230120_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.0.0/PKG-INFO` & `alibabacloud_csas20230120_py2-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_csas20230120_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120_py2-1.0.0/README-CN.md` & `alibabacloud_csas20230120_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.0.0/README.md` & `alibabacloud_csas20230120_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120/client.py` & `alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -196,27 +196,26 @@
             self.call_api(params, req, runtime)
         )
 
     def create_private_access_tag(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_private_access_tag_with_options(request, runtime)
 
-    def create_user_group_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.CreateUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.attributes):
-            request.attributes_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.attributes, 'Attributes', 'json')
+    def create_user_group_with_options(self, request, runtime):
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
@@ -456,20 +455,16 @@
             self.call_api(params, req, runtime)
         )
 
     def get_user_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_user_group_with_options(request, runtime)
 
-    def list_applications_for_private_access_policy_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListApplicationsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+    def list_applications_for_private_access_policy_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -486,20 +481,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_applications_for_private_access_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_applications_for_private_access_policy_with_options(request, runtime)
 
-    def list_applications_for_private_access_tag_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListApplicationsForPrivateAccessTagShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+    def list_applications_for_private_access_tag_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessTag',
             version='2023-01-20',
@@ -516,20 +507,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_applications_for_private_access_tag(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_applications_for_private_access_tag_with_options(request, runtime)
 
-    def list_connectors_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListConnectorsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.connector_ids):
-            request.connector_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.connector_ids, 'ConnectorIds', 'json')
+    def list_connectors_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListConnectors',
             version='2023-01-20',
@@ -546,20 +533,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_connectors(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_connectors_with_options(request, runtime)
 
-    def list_polices_for_private_access_application_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForPrivateAccessApplicationShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+    def list_polices_for_private_access_application_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessApplication',
             version='2023-01-20',
@@ -576,20 +559,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_polices_for_private_access_application(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_polices_for_private_access_application_with_options(request, runtime)
 
-    def list_polices_for_private_access_tag_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForPrivateAccessTagShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+    def list_polices_for_private_access_tag_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessTag',
             version='2023-01-20',
@@ -606,20 +585,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_polices_for_private_access_tag(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_polices_for_private_access_tag_with_options(request, runtime)
 
-    def list_polices_for_user_group_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPolicesForUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_group_ids):
-            request.user_group_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_group_ids, 'UserGroupIds', 'json')
+    def list_polices_for_user_group_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForUserGroup',
             version='2023-01-20',
@@ -636,20 +611,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_polices_for_user_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_polices_for_user_group_with_options(request, runtime)
 
-    def list_private_access_applications_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessApplicationsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+    def list_private_access_applications_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessApplications',
             version='2023-01-20',
@@ -666,20 +637,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_private_access_applications(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_applications_with_options(request, runtime)
 
-    def list_private_access_polices_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessPolicesShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+    def list_private_access_polices_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessPolices',
             version='2023-01-20',
@@ -696,20 +663,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_private_access_polices(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_polices_with_options(request, runtime)
 
-    def list_private_access_tags_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListPrivateAccessTagsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.tag_ids):
-            request.tag_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tag_ids, 'TagIds', 'json')
+    def list_private_access_tags_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessTags',
             version='2023-01-20',
@@ -726,20 +689,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_private_access_tags(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_tags_with_options(request, runtime)
 
-    def list_tags_for_private_access_application_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListTagsForPrivateAccessApplicationShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.application_ids):
-            request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
+    def list_tags_for_private_access_application_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessApplication',
             version='2023-01-20',
@@ -756,20 +715,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_tags_for_private_access_application(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_tags_for_private_access_application_with_options(request, runtime)
 
-    def list_tags_for_private_access_policy_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListTagsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+    def list_tags_for_private_access_policy_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -786,20 +741,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_tags_for_private_access_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_tags_for_private_access_policy_with_options(request, runtime)
 
-    def list_user_groups_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListUserGroupsShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.user_group_ids):
-            request.user_group_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_group_ids, 'UserGroupIds', 'json')
+    def list_user_groups_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroups',
             version='2023-01-20',
@@ -816,20 +767,16 @@
             self.call_api(params, req, runtime)
         )
 
     def list_user_groups(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_user_groups_with_options(request, runtime)
 
-    def list_user_groups_for_private_access_policy_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.ListUserGroupsForPrivateAccessPolicyShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.policy_ids):
-            request.policy_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.policy_ids, 'PolicyIds', 'json')
+    def list_user_groups_for_private_access_policy_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroupsForPrivateAccessPolicy',
             version='2023-01-20',
@@ -956,29 +903,28 @@
             self.call_api(params, req, runtime)
         )
 
     def update_private_access_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.update_private_access_policy_with_options(request, runtime)
 
-    def update_user_group_with_options(self, tmp_req, runtime):
-        UtilClient.validate_model(tmp_req)
-        request = csas_20230120_models.UpdateUserGroupShrinkRequest()
-        OpenApiUtilClient.convert(tmp_req, request)
-        if not UtilClient.is_unset(tmp_req.attributes):
-            request.attributes_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.attributes, 'Attributes', 'json')
+    def update_user_group_with_options(self, request, runtime):
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

### Comparing `alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120/models.py` & `alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,16 +388,20 @@
         self.application_type = application_type  # type: str
         self.custom_user_attributes = custom_user_attributes  # type: list[CreatePrivateAccessPolicyRequestCustomUserAttributes]
         self.description = description  # type: str
         self.name = name  # type: str
         self.policy_action = policy_action  # type: str
         self.priority = priority  # type: int
         self.status = status  # type: str
+        # 内网访问标签ID集合。最多可输入100个内网访问标签ID。当**ApplicationType**为**Tag时**，必填。和**ApplicationIds**互斥。
         self.tag_ids = tag_ids  # type: list[str]
         self.user_group_ids = user_group_ids  # type: list[str]
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode  # type: str
 
     def validate(self):
         if self.custom_user_attributes:
             for k in self.custom_user_attributes:
                 if k:
                     k.validate()
@@ -472,16 +476,20 @@
         self.application_type = application_type  # type: str
         self.custom_user_attributes_shrink = custom_user_attributes_shrink  # type: str
         self.description = description  # type: str
         self.name = name  # type: str
         self.policy_action = policy_action  # type: str
         self.priority = priority  # type: int
         self.status = status  # type: str
+        # 内网访问标签ID集合。最多可输入100个内网访问标签ID。当**ApplicationType**为**Tag时**，必填。和**ApplicationIds**互斥。
         self.tag_ids_shrink = tag_ids_shrink  # type: str
         self.user_group_ids_shrink = user_group_ids_shrink  # type: str
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreatePrivateAccessPolicyShrinkRequest, self).to_map()
@@ -782,48 +790,14 @@
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         return self
 
 
-class CreateUserGroupShrinkRequest(TeaModel):
-    def __init__(self, attributes_shrink=None, description=None, name=None):
-        self.attributes_shrink = attributes_shrink  # type: str
-        self.description = description  # type: str
-        self.name = name  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(CreateUserGroupShrinkRequest, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, request_id=None, user_group_id=None):
         self.request_id = request_id  # type: str
         self.user_group_id = user_group_id  # type: str
 
     def validate(self):
         pass
@@ -1992,38 +1966,14 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         return self
 
 
-class ListApplicationsForPrivateAccessPolicyShrinkRequest(TeaModel):
-    def __init__(self, policy_ids_shrink=None):
-        self.policy_ids_shrink = policy_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListApplicationsForPrivateAccessPolicyShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.policy_ids_shrink is not None:
-            result['PolicyIds'] = self.policy_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('PolicyIds') is not None:
-            self.policy_ids_shrink = m.get('PolicyIds')
-        return self
-
-
 class ListApplicationsForPrivateAccessPolicyResponseBodyPolicesApplicationsPortRanges(TeaModel):
     def __init__(self, begin=None, end=None):
         self.begin = begin  # type: int
         self.end = end  # type: int
 
     def validate(self):
         pass
@@ -2250,38 +2200,14 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('TagIds') is not None:
             self.tag_ids = m.get('TagIds')
         return self
 
 
-class ListApplicationsForPrivateAccessTagShrinkRequest(TeaModel):
-    def __init__(self, tag_ids_shrink=None):
-        self.tag_ids_shrink = tag_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListApplicationsForPrivateAccessTagShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.tag_ids_shrink is not None:
-            result['TagIds'] = self.tag_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('TagIds') is not None:
-            self.tag_ids_shrink = m.get('TagIds')
-        return self
-
-
 class ListApplicationsForPrivateAccessTagResponseBodyTagsApplicationsPortRanges(TeaModel):
     def __init__(self, begin=None, end=None):
         self.begin = begin  # type: int
         self.end = end  # type: int
 
     def validate(self):
         pass
@@ -2308,14 +2234,15 @@
 
 
 class ListApplicationsForPrivateAccessTagResponseBodyTagsApplications(TeaModel):
     def __init__(self, addresses=None, application_id=None, create_time=None, description=None, name=None,
                  port_ranges=None, protocol=None, status=None):
         self.addresses = addresses  # type: list[str]
         self.application_id = application_id  # type: str
+        # 内网访问应用创建时间。
         self.create_time = create_time  # type: str
         self.description = description  # type: str
         self.name = name  # type: str
         self.port_ranges = port_ranges  # type: list[ListApplicationsForPrivateAccessTagResponseBodyTagsApplicationsPortRanges]
         self.protocol = protocol  # type: str
         self.status = status  # type: str
 
@@ -2485,19 +2412,22 @@
         if m.get('body') is not None:
             temp_model = ListApplicationsForPrivateAccessTagResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListConnectorsRequest(TeaModel):
-    def __init__(self, connector_ids=None, current_page=None, name=None, page_size=None):
+    def __init__(self, connector_ids=None, current_page=None, name=None, page_size=None, status=None,
+                 switch_status=None):
         self.connector_ids = connector_ids  # type: list[str]
         self.current_page = current_page  # type: int
         self.name = name  # type: str
         self.page_size = page_size  # type: int
+        self.status = status  # type: str
+        self.switch_status = switch_status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListConnectorsRequest, self).to_map()
         if _map is not None:
@@ -2508,65 +2438,34 @@
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
 
     def from_map(self, m=None):
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
-    def __init__(self, connector_ids_shrink=None, current_page=None, name=None, page_size=None):
-        self.connector_ids_shrink = connector_ids_shrink  # type: str
-        self.current_page = current_page  # type: int
-        self.name = name  # type: str
-        self.page_size = page_size  # type: int
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListConnectorsShrinkRequest, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, application_id=None, application_name=None):
         self.application_id = application_id  # type: str
         self.application_name = application_name  # type: str
@@ -2797,38 +2696,14 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ApplicationIds') is not None:
             self.application_ids = m.get('ApplicationIds')
         return self
 
 
-class ListPolicesForPrivateAccessApplicationShrinkRequest(TeaModel):
-    def __init__(self, application_ids_shrink=None):
-        self.application_ids_shrink = application_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListPolicesForPrivateAccessApplicationShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.application_ids_shrink is not None:
-            result['ApplicationIds'] = self.application_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ApplicationIds') is not None:
-            self.application_ids_shrink = m.get('ApplicationIds')
-        return self
-
-
 class ListPolicesForPrivateAccessApplicationResponseBodyApplicationsPoliciesCustomUserAttributes(TeaModel):
     def __init__(self, idp_id=None, relation=None, user_group_type=None, value=None):
         self.idp_id = idp_id  # type: int
         self.relation = relation  # type: str
         self.user_group_type = user_group_type  # type: str
         self.value = value  # type: str
 
@@ -3075,43 +2950,33 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('TagIds') is not None:
             self.tag_ids = m.get('TagIds')
         return self
 
 
-class ListPolicesForPrivateAccessTagShrinkRequest(TeaModel):
-    def __init__(self, tag_ids_shrink=None):
-        self.tag_ids_shrink = tag_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListPolicesForPrivateAccessTagShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.tag_ids_shrink is not None:
-            result['TagIds'] = self.tag_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('TagIds') is not None:
-            self.tag_ids_shrink = m.get('TagIds')
-        return self
-
-
 class ListPolicesForPrivateAccessTagResponseBodyTagsPolicesCustomUserAttributes(TeaModel):
     def __init__(self, idp_id=None, relation=None, user_group_type=None, value=None):
+        # 用户组的身份源ID。当自定义用户组类型为**department**时，存在该值。
         self.idp_id = idp_id  # type: int
+        # 用户组的关系。取值：
+        # - **Equal**：等于。
+        # - **Unequal**：不等于。
         self.relation = relation  # type: str
+        # 用户组的类型。取值：
+        # - **username**：用户名。
+        # - **department**：部门。
+        # - **email**：邮箱。
+        # - **telephone**：手机。
         self.user_group_type = user_group_type  # type: str
+        # 用户组属性的值。
+        # - 当用户组类型为**username**时，表示用户名的值。长度为1~128个字符，支持中文和大小写英文字母，可包含数字、半角句号（.）、下划线（_）和短划线（-）。
+        # - 当用户组类型为**department**时，表示部门的值。如：OU=部门1,OU=SASE钉钉。
+        # - 当用户组类型为**email**时，表示邮箱的值。如：username@example.com。
+        # - 当用户组类型为**telephone**时，表示手机的值。如：13900001234。
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListPolicesForPrivateAccessTagResponseBodyTagsPolicesCustomUserAttributes, self).to_map()
@@ -3142,15 +3007,17 @@
         return self
 
 
 class ListPolicesForPrivateAccessTagResponseBodyTagsPolices(TeaModel):
     def __init__(self, application_type=None, create_time=None, custom_user_attributes=None, description=None,
                  name=None, policy_action=None, policy_id=None, priority=None, status=None, user_group_type=None):
         self.application_type = application_type  # type: str
+        # 内网访问策略创建时间。
         self.create_time = create_time  # type: str
+        # 自定义用户组属性集合。多个自定义用户组属性之间是或的关系，按照合集生效。
         self.custom_user_attributes = custom_user_attributes  # type: list[ListPolicesForPrivateAccessTagResponseBodyTagsPolicesCustomUserAttributes]
         self.description = description  # type: str
         self.name = name  # type: str
         self.policy_action = policy_action  # type: str
         self.policy_id = policy_id  # type: str
         self.priority = priority  # type: int
         self.status = status  # type: str
@@ -3353,38 +3220,14 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('UserGroupIds') is not None:
             self.user_group_ids = m.get('UserGroupIds')
         return self
 
 
-class ListPolicesForUserGroupShrinkRequest(TeaModel):
-    def __init__(self, user_group_ids_shrink=None):
-        self.user_group_ids_shrink = user_group_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListPolicesForUserGroupShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.user_group_ids_shrink is not None:
-            result['UserGroupIds'] = self.user_group_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('UserGroupIds') is not None:
-            self.user_group_ids_shrink = m.get('UserGroupIds')
-        return self
-
-
 class ListPolicesForUserGroupResponseBodyUserGroupsPolices(TeaModel):
     def __init__(self, name=None, policy_id=None, policy_type=None):
         self.name = name  # type: str
         self.policy_id = policy_id  # type: str
         self.policy_type = policy_type  # type: str
 
     def validate(self):
@@ -3584,74 +3427,14 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
         return self
 
 
-class ListPrivateAccessApplicationsShrinkRequest(TeaModel):
-    def __init__(self, address=None, application_ids_shrink=None, current_page=None, name=None, page_size=None,
-                 policy_id=None, status=None, tag_id=None):
-        self.address = address  # type: str
-        self.application_ids_shrink = application_ids_shrink  # type: str
-        self.current_page = current_page  # type: int
-        self.name = name  # type: str
-        self.page_size = page_size  # type: int
-        self.policy_id = policy_id  # type: str
-        self.status = status  # type: str
-        self.tag_id = tag_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListPrivateAccessApplicationsShrinkRequest, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, begin=None, end=None):
         self.begin = begin  # type: int
         self.end = end  # type: int
 
     def validate(self):
         pass
@@ -3843,14 +3626,17 @@
         self.current_page = current_page  # type: int
         self.name = name  # type: str
         self.page_size = page_size  # type: int
         self.policy_action = policy_action  # type: str
         self.policy_ids = policy_ids  # type: list[str]
         self.status = status  # type: str
         self.tag_id = tag_id  # type: str
+        # 用户组ID。取值来源：
+        # - [ListUserGroups](~~ListUserGroups~~)：批量查询用户组。
+        # - [CreateUserGroup](~~CreateUserGroup~~)：创建用户组。
         self.user_group_id = user_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListPrivateAccessPolicesRequest, self).to_map()
@@ -3897,79 +3683,14 @@
         if m.get('TagId') is not None:
             self.tag_id = m.get('TagId')
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
 
 
-class ListPrivateAccessPolicesShrinkRequest(TeaModel):
-    def __init__(self, application_id=None, current_page=None, name=None, page_size=None, policy_action=None,
-                 policy_ids_shrink=None, status=None, tag_id=None, user_group_id=None):
-        self.application_id = application_id  # type: str
-        self.current_page = current_page  # type: int
-        self.name = name  # type: str
-        self.page_size = page_size  # type: int
-        self.policy_action = policy_action  # type: str
-        self.policy_ids_shrink = policy_ids_shrink  # type: str
-        self.status = status  # type: str
-        self.tag_id = tag_id  # type: str
-        self.user_group_id = user_group_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListPrivateAccessPolicesShrinkRequest, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, idp_id=None, relation=None, user_group_type=None, value=None):
         self.idp_id = idp_id  # type: int
         self.relation = relation  # type: str
         self.user_group_type = user_group_type  # type: str
         self.value = value  # type: str
 
@@ -4226,64 +3947,14 @@
         if m.get('PolicyId') is not None:
             self.policy_id = m.get('PolicyId')
         if m.get('TagIds') is not None:
             self.tag_ids = m.get('TagIds')
         return self
 
 
-class ListPrivateAccessTagsShrinkRequest(TeaModel):
-    def __init__(self, application_id=None, current_page=None, name=None, page_size=None, policy_id=None,
-                 tag_ids_shrink=None):
-        self.application_id = application_id  # type: str
-        self.current_page = current_page  # type: int
-        self.name = name  # type: str
-        self.page_size = page_size  # type: int
-        self.policy_id = policy_id  # type: str
-        self.tag_ids_shrink = tag_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListPrivateAccessTagsShrinkRequest, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, application_ids=None, create_time=None, description=None, name=None, policy_ids=None,
                  tag_id=None, tag_type=None):
         self.application_ids = application_ids  # type: list[str]
         self.create_time = create_time  # type: str
         self.description = description  # type: str
         self.name = name  # type: str
@@ -4436,38 +4107,14 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ApplicationIds') is not None:
             self.application_ids = m.get('ApplicationIds')
         return self
 
 
-class ListTagsForPrivateAccessApplicationShrinkRequest(TeaModel):
-    def __init__(self, application_ids_shrink=None):
-        self.application_ids_shrink = application_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListTagsForPrivateAccessApplicationShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.application_ids_shrink is not None:
-            result['ApplicationIds'] = self.application_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('ApplicationIds') is not None:
-            self.application_ids_shrink = m.get('ApplicationIds')
-        return self
-
-
 class ListTagsForPrivateAccessApplicationResponseBodyApplicationsTags(TeaModel):
     def __init__(self, create_time=None, description=None, name=None, tag_id=None, tag_type=None):
         self.create_time = create_time  # type: str
         self.description = description  # type: str
         self.name = name  # type: str
         self.tag_id = tag_id  # type: str
         self.tag_type = tag_type  # type: str
@@ -4641,40 +4288,17 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         return self
 
 
-class ListTagsForPrivateAccessPolicyShrinkRequest(TeaModel):
-    def __init__(self, policy_ids_shrink=None):
-        self.policy_ids_shrink = policy_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListTagsForPrivateAccessPolicyShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.policy_ids_shrink is not None:
-            result['PolicyIds'] = self.policy_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('PolicyIds') is not None:
-            self.policy_ids_shrink = m.get('PolicyIds')
-        return self
-
-
 class ListTagsForPrivateAccessPolicyResponseBodyPolicesTags(TeaModel):
     def __init__(self, create_time=None, description=None, name=None, tag_id=None, tag_type=None):
+        # 内网访问标签创建时间。
         self.create_time = create_time  # type: str
         self.description = description  # type: str
         self.name = name  # type: str
         self.tag_id = tag_id  # type: str
         self.tag_type = tag_type  # type: str
 
     def validate(self):
@@ -4827,14 +4451,15 @@
 
 
 class ListUserGroupsRequest(TeaModel):
     def __init__(self, attribute_value=None, current_page=None, name=None, papolicy_id=None, page_size=None,
                  user_group_ids=None):
         self.attribute_value = attribute_value  # type: str
         self.current_page = current_page  # type: int
+        # 用户组名称。长度为1~128个字符，支持中文和大小写英文字母，可包含数字、半角句号（.）、下划线（_）和短划线（-）。
         self.name = name  # type: str
         self.papolicy_id = papolicy_id  # type: str
         self.page_size = page_size  # type: int
         self.user_group_ids = user_group_ids  # type: list[str]
 
     def validate(self):
         pass
@@ -4872,64 +4497,14 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         if m.get('UserGroupIds') is not None:
             self.user_group_ids = m.get('UserGroupIds')
         return self
 
 
-class ListUserGroupsShrinkRequest(TeaModel):
-    def __init__(self, attribute_value=None, current_page=None, name=None, papolicy_id=None, page_size=None,
-                 user_group_ids_shrink=None):
-        self.attribute_value = attribute_value  # type: str
-        self.current_page = current_page  # type: int
-        self.name = name  # type: str
-        self.papolicy_id = papolicy_id  # type: str
-        self.page_size = page_size  # type: int
-        self.user_group_ids_shrink = user_group_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListUserGroupsShrinkRequest, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, idp_id=None, relation=None, user_group_type=None, value=None):
         self.idp_id = idp_id  # type: int
         self.relation = relation  # type: str
         self.user_group_type = user_group_type  # type: str
         self.value = value  # type: str
 
@@ -5118,38 +4693,14 @@
     def from_map(self, m=None):
         m = m or dict()
         if m.get('PolicyIds') is not None:
             self.policy_ids = m.get('PolicyIds')
         return self
 
 
-class ListUserGroupsForPrivateAccessPolicyShrinkRequest(TeaModel):
-    def __init__(self, policy_ids_shrink=None):
-        self.policy_ids_shrink = policy_ids_shrink  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(ListUserGroupsForPrivateAccessPolicyShrinkRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.policy_ids_shrink is not None:
-            result['PolicyIds'] = self.policy_ids_shrink
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('PolicyIds') is not None:
-            self.policy_ids_shrink = m.get('PolicyIds')
-        return self
-
-
 class ListUserGroupsForPrivateAccessPolicyResponseBodyPolicesUserGroupsAttributes(TeaModel):
     def __init__(self, idp_id=None, relation=None, user_group_type=None, value=None):
         self.idp_id = idp_id  # type: int
         self.relation = relation  # type: str
         self.user_group_type = user_group_type  # type: str
         self.value = value  # type: str
 
@@ -5184,14 +4735,15 @@
             self.value = m.get('Value')
         return self
 
 
 class ListUserGroupsForPrivateAccessPolicyResponseBodyPolicesUserGroups(TeaModel):
     def __init__(self, attributes=None, create_time=None, description=None, name=None, user_group_id=None):
         self.attributes = attributes  # type: list[ListUserGroupsForPrivateAccessPolicyResponseBodyPolicesUserGroupsAttributes]
+        # 用户组创建时间。
         self.create_time = create_time  # type: str
         self.description = description  # type: str
         self.name = name  # type: str
         self.user_group_id = user_group_id  # type: str
 
     def validate(self):
         if self.attributes:
@@ -5618,16 +5170,20 @@
         self.custom_user_attributes = custom_user_attributes  # type: list[UpdatePrivateAccessPolicyRequestCustomUserAttributes]
         self.description = description  # type: str
         self.modify_type = modify_type  # type: str
         self.policy_action = policy_action  # type: str
         self.policy_id = policy_id  # type: str
         self.priority = priority  # type: int
         self.status = status  # type: str
+        # 内网访问标签ID集合。一条策略最多支持100个内网访问标签ID。
         self.tag_ids = tag_ids  # type: list[str]
         self.user_group_ids = user_group_ids  # type: list[str]
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode  # type: str
 
     def validate(self):
         if self.custom_user_attributes:
             for k in self.custom_user_attributes:
                 if k:
                     k.validate()
@@ -5707,16 +5263,20 @@
         self.custom_user_attributes_shrink = custom_user_attributes_shrink  # type: str
         self.description = description  # type: str
         self.modify_type = modify_type  # type: str
         self.policy_action = policy_action  # type: str
         self.policy_id = policy_id  # type: str
         self.priority = priority  # type: int
         self.status = status  # type: str
+        # 内网访问标签ID集合。一条策略最多支持100个内网访问标签ID。
         self.tag_ids_shrink = tag_ids_shrink  # type: str
         self.user_group_ids_shrink = user_group_ids_shrink  # type: str
+        # 内网访问策略的用户组类型。取值：
+        # - **Normal**：普通用户组。
+        # - **Custom**：自定义用户组。
         self.user_group_mode = user_group_mode  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdatePrivateAccessPolicyShrinkRequest, self).to_map()
@@ -5922,53 +5482,14 @@
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
-    def __init__(self, attributes_shrink=None, description=None, modify_type=None, user_group_id=None):
-        self.attributes_shrink = attributes_shrink  # type: str
-        self.description = description  # type: str
-        self.modify_type = modify_type  # type: str
-        self.user_group_id = user_group_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(UpdateUserGroupShrinkRequest, self).to_map()
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
-    def from_map(self, m=None):
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
     def __init__(self, request_id=None):
         self.request_id = request_id  # type: str
 
     def validate(self):
```

### Comparing `alibabacloud_csas20230120_py2-1.0.0/alibabacloud_csas20230120_py2.egg-info/PKG-INFO` & `alibabacloud_csas20230120_py2-1.0.1/alibabacloud_csas20230120_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-csas20230120-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120_py2-1.0.0/setup.py` & `alibabacloud_csas20230120_py2-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_csas20230120_py2.
 
-Created on 24/03/2023
+Created on 12/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_csas20230120"
 NAME = "alibabacloud_csas20230120_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud csas (20230120) SDK Library for Python2"
```

