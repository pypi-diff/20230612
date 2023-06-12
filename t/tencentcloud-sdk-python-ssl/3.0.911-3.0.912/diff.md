# Comparing `tmp/tencentcloud-sdk-python-ssl-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-ssl-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.911.tar", last modified: Fri Jun  9 02:26:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ssl-3.0.912.tar", last modified: Mon Jun 12 03:11:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ssl-3.0.911.tar` & `tencentcloud-sdk-python-ssl-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)     9587 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   222301 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    49507 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:26:29.000000 tencentcloud-sdk-python-ssl-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud_sdk_python_ssl.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:26:30.000000 tencentcloud-sdk-python-ssl-3.0.911/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)     9587 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223934 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    49507 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:11:12.000000 tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/README.rst` & `tencentcloud-sdk-python-ssl-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2483,22 +2483,25 @@
         :type Filters: list of Filter
         :param OldCertificateId: 原证书ID
         :type OldCertificateId: str
         :param Offset: 分页偏移量，从0开始。	
         :type Offset: int
         :param Limit: 每页数量，默认10。	
         :type Limit: int
+        :param AsyncCache: 是否异步
+        :type AsyncCache: int
         """
         self.CertificateId = None
         self.ResourceType = None
         self.IsCache = None
         self.Filters = None
         self.OldCertificateId = None
         self.Offset = None
         self.Limit = None
+        self.AsyncCache = None
 
 
     def _deserialize(self, params):
         self.CertificateId = params.get("CertificateId")
         self.ResourceType = params.get("ResourceType")
         self.IsCache = params.get("IsCache")
         if params.get("Filters") is not None:
@@ -2506,14 +2509,15 @@
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
         self.OldCertificateId = params.get("OldCertificateId")
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
+        self.AsyncCache = params.get("AsyncCache")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2528,30 +2532,45 @@
         r"""
         :param InstanceList: CDN实例列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceList: list of CdnInstanceDetail
         :param TotalCount: CDN域名总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type TotalCount: int
+        :param AsyncTotalNum: 异步刷新总数	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncTotalNum: int
+        :param AsyncOffset: 异步刷新当前执行数	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncOffset: int
+        :param AsyncCacheTime: 当前缓存读取时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncCacheTime: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceList = None
         self.TotalCount = None
+        self.AsyncTotalNum = None
+        self.AsyncOffset = None
+        self.AsyncCacheTime = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("InstanceList") is not None:
             self.InstanceList = []
             for item in params.get("InstanceList"):
                 obj = CdnInstanceDetail()
                 obj._deserialize(item)
                 self.InstanceList.append(obj)
         self.TotalCount = params.get("TotalCount")
+        self.AsyncTotalNum = params.get("AsyncTotalNum")
+        self.AsyncOffset = params.get("AsyncOffset")
+        self.AsyncCacheTime = params.get("AsyncCacheTime")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeHostClbInstanceListRequest(AbstractModel):
     """DescribeHostClbInstanceList请求参数结构体
 
     """
@@ -2619,34 +2638,39 @@
         :type InstanceList: list of ClbInstanceDetail
         :param AsyncTotalNum: 异步刷新总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type AsyncTotalNum: int
         :param AsyncOffset: 异步刷新当前执行数
 注意：此字段可能返回 null，表示取不到有效值。
         :type AsyncOffset: int
+        :param AsyncCacheTime: 当前缓存读取时间	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncCacheTime: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.InstanceList = None
         self.AsyncTotalNum = None
         self.AsyncOffset = None
+        self.AsyncCacheTime = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.TotalCount = params.get("TotalCount")
         if params.get("InstanceList") is not None:
             self.InstanceList = []
             for item in params.get("InstanceList"):
                 obj = ClbInstanceDetail()
                 obj._deserialize(item)
                 self.InstanceList.append(obj)
         self.AsyncTotalNum = params.get("AsyncTotalNum")
         self.AsyncOffset = params.get("AsyncOffset")
+        self.AsyncCacheTime = params.get("AsyncCacheTime")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeHostCosInstanceListRequest(AbstractModel):
     """DescribeHostCosInstanceList请求参数结构体
 
     """
@@ -2702,34 +2726,39 @@
         :type TotalCount: int
         :param AsyncTotalNum: 异步刷新总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type AsyncTotalNum: int
         :param AsyncOffset: 异步刷新当前执行数
 注意：此字段可能返回 null，表示取不到有效值。
         :type AsyncOffset: int
+        :param AsyncCacheTime: 当前缓存读取时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncCacheTime: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceList = None
         self.TotalCount = None
         self.AsyncTotalNum = None
         self.AsyncOffset = None
+        self.AsyncCacheTime = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         if params.get("InstanceList") is not None:
             self.InstanceList = []
             for item in params.get("InstanceList"):
                 obj = CosInstanceDetail()
                 obj._deserialize(item)
                 self.InstanceList.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.AsyncTotalNum = params.get("AsyncTotalNum")
         self.AsyncOffset = params.get("AsyncOffset")
+        self.AsyncCacheTime = params.get("AsyncCacheTime")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeHostDdosInstanceListRequest(AbstractModel):
     """DescribeHostDdosInstanceList请求参数结构体
 
     """
@@ -3237,34 +3266,39 @@
         :type InstanceList: list of TkeInstanceDetail
         :param AsyncTotalNum: 异步刷新总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type AsyncTotalNum: int
         :param AsyncOffset: 异步刷新当前执行数
 注意：此字段可能返回 null，表示取不到有效值。
         :type AsyncOffset: int
+        :param AsyncCacheTime: 当前缓存读取时间	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AsyncCacheTime: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.InstanceList = None
         self.AsyncTotalNum = None
         self.AsyncOffset = None
+        self.AsyncCacheTime = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.TotalCount = params.get("TotalCount")
         if params.get("InstanceList") is not None:
             self.InstanceList = []
             for item in params.get("InstanceList"):
                 obj = TkeInstanceDetail()
                 obj._deserialize(item)
                 self.InstanceList.append(obj)
         self.AsyncTotalNum = params.get("AsyncTotalNum")
         self.AsyncOffset = params.get("AsyncOffset")
+        self.AsyncCacheTime = params.get("AsyncCacheTime")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeHostUpdateRecordDetailRequest(AbstractModel):
     """DescribeHostUpdateRecordDetail请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.912/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/setup.py` & `tencentcloud-sdk-python-ssl-3.0.912/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ssl-3.0.911/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ssl-3.0.912/tencentcloud_sdk_python_ssl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ssl
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Ssl SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

