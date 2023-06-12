# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.911.tar", last modified: Fri Jun  9 02:31:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.912.tar", last modified: Mon Jun 12 03:16:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.911.tar` & `tencentcloud-sdk-python-vpc-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332322 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41912 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   851887 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:31:29.000000 tencentcloud-sdk-python-vpc-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332322 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    42054 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851887 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:16:11.000000 tencentcloud-sdk-python-vpc-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.912/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/README.rst` & `tencentcloud-sdk-python-vpc-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,14 +733,17 @@
 
 # 当前地域不支持启用组播。
 UNSUPPORTEDOPERATION_ENABLEMULTICAST = 'UnsupportedOperation.EnableMulticast'
 
 # 终端节点服务本身不能是终端节点。
 UNSUPPORTEDOPERATION_ENDPOINTSERVICE = 'UnsupportedOperation.EndPointService'
 
+# 指定ResourceId对应的流日志已经创建
+UNSUPPORTEDOPERATION_FLOWLOGINSTANCEEXISTED = 'UnsupportedOperation.FlowLogInstanceExisted'
+
 # 不支持创建流日志：当前弹性网卡绑定的是KO机型。
 UNSUPPORTEDOPERATION_FLOWLOGSNOTSUPPORTKOINSTANCEENI = 'UnsupportedOperation.FlowLogsNotSupportKoInstanceEni'
 
 # 不支持创建流日志：当前弹性网卡未绑定实例。
 UNSUPPORTEDOPERATION_FLOWLOGSNOTSUPPORTNULLINSTANCEENI = 'UnsupportedOperation.FlowLogsNotSupportNullInstanceEni'
 
 # 该种类型地址不支持此操作。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/vpc/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.912/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.911'
+__version__ = '3.0.912'
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.912/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.911/setup.py` & `tencentcloud-sdk-python-vpc-3.0.912/setup.py`

 * *Files identical despite different names*

