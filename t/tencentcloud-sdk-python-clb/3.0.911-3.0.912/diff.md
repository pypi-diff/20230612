# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.911.tar", last modified: Fri Jun  9 02:15:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.912.tar", last modified: Mon Jun 12 02:59:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.911.tar` & `tencentcloud-sdk-python-clb-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89673 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)   331792 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:15:36.000000 tencentcloud-sdk-python-clb-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89673 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   331792 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 02:59:48.000000 tencentcloud-sdk-python-clb-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-clb-3.0.911/README.rst` & `tencentcloud-sdk-python-clb-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.911/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.912/tencentcloud/clb/v20180317/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8249,31 +8249,31 @@
 
     """
 
     def __init__(self):
         r"""
         :param LoadBalancerId: 负载均衡ID
         :type LoadBalancerId: str
-        :param ListenerId: 监听器ID
-        :type ListenerId: str
         :param TargetGroupId: 目标组ID
         :type TargetGroupId: str
+        :param ListenerId: 监听器ID
+        :type ListenerId: str
         :param LocationId: 转发规则ID
         :type LocationId: str
         """
         self.LoadBalancerId = None
-        self.ListenerId = None
         self.TargetGroupId = None
+        self.ListenerId = None
         self.LocationId = None
 
 
     def _deserialize(self, params):
         self.LoadBalancerId = params.get("LoadBalancerId")
-        self.ListenerId = params.get("ListenerId")
         self.TargetGroupId = params.get("TargetGroupId")
+        self.ListenerId = params.get("ListenerId")
         self.LocationId = params.get("LocationId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-clb-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.911/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.912/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.911/setup.py` & `tencentcloud-sdk-python-clb-3.0.912/setup.py`

 * *Files identical despite different names*

