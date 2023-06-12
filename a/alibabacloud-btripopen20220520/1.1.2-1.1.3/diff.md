# Comparing `tmp/alibabacloud_btripopen20220520-1.1.2.tar.gz` & `tmp/alibabacloud_btripopen20220520-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.2.tar", last modified: Fri Jun  9 03:25:49 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520-1.1.3.tar", last modified: Mon Jun 12 09:18:20 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520-1.1.2.tar` & `alibabacloud_btripopen20220520-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/
--rw-r--r--   0 root         (0) root         (0)     3432 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   524990 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  1979790 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2364 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 03:25:49.000000 alibabacloud_btripopen20220520-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2023-06-09 03:25:48.000000 alibabacloud_btripopen20220520-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)     3469 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   525206 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  1980376 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-06-12 09:18:20.000000 alibabacloud_btripopen20220520-1.1.3/setup.py
```

### Comparing `alibabacloud_btripopen20220520-1.1.2/ChangeLog.md` & `alibabacloud_btripopen20220520-1.1.3/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-09 Version: 1.1.2
+- Update.
+
 2023-06-06 Version: 1.0.74
 - Update.
 
 2023-06-05 Version: 1.0.73
 - Update.
 
 2023-06-01 Version: 1.0.72
```

### Comparing `alibabacloud_btripopen20220520-1.1.2/LICENSE` & `alibabacloud_btripopen20220520-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.2/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.2/README-CN.md` & `alibabacloud_btripopen20220520-1.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.2/README.md` & `alibabacloud_btripopen20220520-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5659,14 +5659,16 @@
             body['outer_dept_id'] = request.outer_dept_id
         if not UtilClient.is_unset(request.outer_dept_pid):
             body['outer_dept_pid'] = request.outer_dept_pid
         if not UtilClient.is_unset(request.status):
             body['status'] = request.status
         if not UtilClient.is_unset(request.sub_corp_id_list_shrink):
             body['sub_corp_id_list'] = request.sub_corp_id_list_shrink
+        if not UtilClient.is_unset(request.sync_group):
+            body['sync_group'] = request.sync_group
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_btrip_corp_token):
             real_headers['x-acs-btrip-corp-token'] = UtilClient.to_jsonstring(headers.x_acs_btrip_corp_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -5708,14 +5710,16 @@
             body['outer_dept_id'] = request.outer_dept_id
         if not UtilClient.is_unset(request.outer_dept_pid):
             body['outer_dept_pid'] = request.outer_dept_pid
         if not UtilClient.is_unset(request.status):
             body['status'] = request.status
         if not UtilClient.is_unset(request.sub_corp_id_list_shrink):
             body['sub_corp_id_list'] = request.sub_corp_id_list_shrink
+        if not UtilClient.is_unset(request.sync_group):
+            body['sync_group'] = request.sync_group
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_btrip_corp_token):
             real_headers['x-acs-btrip-corp-token'] = UtilClient.to_jsonstring(headers.x_acs_btrip_corp_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
```

### Comparing `alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,17 @@
         trace_id: str = None,
     ):
         self.code = code
         self.data = data
         self.message = message
         self.module = module
         self.request_id = request_id
+        # 成功标识
         self.success = success
+        # traceId
         self.trace_id = trace_id
 
     def validate(self):
         if self.data:
             self.data.validate()
         if self.module:
             self.module.validate()
@@ -9386,14 +9388,15 @@
         module: CitySearchResponseBodyModule = None,
         request_id: str = None,
         success: bool = None,
         trace_id: str = None,
     ):
         self.code = code
         self.message = message
+        # module
         self.module = module
         self.request_id = request_id
         self.success = success
         self.trace_id = trace_id
 
     def validate(self):
         if self.module:
@@ -30267,21 +30270,23 @@
         self,
         dept_name: str = None,
         manager_ids: str = None,
         outer_dept_id: str = None,
         outer_dept_pid: str = None,
         status: int = None,
         sub_corp_id_list: List[str] = None,
+        sync_group: bool = None,
     ):
         self.dept_name = dept_name
         self.manager_ids = manager_ids
         self.outer_dept_id = outer_dept_id
         self.outer_dept_pid = outer_dept_pid
         self.status = status
         self.sub_corp_id_list = sub_corp_id_list
+        self.sync_group = sync_group
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -30296,14 +30301,16 @@
             result['outer_dept_id'] = self.outer_dept_id
         if self.outer_dept_pid is not None:
             result['outer_dept_pid'] = self.outer_dept_pid
         if self.status is not None:
             result['status'] = self.status
         if self.sub_corp_id_list is not None:
             result['sub_corp_id_list'] = self.sub_corp_id_list
+        if self.sync_group is not None:
+            result['sync_group'] = self.sync_group
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('dept_name') is not None:
             self.dept_name = m.get('dept_name')
         if m.get('manager_ids') is not None:
@@ -30312,33 +30319,37 @@
             self.outer_dept_id = m.get('outer_dept_id')
         if m.get('outer_dept_pid') is not None:
             self.outer_dept_pid = m.get('outer_dept_pid')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('sub_corp_id_list') is not None:
             self.sub_corp_id_list = m.get('sub_corp_id_list')
+        if m.get('sync_group') is not None:
+            self.sync_group = m.get('sync_group')
         return self
 
 
 class GroupDepartSaveShrinkRequest(TeaModel):
     def __init__(
         self,
         dept_name: str = None,
         manager_ids: str = None,
         outer_dept_id: str = None,
         outer_dept_pid: str = None,
         status: int = None,
         sub_corp_id_list_shrink: str = None,
+        sync_group: bool = None,
     ):
         self.dept_name = dept_name
         self.manager_ids = manager_ids
         self.outer_dept_id = outer_dept_id
         self.outer_dept_pid = outer_dept_pid
         self.status = status
         self.sub_corp_id_list_shrink = sub_corp_id_list_shrink
+        self.sync_group = sync_group
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -30353,14 +30364,16 @@
             result['outer_dept_id'] = self.outer_dept_id
         if self.outer_dept_pid is not None:
             result['outer_dept_pid'] = self.outer_dept_pid
         if self.status is not None:
             result['status'] = self.status
         if self.sub_corp_id_list_shrink is not None:
             result['sub_corp_id_list'] = self.sub_corp_id_list_shrink
+        if self.sync_group is not None:
+            result['sync_group'] = self.sync_group
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('dept_name') is not None:
             self.dept_name = m.get('dept_name')
         if m.get('manager_ids') is not None:
@@ -30369,14 +30382,16 @@
             self.outer_dept_id = m.get('outer_dept_id')
         if m.get('outer_dept_pid') is not None:
             self.outer_dept_pid = m.get('outer_dept_pid')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('sub_corp_id_list') is not None:
             self.sub_corp_id_list_shrink = m.get('sub_corp_id_list')
+        if m.get('sync_group') is not None:
+            self.sync_group = m.get('sync_group')
         return self
 
 
 class GroupDepartSaveResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -41376,14 +41391,15 @@
         success: bool = None,
         trace_id: str = None,
     ):
         self.code = code
         self.message = message
         self.request_id = request_id
         self.success = success
+        # traceId
         self.trace_id = trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_btripopen20220520-1.1.2/alibabacloud_btripopen20220520.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520-1.1.3/alibabacloud_btripopen20220520.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520-1.1.2/setup.py` & `alibabacloud_btripopen20220520-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520.
 
-Created on 09/06/2023
+Created on 12/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python"
```

