# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.911.tar", last modified: Fri Jun  9 02:15:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.912.tar", last modified: Mon Jun 12 02:59:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.911.tar` & `tencentcloud-sdk-python-ckafka-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   475045 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    70499 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:15:29.000000 tencentcloud-sdk-python-ckafka-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   475057 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    70499 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 02:59:42.000000 tencentcloud-sdk-python-ckafka-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2238,15 +2238,15 @@
         :type DiskType: str
         :param DiskSize: 实例硬盘大小，需要满足当前实例的计费规格
         :type DiskSize: int
         :param Partition: 实例最大分区数量，需要满足当前实例的计费规格
         :type Partition: int
         :param TopicNum: 实例最大 topic 数量，需要满足当前实例的计费规格
         :type TopicNum: int
-        :param ZoneId: 实例所在的可用区。当创建多可用区实例时，该参数为创建的默认接入点所在的子网
+        :param ZoneId: 实例所在的可用区。当创建多可用区实例时，该参数为创建的默认接入点所在子网的可用区 id
         :type ZoneId: int
         :param MultiZoneFlag: 当前实例是否为多可用区实例。
         :type MultiZoneFlag: bool
         :param ZoneIds: 当实例为多可用区实例时，多可用区 id 列表。注意参数 ZoneId 对应的多可用区需要包含在该参数数组中
         :type ZoneIds: list of int
         :param InstanceNum: 购买实例数量。非必填，默认值为 1。当传入该参数时，会创建多个 instanceName 加后缀区分的实例
         :type InstanceNum: int
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.912/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.911/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.912/setup.py`

 * *Files identical despite different names*

