# Comparing `tmp/tencentcloud-sdk-python-ape-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-ape-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ape-3.0.911.tar", last modified: Fri Jun  9 02:11:27 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ape-3.0.912.tar", last modified: Mon Jun 12 02:56:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ape-3.0.911.tar` & `tencentcloud-sdk-python-ape-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/
--rw-r--r--   0 root         (0) root         (0)     1570 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25870 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/models.py
--rw-r--r--   0 root         (0) root         (0)     8159 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/ape_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud_sdk_python_ape.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud_sdk_python_ape.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud_sdk_python_ape.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud_sdk_python_ape.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/tencentcloud_sdk_python_ape.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:11:26.000000 tencentcloud-sdk-python-ape-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:11:27.000000 tencentcloud-sdk-python-ape-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25870 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/models.py
+-rw-r--r--   0 root         (0) root         (0)     8159 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/ape_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud_sdk_python_ape.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud_sdk_python_ape.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud_sdk_python_ape.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud_sdk_python_ape.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/tencentcloud_sdk_python_ape.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 02:56:01.000000 tencentcloud-sdk-python-ape-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 02:56:02.000000 tencentcloud-sdk-python-ape-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ape-3.0.911/README.rst` & `tencentcloud-sdk-python-ape-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ape-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ape-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/errorcodes.py` & `tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/models.py` & `tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ape-3.0.911/tencentcloud/ape/v20200513/ape_client.py` & `tencentcloud-sdk-python-ape-3.0.912/tencentcloud/ape/v20200513/ape_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ape-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-ape-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ape
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Ape SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ape-3.0.911/tencentcloud_sdk_python_ape.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ape-3.0.912/tencentcloud_sdk_python_ape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ape
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Ape SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ape-3.0.911/setup.py` & `tencentcloud-sdk-python-ape-3.0.912/setup.py`

 * *Files identical despite different names*

