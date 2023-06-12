# Comparing `tmp/tencentcloud-sdk-python-iotcloud-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-iotcloud-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.911.tar", last modified: Fri Jun  9 02:21:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.912.tar", last modified: Mon Jun 12 03:05:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotcloud-3.0.911.tar` & `tencentcloud-sdk-python-iotcloud-3.0.912.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/
--rw-r--r--   0 root         (0) root         (0)    12668 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175690 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/models.py
--rw-r--r--   0 root         (0) root         (0)    64286 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/iotcloud_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/
--rw-r--r--   0 root         (0) root         (0)    12818 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)   172985 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)    66885 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud_sdk_python_iotcloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:21:21.000000 tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175690 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/models.py
+-rw-r--r--   0 root         (0) root         (0)    64286 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/iotcloud_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/
+-rw-r--r--   0 root         (0) root         (0)    12818 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   173618 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)    66885 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud_sdk_python_iotcloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:05:53.000000 tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/README.rst` & `tencentcloud-sdk-python-iotcloud-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20180614/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20180614/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4040,20 +4040,28 @@
 
     """
 
     def __init__(self):
         r"""
         :param CreationDate: 产品创建时间
         :type CreationDate: int
+        :param CreateUserId: 创建者 Uin
+        :type CreateUserId: int
+        :param UserId: 账号 Uin
+        :type UserId: int
         """
         self.CreationDate = None
+        self.CreateUserId = None
+        self.UserId = None
 
 
     def _deserialize(self, params):
         self.CreationDate = params.get("CreationDate")
+        self.CreateUserId = params.get("CreateUserId")
+        self.UserId = params.get("UserId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4085,24 +4093,28 @@
         :type ModelId: str
         :param ModelName: 产品绑定的物模型名称
         :type ModelName: str
         :param ProductKey: 产品密钥，suite产品才会有
         :type ProductKey: str
         :param RegisterType: 动态注册类型 0-关闭, 1-预定义设备名 2-动态定义设备名
         :type RegisterType: int
-        :param ProductSecret: 动态注册产品秘钥
+        :param ProductSecret: 动态注册产品密钥
         :type ProductSecret: str
         :param RegisterLimit: RegisterType为2时，设备动态创建的限制数量
         :type RegisterLimit: int
         :param OriginProductId: 划归的产品，展示为源产品ID，其余为空
         :type OriginProductId: str
         :param PrivateCAName: 私有CA名称
         :type PrivateCAName: str
         :param OriginUserId: 划归的产品，展示为源用户ID，其余为空
         :type OriginUserId: int
+        :param DeviceLimit: 设备限制
+        :type DeviceLimit: int
+        :param ForbiddenStatus: 产品禁用状态
+        :type ForbiddenStatus: int
         """
         self.ProductDescription = None
         self.EncryptionType = None
         self.Region = None
         self.ProductType = None
         self.Format = None
         self.Platform = None
@@ -4112,14 +4124,16 @@
         self.ProductKey = None
         self.RegisterType = None
         self.ProductSecret = None
         self.RegisterLimit = None
         self.OriginProductId = None
         self.PrivateCAName = None
         self.OriginUserId = None
+        self.DeviceLimit = None
+        self.ForbiddenStatus = None
 
 
     def _deserialize(self, params):
         self.ProductDescription = params.get("ProductDescription")
         self.EncryptionType = params.get("EncryptionType")
         self.Region = params.get("Region")
         self.ProductType = params.get("ProductType")
@@ -4131,14 +4145,16 @@
         self.ProductKey = params.get("ProductKey")
         self.RegisterType = params.get("RegisterType")
         self.ProductSecret = params.get("ProductSecret")
         self.RegisterLimit = params.get("RegisterLimit")
         self.OriginProductId = params.get("OriginProductId")
         self.PrivateCAName = params.get("PrivateCAName")
         self.OriginUserId = params.get("OriginUserId")
+        self.DeviceLimit = params.get("DeviceLimit")
+        self.ForbiddenStatus = params.get("ForbiddenStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/iotcloud/v20210408/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/iotcloud/v20210408/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/setup.py` & `tencentcloud-sdk-python-iotcloud-3.0.912/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.911/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.912/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

