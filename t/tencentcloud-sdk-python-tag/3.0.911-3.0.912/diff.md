# Comparing `tmp/tencentcloud-sdk-python-tag-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-tag-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tag-3.0.911.tar", last modified: Fri Jun  9 02:27:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tag-3.0.912.tar", last modified: Mon Jun 12 03:11:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tag-3.0.911.tar` & `tencentcloud-sdk-python-tag-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/
--rw-r--r--   0 root         (0) root         (0)    28544 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/tag_client.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77724 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud_sdk_python_tag.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud_sdk_python_tag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud_sdk_python_tag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud_sdk_python_tag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/tencentcloud_sdk_python_tag.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:27:00.000000 tencentcloud-sdk-python-tag-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/
+-rw-r--r--   0 root         (0) root         (0)    28544 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/tag_client.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77793 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud_sdk_python_tag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud_sdk_python_tag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud_sdk_python_tag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud_sdk_python_tag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/tencentcloud_sdk_python_tag.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:11:44.000000 tencentcloud-sdk-python-tag-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tag-3.0.911/README.rst` & `tencentcloud-sdk-python-tag-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/tag_client.py` & `tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/tag_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/errorcodes.py` & `tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tag-3.0.911/tencentcloud/tag/v20180813/models.py` & `tencentcloud-sdk-python-tag-3.0.912/tencentcloud/tag/v20180813/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,17 +645,17 @@
         r"""
         :param ServiceType: 业务类型
         :type ServiceType: str
         :param ResourcePrefix: 资源前缀
         :type ResourcePrefix: str
         :param ResourceRegion: 资源地域
         :type ResourceRegion: str
-        :param ResourceIds: 资源唯一标识
+        :param ResourceIds: 资源唯一标识ID的列表，列表容量不超过20
         :type ResourceIds: list of str
-        :param TagKeys: 资源标签键
+        :param TagKeys: 资源标签键列表，列表容量不超过20
         :type TagKeys: list of str
         :param Limit: 每页大小，默认为 400
         :type Limit: int
         :param Offset: 数据偏移量，默认为 0, 必须为Limit参数的整数倍
         :type Offset: int
         """
         self.ServiceType = None
```

### Comparing `tencentcloud-sdk-python-tag-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tag-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tag-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-tag-3.0.912/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tag
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Tag SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tag-3.0.911/tencentcloud_sdk_python_tag.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tag-3.0.912/tencentcloud_sdk_python_tag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tag
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Tag SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tag-3.0.911/setup.py` & `tencentcloud-sdk-python-tag-3.0.912/setup.py`

 * *Files identical despite different names*

