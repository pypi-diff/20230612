# Comparing `tmp/tencentcloud-sdk-python-cloudhsm-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-cloudhsm-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cloudhsm-3.0.911.tar", last modified: Fri Jun  9 02:15:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cloudhsm-3.0.912.tar", last modified: Mon Jun 12 02:59:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911.tar` & `tencentcloud-sdk-python-cloudhsm-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/
--rw-r--r--   0 root         (0) root         (0)    13291 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52136 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud_sdk_python_cloudhsm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud_sdk_python_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud_sdk_python_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud_sdk_python_cloudhsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:15:47.000000 tencentcloud-sdk-python-cloudhsm-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52136 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud_sdk_python_cloudhsm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud_sdk_python_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud_sdk_python_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud_sdk_python_cloudhsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 02:59:58.000000 tencentcloud-sdk-python-cloudhsm-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/README.rst` & `tencentcloud-sdk-python-cloudhsm-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py` & `tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/errorcodes.py` & `tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/cloudhsm/v20191112/models.py` & `tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/cloudhsm/v20191112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cloudhsm-3.0.912/tencentcloud_sdk_python_cloudhsm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudhsm
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Cloudhsm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-cloudhsm-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cloudhsm
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Cloudhsm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cloudhsm-3.0.911/setup.py` & `tencentcloud-sdk-python-cloudhsm-3.0.912/setup.py`

 * *Files identical despite different names*

