# Comparing `tmp/alibabacloud_btripopen20220520_py2-1.1.2.tar.gz` & `tmp/alibabacloud_btripopen20220520_py2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.2.tar", last modified: Fri Jun  9 03:25:37 2023, max compression
+gzip compressed data, was "dist/alibabacloud_btripopen20220520_py2-1.1.3.tar", last modified: Mon Jun 12 09:17:46 2023, max compression
```

## Comparing `alibabacloud_btripopen20220520_py2-1.1.2.tar` & `alibabacloud_btripopen20220520_py2-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/
--rw-r--r--   0 root         (0) root         (0)     3306 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223086 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/client.py
--rw-r--r--   0 root         (0) root         (0)  2001831 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-09 03:25:37.000000 alibabacloud_btripopen20220520_py2-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223194 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/client.py
+-rw-r--r--   0 root         (0) root         (0)  2002413 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-12 09:17:46.000000 alibabacloud_btripopen20220520_py2-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-06-12 09:17:45.000000 alibabacloud_btripopen20220520_py2-1.1.3/setup.py
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/ChangeLog.md` & `alibabacloud_btripopen20220520_py2-1.1.3/ChangeLog.md`

 * *Files 1% similar despite different names*

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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/LICENSE` & `alibabacloud_btripopen20220520_py2-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_btripopen20220520_py2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/README-CN.md` & `alibabacloud_btripopen20220520_py2-1.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/README.md` & `alibabacloud_btripopen20220520_py2-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/client.py` & `alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2441,14 +2441,16 @@
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

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520/models.py` & `alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,17 @@
 class AccessTokenResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, module=None, request_id=None, success=None, trace_id=None):
         self.code = code  # type: str
         self.data = data  # type: AccessTokenResponseBodyData
         self.message = message  # type: str
         self.module = module  # type: AccessTokenResponseBodyModule
         self.request_id = request_id  # type: str
+        # 成功标识
         self.success = success  # type: bool
+        # traceId
         self.trace_id = trace_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
         if self.module:
             self.module.validate()
@@ -8226,14 +8228,15 @@
         return self
 
 
 class CitySearchResponseBody(TeaModel):
     def __init__(self, code=None, message=None, module=None, request_id=None, success=None, trace_id=None):
         self.code = code  # type: str
         self.message = message  # type: str
+        # module
         self.module = module  # type: CitySearchResponseBodyModule
         self.request_id = request_id  # type: str
         self.success = success  # type: bool
         self.trace_id = trace_id  # type: str
 
     def validate(self):
         if self.module:
@@ -26571,21 +26574,22 @@
         if m.get('x-acs-btrip-corp-token') is not None:
             self.x_acs_btrip_corp_token = m.get('x-acs-btrip-corp-token')
         return self
 
 
 class GroupDepartSaveRequest(TeaModel):
     def __init__(self, dept_name=None, manager_ids=None, outer_dept_id=None, outer_dept_pid=None, status=None,
-                 sub_corp_id_list=None):
+                 sub_corp_id_list=None, sync_group=None):
         self.dept_name = dept_name  # type: str
         self.manager_ids = manager_ids  # type: str
         self.outer_dept_id = outer_dept_id  # type: str
         self.outer_dept_pid = outer_dept_pid  # type: str
         self.status = status  # type: int
         self.sub_corp_id_list = sub_corp_id_list  # type: list[str]
+        self.sync_group = sync_group  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GroupDepartSaveRequest, self).to_map()
         if _map is not None:
@@ -26600,14 +26604,16 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('dept_name') is not None:
             self.dept_name = m.get('dept_name')
         if m.get('manager_ids') is not None:
@@ -26616,26 +26622,29 @@
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
     def __init__(self, dept_name=None, manager_ids=None, outer_dept_id=None, outer_dept_pid=None, status=None,
-                 sub_corp_id_list_shrink=None):
+                 sub_corp_id_list_shrink=None, sync_group=None):
         self.dept_name = dept_name  # type: str
         self.manager_ids = manager_ids  # type: str
         self.outer_dept_id = outer_dept_id  # type: str
         self.outer_dept_pid = outer_dept_pid  # type: str
         self.status = status  # type: int
         self.sub_corp_id_list_shrink = sub_corp_id_list_shrink  # type: str
+        self.sync_group = sync_group  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GroupDepartSaveShrinkRequest, self).to_map()
         if _map is not None:
@@ -26650,14 +26659,16 @@
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
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('dept_name') is not None:
             self.dept_name = m.get('dept_name')
         if m.get('manager_ids') is not None:
@@ -26666,14 +26677,16 @@
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
     def __init__(self, code=None, message=None, request_id=None, success=None, trace_id=None):
         self.code = code  # type: str
         self.message = message  # type: str
@@ -36301,14 +36314,15 @@
 
 class InvoiceAddResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None, success=None, trace_id=None):
         self.code = code  # type: str
         self.message = message  # type: str
         self.request_id = request_id  # type: str
         self.success = success  # type: bool
+        # traceId
         self.trace_id = trace_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(InvoiceAddResponseBody, self).to_map()
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO` & `alibabacloud_btripopen20220520_py2-1.1.3/alibabacloud_btripopen20220520_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-btripopen20220520-py2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud btripOpen (20220520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_btripopen20220520_py2-1.1.2/setup.py` & `alibabacloud_btripopen20220520_py2-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_btripopen20220520_py2.
 
-Created on 09/06/2023
+Created on 12/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_btripopen20220520"
 NAME = "alibabacloud_btripopen20220520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud btripOpen (20220520) SDK Library for Python2"
```

