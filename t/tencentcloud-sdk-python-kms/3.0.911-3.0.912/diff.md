# Comparing `tmp/tencentcloud-sdk-python-kms-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-kms-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.911.tar", last modified: Fri Jun  9 02:22:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.912.tar", last modified: Mon Jun 12 03:06:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-kms-3.0.911.tar` & `tencentcloud-sdk-python-kms-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/
--rw-r--r--   0 root         (0) root         (0)    50843 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/kms_client.py
--rw-r--r--   0 root         (0) root         (0)     5342 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104577 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud_sdk_python_kms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/tencentcloud_sdk_python_kms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:22:04.000000 tencentcloud-sdk-python-kms-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/
+-rw-r--r--   0 root         (0) root         (0)    50843 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/kms_client.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104577 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud_sdk_python_kms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/tencentcloud_sdk_python_kms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:06:39.000000 tencentcloud-sdk-python-kms-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-kms-3.0.911/README.rst` & `tencentcloud-sdk-python-kms-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/kms_client.py` & `tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/kms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/errorcodes.py` & `tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.911/tencentcloud/kms/v20190118/models.py` & `tencentcloud-sdk-python-kms-3.0.912/tencentcloud/kms/v20190118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-kms-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-kms-3.0.911/tencentcloud_sdk_python_kms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.912/tencentcloud_sdk_python_kms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.911/setup.py` & `tencentcloud-sdk-python-kms-3.0.912/setup.py`

 * *Files identical despite different names*

