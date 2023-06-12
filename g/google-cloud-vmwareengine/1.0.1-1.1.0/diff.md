# Comparing `tmp/google-cloud-vmwareengine-1.0.1.tar.gz` & `tmp/google-cloud-vmwareengine-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-vmwareengine-1.0.1.tar", last modified: Mon Mar 27 14:58:46 2023, max compression
+gzip compressed data, was "google-cloud-vmwareengine-1.1.0.tar", last modified: Mon Jun 12 18:45:51 2023, max compression
```

## Comparing `google-cloud-vmwareengine-1.0.1.tar` & `google-cloud-vmwareengine-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4615 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3684 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.132944 google-cloud-vmwareengine-1.0.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.132944 google-cloud-vmwareengine-1.0.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.132944 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine/
--rw-rw-r--   0 root         (0)     1003     4059 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.132944 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/
--rw-rw-r--   0 root         (0)     1003     3877 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13039 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.132944 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.136945 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py
--rw-rw-r--   0 root         (0)     1003   209046 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py
--rw-rw-r--   0 root         (0)     1003   222571 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/client.py
--rw-rw-r--   0 root         (0)     1003    36985 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.136945 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    28127 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py
--rw-rw-r--   0 root         (0)     1003    60825 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    62028 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   205945 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.136945 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/types/
--rw-rw-r--   0 root         (0)     1003     3609 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    67319 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/types/vmwareengine.py
--rw-rw-r--   0 root         (0)     1003    35603 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/
--rw-r--r--   0 root         (0)     1003     4615 2023-03-27 14:58:46.000000 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1681 2023-03-27 14:58:46.000000 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:46.000000 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:58:46.000000 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:46.000000 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-03-27 14:58:46.000000 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:46.000000 google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2994 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:46.140945 google-cloud-vmwareengine-1.0.1/tests/unit/gapic/vmwareengine_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/tests/unit/gapic/vmwareengine_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   800296 2023-03-27 14:55:35.000000 google-cloud-vmwareengine-1.0.1/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4615 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3684 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.318116 google-cloud-vmwareengine-1.1.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.318116 google-cloud-vmwareengine-1.1.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/
+-rw-rw-r--   0 root         (0)     1003     4873 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/
+-rw-rw-r--   0 root         (0)     1003     4691 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16363 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.322115 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/
+-rw-rw-r--   0 root         (0)     1003      761 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py
+-rw-rw-r--   0 root         (0)     1003   254602 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py
+-rw-rw-r--   0 root         (0)     1003   268896 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/client.py
+-rw-rw-r--   0 root         (0)     1003    47957 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    33470 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    71402 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    72836 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   249912 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4423 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    83908 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine.py
+-rw-rw-r--   0 root         (0)     1003    48277 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/
+-rw-r--r--   0 root         (0)     1003     4615 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1681 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-12 18:45:51.000000 google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2994 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.326113 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-12 18:45:51.330111 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   986497 2023-06-12 18:42:57.000000 google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py
```

### Comparing `google-cloud-vmwareengine-1.0.1/LICENSE` & `google-cloud-vmwareengine-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/MANIFEST.in` & `google-cloud-vmwareengine-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/PKG-INFO` & `google-cloud-vmwareengine-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vmwareengine
-Version: 1.0.1
+Version: 1.1.0
 Summary: Google Cloud Vmwareengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vmwareengine-1.0.1/README.rst` & `google-cloud-vmwareengine-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine/__init__.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,131 +9,150 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.vmwareengine import gapic_version as package_version
+from google.cloud.vmwareengine_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.vmwareengine_v1.services.vmware_engine.async_client import (
-    VmwareEngineAsyncClient,
-)
-from google.cloud.vmwareengine_v1.services.vmware_engine.client import (
-    VmwareEngineClient,
-)
-from google.cloud.vmwareengine_v1.types.vmwareengine import (
+from .services.vmware_engine import VmwareEngineAsyncClient, VmwareEngineClient
+from .types.vmwareengine import (
     CreateClusterRequest,
     CreateHcxActivationKeyRequest,
     CreateNetworkPolicyRequest,
     CreatePrivateCloudRequest,
+    CreatePrivateConnectionRequest,
     CreateVmwareEngineNetworkRequest,
     DeleteClusterRequest,
     DeleteNetworkPolicyRequest,
     DeletePrivateCloudRequest,
+    DeletePrivateConnectionRequest,
     DeleteVmwareEngineNetworkRequest,
     GetClusterRequest,
     GetHcxActivationKeyRequest,
     GetNetworkPolicyRequest,
     GetNodeTypeRequest,
     GetPrivateCloudRequest,
+    GetPrivateConnectionRequest,
+    GetSubnetRequest,
     GetVmwareEngineNetworkRequest,
     ListClustersRequest,
     ListClustersResponse,
     ListHcxActivationKeysRequest,
     ListHcxActivationKeysResponse,
     ListNetworkPoliciesRequest,
     ListNetworkPoliciesResponse,
     ListNodeTypesRequest,
     ListNodeTypesResponse,
     ListPrivateCloudsRequest,
     ListPrivateCloudsResponse,
+    ListPrivateConnectionPeeringRoutesRequest,
+    ListPrivateConnectionPeeringRoutesResponse,
+    ListPrivateConnectionsRequest,
+    ListPrivateConnectionsResponse,
     ListSubnetsRequest,
     ListSubnetsResponse,
     ListVmwareEngineNetworksRequest,
     ListVmwareEngineNetworksResponse,
     OperationMetadata,
     ResetNsxCredentialsRequest,
     ResetVcenterCredentialsRequest,
     ShowNsxCredentialsRequest,
     ShowVcenterCredentialsRequest,
     UndeletePrivateCloudRequest,
     UpdateClusterRequest,
     UpdateNetworkPolicyRequest,
     UpdatePrivateCloudRequest,
+    UpdatePrivateConnectionRequest,
+    UpdateSubnetRequest,
     UpdateVmwareEngineNetworkRequest,
 )
-from google.cloud.vmwareengine_v1.types.vmwareengine_resources import (
+from .types.vmwareengine_resources import (
     Cluster,
     Credentials,
     Hcx,
     HcxActivationKey,
     NetworkConfig,
     NetworkPolicy,
     NodeType,
     NodeTypeConfig,
     Nsx,
+    PeeringRoute,
     PrivateCloud,
+    PrivateConnection,
     Subnet,
     Vcenter,
     VmwareEngineNetwork,
 )
 
 __all__ = (
-    "VmwareEngineClient",
     "VmwareEngineAsyncClient",
+    "Cluster",
     "CreateClusterRequest",
     "CreateHcxActivationKeyRequest",
     "CreateNetworkPolicyRequest",
     "CreatePrivateCloudRequest",
+    "CreatePrivateConnectionRequest",
     "CreateVmwareEngineNetworkRequest",
+    "Credentials",
     "DeleteClusterRequest",
     "DeleteNetworkPolicyRequest",
     "DeletePrivateCloudRequest",
+    "DeletePrivateConnectionRequest",
     "DeleteVmwareEngineNetworkRequest",
     "GetClusterRequest",
     "GetHcxActivationKeyRequest",
     "GetNetworkPolicyRequest",
     "GetNodeTypeRequest",
     "GetPrivateCloudRequest",
+    "GetPrivateConnectionRequest",
+    "GetSubnetRequest",
     "GetVmwareEngineNetworkRequest",
+    "Hcx",
+    "HcxActivationKey",
     "ListClustersRequest",
     "ListClustersResponse",
     "ListHcxActivationKeysRequest",
     "ListHcxActivationKeysResponse",
     "ListNetworkPoliciesRequest",
     "ListNetworkPoliciesResponse",
     "ListNodeTypesRequest",
     "ListNodeTypesResponse",
     "ListPrivateCloudsRequest",
     "ListPrivateCloudsResponse",
+    "ListPrivateConnectionPeeringRoutesRequest",
+    "ListPrivateConnectionPeeringRoutesResponse",
+    "ListPrivateConnectionsRequest",
+    "ListPrivateConnectionsResponse",
     "ListSubnetsRequest",
     "ListSubnetsResponse",
     "ListVmwareEngineNetworksRequest",
     "ListVmwareEngineNetworksResponse",
+    "NetworkConfig",
+    "NetworkPolicy",
+    "NodeType",
+    "NodeTypeConfig",
+    "Nsx",
     "OperationMetadata",
+    "PeeringRoute",
+    "PrivateCloud",
+    "PrivateConnection",
     "ResetNsxCredentialsRequest",
     "ResetVcenterCredentialsRequest",
     "ShowNsxCredentialsRequest",
     "ShowVcenterCredentialsRequest",
+    "Subnet",
     "UndeletePrivateCloudRequest",
     "UpdateClusterRequest",
     "UpdateNetworkPolicyRequest",
     "UpdatePrivateCloudRequest",
+    "UpdatePrivateConnectionRequest",
+    "UpdateSubnetRequest",
     "UpdateVmwareEngineNetworkRequest",
-    "Cluster",
-    "Credentials",
-    "Hcx",
-    "HcxActivationKey",
-    "NetworkConfig",
-    "NetworkPolicy",
-    "NodeType",
-    "NodeTypeConfig",
-    "Nsx",
-    "PrivateCloud",
-    "Subnet",
     "Vcenter",
+    "VmwareEngineClient",
     "VmwareEngineNetwork",
 )
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine/gapic_version.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "1.0.1"  # {x-release-please-version}
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/__init__.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,126 +9,142 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.vmwareengine_v1 import gapic_version as package_version
-
-__version__ = package_version.__version__
-
-
-from .services.vmware_engine import VmwareEngineAsyncClient, VmwareEngineClient
-from .types.vmwareengine import (
+from .vmwareengine import (
     CreateClusterRequest,
     CreateHcxActivationKeyRequest,
     CreateNetworkPolicyRequest,
     CreatePrivateCloudRequest,
+    CreatePrivateConnectionRequest,
     CreateVmwareEngineNetworkRequest,
     DeleteClusterRequest,
     DeleteNetworkPolicyRequest,
     DeletePrivateCloudRequest,
+    DeletePrivateConnectionRequest,
     DeleteVmwareEngineNetworkRequest,
     GetClusterRequest,
     GetHcxActivationKeyRequest,
     GetNetworkPolicyRequest,
     GetNodeTypeRequest,
     GetPrivateCloudRequest,
+    GetPrivateConnectionRequest,
+    GetSubnetRequest,
     GetVmwareEngineNetworkRequest,
     ListClustersRequest,
     ListClustersResponse,
     ListHcxActivationKeysRequest,
     ListHcxActivationKeysResponse,
     ListNetworkPoliciesRequest,
     ListNetworkPoliciesResponse,
     ListNodeTypesRequest,
     ListNodeTypesResponse,
     ListPrivateCloudsRequest,
     ListPrivateCloudsResponse,
+    ListPrivateConnectionPeeringRoutesRequest,
+    ListPrivateConnectionPeeringRoutesResponse,
+    ListPrivateConnectionsRequest,
+    ListPrivateConnectionsResponse,
     ListSubnetsRequest,
     ListSubnetsResponse,
     ListVmwareEngineNetworksRequest,
     ListVmwareEngineNetworksResponse,
     OperationMetadata,
     ResetNsxCredentialsRequest,
     ResetVcenterCredentialsRequest,
     ShowNsxCredentialsRequest,
     ShowVcenterCredentialsRequest,
     UndeletePrivateCloudRequest,
     UpdateClusterRequest,
     UpdateNetworkPolicyRequest,
     UpdatePrivateCloudRequest,
+    UpdatePrivateConnectionRequest,
+    UpdateSubnetRequest,
     UpdateVmwareEngineNetworkRequest,
 )
-from .types.vmwareengine_resources import (
+from .vmwareengine_resources import (
     Cluster,
     Credentials,
     Hcx,
     HcxActivationKey,
     NetworkConfig,
     NetworkPolicy,
     NodeType,
     NodeTypeConfig,
     Nsx,
+    PeeringRoute,
     PrivateCloud,
+    PrivateConnection,
     Subnet,
     Vcenter,
     VmwareEngineNetwork,
 )
 
 __all__ = (
-    "VmwareEngineAsyncClient",
-    "Cluster",
     "CreateClusterRequest",
     "CreateHcxActivationKeyRequest",
     "CreateNetworkPolicyRequest",
     "CreatePrivateCloudRequest",
+    "CreatePrivateConnectionRequest",
     "CreateVmwareEngineNetworkRequest",
-    "Credentials",
     "DeleteClusterRequest",
     "DeleteNetworkPolicyRequest",
     "DeletePrivateCloudRequest",
+    "DeletePrivateConnectionRequest",
     "DeleteVmwareEngineNetworkRequest",
     "GetClusterRequest",
     "GetHcxActivationKeyRequest",
     "GetNetworkPolicyRequest",
     "GetNodeTypeRequest",
     "GetPrivateCloudRequest",
+    "GetPrivateConnectionRequest",
+    "GetSubnetRequest",
     "GetVmwareEngineNetworkRequest",
-    "Hcx",
-    "HcxActivationKey",
     "ListClustersRequest",
     "ListClustersResponse",
     "ListHcxActivationKeysRequest",
     "ListHcxActivationKeysResponse",
     "ListNetworkPoliciesRequest",
     "ListNetworkPoliciesResponse",
     "ListNodeTypesRequest",
     "ListNodeTypesResponse",
     "ListPrivateCloudsRequest",
     "ListPrivateCloudsResponse",
+    "ListPrivateConnectionPeeringRoutesRequest",
+    "ListPrivateConnectionPeeringRoutesResponse",
+    "ListPrivateConnectionsRequest",
+    "ListPrivateConnectionsResponse",
     "ListSubnetsRequest",
     "ListSubnetsResponse",
     "ListVmwareEngineNetworksRequest",
     "ListVmwareEngineNetworksResponse",
-    "NetworkConfig",
-    "NetworkPolicy",
-    "NodeType",
-    "NodeTypeConfig",
-    "Nsx",
     "OperationMetadata",
-    "PrivateCloud",
     "ResetNsxCredentialsRequest",
     "ResetVcenterCredentialsRequest",
     "ShowNsxCredentialsRequest",
     "ShowVcenterCredentialsRequest",
-    "Subnet",
     "UndeletePrivateCloudRequest",
     "UpdateClusterRequest",
     "UpdateNetworkPolicyRequest",
     "UpdatePrivateCloudRequest",
+    "UpdatePrivateConnectionRequest",
+    "UpdateSubnetRequest",
     "UpdateVmwareEngineNetworkRequest",
+    "Cluster",
+    "Credentials",
+    "Hcx",
+    "HcxActivationKey",
+    "NetworkConfig",
+    "NetworkPolicy",
+    "NodeType",
+    "NodeTypeConfig",
+    "Nsx",
+    "PeeringRoute",
+    "PrivateCloud",
+    "PrivateConnection",
+    "Subnet",
     "Vcenter",
-    "VmwareEngineClient",
     "VmwareEngineNetwork",
 )
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/gapic_metadata.json` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/gapic_metadata.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994658119658121%*

 * *Differences: {"'services'": "{'VmwareEngine': {'clients': {'grpc': {'rpcs': {'CreatePrivateConnection': "*

 * *               "OrderedDict([('methods', ['create_private_connection'])]), "*

 * *               "'DeletePrivateConnection': OrderedDict([('methods', "*

 * *               "['delete_private_connection'])]), 'GetPrivateConnection': OrderedDict([('methods', "*

 * *               "['get_private_connection'])]), 'GetSubnet': OrderedDict([('methods', "*

 * *               "['get_subnet'])]), 'ListPrivateConnectionPeeringRoutes': OrderedDict […]*

```diff
@@ -26,14 +26,19 @@
                             ]
                         },
                         "CreatePrivateCloud": {
                             "methods": [
                                 "create_private_cloud"
                             ]
                         },
+                        "CreatePrivateConnection": {
+                            "methods": [
+                                "create_private_connection"
+                            ]
+                        },
                         "CreateVmwareEngineNetwork": {
                             "methods": [
                                 "create_vmware_engine_network"
                             ]
                         },
                         "DeleteCluster": {
                             "methods": [
@@ -46,14 +51,19 @@
                             ]
                         },
                         "DeletePrivateCloud": {
                             "methods": [
                                 "delete_private_cloud"
                             ]
                         },
+                        "DeletePrivateConnection": {
+                            "methods": [
+                                "delete_private_connection"
+                            ]
+                        },
                         "DeleteVmwareEngineNetwork": {
                             "methods": [
                                 "delete_vmware_engine_network"
                             ]
                         },
                         "GetCluster": {
                             "methods": [
@@ -76,14 +86,24 @@
                             ]
                         },
                         "GetPrivateCloud": {
                             "methods": [
                                 "get_private_cloud"
                             ]
                         },
+                        "GetPrivateConnection": {
+                            "methods": [
+                                "get_private_connection"
+                            ]
+                        },
+                        "GetSubnet": {
+                            "methods": [
+                                "get_subnet"
+                            ]
+                        },
                         "GetVmwareEngineNetwork": {
                             "methods": [
                                 "get_vmware_engine_network"
                             ]
                         },
                         "ListClusters": {
                             "methods": [
@@ -106,14 +126,24 @@
                             ]
                         },
                         "ListPrivateClouds": {
                             "methods": [
                                 "list_private_clouds"
                             ]
                         },
+                        "ListPrivateConnectionPeeringRoutes": {
+                            "methods": [
+                                "list_private_connection_peering_routes"
+                            ]
+                        },
+                        "ListPrivateConnections": {
+                            "methods": [
+                                "list_private_connections"
+                            ]
+                        },
                         "ListSubnets": {
                             "methods": [
                                 "list_subnets"
                             ]
                         },
                         "ListVmwareEngineNetworks": {
                             "methods": [
@@ -156,14 +186,24 @@
                             ]
                         },
                         "UpdatePrivateCloud": {
                             "methods": [
                                 "update_private_cloud"
                             ]
                         },
+                        "UpdatePrivateConnection": {
+                            "methods": [
+                                "update_private_connection"
+                            ]
+                        },
+                        "UpdateSubnet": {
+                            "methods": [
+                                "update_subnet"
+                            ]
+                        },
                         "UpdateVmwareEngineNetwork": {
                             "methods": [
                                 "update_vmware_engine_network"
                             ]
                         }
                     }
                 },
@@ -186,14 +226,19 @@
                             ]
                         },
                         "CreatePrivateCloud": {
                             "methods": [
                                 "create_private_cloud"
                             ]
                         },
+                        "CreatePrivateConnection": {
+                            "methods": [
+                                "create_private_connection"
+                            ]
+                        },
                         "CreateVmwareEngineNetwork": {
                             "methods": [
                                 "create_vmware_engine_network"
                             ]
                         },
                         "DeleteCluster": {
                             "methods": [
@@ -206,14 +251,19 @@
                             ]
                         },
                         "DeletePrivateCloud": {
                             "methods": [
                                 "delete_private_cloud"
                             ]
                         },
+                        "DeletePrivateConnection": {
+                            "methods": [
+                                "delete_private_connection"
+                            ]
+                        },
                         "DeleteVmwareEngineNetwork": {
                             "methods": [
                                 "delete_vmware_engine_network"
                             ]
                         },
                         "GetCluster": {
                             "methods": [
@@ -236,14 +286,24 @@
                             ]
                         },
                         "GetPrivateCloud": {
                             "methods": [
                                 "get_private_cloud"
                             ]
                         },
+                        "GetPrivateConnection": {
+                            "methods": [
+                                "get_private_connection"
+                            ]
+                        },
+                        "GetSubnet": {
+                            "methods": [
+                                "get_subnet"
+                            ]
+                        },
                         "GetVmwareEngineNetwork": {
                             "methods": [
                                 "get_vmware_engine_network"
                             ]
                         },
                         "ListClusters": {
                             "methods": [
@@ -266,14 +326,24 @@
                             ]
                         },
                         "ListPrivateClouds": {
                             "methods": [
                                 "list_private_clouds"
                             ]
                         },
+                        "ListPrivateConnectionPeeringRoutes": {
+                            "methods": [
+                                "list_private_connection_peering_routes"
+                            ]
+                        },
+                        "ListPrivateConnections": {
+                            "methods": [
+                                "list_private_connections"
+                            ]
+                        },
                         "ListSubnets": {
                             "methods": [
                                 "list_subnets"
                             ]
                         },
                         "ListVmwareEngineNetworks": {
                             "methods": [
@@ -316,14 +386,24 @@
                             ]
                         },
                         "UpdatePrivateCloud": {
                             "methods": [
                                 "update_private_cloud"
                             ]
                         },
+                        "UpdatePrivateConnection": {
+                            "methods": [
+                                "update_private_connection"
+                            ]
+                        },
+                        "UpdateSubnet": {
+                            "methods": [
+                                "update_subnet"
+                            ]
+                        },
                         "UpdateVmwareEngineNetwork": {
                             "methods": [
                                 "update_vmware_engine_network"
                             ]
                         }
                     }
                 },
@@ -346,14 +426,19 @@
                             ]
                         },
                         "CreatePrivateCloud": {
                             "methods": [
                                 "create_private_cloud"
                             ]
                         },
+                        "CreatePrivateConnection": {
+                            "methods": [
+                                "create_private_connection"
+                            ]
+                        },
                         "CreateVmwareEngineNetwork": {
                             "methods": [
                                 "create_vmware_engine_network"
                             ]
                         },
                         "DeleteCluster": {
                             "methods": [
@@ -366,14 +451,19 @@
                             ]
                         },
                         "DeletePrivateCloud": {
                             "methods": [
                                 "delete_private_cloud"
                             ]
                         },
+                        "DeletePrivateConnection": {
+                            "methods": [
+                                "delete_private_connection"
+                            ]
+                        },
                         "DeleteVmwareEngineNetwork": {
                             "methods": [
                                 "delete_vmware_engine_network"
                             ]
                         },
                         "GetCluster": {
                             "methods": [
@@ -396,14 +486,24 @@
                             ]
                         },
                         "GetPrivateCloud": {
                             "methods": [
                                 "get_private_cloud"
                             ]
                         },
+                        "GetPrivateConnection": {
+                            "methods": [
+                                "get_private_connection"
+                            ]
+                        },
+                        "GetSubnet": {
+                            "methods": [
+                                "get_subnet"
+                            ]
+                        },
                         "GetVmwareEngineNetwork": {
                             "methods": [
                                 "get_vmware_engine_network"
                             ]
                         },
                         "ListClusters": {
                             "methods": [
@@ -426,14 +526,24 @@
                             ]
                         },
                         "ListPrivateClouds": {
                             "methods": [
                                 "list_private_clouds"
                             ]
                         },
+                        "ListPrivateConnectionPeeringRoutes": {
+                            "methods": [
+                                "list_private_connection_peering_routes"
+                            ]
+                        },
+                        "ListPrivateConnections": {
+                            "methods": [
+                                "list_private_connections"
+                            ]
+                        },
                         "ListSubnets": {
                             "methods": [
                                 "list_subnets"
                             ]
                         },
                         "ListVmwareEngineNetworks": {
                             "methods": [
@@ -476,14 +586,24 @@
                             ]
                         },
                         "UpdatePrivateCloud": {
                             "methods": [
                                 "update_private_cloud"
                             ]
                         },
+                        "UpdatePrivateConnection": {
+                            "methods": [
+                                "update_private_connection"
+                            ]
+                        },
+                        "UpdateSubnet": {
+                            "methods": [
+                                "update_subnet"
+                            ]
+                        },
                         "UpdateVmwareEngineNetwork": {
                             "methods": [
                                 "update_vmware_engine_network"
                             ]
                         }
                     }
                 }
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/gapic_version.py` & `google-cloud-vmwareengine-1.1.0/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "1.0.1"  # {x-release-please-version}
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/__init__.py` & `google-cloud-vmwareengine-1.1.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/async_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,14 +80,18 @@
     parse_network_policy_path = staticmethod(
         VmwareEngineClient.parse_network_policy_path
     )
     node_type_path = staticmethod(VmwareEngineClient.node_type_path)
     parse_node_type_path = staticmethod(VmwareEngineClient.parse_node_type_path)
     private_cloud_path = staticmethod(VmwareEngineClient.private_cloud_path)
     parse_private_cloud_path = staticmethod(VmwareEngineClient.parse_private_cloud_path)
+    private_connection_path = staticmethod(VmwareEngineClient.private_connection_path)
+    parse_private_connection_path = staticmethod(
+        VmwareEngineClient.parse_private_connection_path
+    )
     subnet_path = staticmethod(VmwareEngineClient.subnet_path)
     parse_subnet_path = staticmethod(VmwareEngineClient.parse_subnet_path)
     vmware_engine_network_path = staticmethod(
         VmwareEngineClient.vmware_engine_network_path
     )
     parse_vmware_engine_network_path = staticmethod(
         VmwareEngineClient.parse_vmware_engine_network_path
@@ -1851,14 +1855,265 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    async def get_subnet(
+        self,
+        request: Optional[Union[vmwareengine.GetSubnetRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> vmwareengine_resources.Subnet:
+        r"""Gets details of a single subnet.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_get_subnet():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.GetSubnetRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = await client.get_subnet(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.GetSubnetRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.GetSubnet][google.cloud.vmwareengine.v1.VmwareEngine.GetSubnet]
+            name (:class:`str`):
+                Required. The resource name of the subnet to retrieve.
+                Resource names are schemeless URIs that follow the
+                conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-central1-a/privateClouds/my-cloud/subnets/my-subnet``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.types.Subnet:
+                Subnet in a private cloud. Either management subnets (such as vMotion) that
+                   are read-only, or userDefined, which can also be
+                   updated.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.GetSubnetRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.get_subnet,
+            default_retry=retries.Retry(
+                initial=1.0,
+                maximum=10.0,
+                multiplier=1.3,
+                predicate=retries.if_exception_type(
+                    core_exceptions.ServiceUnavailable,
+                ),
+                deadline=120.0,
+            ),
+            default_timeout=120.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def update_subnet(
+        self,
+        request: Optional[Union[vmwareengine.UpdateSubnetRequest, dict]] = None,
+        *,
+        subnet: Optional[vmwareengine_resources.Subnet] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""Updates the parameters of a single subnet. Only fields specified
+        in ``update_mask`` are applied.
+
+        *Note*: This API is synchronous and always returns a successful
+        ``google.longrunning.Operation`` (LRO). The returned LRO will
+        only have ``done`` and ``response`` fields.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_update_subnet():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.UpdateSubnetRequest(
+                )
+
+                # Make the request
+                operation = client.update_subnet(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.UpdateSubnetRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.UpdateSubnet][google.cloud.vmwareengine.v1.VmwareEngine.UpdateSubnet]
+            subnet (:class:`google.cloud.vmwareengine_v1.types.Subnet`):
+                Required. Subnet description.
+                This corresponds to the ``subnet`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
+                Required. Field mask is used to specify the fields to be
+                overwritten in the ``Subnet`` resource by the update.
+                The fields specified in the ``update_mask`` are relative
+                to the resource, not the full request. A field will be
+                overwritten if it is in the mask. If the user does not
+                provide a mask then all fields will be overwritten.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.vmwareengine_v1.types.Subnet` Subnet in a private cloud. Either management subnets (such as vMotion) that
+                   are read-only, or userDefined, which can also be
+                   updated.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([subnet, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.UpdateSubnetRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if subnet is not None:
+            request.subnet = subnet
+        if update_mask is not None:
+            request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.update_subnet,
+            default_timeout=60.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("subnet.name", request.subnet.name),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            vmwareengine_resources.Subnet,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def list_node_types(
         self,
         request: Optional[Union[vmwareengine.ListNodeTypesRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
@@ -4384,14 +4639,829 @@
             method=rpc,
             request=request,
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
+        return response
+
+    async def create_private_connection(
+        self,
+        request: Optional[
+            Union[vmwareengine.CreatePrivateConnectionRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        private_connection: Optional[vmwareengine_resources.PrivateConnection] = None,
+        private_connection_id: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""Creates a new private connection that can be used for
+        accessing private Clouds.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_create_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                private_connection = vmwareengine_v1.PrivateConnection()
+                private_connection.vmware_engine_network = "vmware_engine_network_value"
+                private_connection.type_ = "THIRD_PARTY_SERVICE"
+                private_connection.service_network = "service_network_value"
+
+                request = vmwareengine_v1.CreatePrivateConnectionRequest(
+                    parent="parent_value",
+                    private_connection_id="private_connection_id_value",
+                    private_connection=private_connection,
+                )
+
+                # Make the request
+                operation = client.create_private_connection(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.CreatePrivateConnectionRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.CreatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.CreatePrivateConnection]
+            parent (:class:`str`):
+                Required. The resource name of the location to create
+                the new private connection in. Private connection is a
+                regional resource. Resource names are schemeless URIs
+                that follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example: ``projects/my-project/locations/us-central1``
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            private_connection (:class:`google.cloud.vmwareengine_v1.types.PrivateConnection`):
+                Required. The initial description of
+                the new private connection.
+
+                This corresponds to the ``private_connection`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            private_connection_id (:class:`str`):
+                Required. The user-provided identifier of the new
+                private connection. This identifier must be unique among
+                private connection resources within the parent and
+                becomes the final token in the name URI. The identifier
+                must meet the following requirements:
+
+                -  Only contains 1-63 alphanumeric characters and
+                   hyphens
+                -  Begins with an alphabetical character
+                -  Ends with a non-hyphen character
+                -  Not formatted as a UUID
+                -  Complies with `RFC
+                   1034 <https://datatracker.ietf.org/doc/html/rfc1034>`__
+                   (section 3.5)
+
+                This corresponds to the ``private_connection_id`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.vmwareengine_v1.types.PrivateConnection` Private connection resource that provides connectivity for VMware Engine
+                   private clouds.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent, private_connection, private_connection_id])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.CreatePrivateConnectionRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+        if private_connection is not None:
+            request.private_connection = private_connection
+        if private_connection_id is not None:
+            request.private_connection_id = private_connection_id
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.create_private_connection,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            vmwareengine_resources.PrivateConnection,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_private_connection(
+        self,
+        request: Optional[Union[vmwareengine.GetPrivateConnectionRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> vmwareengine_resources.PrivateConnection:
+        r"""Retrieves a ``PrivateConnection`` resource by its resource name.
+        The resource contains details of the private connection, such as
+        connected network, routing mode and state.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_get_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.GetPrivateConnectionRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = await client.get_private_connection(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.GetPrivateConnectionRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.GetPrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.GetPrivateConnection]
+            name (:class:`str`):
+                Required. The resource name of the private connection to
+                retrieve. Resource names are schemeless URIs that follow
+                the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-central1/privateConnections/my-connection``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.types.PrivateConnection:
+                Private connection resource that
+                provides connectivity for VMware Engine
+                private clouds.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.GetPrivateConnectionRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.get_private_connection,
+            default_retry=retries.Retry(
+                initial=1.0,
+                maximum=10.0,
+                multiplier=1.3,
+                predicate=retries.if_exception_type(
+                    core_exceptions.ServiceUnavailable,
+                ),
+                deadline=120.0,
+            ),
+            default_timeout=120.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_private_connections(
+        self,
+        request: Optional[
+            Union[vmwareengine.ListPrivateConnectionsRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListPrivateConnectionsAsyncPager:
+        r"""Lists ``PrivateConnection`` resources in a given project and
+        location.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_list_private_connections():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.ListPrivateConnectionsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_private_connections(request=request)
+
+                # Handle the response
+                async for response in page_result:
+                    print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.ListPrivateConnectionsRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+            parent (:class:`str`):
+                Required. The resource name of the location to query for
+                private connections. Resource names are schemeless URIs
+                that follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example: ``projects/my-project/locations/us-central1``
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.services.vmware_engine.pagers.ListPrivateConnectionsAsyncPager:
+                Response message for
+                   [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+
+                Iterating over this object will yield results and
+                resolve additional pages automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.ListPrivateConnectionsRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.list_private_connections,
+            default_retry=retries.Retry(
+                initial=1.0,
+                maximum=10.0,
+                multiplier=1.3,
+                predicate=retries.if_exception_type(
+                    core_exceptions.ServiceUnavailable,
+                ),
+                deadline=120.0,
+            ),
+            default_timeout=120.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__aiter__` convenience method.
+        response = pagers.ListPrivateConnectionsAsyncPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def update_private_connection(
+        self,
+        request: Optional[
+            Union[vmwareengine.UpdatePrivateConnectionRequest, dict]
+        ] = None,
+        *,
+        private_connection: Optional[vmwareengine_resources.PrivateConnection] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""Modifies a ``PrivateConnection`` resource. Only ``description``
+        and ``routing_mode`` fields can be updated. Only fields
+        specified in ``updateMask`` are applied.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_update_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                private_connection = vmwareengine_v1.PrivateConnection()
+                private_connection.vmware_engine_network = "vmware_engine_network_value"
+                private_connection.type_ = "THIRD_PARTY_SERVICE"
+                private_connection.service_network = "service_network_value"
+
+                request = vmwareengine_v1.UpdatePrivateConnectionRequest(
+                    private_connection=private_connection,
+                )
+
+                # Make the request
+                operation = client.update_private_connection(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.UpdatePrivateConnectionRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.UpdatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.UpdatePrivateConnection]
+            private_connection (:class:`google.cloud.vmwareengine_v1.types.PrivateConnection`):
+                Required. Private connection
+                description.
+
+                This corresponds to the ``private_connection`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
+                Required. Field mask is used to specify the fields to be
+                overwritten in the ``PrivateConnection`` resource by the
+                update. The fields specified in the ``update_mask`` are
+                relative to the resource, not the full request. A field
+                will be overwritten if it is in the mask. If the user
+                does not provide a mask then all fields will be
+                overwritten.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.vmwareengine_v1.types.PrivateConnection` Private connection resource that provides connectivity for VMware Engine
+                   private clouds.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([private_connection, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.UpdatePrivateConnectionRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if private_connection is not None:
+            request.private_connection = private_connection
+        if update_mask is not None:
+            request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.update_private_connection,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("private_connection.name", request.private_connection.name),)
+            ),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            vmwareengine_resources.PrivateConnection,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def delete_private_connection(
+        self,
+        request: Optional[
+            Union[vmwareengine.DeletePrivateConnectionRequest, dict]
+        ] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation_async.AsyncOperation:
+        r"""Deletes a ``PrivateConnection`` resource. When a private
+        connection is deleted for a VMware Engine network, the connected
+        network becomes inaccessible to that VMware Engine network.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_delete_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.DeletePrivateConnectionRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                operation = client.delete_private_connection(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = (await operation).result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.DeletePrivateConnectionRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.DeletePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.DeletePrivateConnection]
+            name (:class:`str`):
+                Required. The resource name of the private connection to
+                be deleted. Resource names are schemeless URIs that
+                follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-central1/privateConnections/my-connection``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation_async.AsyncOperation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.protobuf.empty_pb2.Empty` A generic empty message that you can re-use to avoid defining duplicated
+                   empty messages in your APIs. A typical example is to
+                   use it as the request or the response type of an API
+                   method. For instance:
+
+                      service Foo {
+                         rpc Bar(google.protobuf.Empty) returns
+                         (google.protobuf.Empty);
+
+                      }
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.DeletePrivateConnectionRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.delete_private_connection,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation_async.from_gapic(
+            response,
+            self._client._transport.operations_client,
+            empty_pb2.Empty,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_private_connection_peering_routes(
+        self,
+        request: Optional[
+            Union[vmwareengine.ListPrivateConnectionPeeringRoutesRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListPrivateConnectionPeeringRoutesAsyncPager:
+        r"""Lists the private connection routes exchanged over a
+        peering connection.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            async def sample_list_private_connection_peering_routes():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineAsyncClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.ListPrivateConnectionPeeringRoutesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_private_connection_peering_routes(request=request)
+
+                # Handle the response
+                async for response in page_result:
+                    print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesRequest, dict]]):
+                The request object. Request message for
+                [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+            parent (:class:`str`):
+                Required. The resource name of the private connection to
+                retrieve peering routes from. Resource names are
+                schemeless URIs that follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-west1/privateConnections/my-connection``
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.services.vmware_engine.pagers.ListPrivateConnectionPeeringRoutesAsyncPager:
+                Response message for
+                   [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+
+                Iterating over this object will yield results and
+                resolve additional pages automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.list_private_connection_peering_routes,
+            default_retry=retries.Retry(
+                initial=1.0,
+                maximum=10.0,
+                multiplier=1.3,
+                predicate=retries.if_exception_type(
+                    core_exceptions.ServiceUnavailable,
+                ),
+                deadline=120.0,
+            ),
+            default_timeout=120.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__aiter__` convenience method.
+        response = pagers.ListPrivateConnectionPeeringRoutesAsyncPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
         return response
 
     async def list_operations(
         self,
         request: Optional[operations_pb2.ListOperationsRequest] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/client.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -315,14 +315,36 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/privateClouds/(?P<private_cloud>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def private_connection_path(
+        project: str,
+        location: str,
+        private_connection: str,
+    ) -> str:
+        """Returns a fully-qualified private_connection string."""
+        return "projects/{project}/locations/{location}/privateConnections/{private_connection}".format(
+            project=project,
+            location=location,
+            private_connection=private_connection,
+        )
+
+    @staticmethod
+    def parse_private_connection_path(path: str) -> Dict[str, str]:
+        """Parses a private_connection path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/privateConnections/(?P<private_connection>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def subnet_path(
         project: str,
         location: str,
         private_cloud: str,
         subnet: str,
     ) -> str:
         """Returns a fully-qualified subnet string."""
@@ -2172,14 +2194,256 @@
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    def get_subnet(
+        self,
+        request: Optional[Union[vmwareengine.GetSubnetRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> vmwareengine_resources.Subnet:
+        r"""Gets details of a single subnet.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_get_subnet():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.GetSubnetRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_subnet(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.GetSubnetRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.GetSubnet][google.cloud.vmwareengine.v1.VmwareEngine.GetSubnet]
+            name (str):
+                Required. The resource name of the subnet to retrieve.
+                Resource names are schemeless URIs that follow the
+                conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-central1-a/privateClouds/my-cloud/subnets/my-subnet``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.types.Subnet:
+                Subnet in a private cloud. Either management subnets (such as vMotion) that
+                   are read-only, or userDefined, which can also be
+                   updated.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.GetSubnetRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, vmwareengine.GetSubnetRequest):
+            request = vmwareengine.GetSubnetRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.get_subnet]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def update_subnet(
+        self,
+        request: Optional[Union[vmwareengine.UpdateSubnetRequest, dict]] = None,
+        *,
+        subnet: Optional[vmwareengine_resources.Subnet] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Updates the parameters of a single subnet. Only fields specified
+        in ``update_mask`` are applied.
+
+        *Note*: This API is synchronous and always returns a successful
+        ``google.longrunning.Operation`` (LRO). The returned LRO will
+        only have ``done`` and ``response`` fields.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_update_subnet():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.UpdateSubnetRequest(
+                )
+
+                # Make the request
+                operation = client.update_subnet(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.UpdateSubnetRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.UpdateSubnet][google.cloud.vmwareengine.v1.VmwareEngine.UpdateSubnet]
+            subnet (google.cloud.vmwareengine_v1.types.Subnet):
+                Required. Subnet description.
+                This corresponds to the ``subnet`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                Required. Field mask is used to specify the fields to be
+                overwritten in the ``Subnet`` resource by the update.
+                The fields specified in the ``update_mask`` are relative
+                to the resource, not the full request. A field will be
+                overwritten if it is in the mask. If the user does not
+                provide a mask then all fields will be overwritten.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.vmwareengine_v1.types.Subnet` Subnet in a private cloud. Either management subnets (such as vMotion) that
+                   are read-only, or userDefined, which can also be
+                   updated.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([subnet, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.UpdateSubnetRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, vmwareengine.UpdateSubnetRequest):
+            request = vmwareengine.UpdateSubnetRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if subnet is not None:
+                request.subnet = subnet
+            if update_mask is not None:
+                request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.update_subnet]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("subnet.name", request.subnet.name),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            vmwareengine_resources.Subnet,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def list_node_types(
         self,
         request: Optional[Union[vmwareengine.ListNodeTypesRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
@@ -4629,14 +4893,812 @@
             method=rpc,
             request=request,
             response=response,
             metadata=metadata,
         )
 
         # Done; return the response.
+        return response
+
+    def create_private_connection(
+        self,
+        request: Optional[
+            Union[vmwareengine.CreatePrivateConnectionRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        private_connection: Optional[vmwareengine_resources.PrivateConnection] = None,
+        private_connection_id: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Creates a new private connection that can be used for
+        accessing private Clouds.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_create_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                private_connection = vmwareengine_v1.PrivateConnection()
+                private_connection.vmware_engine_network = "vmware_engine_network_value"
+                private_connection.type_ = "THIRD_PARTY_SERVICE"
+                private_connection.service_network = "service_network_value"
+
+                request = vmwareengine_v1.CreatePrivateConnectionRequest(
+                    parent="parent_value",
+                    private_connection_id="private_connection_id_value",
+                    private_connection=private_connection,
+                )
+
+                # Make the request
+                operation = client.create_private_connection(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.CreatePrivateConnectionRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.CreatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.CreatePrivateConnection]
+            parent (str):
+                Required. The resource name of the location to create
+                the new private connection in. Private connection is a
+                regional resource. Resource names are schemeless URIs
+                that follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example: ``projects/my-project/locations/us-central1``
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            private_connection (google.cloud.vmwareengine_v1.types.PrivateConnection):
+                Required. The initial description of
+                the new private connection.
+
+                This corresponds to the ``private_connection`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            private_connection_id (str):
+                Required. The user-provided identifier of the new
+                private connection. This identifier must be unique among
+                private connection resources within the parent and
+                becomes the final token in the name URI. The identifier
+                must meet the following requirements:
+
+                -  Only contains 1-63 alphanumeric characters and
+                   hyphens
+                -  Begins with an alphabetical character
+                -  Ends with a non-hyphen character
+                -  Not formatted as a UUID
+                -  Complies with `RFC
+                   1034 <https://datatracker.ietf.org/doc/html/rfc1034>`__
+                   (section 3.5)
+
+                This corresponds to the ``private_connection_id`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.vmwareengine_v1.types.PrivateConnection` Private connection resource that provides connectivity for VMware Engine
+                   private clouds.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent, private_connection, private_connection_id])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.CreatePrivateConnectionRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, vmwareengine.CreatePrivateConnectionRequest):
+            request = vmwareengine.CreatePrivateConnectionRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+            if private_connection is not None:
+                request.private_connection = private_connection
+            if private_connection_id is not None:
+                request.private_connection_id = private_connection_id
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.create_private_connection
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            vmwareengine_resources.PrivateConnection,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def get_private_connection(
+        self,
+        request: Optional[Union[vmwareengine.GetPrivateConnectionRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> vmwareengine_resources.PrivateConnection:
+        r"""Retrieves a ``PrivateConnection`` resource by its resource name.
+        The resource contains details of the private connection, such as
+        connected network, routing mode and state.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_get_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.GetPrivateConnectionRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_private_connection(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.GetPrivateConnectionRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.GetPrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.GetPrivateConnection]
+            name (str):
+                Required. The resource name of the private connection to
+                retrieve. Resource names are schemeless URIs that follow
+                the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-central1/privateConnections/my-connection``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.types.PrivateConnection:
+                Private connection resource that
+                provides connectivity for VMware Engine
+                private clouds.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.GetPrivateConnectionRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, vmwareengine.GetPrivateConnectionRequest):
+            request = vmwareengine.GetPrivateConnectionRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.get_private_connection]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_private_connections(
+        self,
+        request: Optional[
+            Union[vmwareengine.ListPrivateConnectionsRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListPrivateConnectionsPager:
+        r"""Lists ``PrivateConnection`` resources in a given project and
+        location.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_list_private_connections():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.ListPrivateConnectionsRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_private_connections(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.ListPrivateConnectionsRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+            parent (str):
+                Required. The resource name of the location to query for
+                private connections. Resource names are schemeless URIs
+                that follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example: ``projects/my-project/locations/us-central1``
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.services.vmware_engine.pagers.ListPrivateConnectionsPager:
+                Response message for
+                   [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+
+                Iterating over this object will yield results and
+                resolve additional pages automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.ListPrivateConnectionsRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, vmwareengine.ListPrivateConnectionsRequest):
+            request = vmwareengine.ListPrivateConnectionsRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.list_private_connections]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__iter__` convenience method.
+        response = pagers.ListPrivateConnectionsPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def update_private_connection(
+        self,
+        request: Optional[
+            Union[vmwareengine.UpdatePrivateConnectionRequest, dict]
+        ] = None,
+        *,
+        private_connection: Optional[vmwareengine_resources.PrivateConnection] = None,
+        update_mask: Optional[field_mask_pb2.FieldMask] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Modifies a ``PrivateConnection`` resource. Only ``description``
+        and ``routing_mode`` fields can be updated. Only fields
+        specified in ``updateMask`` are applied.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_update_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                private_connection = vmwareengine_v1.PrivateConnection()
+                private_connection.vmware_engine_network = "vmware_engine_network_value"
+                private_connection.type_ = "THIRD_PARTY_SERVICE"
+                private_connection.service_network = "service_network_value"
+
+                request = vmwareengine_v1.UpdatePrivateConnectionRequest(
+                    private_connection=private_connection,
+                )
+
+                # Make the request
+                operation = client.update_private_connection(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.UpdatePrivateConnectionRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.UpdatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.UpdatePrivateConnection]
+            private_connection (google.cloud.vmwareengine_v1.types.PrivateConnection):
+                Required. Private connection
+                description.
+
+                This corresponds to the ``private_connection`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            update_mask (google.protobuf.field_mask_pb2.FieldMask):
+                Required. Field mask is used to specify the fields to be
+                overwritten in the ``PrivateConnection`` resource by the
+                update. The fields specified in the ``update_mask`` are
+                relative to the resource, not the full request. A field
+                will be overwritten if it is in the mask. If the user
+                does not provide a mask then all fields will be
+                overwritten.
+
+                This corresponds to the ``update_mask`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.cloud.vmwareengine_v1.types.PrivateConnection` Private connection resource that provides connectivity for VMware Engine
+                   private clouds.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([private_connection, update_mask])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.UpdatePrivateConnectionRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, vmwareengine.UpdatePrivateConnectionRequest):
+            request = vmwareengine.UpdatePrivateConnectionRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if private_connection is not None:
+                request.private_connection = private_connection
+            if update_mask is not None:
+                request.update_mask = update_mask
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.update_private_connection
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(
+                (("private_connection.name", request.private_connection.name),)
+            ),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            vmwareengine_resources.PrivateConnection,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def delete_private_connection(
+        self,
+        request: Optional[
+            Union[vmwareengine.DeletePrivateConnectionRequest, dict]
+        ] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operation.Operation:
+        r"""Deletes a ``PrivateConnection`` resource. When a private
+        connection is deleted for a VMware Engine network, the connected
+        network becomes inaccessible to that VMware Engine network.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_delete_private_connection():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.DeletePrivateConnectionRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                operation = client.delete_private_connection(request=request)
+
+                print("Waiting for operation to complete...")
+
+                response = operation.result()
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.DeletePrivateConnectionRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.DeletePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.DeletePrivateConnection]
+            name (str):
+                Required. The resource name of the private connection to
+                be deleted. Resource names are schemeless URIs that
+                follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-central1/privateConnections/my-connection``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.api_core.operation.Operation:
+                An object representing a long-running operation.
+
+                The result type for the operation will be :class:`google.protobuf.empty_pb2.Empty` A generic empty message that you can re-use to avoid defining duplicated
+                   empty messages in your APIs. A typical example is to
+                   use it as the request or the response type of an API
+                   method. For instance:
+
+                      service Foo {
+                         rpc Bar(google.protobuf.Empty) returns
+                         (google.protobuf.Empty);
+
+                      }
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.DeletePrivateConnectionRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, vmwareengine.DeletePrivateConnectionRequest):
+            request = vmwareengine.DeletePrivateConnectionRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.delete_private_connection
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Wrap the response in an operation future.
+        response = operation.from_gapic(
+            response,
+            self._transport.operations_client,
+            empty_pb2.Empty,
+            metadata_type=vmwareengine.OperationMetadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_private_connection_peering_routes(
+        self,
+        request: Optional[
+            Union[vmwareengine.ListPrivateConnectionPeeringRoutesRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListPrivateConnectionPeeringRoutesPager:
+        r"""Lists the private connection routes exchanged over a
+        peering connection.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import vmwareengine_v1
+
+            def sample_list_private_connection_peering_routes():
+                # Create a client
+                client = vmwareengine_v1.VmwareEngineClient()
+
+                # Initialize request argument(s)
+                request = vmwareengine_v1.ListPrivateConnectionPeeringRoutesRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_private_connection_peering_routes(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
+        Args:
+            request (Union[google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesRequest, dict]):
+                The request object. Request message for
+                [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+            parent (str):
+                Required. The resource name of the private connection to
+                retrieve peering routes from. Resource names are
+                schemeless URIs that follow the conventions in
+                https://cloud.google.com/apis/design/resource_names. For
+                example:
+                ``projects/my-project/locations/us-west1/privateConnections/my-connection``
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.vmwareengine_v1.services.vmware_engine.pagers.ListPrivateConnectionPeeringRoutesPager:
+                Response message for
+                   [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+
+                Iterating over this object will yield results and
+                resolve additional pages automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a vmwareengine.ListPrivateConnectionPeeringRoutesRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(
+            request, vmwareengine.ListPrivateConnectionPeeringRoutesRequest
+        ):
+            request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[
+            self._transport.list_private_connection_peering_routes
+        ]
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__iter__` convenience method.
+        response = pagers.ListPrivateConnectionPeeringRoutesPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
         return response
 
     def __enter__(self) -> "VmwareEngineClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/pagers.py`

 * *Files 14% similar despite different names*

```diff
@@ -919,7 +919,269 @@
                 for response in page.vmware_engine_networks:
                     yield response
 
         return async_generator()
 
     def __repr__(self) -> str:
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
+
+
+class ListPrivateConnectionsPager:
+    """A pager for iterating through ``list_private_connections`` requests.
+
+    This class thinly wraps an initial
+    :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionsResponse` object, and
+    provides an ``__iter__`` method to iterate through its
+    ``private_connections`` field.
+
+    If there are more pages, the ``__iter__`` method will make additional
+    ``ListPrivateConnections`` requests and continue to iterate
+    through the ``private_connections`` field on the
+    corresponding responses.
+
+    All the usual :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionsResponse`
+    attributes are available on the pager. If multiple requests are made, only
+    the most recent response is retained, and thus used for attribute lookup.
+    """
+
+    def __init__(
+        self,
+        method: Callable[..., vmwareengine.ListPrivateConnectionsResponse],
+        request: vmwareengine.ListPrivateConnectionsRequest,
+        response: vmwareengine.ListPrivateConnectionsResponse,
+        *,
+        metadata: Sequence[Tuple[str, str]] = ()
+    ):
+        """Instantiate the pager.
+
+        Args:
+            method (Callable): The method that was originally called, and
+                which instantiated this pager.
+            request (google.cloud.vmwareengine_v1.types.ListPrivateConnectionsRequest):
+                The initial request object.
+            response (google.cloud.vmwareengine_v1.types.ListPrivateConnectionsResponse):
+                The initial response object.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        self._method = method
+        self._request = vmwareengine.ListPrivateConnectionsRequest(request)
+        self._response = response
+        self._metadata = metadata
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self._response, name)
+
+    @property
+    def pages(self) -> Iterator[vmwareengine.ListPrivateConnectionsResponse]:
+        yield self._response
+        while self._response.next_page_token:
+            self._request.page_token = self._response.next_page_token
+            self._response = self._method(self._request, metadata=self._metadata)
+            yield self._response
+
+    def __iter__(self) -> Iterator[vmwareengine_resources.PrivateConnection]:
+        for page in self.pages:
+            yield from page.private_connections
+
+    def __repr__(self) -> str:
+        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
+
+
+class ListPrivateConnectionsAsyncPager:
+    """A pager for iterating through ``list_private_connections`` requests.
+
+    This class thinly wraps an initial
+    :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionsResponse` object, and
+    provides an ``__aiter__`` method to iterate through its
+    ``private_connections`` field.
+
+    If there are more pages, the ``__aiter__`` method will make additional
+    ``ListPrivateConnections`` requests and continue to iterate
+    through the ``private_connections`` field on the
+    corresponding responses.
+
+    All the usual :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionsResponse`
+    attributes are available on the pager. If multiple requests are made, only
+    the most recent response is retained, and thus used for attribute lookup.
+    """
+
+    def __init__(
+        self,
+        method: Callable[..., Awaitable[vmwareengine.ListPrivateConnectionsResponse]],
+        request: vmwareengine.ListPrivateConnectionsRequest,
+        response: vmwareengine.ListPrivateConnectionsResponse,
+        *,
+        metadata: Sequence[Tuple[str, str]] = ()
+    ):
+        """Instantiates the pager.
+
+        Args:
+            method (Callable): The method that was originally called, and
+                which instantiated this pager.
+            request (google.cloud.vmwareengine_v1.types.ListPrivateConnectionsRequest):
+                The initial request object.
+            response (google.cloud.vmwareengine_v1.types.ListPrivateConnectionsResponse):
+                The initial response object.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        self._method = method
+        self._request = vmwareengine.ListPrivateConnectionsRequest(request)
+        self._response = response
+        self._metadata = metadata
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self._response, name)
+
+    @property
+    async def pages(self) -> AsyncIterator[vmwareengine.ListPrivateConnectionsResponse]:
+        yield self._response
+        while self._response.next_page_token:
+            self._request.page_token = self._response.next_page_token
+            self._response = await self._method(self._request, metadata=self._metadata)
+            yield self._response
+
+    def __aiter__(self) -> AsyncIterator[vmwareengine_resources.PrivateConnection]:
+        async def async_generator():
+            async for page in self.pages:
+                for response in page.private_connections:
+                    yield response
+
+        return async_generator()
+
+    def __repr__(self) -> str:
+        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
+
+
+class ListPrivateConnectionPeeringRoutesPager:
+    """A pager for iterating through ``list_private_connection_peering_routes`` requests.
+
+    This class thinly wraps an initial
+    :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesResponse` object, and
+    provides an ``__iter__`` method to iterate through its
+    ``peering_routes`` field.
+
+    If there are more pages, the ``__iter__`` method will make additional
+    ``ListPrivateConnectionPeeringRoutes`` requests and continue to iterate
+    through the ``peering_routes`` field on the
+    corresponding responses.
+
+    All the usual :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesResponse`
+    attributes are available on the pager. If multiple requests are made, only
+    the most recent response is retained, and thus used for attribute lookup.
+    """
+
+    def __init__(
+        self,
+        method: Callable[..., vmwareengine.ListPrivateConnectionPeeringRoutesResponse],
+        request: vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+        response: vmwareengine.ListPrivateConnectionPeeringRoutesResponse,
+        *,
+        metadata: Sequence[Tuple[str, str]] = ()
+    ):
+        """Instantiate the pager.
+
+        Args:
+            method (Callable): The method that was originally called, and
+                which instantiated this pager.
+            request (google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesRequest):
+                The initial request object.
+            response (google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesResponse):
+                The initial response object.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        self._method = method
+        self._request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest(request)
+        self._response = response
+        self._metadata = metadata
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self._response, name)
+
+    @property
+    def pages(
+        self,
+    ) -> Iterator[vmwareengine.ListPrivateConnectionPeeringRoutesResponse]:
+        yield self._response
+        while self._response.next_page_token:
+            self._request.page_token = self._response.next_page_token
+            self._response = self._method(self._request, metadata=self._metadata)
+            yield self._response
+
+    def __iter__(self) -> Iterator[vmwareengine_resources.PeeringRoute]:
+        for page in self.pages:
+            yield from page.peering_routes
+
+    def __repr__(self) -> str:
+        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
+
+
+class ListPrivateConnectionPeeringRoutesAsyncPager:
+    """A pager for iterating through ``list_private_connection_peering_routes`` requests.
+
+    This class thinly wraps an initial
+    :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesResponse` object, and
+    provides an ``__aiter__`` method to iterate through its
+    ``peering_routes`` field.
+
+    If there are more pages, the ``__aiter__`` method will make additional
+    ``ListPrivateConnectionPeeringRoutes`` requests and continue to iterate
+    through the ``peering_routes`` field on the
+    corresponding responses.
+
+    All the usual :class:`google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesResponse`
+    attributes are available on the pager. If multiple requests are made, only
+    the most recent response is retained, and thus used for attribute lookup.
+    """
+
+    def __init__(
+        self,
+        method: Callable[
+            ..., Awaitable[vmwareengine.ListPrivateConnectionPeeringRoutesResponse]
+        ],
+        request: vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+        response: vmwareengine.ListPrivateConnectionPeeringRoutesResponse,
+        *,
+        metadata: Sequence[Tuple[str, str]] = ()
+    ):
+        """Instantiates the pager.
+
+        Args:
+            method (Callable): The method that was originally called, and
+                which instantiated this pager.
+            request (google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesRequest):
+                The initial request object.
+            response (google.cloud.vmwareengine_v1.types.ListPrivateConnectionPeeringRoutesResponse):
+                The initial response object.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        self._method = method
+        self._request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest(request)
+        self._response = response
+        self._metadata = metadata
+
+    def __getattr__(self, name: str) -> Any:
+        return getattr(self._response, name)
+
+    @property
+    async def pages(
+        self,
+    ) -> AsyncIterator[vmwareengine.ListPrivateConnectionPeeringRoutesResponse]:
+        yield self._response
+        while self._response.next_page_token:
+            self._request.page_token = self._response.next_page_token
+            self._response = await self._method(self._request, metadata=self._metadata)
+            yield self._response
+
+    def __aiter__(self) -> AsyncIterator[vmwareengine_resources.PeeringRoute]:
+        async def async_generator():
+            async for page in self.pages:
+                for response in page.peering_routes:
+                    yield response
+
+        return async_generator()
+
+    def __repr__(self) -> str:
+        return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -227,14 +227,33 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=120.0,
                 ),
                 default_timeout=120.0,
                 client_info=client_info,
             ),
+            self.get_subnet: gapic_v1.method.wrap_method(
+                self.get_subnet,
+                default_retry=retries.Retry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=120.0,
+                ),
+                default_timeout=120.0,
+                client_info=client_info,
+            ),
+            self.update_subnet: gapic_v1.method.wrap_method(
+                self.update_subnet,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
             self.list_node_types: gapic_v1.method.wrap_method(
                 self.list_node_types,
                 default_retry=retries.Retry(
                     initial=1.0,
                     maximum=10.0,
                     multiplier=1.3,
                     predicate=retries.if_exception_type(
@@ -412,14 +431,71 @@
                         core_exceptions.ServiceUnavailable,
                     ),
                     deadline=120.0,
                 ),
                 default_timeout=120.0,
                 client_info=client_info,
             ),
+            self.create_private_connection: gapic_v1.method.wrap_method(
+                self.create_private_connection,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.get_private_connection: gapic_v1.method.wrap_method(
+                self.get_private_connection,
+                default_retry=retries.Retry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=120.0,
+                ),
+                default_timeout=120.0,
+                client_info=client_info,
+            ),
+            self.list_private_connections: gapic_v1.method.wrap_method(
+                self.list_private_connections,
+                default_retry=retries.Retry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=120.0,
+                ),
+                default_timeout=120.0,
+                client_info=client_info,
+            ),
+            self.update_private_connection: gapic_v1.method.wrap_method(
+                self.update_private_connection,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.delete_private_connection: gapic_v1.method.wrap_method(
+                self.delete_private_connection,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.list_private_connection_peering_routes: gapic_v1.method.wrap_method(
+                self.list_private_connection_peering_routes,
+                default_retry=retries.Retry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=120.0,
+                ),
+                default_timeout=120.0,
+                client_info=client_info,
+            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -551,14 +627,32 @@
             vmwareengine.ListSubnetsResponse,
             Awaitable[vmwareengine.ListSubnetsResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def get_subnet(
+        self,
+    ) -> Callable[
+        [vmwareengine.GetSubnetRequest],
+        Union[vmwareengine_resources.Subnet, Awaitable[vmwareengine_resources.Subnet]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def update_subnet(
+        self,
+    ) -> Callable[
+        [vmwareengine.UpdateSubnetRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def list_node_types(
         self,
     ) -> Callable[
         [vmwareengine.ListNodeTypesRequest],
         Union[
             vmwareengine.ListNodeTypesResponse,
             Awaitable[vmwareengine.ListNodeTypesResponse],
@@ -751,14 +845,77 @@
             vmwareengine.ListVmwareEngineNetworksResponse,
             Awaitable[vmwareengine.ListVmwareEngineNetworksResponse],
         ],
     ]:
         raise NotImplementedError()
 
     @property
+    def create_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.CreatePrivateConnectionRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def get_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.GetPrivateConnectionRequest],
+        Union[
+            vmwareengine_resources.PrivateConnection,
+            Awaitable[vmwareengine_resources.PrivateConnection],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_private_connections(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionsRequest],
+        Union[
+            vmwareengine.ListPrivateConnectionsResponse,
+            Awaitable[vmwareengine.ListPrivateConnectionsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def update_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.UpdatePrivateConnectionRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def delete_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.DeletePrivateConnectionRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_private_connection_peering_routes(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionPeeringRoutesRequest],
+        Union[
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse,
+            Awaitable[vmwareengine.ListPrivateConnectionPeeringRoutesResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def list_operations(
         self,
     ) -> Callable[
         [operations_pb2.ListOperationsRequest],
         Union[
             operations_pb2.ListOperationsResponse,
             Awaitable[operations_pb2.ListOperationsResponse],
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -610,14 +610,71 @@
                 "/google.cloud.vmwareengine.v1.VmwareEngine/ListSubnets",
                 request_serializer=vmwareengine.ListSubnetsRequest.serialize,
                 response_deserializer=vmwareengine.ListSubnetsResponse.deserialize,
             )
         return self._stubs["list_subnets"]
 
     @property
+    def get_subnet(
+        self,
+    ) -> Callable[[vmwareengine.GetSubnetRequest], vmwareengine_resources.Subnet]:
+        r"""Return a callable for the get subnet method over gRPC.
+
+        Gets details of a single subnet.
+
+        Returns:
+            Callable[[~.GetSubnetRequest],
+                    ~.Subnet]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_subnet" not in self._stubs:
+            self._stubs["get_subnet"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/GetSubnet",
+                request_serializer=vmwareengine.GetSubnetRequest.serialize,
+                response_deserializer=vmwareengine_resources.Subnet.deserialize,
+            )
+        return self._stubs["get_subnet"]
+
+    @property
+    def update_subnet(
+        self,
+    ) -> Callable[[vmwareengine.UpdateSubnetRequest], operations_pb2.Operation]:
+        r"""Return a callable for the update subnet method over gRPC.
+
+        Updates the parameters of a single subnet. Only fields specified
+        in ``update_mask`` are applied.
+
+        *Note*: This API is synchronous and always returns a successful
+        ``google.longrunning.Operation`` (LRO). The returned LRO will
+        only have ``done`` and ``response`` fields.
+
+        Returns:
+            Callable[[~.UpdateSubnetRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_subnet" not in self._stubs:
+            self._stubs["update_subnet"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/UpdateSubnet",
+                request_serializer=vmwareengine.UpdateSubnetRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["update_subnet"]
+
+    @property
     def list_node_types(
         self,
     ) -> Callable[
         [vmwareengine.ListNodeTypesRequest], vmwareengine.ListNodeTypesResponse
     ]:
         r"""Return a callable for the list node types method over gRPC.
 
@@ -1166,14 +1223,197 @@
             self._stubs["list_vmware_engine_networks"] = self.grpc_channel.unary_unary(
                 "/google.cloud.vmwareengine.v1.VmwareEngine/ListVmwareEngineNetworks",
                 request_serializer=vmwareengine.ListVmwareEngineNetworksRequest.serialize,
                 response_deserializer=vmwareengine.ListVmwareEngineNetworksResponse.deserialize,
             )
         return self._stubs["list_vmware_engine_networks"]
 
+    @property
+    def create_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.CreatePrivateConnectionRequest], operations_pb2.Operation
+    ]:
+        r"""Return a callable for the create private connection method over gRPC.
+
+        Creates a new private connection that can be used for
+        accessing private Clouds.
+
+        Returns:
+            Callable[[~.CreatePrivateConnectionRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "create_private_connection" not in self._stubs:
+            self._stubs["create_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/CreatePrivateConnection",
+                request_serializer=vmwareengine.CreatePrivateConnectionRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["create_private_connection"]
+
+    @property
+    def get_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.GetPrivateConnectionRequest],
+        vmwareengine_resources.PrivateConnection,
+    ]:
+        r"""Return a callable for the get private connection method over gRPC.
+
+        Retrieves a ``PrivateConnection`` resource by its resource name.
+        The resource contains details of the private connection, such as
+        connected network, routing mode and state.
+
+        Returns:
+            Callable[[~.GetPrivateConnectionRequest],
+                    ~.PrivateConnection]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_private_connection" not in self._stubs:
+            self._stubs["get_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/GetPrivateConnection",
+                request_serializer=vmwareengine.GetPrivateConnectionRequest.serialize,
+                response_deserializer=vmwareengine_resources.PrivateConnection.deserialize,
+            )
+        return self._stubs["get_private_connection"]
+
+    @property
+    def list_private_connections(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionsRequest],
+        vmwareengine.ListPrivateConnectionsResponse,
+    ]:
+        r"""Return a callable for the list private connections method over gRPC.
+
+        Lists ``PrivateConnection`` resources in a given project and
+        location.
+
+        Returns:
+            Callable[[~.ListPrivateConnectionsRequest],
+                    ~.ListPrivateConnectionsResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_private_connections" not in self._stubs:
+            self._stubs["list_private_connections"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/ListPrivateConnections",
+                request_serializer=vmwareengine.ListPrivateConnectionsRequest.serialize,
+                response_deserializer=vmwareengine.ListPrivateConnectionsResponse.deserialize,
+            )
+        return self._stubs["list_private_connections"]
+
+    @property
+    def update_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.UpdatePrivateConnectionRequest], operations_pb2.Operation
+    ]:
+        r"""Return a callable for the update private connection method over gRPC.
+
+        Modifies a ``PrivateConnection`` resource. Only ``description``
+        and ``routing_mode`` fields can be updated. Only fields
+        specified in ``updateMask`` are applied.
+
+        Returns:
+            Callable[[~.UpdatePrivateConnectionRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_private_connection" not in self._stubs:
+            self._stubs["update_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/UpdatePrivateConnection",
+                request_serializer=vmwareengine.UpdatePrivateConnectionRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["update_private_connection"]
+
+    @property
+    def delete_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.DeletePrivateConnectionRequest], operations_pb2.Operation
+    ]:
+        r"""Return a callable for the delete private connection method over gRPC.
+
+        Deletes a ``PrivateConnection`` resource. When a private
+        connection is deleted for a VMware Engine network, the connected
+        network becomes inaccessible to that VMware Engine network.
+
+        Returns:
+            Callable[[~.DeletePrivateConnectionRequest],
+                    ~.Operation]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_private_connection" not in self._stubs:
+            self._stubs["delete_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/DeletePrivateConnection",
+                request_serializer=vmwareengine.DeletePrivateConnectionRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["delete_private_connection"]
+
+    @property
+    def list_private_connection_peering_routes(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionPeeringRoutesRequest],
+        vmwareengine.ListPrivateConnectionPeeringRoutesResponse,
+    ]:
+        r"""Return a callable for the list private connection
+        peering routes method over gRPC.
+
+        Lists the private connection routes exchanged over a
+        peering connection.
+
+        Returns:
+            Callable[[~.ListPrivateConnectionPeeringRoutesRequest],
+                    ~.ListPrivateConnectionPeeringRoutesResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_private_connection_peering_routes" not in self._stubs:
+            self._stubs[
+                "list_private_connection_peering_routes"
+            ] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/ListPrivateConnectionPeeringRoutes",
+                request_serializer=vmwareengine.ListPrivateConnectionPeeringRoutesRequest.serialize,
+                response_deserializer=vmwareengine.ListPrivateConnectionPeeringRoutesResponse.deserialize,
+            )
+        return self._stubs["list_private_connection_peering_routes"]
+
     def close(self):
         self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/grpc_asyncio.py`

 * *Files 10% similar despite different names*

```diff
@@ -635,14 +635,75 @@
                 "/google.cloud.vmwareengine.v1.VmwareEngine/ListSubnets",
                 request_serializer=vmwareengine.ListSubnetsRequest.serialize,
                 response_deserializer=vmwareengine.ListSubnetsResponse.deserialize,
             )
         return self._stubs["list_subnets"]
 
     @property
+    def get_subnet(
+        self,
+    ) -> Callable[
+        [vmwareengine.GetSubnetRequest], Awaitable[vmwareengine_resources.Subnet]
+    ]:
+        r"""Return a callable for the get subnet method over gRPC.
+
+        Gets details of a single subnet.
+
+        Returns:
+            Callable[[~.GetSubnetRequest],
+                    Awaitable[~.Subnet]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_subnet" not in self._stubs:
+            self._stubs["get_subnet"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/GetSubnet",
+                request_serializer=vmwareengine.GetSubnetRequest.serialize,
+                response_deserializer=vmwareengine_resources.Subnet.deserialize,
+            )
+        return self._stubs["get_subnet"]
+
+    @property
+    def update_subnet(
+        self,
+    ) -> Callable[
+        [vmwareengine.UpdateSubnetRequest], Awaitable[operations_pb2.Operation]
+    ]:
+        r"""Return a callable for the update subnet method over gRPC.
+
+        Updates the parameters of a single subnet. Only fields specified
+        in ``update_mask`` are applied.
+
+        *Note*: This API is synchronous and always returns a successful
+        ``google.longrunning.Operation`` (LRO). The returned LRO will
+        only have ``done`` and ``response`` fields.
+
+        Returns:
+            Callable[[~.UpdateSubnetRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_subnet" not in self._stubs:
+            self._stubs["update_subnet"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/UpdateSubnet",
+                request_serializer=vmwareengine.UpdateSubnetRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["update_subnet"]
+
+    @property
     def list_node_types(
         self,
     ) -> Callable[
         [vmwareengine.ListNodeTypesRequest],
         Awaitable[vmwareengine.ListNodeTypesResponse],
     ]:
         r"""Return a callable for the list node types method over gRPC.
@@ -1210,14 +1271,200 @@
             self._stubs["list_vmware_engine_networks"] = self.grpc_channel.unary_unary(
                 "/google.cloud.vmwareengine.v1.VmwareEngine/ListVmwareEngineNetworks",
                 request_serializer=vmwareengine.ListVmwareEngineNetworksRequest.serialize,
                 response_deserializer=vmwareengine.ListVmwareEngineNetworksResponse.deserialize,
             )
         return self._stubs["list_vmware_engine_networks"]
 
+    @property
+    def create_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.CreatePrivateConnectionRequest],
+        Awaitable[operations_pb2.Operation],
+    ]:
+        r"""Return a callable for the create private connection method over gRPC.
+
+        Creates a new private connection that can be used for
+        accessing private Clouds.
+
+        Returns:
+            Callable[[~.CreatePrivateConnectionRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "create_private_connection" not in self._stubs:
+            self._stubs["create_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/CreatePrivateConnection",
+                request_serializer=vmwareengine.CreatePrivateConnectionRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["create_private_connection"]
+
+    @property
+    def get_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.GetPrivateConnectionRequest],
+        Awaitable[vmwareengine_resources.PrivateConnection],
+    ]:
+        r"""Return a callable for the get private connection method over gRPC.
+
+        Retrieves a ``PrivateConnection`` resource by its resource name.
+        The resource contains details of the private connection, such as
+        connected network, routing mode and state.
+
+        Returns:
+            Callable[[~.GetPrivateConnectionRequest],
+                    Awaitable[~.PrivateConnection]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_private_connection" not in self._stubs:
+            self._stubs["get_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/GetPrivateConnection",
+                request_serializer=vmwareengine.GetPrivateConnectionRequest.serialize,
+                response_deserializer=vmwareengine_resources.PrivateConnection.deserialize,
+            )
+        return self._stubs["get_private_connection"]
+
+    @property
+    def list_private_connections(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionsRequest],
+        Awaitable[vmwareengine.ListPrivateConnectionsResponse],
+    ]:
+        r"""Return a callable for the list private connections method over gRPC.
+
+        Lists ``PrivateConnection`` resources in a given project and
+        location.
+
+        Returns:
+            Callable[[~.ListPrivateConnectionsRequest],
+                    Awaitable[~.ListPrivateConnectionsResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_private_connections" not in self._stubs:
+            self._stubs["list_private_connections"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/ListPrivateConnections",
+                request_serializer=vmwareengine.ListPrivateConnectionsRequest.serialize,
+                response_deserializer=vmwareengine.ListPrivateConnectionsResponse.deserialize,
+            )
+        return self._stubs["list_private_connections"]
+
+    @property
+    def update_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.UpdatePrivateConnectionRequest],
+        Awaitable[operations_pb2.Operation],
+    ]:
+        r"""Return a callable for the update private connection method over gRPC.
+
+        Modifies a ``PrivateConnection`` resource. Only ``description``
+        and ``routing_mode`` fields can be updated. Only fields
+        specified in ``updateMask`` are applied.
+
+        Returns:
+            Callable[[~.UpdatePrivateConnectionRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "update_private_connection" not in self._stubs:
+            self._stubs["update_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/UpdatePrivateConnection",
+                request_serializer=vmwareengine.UpdatePrivateConnectionRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["update_private_connection"]
+
+    @property
+    def delete_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.DeletePrivateConnectionRequest],
+        Awaitable[operations_pb2.Operation],
+    ]:
+        r"""Return a callable for the delete private connection method over gRPC.
+
+        Deletes a ``PrivateConnection`` resource. When a private
+        connection is deleted for a VMware Engine network, the connected
+        network becomes inaccessible to that VMware Engine network.
+
+        Returns:
+            Callable[[~.DeletePrivateConnectionRequest],
+                    Awaitable[~.Operation]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_private_connection" not in self._stubs:
+            self._stubs["delete_private_connection"] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/DeletePrivateConnection",
+                request_serializer=vmwareengine.DeletePrivateConnectionRequest.serialize,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["delete_private_connection"]
+
+    @property
+    def list_private_connection_peering_routes(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionPeeringRoutesRequest],
+        Awaitable[vmwareengine.ListPrivateConnectionPeeringRoutesResponse],
+    ]:
+        r"""Return a callable for the list private connection
+        peering routes method over gRPC.
+
+        Lists the private connection routes exchanged over a
+        peering connection.
+
+        Returns:
+            Callable[[~.ListPrivateConnectionPeeringRoutesRequest],
+                    Awaitable[~.ListPrivateConnectionPeeringRoutesResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_private_connection_peering_routes" not in self._stubs:
+            self._stubs[
+                "list_private_connection_peering_routes"
+            ] = self.grpc_channel.unary_unary(
+                "/google.cloud.vmwareengine.v1.VmwareEngine/ListPrivateConnectionPeeringRoutes",
+                request_serializer=vmwareengine.ListPrivateConnectionPeeringRoutesRequest.serialize,
+                response_deserializer=vmwareengine.ListPrivateConnectionPeeringRoutesResponse.deserialize,
+            )
+        return self._stubs["list_private_connection_peering_routes"]
+
     def close(self):
         return self.grpc_channel.close()
 
     @property
     def delete_operation(
         self,
     ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/services/vmware_engine/transports/rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,14 +103,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_create_private_cloud(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_create_private_connection(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_create_private_connection(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_create_vmware_engine_network(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_create_vmware_engine_network(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -135,14 +143,22 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_delete_private_cloud(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_delete_private_connection(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_delete_private_connection(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_delete_vmware_engine_network(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_delete_vmware_engine_network(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -183,14 +199,30 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_private_cloud(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_get_private_connection(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_get_private_connection(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
+            def pre_get_subnet(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_get_subnet(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_get_vmware_engine_network(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_get_vmware_engine_network(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -231,14 +263,30 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_list_private_clouds(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_list_private_connection_peering_routes(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_list_private_connection_peering_routes(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
+            def pre_list_private_connections(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_list_private_connections(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_list_subnets(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_list_subnets(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -311,14 +359,30 @@
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_private_cloud(self, response):
                 logging.log(f"Received response: {response}")
                 return response
 
+            def pre_update_private_connection(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_update_private_connection(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
+            def pre_update_subnet(self, request, metadata):
+                logging.log(f"Received request: {request}")
+                return request, metadata
+
+            def post_update_subnet(self, response):
+                logging.log(f"Received response: {response}")
+                return response
+
             def pre_update_vmware_engine_network(self, request, metadata):
                 logging.log(f"Received request: {request}")
                 return request, metadata
 
             def post_update_vmware_engine_network(self, response):
                 logging.log(f"Received response: {response}")
                 return response
@@ -417,14 +481,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the VmwareEngine server but before
         it is returned to user code.
         """
         return response
 
+    def pre_create_private_connection(
+        self,
+        request: vmwareengine.CreatePrivateConnectionRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[vmwareengine.CreatePrivateConnectionRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for create_private_connection
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_create_private_connection(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for create_private_connection
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_create_vmware_engine_network(
         self,
         request: vmwareengine.CreateVmwareEngineNetworkRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[
         vmwareengine.CreateVmwareEngineNetworkRequest, Sequence[Tuple[str, str]]
     ]:
@@ -511,14 +598,37 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the VmwareEngine server but before
         it is returned to user code.
         """
         return response
 
+    def pre_delete_private_connection(
+        self,
+        request: vmwareengine.DeletePrivateConnectionRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[vmwareengine.DeletePrivateConnectionRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for delete_private_connection
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_delete_private_connection(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for delete_private_connection
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_delete_vmware_engine_network(
         self,
         request: vmwareengine.DeleteVmwareEngineNetworkRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[
         vmwareengine.DeleteVmwareEngineNetworkRequest, Sequence[Tuple[str, str]]
     ]:
@@ -651,14 +761,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the VmwareEngine server but before
         it is returned to user code.
         """
         return response
 
+    def pre_get_private_connection(
+        self,
+        request: vmwareengine.GetPrivateConnectionRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[vmwareengine.GetPrivateConnectionRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_private_connection
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_get_private_connection(
+        self, response: vmwareengine_resources.PrivateConnection
+    ) -> vmwareengine_resources.PrivateConnection:
+        """Post-rpc interceptor for get_private_connection
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_get_subnet(
+        self,
+        request: vmwareengine.GetSubnetRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[vmwareengine.GetSubnetRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_subnet
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_get_subnet(
+        self, response: vmwareengine_resources.Subnet
+    ) -> vmwareengine_resources.Subnet:
+        """Post-rpc interceptor for get_subnet
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_get_vmware_engine_network(
         self,
         request: vmwareengine.GetVmwareEngineNetworkRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[vmwareengine.GetVmwareEngineNetworkRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for get_vmware_engine_network
 
@@ -789,14 +945,63 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the VmwareEngine server but before
         it is returned to user code.
         """
         return response
 
+    def pre_list_private_connection_peering_routes(
+        self,
+        request: vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[
+        vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+        Sequence[Tuple[str, str]],
+    ]:
+        """Pre-rpc interceptor for list_private_connection_peering_routes
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_list_private_connection_peering_routes(
+        self, response: vmwareengine.ListPrivateConnectionPeeringRoutesResponse
+    ) -> vmwareengine.ListPrivateConnectionPeeringRoutesResponse:
+        """Post-rpc interceptor for list_private_connection_peering_routes
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_list_private_connections(
+        self,
+        request: vmwareengine.ListPrivateConnectionsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[vmwareengine.ListPrivateConnectionsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for list_private_connections
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_list_private_connections(
+        self, response: vmwareengine.ListPrivateConnectionsResponse
+    ) -> vmwareengine.ListPrivateConnectionsResponse:
+        """Post-rpc interceptor for list_private_connections
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_list_subnets(
         self,
         request: vmwareengine.ListSubnetsRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[vmwareengine.ListSubnetsRequest, Sequence[Tuple[str, str]]]:
         """Pre-rpc interceptor for list_subnets
 
@@ -1019,14 +1224,60 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the VmwareEngine server but before
         it is returned to user code.
         """
         return response
 
+    def pre_update_private_connection(
+        self,
+        request: vmwareengine.UpdatePrivateConnectionRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[vmwareengine.UpdatePrivateConnectionRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for update_private_connection
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_update_private_connection(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for update_private_connection
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_update_subnet(
+        self,
+        request: vmwareengine.UpdateSubnetRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[vmwareengine.UpdateSubnetRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for update_subnet
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the VmwareEngine server.
+        """
+        return request, metadata
+
+    def post_update_subnet(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for update_subnet
+
+        Override in a subclass to manipulate the response
+        after it is returned by the VmwareEngine server but before
+        it is returned to user code.
+        """
+        return response
+
     def pre_update_vmware_engine_network(
         self,
         request: vmwareengine.UpdateVmwareEngineNetworkRequest,
         metadata: Sequence[Tuple[str, str]],
     ) -> Tuple[
         vmwareengine.UpdateVmwareEngineNetworkRequest, Sequence[Tuple[str, str]]
     ]:
@@ -1768,14 +2019,115 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_create_private_cloud(resp)
             return resp
 
+    class _CreatePrivateConnection(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("CreatePrivateConnection")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
+            "privateConnectionId": "",
+        }
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.CreatePrivateConnectionRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the create private connection method over HTTP.
+
+            Args:
+                request (~.vmwareengine.CreatePrivateConnectionRequest):
+                    The request object. Request message for
+                [VmwareEngine.CreatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.CreatePrivateConnection]
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{parent=projects/*/locations/*}/privateConnections",
+                    "body": "private_connection",
+                },
+            ]
+            request, metadata = self._interceptor.pre_create_private_connection(
+                request, metadata
+            )
+            pb_request = vmwareengine.CreatePrivateConnectionRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_create_private_connection(resp)
+            return resp
+
     class _CreateVmwareEngineNetwork(VmwareEngineRestStub):
         def __hash__(self):
             return hash("CreateVmwareEngineNetwork")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
             "vmwareEngineNetworkId": "",
         }
@@ -2138,14 +2490,104 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_delete_private_cloud(resp)
             return resp
 
+    class _DeletePrivateConnection(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("DeletePrivateConnection")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.DeletePrivateConnectionRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the delete private connection method over HTTP.
+
+            Args:
+                request (~.vmwareengine.DeletePrivateConnectionRequest):
+                    The request object. Request message for
+                [VmwareEngine.DeletePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.DeletePrivateConnection]
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "delete",
+                    "uri": "/v1/{name=projects/*/locations/*/privateConnections/*}",
+                },
+            ]
+            request, metadata = self._interceptor.pre_delete_private_connection(
+                request, metadata
+            )
+            pb_request = vmwareengine.DeletePrivateConnectionRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_delete_private_connection(resp)
+            return resp
+
     class _DeleteVmwareEngineNetwork(VmwareEngineRestStub):
         def __hash__(self):
             return hash("DeleteVmwareEngineNetwork")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -2690,14 +3132,196 @@
             resp = vmwareengine_resources.PrivateCloud()
             pb_resp = vmwareengine_resources.PrivateCloud.pb(resp)
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_get_private_cloud(resp)
             return resp
 
+    class _GetPrivateConnection(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("GetPrivateConnection")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.GetPrivateConnectionRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> vmwareengine_resources.PrivateConnection:
+            r"""Call the get private connection method over HTTP.
+
+            Args:
+                request (~.vmwareengine.GetPrivateConnectionRequest):
+                    The request object. Request message for
+                [VmwareEngine.GetPrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.GetPrivateConnection]
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.vmwareengine_resources.PrivateConnection:
+                    Private connection resource that
+                provides connectivity for VMware Engine
+                private clouds.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*/privateConnections/*}",
+                },
+            ]
+            request, metadata = self._interceptor.pre_get_private_connection(
+                request, metadata
+            )
+            pb_request = vmwareengine.GetPrivateConnectionRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = vmwareengine_resources.PrivateConnection()
+            pb_resp = vmwareengine_resources.PrivateConnection.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_get_private_connection(resp)
+            return resp
+
+    class _GetSubnet(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("GetSubnet")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.GetSubnetRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> vmwareengine_resources.Subnet:
+            r"""Call the get subnet method over HTTP.
+
+            Args:
+                request (~.vmwareengine.GetSubnetRequest):
+                    The request object. Request message for
+                [VmwareEngine.GetSubnet][google.cloud.vmwareengine.v1.VmwareEngine.GetSubnet]
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.vmwareengine_resources.Subnet:
+                    Subnet in a private cloud. Either ``management`` subnets
+                (such as vMotion) that are read-only, or
+                ``userDefined``, which can also be updated.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*/privateClouds/*/subnets/*}",
+                },
+            ]
+            request, metadata = self._interceptor.pre_get_subnet(request, metadata)
+            pb_request = vmwareengine.GetSubnetRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = vmwareengine_resources.Subnet()
+            pb_resp = vmwareengine_resources.Subnet.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_get_subnet(resp)
+            return resp
+
     class _GetVmwareEngineNetwork(VmwareEngineRestStub):
         def __hash__(self):
             return hash("GetVmwareEngineNetwork")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -3233,14 +3857,202 @@
             resp = vmwareengine.ListPrivateCloudsResponse()
             pb_resp = vmwareengine.ListPrivateCloudsResponse.pb(resp)
 
             json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_list_private_clouds(resp)
             return resp
 
+    class _ListPrivateConnectionPeeringRoutes(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("ListPrivateConnectionPeeringRoutes")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> vmwareengine.ListPrivateConnectionPeeringRoutesResponse:
+            r"""Call the list private connection
+            peering routes method over HTTP.
+
+                Args:
+                    request (~.vmwareengine.ListPrivateConnectionPeeringRoutesRequest):
+                        The request object. Request message for
+                    [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+                    retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                        should be retried.
+                    timeout (float): The timeout for this request.
+                    metadata (Sequence[Tuple[str, str]]): Strings which should be
+                        sent along with the request as metadata.
+
+                Returns:
+                    ~.vmwareengine.ListPrivateConnectionPeeringRoutesResponse:
+                        Response message for
+                    [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{parent=projects/*/locations/*/privateConnections/*}/peeringRoutes",
+                },
+            ]
+            (
+                request,
+                metadata,
+            ) = self._interceptor.pre_list_private_connection_peering_routes(
+                request, metadata
+            )
+            pb_request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest.pb(
+                request
+            )
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+            pb_resp = vmwareengine.ListPrivateConnectionPeeringRoutesResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_list_private_connection_peering_routes(resp)
+            return resp
+
+    class _ListPrivateConnections(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("ListPrivateConnections")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.ListPrivateConnectionsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> vmwareengine.ListPrivateConnectionsResponse:
+            r"""Call the list private connections method over HTTP.
+
+            Args:
+                request (~.vmwareengine.ListPrivateConnectionsRequest):
+                    The request object. Request message for
+                [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.vmwareengine.ListPrivateConnectionsResponse:
+                    Response message for
+                [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{parent=projects/*/locations/*}/privateConnections",
+                },
+            ]
+            request, metadata = self._interceptor.pre_list_private_connections(
+                request, metadata
+            )
+            pb_request = vmwareengine.ListPrivateConnectionsRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = vmwareengine.ListPrivateConnectionsResponse()
+            pb_resp = vmwareengine.ListPrivateConnectionsResponse.pb(resp)
+
+            json_format.Parse(response.content, pb_resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_list_private_connections(resp)
+            return resp
+
     class _ListSubnets(VmwareEngineRestStub):
         def __hash__(self):
             return hash("ListSubnets")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {}
 
         @classmethod
@@ -4190,14 +5002,214 @@
 
             # Return the response
             resp = operations_pb2.Operation()
             json_format.Parse(response.content, resp, ignore_unknown_fields=True)
             resp = self._interceptor.post_update_private_cloud(resp)
             return resp
 
+    class _UpdatePrivateConnection(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("UpdatePrivateConnection")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
+            "updateMask": {},
+        }
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.UpdatePrivateConnectionRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the update private connection method over HTTP.
+
+            Args:
+                request (~.vmwareengine.UpdatePrivateConnectionRequest):
+                    The request object. Request message for
+                [VmwareEngine.UpdatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.UpdatePrivateConnection]
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "patch",
+                    "uri": "/v1/{private_connection.name=projects/*/locations/*/privateConnections/*}",
+                    "body": "private_connection",
+                },
+            ]
+            request, metadata = self._interceptor.pre_update_private_connection(
+                request, metadata
+            )
+            pb_request = vmwareengine.UpdatePrivateConnectionRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_update_private_connection(resp)
+            return resp
+
+    class _UpdateSubnet(VmwareEngineRestStub):
+        def __hash__(self):
+            return hash("UpdateSubnet")
+
+        __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
+            "updateMask": {},
+        }
+
+        @classmethod
+        def _get_unset_required_fields(cls, message_dict):
+            return {
+                k: v
+                for k, v in cls.__REQUIRED_FIELDS_DEFAULT_VALUES.items()
+                if k not in message_dict
+            }
+
+        def __call__(
+            self,
+            request: vmwareengine.UpdateSubnetRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+            r"""Call the update subnet method over HTTP.
+
+            Args:
+                request (~.vmwareengine.UpdateSubnetRequest):
+                    The request object. Request message for
+                [VmwareEngine.UpdateSubnet][google.cloud.vmwareengine.v1.VmwareEngine.UpdateSubnet]
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                ~.operations_pb2.Operation:
+                    This resource represents a
+                long-running operation that is the
+                result of a network API call.
+
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "patch",
+                    "uri": "/v1/{subnet.name=projects/*/locations/*/privateClouds/*/subnets/*}",
+                    "body": "subnet",
+                },
+            ]
+            request, metadata = self._interceptor.pre_update_subnet(request, metadata)
+            pb_request = vmwareengine.UpdateSubnetRequest.pb(request)
+            transcoded_request = path_template.transcode(http_options, pb_request)
+
+            # Jsonify the request body
+
+            body = json_format.MessageToJson(
+                transcoded_request["body"],
+                including_default_value_fields=False,
+                use_integers_for_enums=True,
+            )
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(
+                json_format.MessageToJson(
+                    transcoded_request["query_params"],
+                    including_default_value_fields=False,
+                    use_integers_for_enums=True,
+                )
+            )
+            query_params.update(self._get_unset_required_fields(query_params))
+
+            query_params["$alt"] = "json;enum-encoding=int"
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params, strict=True),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            # Return the response
+            resp = operations_pb2.Operation()
+            json_format.Parse(response.content, resp, ignore_unknown_fields=True)
+            resp = self._interceptor.post_update_subnet(resp)
+            return resp
+
     class _UpdateVmwareEngineNetwork(VmwareEngineRestStub):
         def __hash__(self):
             return hash("UpdateVmwareEngineNetwork")
 
         __REQUIRED_FIELDS_DEFAULT_VALUES: Dict[str, Any] = {
             "updateMask": {},
         }
@@ -4327,14 +5339,24 @@
         self,
     ) -> Callable[[vmwareengine.CreatePrivateCloudRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._CreatePrivateCloud(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def create_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.CreatePrivateConnectionRequest], operations_pb2.Operation
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._CreatePrivateConnection(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def create_vmware_engine_network(
         self,
     ) -> Callable[
         [vmwareengine.CreateVmwareEngineNetworkRequest], operations_pb2.Operation
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
@@ -4361,14 +5383,24 @@
         self,
     ) -> Callable[[vmwareengine.DeletePrivateCloudRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._DeletePrivateCloud(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def delete_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.DeletePrivateConnectionRequest], operations_pb2.Operation
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._DeletePrivateConnection(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def delete_vmware_engine_network(
         self,
     ) -> Callable[
         [vmwareengine.DeleteVmwareEngineNetworkRequest], operations_pb2.Operation
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
@@ -4418,14 +5450,33 @@
         [vmwareengine.GetPrivateCloudRequest], vmwareengine_resources.PrivateCloud
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._GetPrivateCloud(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def get_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.GetPrivateConnectionRequest],
+        vmwareengine_resources.PrivateConnection,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._GetPrivateConnection(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
+    def get_subnet(
+        self,
+    ) -> Callable[[vmwareengine.GetSubnetRequest], vmwareengine_resources.Subnet]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._GetSubnet(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def get_vmware_engine_network(
         self,
     ) -> Callable[
         [vmwareengine.GetVmwareEngineNetworkRequest],
         vmwareengine_resources.VmwareEngineNetwork,
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
@@ -4481,14 +5532,36 @@
         [vmwareengine.ListPrivateCloudsRequest], vmwareengine.ListPrivateCloudsResponse
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._ListPrivateClouds(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def list_private_connection_peering_routes(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionPeeringRoutesRequest],
+        vmwareengine.ListPrivateConnectionPeeringRoutesResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._ListPrivateConnectionPeeringRoutes(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
+    def list_private_connections(
+        self,
+    ) -> Callable[
+        [vmwareengine.ListPrivateConnectionsRequest],
+        vmwareengine.ListPrivateConnectionsResponse,
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._ListPrivateConnections(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def list_subnets(
         self,
     ) -> Callable[[vmwareengine.ListSubnetsRequest], vmwareengine.ListSubnetsResponse]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._ListSubnets(self._session, self._host, self._interceptor)  # type: ignore
 
@@ -4570,14 +5643,32 @@
         self,
     ) -> Callable[[vmwareengine.UpdatePrivateCloudRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdatePrivateCloud(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def update_private_connection(
+        self,
+    ) -> Callable[
+        [vmwareengine.UpdatePrivateConnectionRequest], operations_pb2.Operation
+    ]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._UpdatePrivateConnection(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
+    def update_subnet(
+        self,
+    ) -> Callable[[vmwareengine.UpdateSubnetRequest], operations_pb2.Operation]:
+        # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
+        # In C++ this would require a dynamic_cast
+        return self._UpdateSubnet(self._session, self._host, self._interceptor)  # type: ignore
+
+    @property
     def update_vmware_engine_network(
         self,
     ) -> Callable[
         [vmwareengine.UpdateVmwareEngineNetworkRequest], operations_pb2.Operation
     ]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/types/vmwareengine.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         "ListClustersResponse",
         "GetClusterRequest",
         "CreateClusterRequest",
         "UpdateClusterRequest",
         "DeleteClusterRequest",
         "ListSubnetsRequest",
         "ListSubnetsResponse",
+        "GetSubnetRequest",
+        "UpdateSubnetRequest",
         "OperationMetadata",
         "ListNodeTypesRequest",
         "ListNodeTypesResponse",
         "GetNodeTypeRequest",
         "ShowNsxCredentialsRequest",
         "ShowVcenterCredentialsRequest",
         "ResetNsxCredentialsRequest",
@@ -61,14 +63,22 @@
         "DeleteNetworkPolicyRequest",
         "CreateVmwareEngineNetworkRequest",
         "UpdateVmwareEngineNetworkRequest",
         "DeleteVmwareEngineNetworkRequest",
         "GetVmwareEngineNetworkRequest",
         "ListVmwareEngineNetworksRequest",
         "ListVmwareEngineNetworksResponse",
+        "CreatePrivateConnectionRequest",
+        "GetPrivateConnectionRequest",
+        "ListPrivateConnectionsRequest",
+        "ListPrivateConnectionsResponse",
+        "UpdatePrivateConnectionRequest",
+        "DeletePrivateConnectionRequest",
+        "ListPrivateConnectionPeeringRoutesRequest",
+        "ListPrivateConnectionPeeringRoutesResponse",
     },
 )
 
 
 class ListPrivateCloudsRequest(proto.Message):
     r"""Request message for
     [VmwareEngine.ListPrivateClouds][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateClouds]
@@ -712,14 +722,17 @@
     Attributes:
         subnets (MutableSequence[google.cloud.vmwareengine_v1.types.Subnet]):
             A list of subnets.
         next_page_token (str):
             A token, which can be sent as ``page_token`` to retrieve the
             next page. If this field is omitted, there are no subsequent
             pages.
+        unreachable (MutableSequence[str]):
+            Locations that could not be reached when
+            making an aggregated query using wildcards.
     """
 
     @property
     def raw_page(self):
         return self
 
     subnets: MutableSequence[vmwareengine_resources.Subnet] = proto.RepeatedField(
@@ -727,14 +740,66 @@
         number=1,
         message=vmwareengine_resources.Subnet,
     )
     next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
+    unreachable: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=3,
+    )
+
+
+class GetSubnetRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.GetSubnet][google.cloud.vmwareengine.v1.VmwareEngine.GetSubnet]
+
+    Attributes:
+        name (str):
+            Required. The resource name of the subnet to retrieve.
+            Resource names are schemeless URIs that follow the
+            conventions in
+            https://cloud.google.com/apis/design/resource_names. For
+            example:
+            ``projects/my-project/locations/us-central1-a/privateClouds/my-cloud/subnets/my-subnet``
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class UpdateSubnetRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.UpdateSubnet][google.cloud.vmwareengine.v1.VmwareEngine.UpdateSubnet]
+
+    Attributes:
+        update_mask (google.protobuf.field_mask_pb2.FieldMask):
+            Required. Field mask is used to specify the fields to be
+            overwritten in the ``Subnet`` resource by the update. The
+            fields specified in the ``update_mask`` are relative to the
+            resource, not the full request. A field will be overwritten
+            if it is in the mask. If the user does not provide a mask
+            then all fields will be overwritten.
+        subnet (google.cloud.vmwareengine_v1.types.Subnet):
+            Required. Subnet description.
+    """
+
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=field_mask_pb2.FieldMask,
+    )
+    subnet: vmwareengine_resources.Subnet = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=vmwareengine_resources.Subnet,
+    )
 
 
 class OperationMetadata(proto.Message):
     r"""Represents the metadata of the long-running operation.
 
     Attributes:
         create_time (google.protobuf.timestamp_pb2.Timestamp):
@@ -1841,8 +1906,384 @@
     )
     unreachable: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
 
 
+class CreatePrivateConnectionRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.CreatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.CreatePrivateConnection]
+
+    Attributes:
+        parent (str):
+            Required. The resource name of the location to create the
+            new private connection in. Private connection is a regional
+            resource. Resource names are schemeless URIs that follow the
+            conventions in
+            https://cloud.google.com/apis/design/resource_names. For
+            example: ``projects/my-project/locations/us-central1``
+        private_connection_id (str):
+            Required. The user-provided identifier of the new private
+            connection. This identifier must be unique among private
+            connection resources within the parent and becomes the final
+            token in the name URI. The identifier must meet the
+            following requirements:
+
+            -  Only contains 1-63 alphanumeric characters and hyphens
+            -  Begins with an alphabetical character
+            -  Ends with a non-hyphen character
+            -  Not formatted as a UUID
+            -  Complies with `RFC
+               1034 <https://datatracker.ietf.org/doc/html/rfc1034>`__
+               (section 3.5)
+        private_connection (google.cloud.vmwareengine_v1.types.PrivateConnection):
+            Required. The initial description of the new
+            private connection.
+        request_id (str):
+            Optional. A request ID to identify requests.
+            Specify a unique request ID so that if you must
+            retry your request, the server will know to
+            ignore the request if it has already been
+            completed. The server guarantees that a request
+            doesn't result in creation of duplicate
+            commitments for at least 60 minutes.
+
+            For example, consider a situation where you make
+            an initial request and the request times out. If
+            you make the request again with the same request
+            ID, the server can check if original operation
+            with the same request ID was received, and if
+            so, will ignore the second request. This
+            prevents clients from accidentally creating
+            duplicate commitments.
+            The request ID must be a valid UUID with the
+            exception that zero UUID is not supported
+            (00000000-0000-0000-0000-000000000000).
+    """
+
+    parent: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    private_connection_id: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    private_connection: vmwareengine_resources.PrivateConnection = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=vmwareengine_resources.PrivateConnection,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+
+
+class GetPrivateConnectionRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.GetPrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.GetPrivateConnection]
+
+    Attributes:
+        name (str):
+            Required. The resource name of the private connection to
+            retrieve. Resource names are schemeless URIs that follow the
+            conventions in
+            https://cloud.google.com/apis/design/resource_names. For
+            example:
+            ``projects/my-project/locations/us-central1/privateConnections/my-connection``
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+
+
+class ListPrivateConnectionsRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+
+    Attributes:
+        parent (str):
+            Required. The resource name of the location to query for
+            private connections. Resource names are schemeless URIs that
+            follow the conventions in
+            https://cloud.google.com/apis/design/resource_names. For
+            example: ``projects/my-project/locations/us-central1``
+        page_size (int):
+            The maximum number of private connections to
+            return in one page. The maximum value is coerced
+            to 1000. The default value of this field is 500.
+        page_token (str):
+            A page token, received from a previous
+            ``ListPrivateConnections`` call. Provide this to retrieve
+            the subsequent page.
+
+            When paginating, all other parameters provided to
+            ``ListPrivateConnections`` must match the call that provided
+            the page token.
+        filter (str):
+            A filter expression that matches resources returned in the
+            response. The expression must specify the field name, a
+            comparison operator, and the value that you want to use for
+            filtering. The value must be a string, a number, or a
+            boolean. The comparison operator must be ``=``, ``!=``,
+            ``>``, or ``<``.
+
+            For example, if you are filtering a list of private
+            connections, you can exclude the ones named
+            ``example-connection`` by specifying
+            ``name != "example-connection"``.
+
+            To filter on multiple expressions, provide each separate
+            expression within parentheses. For example:
+
+            ::
+
+               (name = "example-connection")
+               (createTime > "2022-09-22T08:15:10.40Z")
+
+            By default, each expression is an ``AND`` expression.
+            However, you can include ``AND`` and ``OR`` expressions
+            explicitly. For example:
+
+            ::
+
+               (name = "example-connection-1") AND
+               (createTime > "2021-04-12T08:15:10.40Z") OR
+               (name = "example-connection-2")
+        order_by (str):
+            Sorts list results by a certain order. By default, returned
+            results are ordered by ``name`` in ascending order. You can
+            also sort results in descending order based on the ``name``
+            value using ``orderBy="name desc"``. Currently, only
+            ordering by ``name`` is supported.
+    """
+
+    parent: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    page_size: int = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    page_token: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    filter: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    order_by: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+
+
+class ListPrivateConnectionsResponse(proto.Message):
+    r"""Response message for
+    [VmwareEngine.ListPrivateConnections][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnections]
+
+    Attributes:
+        private_connections (MutableSequence[google.cloud.vmwareengine_v1.types.PrivateConnection]):
+            A list of private connections.
+        next_page_token (str):
+            A token, which can be sent as ``page_token`` to retrieve the
+            next page. If this field is omitted, there are no subsequent
+            pages.
+        unreachable (MutableSequence[str]):
+            Unreachable resources.
+    """
+
+    @property
+    def raw_page(self):
+        return self
+
+    private_connections: MutableSequence[
+        vmwareengine_resources.PrivateConnection
+    ] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message=vmwareengine_resources.PrivateConnection,
+    )
+    next_page_token: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+    unreachable: MutableSequence[str] = proto.RepeatedField(
+        proto.STRING,
+        number=3,
+    )
+
+
+class UpdatePrivateConnectionRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.UpdatePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.UpdatePrivateConnection]
+
+    Attributes:
+        private_connection (google.cloud.vmwareengine_v1.types.PrivateConnection):
+            Required. Private connection description.
+        update_mask (google.protobuf.field_mask_pb2.FieldMask):
+            Required. Field mask is used to specify the fields to be
+            overwritten in the ``PrivateConnection`` resource by the
+            update. The fields specified in the ``update_mask`` are
+            relative to the resource, not the full request. A field will
+            be overwritten if it is in the mask. If the user does not
+            provide a mask then all fields will be overwritten.
+        request_id (str):
+            Optional. A request ID to identify requests.
+            Specify a unique request ID so that if you must
+            retry your request, the server will know to
+            ignore the request if it has already been
+            completed. The server guarantees that a request
+            doesn't result in creation of duplicate
+            commitments for at least 60 minutes.
+
+            For example, consider a situation where you make
+            an initial request and the request times out. If
+            you make the request again with the same request
+            ID, the server can check if original operation
+            with the same request ID was received, and if
+            so, will ignore the second request. This
+            prevents clients from accidentally creating
+            duplicate commitments.
+            The request ID must be a valid UUID with the
+            exception that zero UUID is not supported
+            (00000000-0000-0000-0000-000000000000).
+    """
+
+    private_connection: vmwareengine_resources.PrivateConnection = proto.Field(
+        proto.MESSAGE,
+        number=1,
+        message=vmwareengine_resources.PrivateConnection,
+    )
+    update_mask: field_mask_pb2.FieldMask = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=field_mask_pb2.FieldMask,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+
+
+class DeletePrivateConnectionRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.DeletePrivateConnection][google.cloud.vmwareengine.v1.VmwareEngine.DeletePrivateConnection]
+
+    Attributes:
+        name (str):
+            Required. The resource name of the private connection to be
+            deleted. Resource names are schemeless URIs that follow the
+            conventions in
+            https://cloud.google.com/apis/design/resource_names. For
+            example:
+            ``projects/my-project/locations/us-central1/privateConnections/my-connection``
+        request_id (str):
+            Optional. A request ID to identify requests.
+            Specify a unique request ID so that if you must
+            retry your request, the server will know to
+            ignore the request if it has already been
+            completed. The server guarantees that a request
+            doesn't result in creation of duplicate
+            commitments for at least 60 minutes.
+
+            For example, consider a situation where you make
+            an initial request and the request times out. If
+            you make the request again with the same request
+            ID, the server can check if original operation
+            with the same request ID was received, and if
+            so, will ignore the second request. This
+            prevents clients from accidentally creating
+            duplicate commitments.
+            The request ID must be a valid UUID with the
+            exception that zero UUID is not supported
+            (00000000-0000-0000-0000-000000000000).
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+
+
+class ListPrivateConnectionPeeringRoutesRequest(proto.Message):
+    r"""Request message for
+    [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+
+    Attributes:
+        parent (str):
+            Required. The resource name of the private connection to
+            retrieve peering routes from. Resource names are schemeless
+            URIs that follow the conventions in
+            https://cloud.google.com/apis/design/resource_names. For
+            example:
+            ``projects/my-project/locations/us-west1/privateConnections/my-connection``
+        page_size (int):
+            The maximum number of peering routes to
+            return in one page. The service may return fewer
+            than this value. The maximum value is coerced to
+            1000.
+            The default value of this field is 500.
+        page_token (str):
+            A page token, received from a previous
+            ``ListPrivateConnectionPeeringRoutes`` call. Provide this to
+            retrieve the subsequent page. When paginating, all other
+            parameters provided to
+            ``ListPrivateConnectionPeeringRoutes`` must match the call
+            that provided the page token.
+    """
+
+    parent: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    page_size: int = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    page_token: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+
+
+class ListPrivateConnectionPeeringRoutesResponse(proto.Message):
+    r"""Response message for
+    [VmwareEngine.ListPrivateConnectionPeeringRoutes][google.cloud.vmwareengine.v1.VmwareEngine.ListPrivateConnectionPeeringRoutes]
+
+    Attributes:
+        peering_routes (MutableSequence[google.cloud.vmwareengine_v1.types.PeeringRoute]):
+            A list of peering routes.
+        next_page_token (str):
+            A token, which can be sent as ``page_token`` to retrieve the
+            next page. If this field is omitted, there are no subsequent
+            pages.
+    """
+
+    @property
+    def raw_page(self):
+        return self
+
+    peering_routes: MutableSequence[
+        vmwareengine_resources.PeeringRoute
+    ] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message=vmwareengine_resources.PeeringRoute,
+    )
+    next_page_token: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-vmwareengine-1.0.1/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py` & `google-cloud-vmwareengine-1.1.0/google/cloud/vmwareengine_v1/types/vmwareengine_resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,16 +30,18 @@
         "Subnet",
         "NodeType",
         "Credentials",
         "HcxActivationKey",
         "Hcx",
         "Nsx",
         "Vcenter",
+        "PeeringRoute",
         "NetworkPolicy",
         "VmwareEngineNetwork",
+        "PrivateConnection",
     },
 )
 
 
 class NetworkConfig(proto.Message):
     r"""Network configuration in the consumer project
     with which the peering has to be done.
@@ -163,14 +165,17 @@
         nsx (google.cloud.vmwareengine_v1.types.Nsx):
             Output only. NSX appliance.
         vcenter (google.cloud.vmwareengine_v1.types.Vcenter):
             Output only. Vcenter appliance.
         uid (str):
             Output only. System-generated unique
             identifier for the resource.
+        type_ (google.cloud.vmwareengine_v1.types.PrivateCloud.Type):
+            Optional. Type of the private cloud. Defaults
+            to STANDARD.
     """
 
     class State(proto.Enum):
         r"""Enum State defines possible states of private clouds.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -196,14 +201,31 @@
         ACTIVE = 1
         CREATING = 2
         UPDATING = 3
         FAILED = 5
         DELETED = 6
         PURGING = 7
 
+    class Type(proto.Enum):
+        r"""Enum Type defines private cloud type.
+
+        Values:
+            STANDARD (0):
+                Standard private is a zonal resource, with 3+
+                nodes. Default type.
+            TIME_LIMITED (1):
+                Time limited private cloud is a zonal
+                resource, can have only 1 node and has limited
+                life span. Will be deleted after defined period
+                of time, can be converted into standard private
+                cloud by expanding it up to 3 or more nodes.
+        """
+        STANDARD = 0
+        TIME_LIMITED = 1
+
     class ManagementCluster(proto.Message):
         r"""Management cluster configuration.
 
         Attributes:
             cluster_id (str):
                 Required. The user-provided identifier of the new
                 ``Cluster``. The identifier must meet the following
@@ -291,14 +313,19 @@
         number=19,
         message="Vcenter",
     )
     uid: str = proto.Field(
         proto.STRING,
         number=20,
     )
+    type_: Type = proto.Field(
+        proto.ENUM,
+        number=22,
+        enum=Type,
+    )
 
 
 class Cluster(proto.Message):
     r"""A cluster in a private cloud.
 
     Attributes:
         name (str):
@@ -427,20 +454,29 @@
                 The subnet is ready.
             CREATING (2):
                 The subnet is being created.
             UPDATING (3):
                 The subnet is being updated.
             DELETING (4):
                 The subnet is being deleted.
+            RECONCILING (5):
+                Changes requested in the last operation are
+                being propagated.
+            FAILED (6):
+                Last operation on the subnet did not succeed.
+                Subnet's payload is reverted back to its most
+                recent working state.
         """
         STATE_UNSPECIFIED = 0
         ACTIVE = 1
         CREATING = 2
         UPDATING = 3
         DELETING = 4
+        RECONCILING = 5
+        FAILED = 6
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     ip_cidr_range: str = proto.Field(
         proto.STRING,
@@ -763,14 +799,114 @@
     )
     fqdn: str = proto.Field(
         proto.STRING,
         number=6,
     )
 
 
+class PeeringRoute(proto.Message):
+    r"""Exchanged network peering route.
+
+    Attributes:
+        dest_range (str):
+            Output only. Destination range of the peering
+            route in CIDR notation.
+        type_ (google.cloud.vmwareengine_v1.types.PeeringRoute.Type):
+            Output only. Type of the route in the peer
+            VPC network.
+        next_hop_region (str):
+            Output only. Region containing the next hop
+            of the peering route. This field only applies to
+            dynamic routes in the peer VPC network.
+        priority (int):
+            Output only. The priority of the peering
+            route.
+        imported (bool):
+            Output only. True if the peering route has been imported
+            from a peered VPC network; false otherwise. The import
+            happens if the field ``NetworkPeering.importCustomRoutes``
+            is true for this network,
+            ``NetworkPeering.exportCustomRoutes`` is true for the peer
+            VPC network, and the import does not result in a route
+            conflict.
+        direction (google.cloud.vmwareengine_v1.types.PeeringRoute.Direction):
+            Output only. Direction of the routes exchanged with the peer
+            network, from the VMware Engine network perspective:
+
+            -  Routes of direction ``INCOMING`` are imported from the
+               peer network.
+            -  Routes of direction ``OUTGOING`` are exported from the
+               intranet VPC network of the VMware Engine network.
+    """
+
+    class Type(proto.Enum):
+        r"""The type of the peering route.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                Unspecified peering route type. This is the
+                default value.
+            DYNAMIC_PEERING_ROUTE (1):
+                Dynamic routes in the peer network.
+            STATIC_PEERING_ROUTE (2):
+                Static routes in the peer network.
+            SUBNET_PEERING_ROUTE (3):
+                Created, updated, and removed automatically
+                by Google Cloud when subnets are created,
+                modified, or deleted in the peer network.
+        """
+        TYPE_UNSPECIFIED = 0
+        DYNAMIC_PEERING_ROUTE = 1
+        STATIC_PEERING_ROUTE = 2
+        SUBNET_PEERING_ROUTE = 3
+
+    class Direction(proto.Enum):
+        r"""The direction of the exchanged routes.
+
+        Values:
+            DIRECTION_UNSPECIFIED (0):
+                Unspecified exchanged routes direction. This
+                is default.
+            INCOMING (1):
+                Routes imported from the peer network.
+            OUTGOING (2):
+                Routes exported to the peer network.
+        """
+        DIRECTION_UNSPECIFIED = 0
+        INCOMING = 1
+        OUTGOING = 2
+
+    dest_range: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    type_: Type = proto.Field(
+        proto.ENUM,
+        number=2,
+        enum=Type,
+    )
+    next_hop_region: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    priority: int = proto.Field(
+        proto.INT64,
+        number=4,
+    )
+    imported: bool = proto.Field(
+        proto.BOOL,
+        number=5,
+    )
+    direction: Direction = proto.Field(
+        proto.ENUM,
+        number=6,
+        enum=Direction,
+    )
+
+
 class NetworkPolicy(proto.Message):
     r"""Represents a network policy resource. Network policies are
     regional resources. You can use a network policy to enable or
     disable internet access and external IP access. Network policies
     are associated with a VMware Engine network, which might span
     across regions. For a given region, a network policy applies to
     all private clouds in the VMware Engine network associated with
@@ -1084,8 +1220,228 @@
     )
     etag: str = proto.Field(
         proto.STRING,
         number=10,
     )
 
 
+class PrivateConnection(proto.Message):
+    r"""Private connection resource that provides connectivity for
+    VMware Engine private clouds.
+
+    Attributes:
+        name (str):
+            Output only. The resource name of the private connection.
+            Resource names are schemeless URIs that follow the
+            conventions in
+            https://cloud.google.com/apis/design/resource_names. For
+            example:
+            ``projects/my-project/locations/us-central1/privateConnections/my-connection``
+        create_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. Creation time of this resource.
+        update_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. Last update time of this
+            resource.
+        description (str):
+            Optional. User-provided description for this
+            private connection.
+        state (google.cloud.vmwareengine_v1.types.PrivateConnection.State):
+            Output only. State of the private connection.
+        vmware_engine_network (str):
+            Required. The relative resource name of Legacy VMware Engine
+            network. Specify the name in the following form:
+            ``projects/{project}/locations/{location}/vmwareEngineNetworks/{vmware_engine_network_id}``
+            where ``{project}``, ``{location}`` will be same as
+            specified in private connection resource name and
+            ``{vmware_engine_network_id}`` will be in the form of
+            ``{location}``-default e.g.
+            projects/project/locations/us-central1/vmwareEngineNetworks/us-central1-default.
+        vmware_engine_network_canonical (str):
+            Output only. The canonical name of the VMware Engine network
+            in the form:
+            ``projects/{project_number}/locations/{location}/vmwareEngineNetworks/{vmware_engine_network_id}``
+        type_ (google.cloud.vmwareengine_v1.types.PrivateConnection.Type):
+            Required. Private connection type.
+        peering_id (str):
+            Output only. VPC network peering id between
+            given network VPC and VMwareEngineNetwork.
+        routing_mode (google.cloud.vmwareengine_v1.types.PrivateConnection.RoutingMode):
+            Optional. Routing Mode. Default value is set to GLOBAL. For
+            type = PRIVATE_SERVICE_ACCESS, this field can be set to
+            GLOBAL or REGIONAL, for other types only GLOBAL is
+            supported.
+        uid (str):
+            Output only. System-generated unique
+            identifier for the resource.
+        service_network (str):
+            Required. Service network to create private connection.
+            Specify the name in the following form:
+            ``projects/{project}/global/networks/{network_id}`` For type
+            = PRIVATE_SERVICE_ACCESS, this field represents
+            servicenetworking VPC, e.g.
+            projects/project-tp/global/networks/servicenetworking. For
+            type = NETAPP_CLOUD_VOLUME, this field represents NetApp
+            service VPC, e.g.
+            projects/project-tp/global/networks/netapp-tenant-vpc. For
+            type = DELL_POWERSCALE, this field represent Dell service
+            VPC, e.g.
+            projects/project-tp/global/networks/dell-tenant-vpc. For
+            type= THIRD_PARTY_SERVICE, this field could represent a
+            consumer VPC or any other producer VPC to which the VMware
+            Engine Network needs to be connected, e.g.
+            projects/project/global/networks/vpc.
+        peering_state (google.cloud.vmwareengine_v1.types.PrivateConnection.PeeringState):
+            Output only. Peering state between service
+            network and VMware Engine network.
+    """
+
+    class State(proto.Enum):
+        r"""Enum State defines possible states of private connection.
+
+        Values:
+            STATE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                state is omitted.
+            CREATING (1):
+                The private connection is being created.
+            ACTIVE (2):
+                The private connection is ready.
+            UPDATING (3):
+                The private connection is being updated.
+            DELETING (4):
+                The private connection is being deleted.
+            UNPROVISIONED (5):
+                The private connection is not provisioned,
+                since no private cloud is present for which this
+                private connection is needed.
+            FAILED (6):
+                The private connection is in failed state.
+        """
+        STATE_UNSPECIFIED = 0
+        CREATING = 1
+        ACTIVE = 2
+        UPDATING = 3
+        DELETING = 4
+        UNPROVISIONED = 5
+        FAILED = 6
+
+    class Type(proto.Enum):
+        r"""Enum Type defines possible types of private connection.
+
+        Values:
+            TYPE_UNSPECIFIED (0):
+                The default value. This value should never be
+                used.
+            PRIVATE_SERVICE_ACCESS (1):
+                Connection used for establishing `private services
+                access <https://cloud.google.com/vpc/docs/private-services-access>`__.
+            NETAPP_CLOUD_VOLUMES (2):
+                Connection used for connecting to NetApp
+                Cloud Volumes.
+            DELL_POWERSCALE (3):
+                Connection used for connecting to Dell
+                PowerScale.
+            THIRD_PARTY_SERVICE (4):
+                Connection used for connecting to third-party
+                services.
+        """
+        TYPE_UNSPECIFIED = 0
+        PRIVATE_SERVICE_ACCESS = 1
+        NETAPP_CLOUD_VOLUMES = 2
+        DELL_POWERSCALE = 3
+        THIRD_PARTY_SERVICE = 4
+
+    class RoutingMode(proto.Enum):
+        r"""Possible types for RoutingMode
+
+        Values:
+            ROUTING_MODE_UNSPECIFIED (0):
+                The default value. This value should never be
+                used.
+            GLOBAL (1):
+                Global Routing Mode
+            REGIONAL (2):
+                Regional Routing Mode
+        """
+        ROUTING_MODE_UNSPECIFIED = 0
+        GLOBAL = 1
+        REGIONAL = 2
+
+    class PeeringState(proto.Enum):
+        r"""Enum PeeringState defines the possible states of peering
+        between service network and the vpc network peered to service
+        network
+
+        Values:
+            PEERING_STATE_UNSPECIFIED (0):
+                The default value. This value is used if the
+                peering state is omitted or unknown.
+            PEERING_ACTIVE (1):
+                The peering is in active state.
+            PEERING_INACTIVE (2):
+                The peering is in inactive state.
+        """
+        PEERING_STATE_UNSPECIFIED = 0
+        PEERING_ACTIVE = 1
+        PEERING_INACTIVE = 2
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    create_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message=timestamp_pb2.Timestamp,
+    )
+    update_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=3,
+        message=timestamp_pb2.Timestamp,
+    )
+    description: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    state: State = proto.Field(
+        proto.ENUM,
+        number=5,
+        enum=State,
+    )
+    vmware_engine_network: str = proto.Field(
+        proto.STRING,
+        number=8,
+    )
+    vmware_engine_network_canonical: str = proto.Field(
+        proto.STRING,
+        number=9,
+    )
+    type_: Type = proto.Field(
+        proto.ENUM,
+        number=10,
+        enum=Type,
+    )
+    peering_id: str = proto.Field(
+        proto.STRING,
+        number=12,
+    )
+    routing_mode: RoutingMode = proto.Field(
+        proto.ENUM,
+        number=13,
+        enum=RoutingMode,
+    )
+    uid: str = proto.Field(
+        proto.STRING,
+        number=14,
+    )
+    service_network: str = proto.Field(
+        proto.STRING,
+        number=16,
+    )
+    peering_state: PeeringState = proto.Field(
+        proto.ENUM,
+        number=17,
+        enum=PeeringState,
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/PKG-INFO` & `google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vmwareengine
-Version: 1.0.1
+Version: 1.1.0
 Summary: Google Cloud Vmwareengine API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vmwareengine-1.0.1/google_cloud_vmwareengine.egg-info/SOURCES.txt` & `google-cloud-vmwareengine-1.1.0/google_cloud_vmwareengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/setup.py` & `google-cloud-vmwareengine-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/tests/__init__.py` & `google-cloud-vmwareengine-1.1.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/tests/unit/__init__.py` & `google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vmwareengine-1.0.1/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py` & `google-cloud-vmwareengine-1.1.0/tests/unit/gapic/vmwareengine_v1/test_vmware_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1177,28 +1177,30 @@
     ) as call:
         # Designate an appropriate return value for the call.
         call.return_value = vmwareengine_resources.PrivateCloud(
             name="name_value",
             state=vmwareengine_resources.PrivateCloud.State.ACTIVE,
             description="description_value",
             uid="uid_value",
+            type_=vmwareengine_resources.PrivateCloud.Type.TIME_LIMITED,
         )
         response = client.get_private_cloud(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmwareengine.GetPrivateCloudRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vmwareengine_resources.PrivateCloud)
     assert response.name == "name_value"
     assert response.state == vmwareengine_resources.PrivateCloud.State.ACTIVE
     assert response.description == "description_value"
     assert response.uid == "uid_value"
+    assert response.type_ == vmwareengine_resources.PrivateCloud.Type.TIME_LIMITED
 
 
 def test_get_private_cloud_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = VmwareEngineClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1235,14 +1237,15 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             vmwareengine_resources.PrivateCloud(
                 name="name_value",
                 state=vmwareengine_resources.PrivateCloud.State.ACTIVE,
                 description="description_value",
                 uid="uid_value",
+                type_=vmwareengine_resources.PrivateCloud.Type.TIME_LIMITED,
             )
         )
         response = await client.get_private_cloud(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
@@ -1250,14 +1253,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vmwareengine_resources.PrivateCloud)
     assert response.name == "name_value"
     assert response.state == vmwareengine_resources.PrivateCloud.State.ACTIVE
     assert response.description == "description_value"
     assert response.uid == "uid_value"
+    assert response.type_ == vmwareengine_resources.PrivateCloud.Type.TIME_LIMITED
 
 
 @pytest.mark.asyncio
 async def test_get_private_cloud_async_from_dict():
     await test_get_private_cloud_async(request_type=dict)
 
 
@@ -3797,25 +3801,27 @@
     request = request_type()
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_subnets), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = vmwareengine.ListSubnetsResponse(
             next_page_token="next_page_token_value",
+            unreachable=["unreachable_value"],
         )
         response = client.list_subnets(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmwareengine.ListSubnetsRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListSubnetsPager)
     assert response.next_page_token == "next_page_token_value"
+    assert response.unreachable == ["unreachable_value"]
 
 
 def test_list_subnets_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = VmwareEngineClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -3845,26 +3851,28 @@
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_subnets), "__call__") as call:
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
             vmwareengine.ListSubnetsResponse(
                 next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
             )
         )
         response = await client.list_subnets(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
         assert args[0] == vmwareengine.ListSubnetsRequest()
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListSubnetsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
+    assert response.unreachable == ["unreachable_value"]
 
 
 @pytest.mark.asyncio
 async def test_list_subnets_async_from_dict():
     await test_list_subnets_async(request_type=dict)
 
 
@@ -4198,14 +4206,498 @@
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        vmwareengine.GetSubnetRequest,
+        dict,
+    ],
+)
+def test_get_subnet(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine_resources.Subnet(
+            name="name_value",
+            ip_cidr_range="ip_cidr_range_value",
+            gateway_ip="gateway_ip_value",
+            type_="type__value",
+            state=vmwareengine_resources.Subnet.State.ACTIVE,
+        )
+        response = client.get_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.GetSubnetRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, vmwareengine_resources.Subnet)
+    assert response.name == "name_value"
+    assert response.ip_cidr_range == "ip_cidr_range_value"
+    assert response.gateway_ip == "gateway_ip_value"
+    assert response.type_ == "type__value"
+    assert response.state == vmwareengine_resources.Subnet.State.ACTIVE
+
+
+def test_get_subnet_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_subnet), "__call__") as call:
+        client.get_subnet()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.GetSubnetRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_subnet_async(
+    transport: str = "grpc_asyncio", request_type=vmwareengine.GetSubnetRequest
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine_resources.Subnet(
+                name="name_value",
+                ip_cidr_range="ip_cidr_range_value",
+                gateway_ip="gateway_ip_value",
+                type_="type__value",
+                state=vmwareengine_resources.Subnet.State.ACTIVE,
+            )
+        )
+        response = await client.get_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.GetSubnetRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, vmwareengine_resources.Subnet)
+    assert response.name == "name_value"
+    assert response.ip_cidr_range == "ip_cidr_range_value"
+    assert response.gateway_ip == "gateway_ip_value"
+    assert response.type_ == "type__value"
+    assert response.state == vmwareengine_resources.Subnet.State.ACTIVE
+
+
+@pytest.mark.asyncio
+async def test_get_subnet_async_from_dict():
+    await test_get_subnet_async(request_type=dict)
+
+
+def test_get_subnet_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.GetSubnetRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_subnet), "__call__") as call:
+        call.return_value = vmwareengine_resources.Subnet()
+        client.get_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_subnet_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.GetSubnetRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_subnet), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine_resources.Subnet()
+        )
+        await client.get_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+def test_get_subnet_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine_resources.Subnet()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.get_subnet(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+def test_get_subnet_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.get_subnet(
+            vmwareengine.GetSubnetRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_subnet_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine_resources.Subnet()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine_resources.Subnet()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.get_subnet(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_get_subnet_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.get_subnet(
+            vmwareengine.GetSubnetRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.UpdateSubnetRequest,
+        dict,
+    ],
+)
+def test_update_subnet(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.update_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.UpdateSubnetRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_update_subnet_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_subnet), "__call__") as call:
+        client.update_subnet()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.UpdateSubnetRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_subnet_async(
+    transport: str = "grpc_asyncio", request_type=vmwareengine.UpdateSubnetRequest
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.update_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.UpdateSubnetRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_update_subnet_async_from_dict():
+    await test_update_subnet_async(request_type=dict)
+
+
+def test_update_subnet_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.UpdateSubnetRequest()
+
+    request.subnet.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_subnet), "__call__") as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.update_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "subnet.name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_update_subnet_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.UpdateSubnetRequest()
+
+    request.subnet.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_subnet), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.update_subnet(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "subnet.name=name_value",
+    ) in kw["metadata"]
+
+
+def test_update_subnet_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.update_subnet(
+            subnet=vmwareengine_resources.Subnet(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].subnet
+        mock_val = vmwareengine_resources.Subnet(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+def test_update_subnet_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_subnet(
+            vmwareengine.UpdateSubnetRequest(),
+            subnet=vmwareengine_resources.Subnet(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_subnet_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_subnet), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.update_subnet(
+            subnet=vmwareengine_resources.Subnet(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].subnet
+        mock_val = vmwareengine_resources.Subnet(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_update_subnet_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.update_subnet(
+            vmwareengine.UpdateSubnetRequest(),
+            subnet=vmwareengine_resources.Subnet(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         vmwareengine.ListNodeTypesRequest,
         dict,
     ],
 )
 def test_list_node_types(request_type, transport: str = "grpc"):
     client = VmwareEngineClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -9805,14 +10297,1990 @@
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        vmwareengine.CreatePrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_create_private_connection(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.create_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.CreatePrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_create_private_connection_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_private_connection), "__call__"
+    ) as call:
+        client.create_private_connection()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.CreatePrivateConnectionRequest()
+
+
+@pytest.mark.asyncio
+async def test_create_private_connection_async(
+    transport: str = "grpc_asyncio",
+    request_type=vmwareengine.CreatePrivateConnectionRequest,
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.create_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.CreatePrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_create_private_connection_async_from_dict():
+    await test_create_private_connection_async(request_type=dict)
+
+
+def test_create_private_connection_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.CreatePrivateConnectionRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_private_connection), "__call__"
+    ) as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.create_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_create_private_connection_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.CreatePrivateConnectionRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_private_connection), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.create_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+def test_create_private_connection_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.create_private_connection(
+            parent="parent_value",
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            private_connection_id="private_connection_id_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].private_connection
+        mock_val = vmwareengine_resources.PrivateConnection(name="name_value")
+        assert arg == mock_val
+        arg = args[0].private_connection_id
+        mock_val = "private_connection_id_value"
+        assert arg == mock_val
+
+
+def test_create_private_connection_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.create_private_connection(
+            vmwareengine.CreatePrivateConnectionRequest(),
+            parent="parent_value",
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            private_connection_id="private_connection_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_private_connection_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.create_private_connection(
+            parent="parent_value",
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            private_connection_id="private_connection_id_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].private_connection
+        mock_val = vmwareengine_resources.PrivateConnection(name="name_value")
+        assert arg == mock_val
+        arg = args[0].private_connection_id
+        mock_val = "private_connection_id_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_create_private_connection_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.create_private_connection(
+            vmwareengine.CreatePrivateConnectionRequest(),
+            parent="parent_value",
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            private_connection_id="private_connection_id_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.GetPrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_get_private_connection(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine_resources.PrivateConnection(
+            name="name_value",
+            description="description_value",
+            state=vmwareengine_resources.PrivateConnection.State.CREATING,
+            vmware_engine_network="vmware_engine_network_value",
+            vmware_engine_network_canonical="vmware_engine_network_canonical_value",
+            type_=vmwareengine_resources.PrivateConnection.Type.PRIVATE_SERVICE_ACCESS,
+            peering_id="peering_id_value",
+            routing_mode=vmwareengine_resources.PrivateConnection.RoutingMode.GLOBAL,
+            uid="uid_value",
+            service_network="service_network_value",
+            peering_state=vmwareengine_resources.PrivateConnection.PeeringState.PEERING_ACTIVE,
+        )
+        response = client.get_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.GetPrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, vmwareengine_resources.PrivateConnection)
+    assert response.name == "name_value"
+    assert response.description == "description_value"
+    assert response.state == vmwareengine_resources.PrivateConnection.State.CREATING
+    assert response.vmware_engine_network == "vmware_engine_network_value"
+    assert (
+        response.vmware_engine_network_canonical
+        == "vmware_engine_network_canonical_value"
+    )
+    assert (
+        response.type_
+        == vmwareengine_resources.PrivateConnection.Type.PRIVATE_SERVICE_ACCESS
+    )
+    assert response.peering_id == "peering_id_value"
+    assert (
+        response.routing_mode
+        == vmwareengine_resources.PrivateConnection.RoutingMode.GLOBAL
+    )
+    assert response.uid == "uid_value"
+    assert response.service_network == "service_network_value"
+    assert (
+        response.peering_state
+        == vmwareengine_resources.PrivateConnection.PeeringState.PEERING_ACTIVE
+    )
+
+
+def test_get_private_connection_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_private_connection), "__call__"
+    ) as call:
+        client.get_private_connection()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.GetPrivateConnectionRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_private_connection_async(
+    transport: str = "grpc_asyncio",
+    request_type=vmwareengine.GetPrivateConnectionRequest,
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine_resources.PrivateConnection(
+                name="name_value",
+                description="description_value",
+                state=vmwareengine_resources.PrivateConnection.State.CREATING,
+                vmware_engine_network="vmware_engine_network_value",
+                vmware_engine_network_canonical="vmware_engine_network_canonical_value",
+                type_=vmwareengine_resources.PrivateConnection.Type.PRIVATE_SERVICE_ACCESS,
+                peering_id="peering_id_value",
+                routing_mode=vmwareengine_resources.PrivateConnection.RoutingMode.GLOBAL,
+                uid="uid_value",
+                service_network="service_network_value",
+                peering_state=vmwareengine_resources.PrivateConnection.PeeringState.PEERING_ACTIVE,
+            )
+        )
+        response = await client.get_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.GetPrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, vmwareengine_resources.PrivateConnection)
+    assert response.name == "name_value"
+    assert response.description == "description_value"
+    assert response.state == vmwareengine_resources.PrivateConnection.State.CREATING
+    assert response.vmware_engine_network == "vmware_engine_network_value"
+    assert (
+        response.vmware_engine_network_canonical
+        == "vmware_engine_network_canonical_value"
+    )
+    assert (
+        response.type_
+        == vmwareengine_resources.PrivateConnection.Type.PRIVATE_SERVICE_ACCESS
+    )
+    assert response.peering_id == "peering_id_value"
+    assert (
+        response.routing_mode
+        == vmwareengine_resources.PrivateConnection.RoutingMode.GLOBAL
+    )
+    assert response.uid == "uid_value"
+    assert response.service_network == "service_network_value"
+    assert (
+        response.peering_state
+        == vmwareengine_resources.PrivateConnection.PeeringState.PEERING_ACTIVE
+    )
+
+
+@pytest.mark.asyncio
+async def test_get_private_connection_async_from_dict():
+    await test_get_private_connection_async(request_type=dict)
+
+
+def test_get_private_connection_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.GetPrivateConnectionRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_private_connection), "__call__"
+    ) as call:
+        call.return_value = vmwareengine_resources.PrivateConnection()
+        client.get_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_private_connection_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.GetPrivateConnectionRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_private_connection), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine_resources.PrivateConnection()
+        )
+        await client.get_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+def test_get_private_connection_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine_resources.PrivateConnection()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.get_private_connection(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+def test_get_private_connection_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.get_private_connection(
+            vmwareengine.GetPrivateConnectionRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_private_connection_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine_resources.PrivateConnection()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine_resources.PrivateConnection()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.get_private_connection(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_get_private_connection_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.get_private_connection(
+            vmwareengine.GetPrivateConnectionRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.ListPrivateConnectionsRequest,
+        dict,
+    ],
+)
+def test_list_private_connections(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine.ListPrivateConnectionsResponse(
+            next_page_token="next_page_token_value",
+            unreachable=["unreachable_value"],
+        )
+        response = client.list_private_connections(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.ListPrivateConnectionsRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListPrivateConnectionsPager)
+    assert response.next_page_token == "next_page_token_value"
+    assert response.unreachable == ["unreachable_value"]
+
+
+def test_list_private_connections_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        client.list_private_connections()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.ListPrivateConnectionsRequest()
+
+
+@pytest.mark.asyncio
+async def test_list_private_connections_async(
+    transport: str = "grpc_asyncio",
+    request_type=vmwareengine.ListPrivateConnectionsRequest,
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine.ListPrivateConnectionsResponse(
+                next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
+            )
+        )
+        response = await client.list_private_connections(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.ListPrivateConnectionsRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListPrivateConnectionsAsyncPager)
+    assert response.next_page_token == "next_page_token_value"
+    assert response.unreachable == ["unreachable_value"]
+
+
+@pytest.mark.asyncio
+async def test_list_private_connections_async_from_dict():
+    await test_list_private_connections_async(request_type=dict)
+
+
+def test_list_private_connections_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.ListPrivateConnectionsRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        call.return_value = vmwareengine.ListPrivateConnectionsResponse()
+        client.list_private_connections(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_private_connections_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.ListPrivateConnectionsRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine.ListPrivateConnectionsResponse()
+        )
+        await client.list_private_connections(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+def test_list_private_connections_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine.ListPrivateConnectionsResponse()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.list_private_connections(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+def test_list_private_connections_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_private_connections(
+            vmwareengine.ListPrivateConnectionsRequest(),
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_private_connections_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine.ListPrivateConnectionsResponse()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine.ListPrivateConnectionsResponse()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.list_private_connections(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_list_private_connections_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.list_private_connections(
+            vmwareengine.ListPrivateConnectionsRequest(),
+            parent="parent_value",
+        )
+
+
+def test_list_private_connections_pager(transport_name: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+            ),
+            RuntimeError,
+        )
+
+        metadata = ()
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", ""),)),
+        )
+        pager = client.list_private_connections(request={})
+
+        assert pager._metadata == metadata
+
+        results = list(pager)
+        assert len(results) == 6
+        assert all(
+            isinstance(i, vmwareengine_resources.PrivateConnection) for i in results
+        )
+
+
+def test_list_private_connections_pages(transport_name: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = list(client.list_private_connections(request={}).pages)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.asyncio
+async def test_list_private_connections_async_pager():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+            ),
+            RuntimeError,
+        )
+        async_pager = await client.list_private_connections(
+            request={},
+        )
+        assert async_pager.next_page_token == "abc"
+        responses = []
+        async for response in async_pager:  # pragma: no branch
+            responses.append(response)
+
+        assert len(responses) == 6
+        assert all(
+            isinstance(i, vmwareengine_resources.PrivateConnection) for i in responses
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_private_connections_async_pages():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connections),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = []
+        async for page_ in (
+            await client.list_private_connections(request={})
+        ).pages:  # pragma: no branch
+            pages.append(page_)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.UpdatePrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_update_private_connection(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.update_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.UpdatePrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_update_private_connection_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_private_connection), "__call__"
+    ) as call:
+        client.update_private_connection()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.UpdatePrivateConnectionRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_private_connection_async(
+    transport: str = "grpc_asyncio",
+    request_type=vmwareengine.UpdatePrivateConnectionRequest,
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.update_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.UpdatePrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_update_private_connection_async_from_dict():
+    await test_update_private_connection_async(request_type=dict)
+
+
+def test_update_private_connection_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.UpdatePrivateConnectionRequest()
+
+    request.private_connection.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_private_connection), "__call__"
+    ) as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.update_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "private_connection.name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_update_private_connection_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.UpdatePrivateConnectionRequest()
+
+    request.private_connection.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_private_connection), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.update_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "private_connection.name=name_value",
+    ) in kw["metadata"]
+
+
+def test_update_private_connection_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.update_private_connection(
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].private_connection
+        mock_val = vmwareengine_resources.PrivateConnection(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+def test_update_private_connection_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_private_connection(
+            vmwareengine.UpdatePrivateConnectionRequest(),
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_private_connection_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.update_private_connection(
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].private_connection
+        mock_val = vmwareengine_resources.PrivateConnection(name="name_value")
+        assert arg == mock_val
+        arg = args[0].update_mask
+        mock_val = field_mask_pb2.FieldMask(paths=["paths_value"])
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_update_private_connection_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.update_private_connection(
+            vmwareengine.UpdatePrivateConnectionRequest(),
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.DeletePrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_delete_private_connection(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/spam")
+        response = client.delete_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.DeletePrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+def test_delete_private_connection_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_private_connection), "__call__"
+    ) as call:
+        client.delete_private_connection()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.DeletePrivateConnectionRequest()
+
+
+@pytest.mark.asyncio
+async def test_delete_private_connection_async(
+    transport: str = "grpc_asyncio",
+    request_type=vmwareengine.DeletePrivateConnectionRequest,
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.delete_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.DeletePrivateConnectionRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, future.Future)
+
+
+@pytest.mark.asyncio
+async def test_delete_private_connection_async_from_dict():
+    await test_delete_private_connection_async(request_type=dict)
+
+
+def test_delete_private_connection_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.DeletePrivateConnectionRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_private_connection), "__call__"
+    ) as call:
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        client.delete_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_delete_private_connection_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.DeletePrivateConnectionRequest()
+
+    request.name = "name_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_private_connection), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/op")
+        )
+        await client.delete_private_connection(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=name_value",
+    ) in kw["metadata"]
+
+
+def test_delete_private_connection_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.delete_private_connection(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+def test_delete_private_connection_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.delete_private_connection(
+            vmwareengine.DeletePrivateConnectionRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_private_connection_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_private_connection), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation(name="operations/op")
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.delete_private_connection(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_delete_private_connection_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.delete_private_connection(
+            vmwareengine.DeletePrivateConnectionRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+        dict,
+    ],
+)
+def test_list_private_connection_peering_routes(request_type, transport: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+            next_page_token="next_page_token_value",
+        )
+        response = client.list_private_connection_peering_routes(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.ListPrivateConnectionPeeringRoutesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListPrivateConnectionPeeringRoutesPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+def test_list_private_connection_peering_routes_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        client.list_private_connection_peering_routes()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.ListPrivateConnectionPeeringRoutesRequest()
+
+
+@pytest.mark.asyncio
+async def test_list_private_connection_peering_routes_async(
+    transport: str = "grpc_asyncio",
+    request_type=vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+):
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_private_connection_peering_routes(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == vmwareengine.ListPrivateConnectionPeeringRoutesRequest()
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListPrivateConnectionPeeringRoutesAsyncPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+@pytest.mark.asyncio
+async def test_list_private_connection_peering_routes_async_from_dict():
+    await test_list_private_connection_peering_routes_async(request_type=dict)
+
+
+def test_list_private_connection_peering_routes_field_headers():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        call.return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+        client.list_private_connection_peering_routes(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_private_connection_peering_routes_field_headers_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest()
+
+    request.parent = "parent_value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+        )
+        await client.list_private_connection_peering_routes(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "parent=parent_value",
+    ) in kw["metadata"]
+
+
+def test_list_private_connection_peering_routes_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.list_private_connection_peering_routes(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+def test_list_private_connection_peering_routes_flattened_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_private_connection_peering_routes(
+            vmwareengine.ListPrivateConnectionPeeringRoutesRequest(),
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_private_connection_peering_routes_flattened_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.list_private_connection_peering_routes(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_list_private_connection_peering_routes_flattened_error_async():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.list_private_connection_peering_routes(
+            vmwareengine.ListPrivateConnectionPeeringRoutesRequest(),
+            parent="parent_value",
+        )
+
+
+def test_list_private_connection_peering_routes_pager(transport_name: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+            ),
+            RuntimeError,
+        )
+
+        metadata = ()
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("parent", ""),)),
+        )
+        pager = client.list_private_connection_peering_routes(request={})
+
+        assert pager._metadata == metadata
+
+        results = list(pager)
+        assert len(results) == 6
+        assert all(isinstance(i, vmwareengine_resources.PeeringRoute) for i in results)
+
+
+def test_list_private_connection_peering_routes_pages(transport_name: str = "grpc"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials,
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = list(client.list_private_connection_peering_routes(request={}).pages)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.asyncio
+async def test_list_private_connection_peering_routes_async_pager():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+            ),
+            RuntimeError,
+        )
+        async_pager = await client.list_private_connection_peering_routes(
+            request={},
+        )
+        assert async_pager.next_page_token == "abc"
+        responses = []
+        async for response in async_pager:  # pragma: no branch
+            responses.append(response)
+
+        assert len(responses) == 6
+        assert all(
+            isinstance(i, vmwareengine_resources.PeeringRoute) for i in responses
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_private_connection_peering_routes_async_pages():
+    client = VmwareEngineAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_private_connection_peering_routes),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = []
+        async for page_ in (
+            await client.list_private_connection_peering_routes(request={})
+        ).pages:  # pragma: no branch
+            pages.append(page_)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         vmwareengine.ListPrivateCloudsRequest,
         dict,
     ],
 )
 def test_list_private_clouds_rest(request_type):
     client = VmwareEngineClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -10173,14 +12641,15 @@
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = vmwareengine_resources.PrivateCloud(
             name="name_value",
             state=vmwareengine_resources.PrivateCloud.State.ACTIVE,
             description="description_value",
             uid="uid_value",
+            type_=vmwareengine_resources.PrivateCloud.Type.TIME_LIMITED,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = vmwareengine_resources.PrivateCloud.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -10191,14 +12660,15 @@
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, vmwareengine_resources.PrivateCloud)
     assert response.name == "name_value"
     assert response.state == vmwareengine_resources.PrivateCloud.State.ACTIVE
     assert response.description == "description_value"
     assert response.uid == "uid_value"
+    assert response.type_ == vmwareengine_resources.PrivateCloud.Type.TIME_LIMITED
 
 
 def test_get_private_cloud_rest_required_fields(
     request_type=vmwareengine.GetPrivateCloudRequest,
 ):
     transport_class = transports.VmwareEngineRestTransport
 
@@ -10476,14 +12946,15 @@
         "vcenter": {
             "internal_ip": "internal_ip_value",
             "version": "version_value",
             "state": 1,
             "fqdn": "fqdn_value",
         },
         "uid": "uid_value",
+        "type_": 1,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -10724,14 +13195,15 @@
         "vcenter": {
             "internal_ip": "internal_ip_value",
             "version": "version_value",
             "state": 1,
             "fqdn": "fqdn_value",
         },
         "uid": "uid_value",
+        "type_": 1,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -10860,14 +13332,15 @@
         "vcenter": {
             "internal_ip": "internal_ip_value",
             "version": "version_value",
             "state": 1,
             "fqdn": "fqdn_value",
         },
         "uid": "uid_value",
+        "type_": 1,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = operations_pb2.Operation(name="operations/spam")
@@ -11091,14 +13564,15 @@
         "vcenter": {
             "internal_ip": "internal_ip_value",
             "version": "version_value",
             "state": 1,
             "fqdn": "fqdn_value",
         },
         "uid": "uid_value",
+        "type_": 1,
     }
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a BadRequest error.
     with mock.patch.object(Session, "request") as req, pytest.raises(
         core_exceptions.BadRequest
     ):
@@ -13285,14 +15759,15 @@
     request = request_type(**request_init)
 
     # Mock the http request call within the method and fake a response.
     with mock.patch.object(type(client.transport._session), "request") as req:
         # Designate an appropriate value for the returned response.
         return_value = vmwareengine.ListSubnetsResponse(
             next_page_token="next_page_token_value",
+            unreachable=["unreachable_value"],
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = vmwareengine.ListSubnetsResponse.pb(return_value)
         json_return_value = json_format.MessageToJson(pb_return_value)
@@ -13300,14 +15775,15 @@
         response_value._content = json_return_value.encode("UTF-8")
         req.return_value = response_value
         response = client.list_subnets(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListSubnetsPager)
     assert response.next_page_token == "next_page_token_value"
+    assert response.unreachable == ["unreachable_value"]
 
 
 def test_list_subnets_rest_required_fields(
     request_type=vmwareengine.ListSubnetsRequest,
 ):
     transport_class = transports.VmwareEngineRestTransport
 
@@ -13610,14 +16086,589 @@
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
 @pytest.mark.parametrize(
     "request_type",
     [
+        vmwareengine.GetSubnetRequest,
+        dict,
+    ],
+)
+def test_get_subnet_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine_resources.Subnet(
+            name="name_value",
+            ip_cidr_range="ip_cidr_range_value",
+            gateway_ip="gateway_ip_value",
+            type_="type__value",
+            state=vmwareengine_resources.Subnet.State.ACTIVE,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine_resources.Subnet.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.get_subnet(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, vmwareengine_resources.Subnet)
+    assert response.name == "name_value"
+    assert response.ip_cidr_range == "ip_cidr_range_value"
+    assert response.gateway_ip == "gateway_ip_value"
+    assert response.type_ == "type__value"
+    assert response.state == vmwareengine_resources.Subnet.State.ACTIVE
+
+
+def test_get_subnet_rest_required_fields(request_type=vmwareengine.GetSubnetRequest):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request_init["name"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).get_subnet._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["name"] = "name_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).get_subnet._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "name" in jsonified_request
+    assert jsonified_request["name"] == "name_value"
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = vmwareengine_resources.Subnet()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = vmwareengine_resources.Subnet.pb(return_value)
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.get_subnet(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_get_subnet_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.get_subnet._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("name",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_get_subnet_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "post_get_subnet"
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "pre_get_subnet"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.GetSubnetRequest.pb(vmwareengine.GetSubnetRequest())
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = vmwareengine_resources.Subnet.to_json(
+            vmwareengine_resources.Subnet()
+        )
+
+        request = vmwareengine.GetSubnetRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = vmwareengine_resources.Subnet()
+
+        client.get_subnet(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_get_subnet_rest_bad_request(
+    transport: str = "rest", request_type=vmwareengine.GetSubnetRequest
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_subnet(request)
+
+
+def test_get_subnet_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine_resources.Subnet()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4"
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            name="name_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine_resources.Subnet.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.get_subnet(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{name=projects/*/locations/*/privateClouds/*/subnets/*}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_get_subnet_rest_flattened_error(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.get_subnet(
+            vmwareengine.GetSubnetRequest(),
+            name="name_value",
+        )
+
+
+def test_get_subnet_rest_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.UpdateSubnetRequest,
+        dict,
+    ],
+)
+def test_update_subnet_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "subnet": {
+            "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4"
+        }
+    }
+    request_init["subnet"] = {
+        "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4",
+        "ip_cidr_range": "ip_cidr_range_value",
+        "gateway_ip": "gateway_ip_value",
+        "type_": "type__value",
+        "state": 1,
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.update_subnet(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+def test_update_subnet_rest_required_fields(
+    request_type=vmwareengine.UpdateSubnetRequest,
+):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_subnet._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_subnet._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(("update_mask",))
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = operations_pb2.Operation(name="operations/spam")
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "patch",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.update_subnet(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_update_subnet_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.update_subnet._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(("updateMask",))
+        & set(
+            (
+                "updateMask",
+                "subnet",
+            )
+        )
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_update_subnet_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "post_update_subnet"
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "pre_update_subnet"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.UpdateSubnetRequest.pb(
+            vmwareengine.UpdateSubnetRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = vmwareengine.UpdateSubnetRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.update_subnet(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_update_subnet_rest_bad_request(
+    transport: str = "rest", request_type=vmwareengine.UpdateSubnetRequest
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "subnet": {
+            "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4"
+        }
+    }
+    request_init["subnet"] = {
+        "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4",
+        "ip_cidr_range": "ip_cidr_range_value",
+        "gateway_ip": "gateway_ip_value",
+        "type_": "type__value",
+        "state": 1,
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.update_subnet(request)
+
+
+def test_update_subnet_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "subnet": {
+                "name": "projects/sample1/locations/sample2/privateClouds/sample3/subnets/sample4"
+            }
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            subnet=vmwareengine_resources.Subnet(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.update_subnet(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{subnet.name=projects/*/locations/*/privateClouds/*/subnets/*}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_update_subnet_rest_flattened_error(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_subnet(
+            vmwareengine.UpdateSubnetRequest(),
+            subnet=vmwareengine_resources.Subnet(name="name_value"),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+def test_update_subnet_rest_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
         vmwareengine.ListNodeTypesRequest,
         dict,
     ],
 )
 def test_list_node_types_rest(request_type):
     client = VmwareEngineClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -19408,14 +22459,1977 @@
         )
 
         pages = list(client.list_vmware_engine_networks(request=sample_request).pages)
         for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
             assert page_.raw_page.next_page_token == token
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.CreatePrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_create_private_connection_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"parent": "projects/sample1/locations/sample2"}
+    request_init["private_connection"] = {
+        "name": "name_value",
+        "create_time": {"seconds": 751, "nanos": 543},
+        "update_time": {},
+        "description": "description_value",
+        "state": 1,
+        "vmware_engine_network": "vmware_engine_network_value",
+        "vmware_engine_network_canonical": "vmware_engine_network_canonical_value",
+        "type_": 1,
+        "peering_id": "peering_id_value",
+        "routing_mode": 1,
+        "uid": "uid_value",
+        "service_network": "service_network_value",
+        "peering_state": 1,
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.create_private_connection(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+def test_create_private_connection_rest_required_fields(
+    request_type=vmwareengine.CreatePrivateConnectionRequest,
+):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request_init["parent"] = ""
+    request_init["private_connection_id"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+    assert "privateConnectionId" not in jsonified_request
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).create_private_connection._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+    assert "privateConnectionId" in jsonified_request
+    assert (
+        jsonified_request["privateConnectionId"]
+        == request_init["private_connection_id"]
+    )
+
+    jsonified_request["parent"] = "parent_value"
+    jsonified_request["privateConnectionId"] = "private_connection_id_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).create_private_connection._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(
+        (
+            "private_connection_id",
+            "request_id",
+        )
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "parent" in jsonified_request
+    assert jsonified_request["parent"] == "parent_value"
+    assert "privateConnectionId" in jsonified_request
+    assert jsonified_request["privateConnectionId"] == "private_connection_id_value"
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = operations_pb2.Operation(name="operations/spam")
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "post",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.create_private_connection(request)
+
+            expected_params = [
+                (
+                    "privateConnectionId",
+                    "",
+                ),
+                ("$alt", "json;enum-encoding=int"),
+            ]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_create_private_connection_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.create_private_connection._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(
+            (
+                "privateConnectionId",
+                "requestId",
+            )
+        )
+        & set(
+            (
+                "parent",
+                "privateConnectionId",
+                "privateConnection",
+            )
+        )
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_create_private_connection_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "post_create_private_connection"
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "pre_create_private_connection"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.CreatePrivateConnectionRequest.pb(
+            vmwareengine.CreatePrivateConnectionRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = vmwareengine.CreatePrivateConnectionRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.create_private_connection(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_create_private_connection_rest_bad_request(
+    transport: str = "rest", request_type=vmwareengine.CreatePrivateConnectionRequest
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"parent": "projects/sample1/locations/sample2"}
+    request_init["private_connection"] = {
+        "name": "name_value",
+        "create_time": {"seconds": 751, "nanos": 543},
+        "update_time": {},
+        "description": "description_value",
+        "state": 1,
+        "vmware_engine_network": "vmware_engine_network_value",
+        "vmware_engine_network_canonical": "vmware_engine_network_canonical_value",
+        "type_": 1,
+        "peering_id": "peering_id_value",
+        "routing_mode": 1,
+        "uid": "uid_value",
+        "service_network": "service_network_value",
+        "peering_state": 1,
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.create_private_connection(request)
+
+
+def test_create_private_connection_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {"parent": "projects/sample1/locations/sample2"}
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            parent="parent_value",
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            private_connection_id="private_connection_id_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.create_private_connection(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{parent=projects/*/locations/*}/privateConnections"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_create_private_connection_rest_flattened_error(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.create_private_connection(
+            vmwareengine.CreatePrivateConnectionRequest(),
+            parent="parent_value",
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            private_connection_id="private_connection_id_value",
+        )
+
+
+def test_create_private_connection_rest_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.GetPrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_get_private_connection_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine_resources.PrivateConnection(
+            name="name_value",
+            description="description_value",
+            state=vmwareengine_resources.PrivateConnection.State.CREATING,
+            vmware_engine_network="vmware_engine_network_value",
+            vmware_engine_network_canonical="vmware_engine_network_canonical_value",
+            type_=vmwareengine_resources.PrivateConnection.Type.PRIVATE_SERVICE_ACCESS,
+            peering_id="peering_id_value",
+            routing_mode=vmwareengine_resources.PrivateConnection.RoutingMode.GLOBAL,
+            uid="uid_value",
+            service_network="service_network_value",
+            peering_state=vmwareengine_resources.PrivateConnection.PeeringState.PEERING_ACTIVE,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine_resources.PrivateConnection.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.get_private_connection(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, vmwareengine_resources.PrivateConnection)
+    assert response.name == "name_value"
+    assert response.description == "description_value"
+    assert response.state == vmwareengine_resources.PrivateConnection.State.CREATING
+    assert response.vmware_engine_network == "vmware_engine_network_value"
+    assert (
+        response.vmware_engine_network_canonical
+        == "vmware_engine_network_canonical_value"
+    )
+    assert (
+        response.type_
+        == vmwareengine_resources.PrivateConnection.Type.PRIVATE_SERVICE_ACCESS
+    )
+    assert response.peering_id == "peering_id_value"
+    assert (
+        response.routing_mode
+        == vmwareengine_resources.PrivateConnection.RoutingMode.GLOBAL
+    )
+    assert response.uid == "uid_value"
+    assert response.service_network == "service_network_value"
+    assert (
+        response.peering_state
+        == vmwareengine_resources.PrivateConnection.PeeringState.PEERING_ACTIVE
+    )
+
+
+def test_get_private_connection_rest_required_fields(
+    request_type=vmwareengine.GetPrivateConnectionRequest,
+):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request_init["name"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).get_private_connection._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["name"] = "name_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).get_private_connection._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "name" in jsonified_request
+    assert jsonified_request["name"] == "name_value"
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = vmwareengine_resources.PrivateConnection()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = vmwareengine_resources.PrivateConnection.pb(return_value)
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.get_private_connection(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_get_private_connection_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.get_private_connection._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("name",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_get_private_connection_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "post_get_private_connection"
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "pre_get_private_connection"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.GetPrivateConnectionRequest.pb(
+            vmwareengine.GetPrivateConnectionRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = vmwareengine_resources.PrivateConnection.to_json(
+            vmwareengine_resources.PrivateConnection()
+        )
+
+        request = vmwareengine.GetPrivateConnectionRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = vmwareengine_resources.PrivateConnection()
+
+        client.get_private_connection(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_get_private_connection_rest_bad_request(
+    transport: str = "rest", request_type=vmwareengine.GetPrivateConnectionRequest
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_private_connection(request)
+
+
+def test_get_private_connection_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine_resources.PrivateConnection()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            name="name_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine_resources.PrivateConnection.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.get_private_connection(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{name=projects/*/locations/*/privateConnections/*}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_get_private_connection_rest_flattened_error(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.get_private_connection(
+            vmwareengine.GetPrivateConnectionRequest(),
+            name="name_value",
+        )
+
+
+def test_get_private_connection_rest_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.ListPrivateConnectionsRequest,
+        dict,
+    ],
+)
+def test_list_private_connections_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"parent": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine.ListPrivateConnectionsResponse(
+            next_page_token="next_page_token_value",
+            unreachable=["unreachable_value"],
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine.ListPrivateConnectionsResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.list_private_connections(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListPrivateConnectionsPager)
+    assert response.next_page_token == "next_page_token_value"
+    assert response.unreachable == ["unreachable_value"]
+
+
+def test_list_private_connections_rest_required_fields(
+    request_type=vmwareengine.ListPrivateConnectionsRequest,
+):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request_init["parent"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_private_connections._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["parent"] = "parent_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_private_connections._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(
+        (
+            "filter",
+            "order_by",
+            "page_size",
+            "page_token",
+        )
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "parent" in jsonified_request
+    assert jsonified_request["parent"] == "parent_value"
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = vmwareengine.ListPrivateConnectionsResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = vmwareengine.ListPrivateConnectionsResponse.pb(
+                return_value
+            )
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.list_private_connections(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_list_private_connections_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.list_private_connections._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(
+            (
+                "filter",
+                "orderBy",
+                "pageSize",
+                "pageToken",
+            )
+        )
+        & set(("parent",))
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_list_private_connections_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "post_list_private_connections"
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "pre_list_private_connections"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.ListPrivateConnectionsRequest.pb(
+            vmwareengine.ListPrivateConnectionsRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = vmwareengine.ListPrivateConnectionsResponse.to_json(
+            vmwareengine.ListPrivateConnectionsResponse()
+        )
+
+        request = vmwareengine.ListPrivateConnectionsRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = vmwareengine.ListPrivateConnectionsResponse()
+
+        client.list_private_connections(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_list_private_connections_rest_bad_request(
+    transport: str = "rest", request_type=vmwareengine.ListPrivateConnectionsRequest
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"parent": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_private_connections(request)
+
+
+def test_list_private_connections_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine.ListPrivateConnectionsResponse()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {"parent": "projects/sample1/locations/sample2"}
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            parent="parent_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine.ListPrivateConnectionsResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.list_private_connections(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{parent=projects/*/locations/*}/privateConnections"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_list_private_connections_rest_flattened_error(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_private_connections(
+            vmwareengine.ListPrivateConnectionsRequest(),
+            parent="parent_value",
+        )
+
+
+def test_list_private_connections_rest_pager(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # TODO(kbandes): remove this mock unless there's a good reason for it.
+        # with mock.patch.object(path_template, 'transcode') as transcode:
+        # Set the response as a series of pages
+        response = (
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionsResponse(
+                private_connections=[
+                    vmwareengine_resources.PrivateConnection(),
+                    vmwareengine_resources.PrivateConnection(),
+                ],
+            ),
+        )
+        # Two responses for two calls
+        response = response + response
+
+        # Wrap the values into proper Response objs
+        response = tuple(
+            vmwareengine.ListPrivateConnectionsResponse.to_json(x) for x in response
+        )
+        return_values = tuple(Response() for i in response)
+        for return_val, response_val in zip(return_values, response):
+            return_val._content = response_val.encode("UTF-8")
+            return_val.status_code = 200
+        req.side_effect = return_values
+
+        sample_request = {"parent": "projects/sample1/locations/sample2"}
+
+        pager = client.list_private_connections(request=sample_request)
+
+        results = list(pager)
+        assert len(results) == 6
+        assert all(
+            isinstance(i, vmwareengine_resources.PrivateConnection) for i in results
+        )
+
+        pages = list(client.list_private_connections(request=sample_request).pages)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.UpdatePrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_update_private_connection_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "private_connection": {
+            "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+        }
+    }
+    request_init["private_connection"] = {
+        "name": "projects/sample1/locations/sample2/privateConnections/sample3",
+        "create_time": {"seconds": 751, "nanos": 543},
+        "update_time": {},
+        "description": "description_value",
+        "state": 1,
+        "vmware_engine_network": "vmware_engine_network_value",
+        "vmware_engine_network_canonical": "vmware_engine_network_canonical_value",
+        "type_": 1,
+        "peering_id": "peering_id_value",
+        "routing_mode": 1,
+        "uid": "uid_value",
+        "service_network": "service_network_value",
+        "peering_state": 1,
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.update_private_connection(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+def test_update_private_connection_rest_required_fields(
+    request_type=vmwareengine.UpdatePrivateConnectionRequest,
+):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_private_connection._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_private_connection._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(
+        (
+            "request_id",
+            "update_mask",
+        )
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = operations_pb2.Operation(name="operations/spam")
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "patch",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.update_private_connection(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_update_private_connection_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.update_private_connection._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(
+            (
+                "requestId",
+                "updateMask",
+            )
+        )
+        & set(
+            (
+                "privateConnection",
+                "updateMask",
+            )
+        )
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_update_private_connection_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "post_update_private_connection"
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "pre_update_private_connection"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.UpdatePrivateConnectionRequest.pb(
+            vmwareengine.UpdatePrivateConnectionRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = vmwareengine.UpdatePrivateConnectionRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.update_private_connection(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_update_private_connection_rest_bad_request(
+    transport: str = "rest", request_type=vmwareengine.UpdatePrivateConnectionRequest
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "private_connection": {
+            "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+        }
+    }
+    request_init["private_connection"] = {
+        "name": "projects/sample1/locations/sample2/privateConnections/sample3",
+        "create_time": {"seconds": 751, "nanos": 543},
+        "update_time": {},
+        "description": "description_value",
+        "state": 1,
+        "vmware_engine_network": "vmware_engine_network_value",
+        "vmware_engine_network_canonical": "vmware_engine_network_canonical_value",
+        "type_": 1,
+        "peering_id": "peering_id_value",
+        "routing_mode": 1,
+        "uid": "uid_value",
+        "service_network": "service_network_value",
+        "peering_state": 1,
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.update_private_connection(request)
+
+
+def test_update_private_connection_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "private_connection": {
+                "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+            }
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.update_private_connection(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{private_connection.name=projects/*/locations/*/privateConnections/*}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_update_private_connection_rest_flattened_error(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_private_connection(
+            vmwareengine.UpdatePrivateConnectionRequest(),
+            private_connection=vmwareengine_resources.PrivateConnection(
+                name="name_value"
+            ),
+            update_mask=field_mask_pb2.FieldMask(paths=["paths_value"]),
+        )
+
+
+def test_update_private_connection_rest_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.DeletePrivateConnectionRequest,
+        dict,
+    ],
+)
+def test_delete_private_connection_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.delete_private_connection(request)
+
+    # Establish that the response is the type that we expect.
+    assert response.operation.name == "operations/spam"
+
+
+def test_delete_private_connection_rest_required_fields(
+    request_type=vmwareengine.DeletePrivateConnectionRequest,
+):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request_init["name"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).delete_private_connection._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["name"] = "name_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).delete_private_connection._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(("request_id",))
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "name" in jsonified_request
+    assert jsonified_request["name"] == "name_value"
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = operations_pb2.Operation(name="operations/spam")
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "delete",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+            json_return_value = json_format.MessageToJson(return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.delete_private_connection(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_delete_private_connection_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.delete_private_connection._get_unset_required_fields({})
+    assert set(unset_fields) == (set(("requestId",)) & set(("name",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_delete_private_connection_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        operation.Operation, "_set_result_from_operation"
+    ), mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "post_delete_private_connection"
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor, "pre_delete_private_connection"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.DeletePrivateConnectionRequest.pb(
+            vmwareengine.DeletePrivateConnectionRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = json_format.MessageToJson(
+            operations_pb2.Operation()
+        )
+
+        request = vmwareengine.DeletePrivateConnectionRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = operations_pb2.Operation()
+
+        client.delete_private_connection(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_delete_private_connection_rest_bad_request(
+    transport: str = "rest", request_type=vmwareengine.DeletePrivateConnectionRequest
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.delete_private_connection(request)
+
+
+def test_delete_private_connection_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation(name="operations/spam")
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "name": "projects/sample1/locations/sample2/privateConnections/sample3"
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            name="name_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.delete_private_connection(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{name=projects/*/locations/*/privateConnections/*}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_delete_private_connection_rest_flattened_error(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.delete_private_connection(
+            vmwareengine.DeletePrivateConnectionRequest(),
+            name="name_value",
+        )
+
+
+def test_delete_private_connection_rest_error():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+        dict,
+    ],
+)
+def test_list_private_connection_peering_routes_rest(request_type):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "parent": "projects/sample1/locations/sample2/privateConnections/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+            next_page_token="next_page_token_value",
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse.pb(
+            return_value
+        )
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.list_private_connection_peering_routes(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListPrivateConnectionPeeringRoutesPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+def test_list_private_connection_peering_routes_rest_required_fields(
+    request_type=vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+):
+    transport_class = transports.VmwareEngineRestTransport
+
+    request_init = {}
+    request_init["parent"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_private_connection_peering_routes._get_unset_required_fields(
+        jsonified_request
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["parent"] = "parent_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_private_connection_peering_routes._get_unset_required_fields(
+        jsonified_request
+    )
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(
+        (
+            "page_size",
+            "page_token",
+        )
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "parent" in jsonified_request
+    assert jsonified_request["parent"] == "parent_value"
+
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = (
+                vmwareengine.ListPrivateConnectionPeeringRoutesResponse.pb(return_value)
+            )
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.list_private_connection_peering_routes(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_list_private_connection_peering_routes_rest_unset_required_fields():
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = (
+        transport.list_private_connection_peering_routes._get_unset_required_fields({})
+    )
+    assert set(unset_fields) == (
+        set(
+            (
+                "pageSize",
+                "pageToken",
+            )
+        )
+        & set(("parent",))
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_list_private_connection_peering_routes_rest_interceptors(null_interceptor):
+    transport = transports.VmwareEngineRestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.VmwareEngineRestInterceptor(),
+    )
+    client = VmwareEngineClient(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.VmwareEngineRestInterceptor,
+        "post_list_private_connection_peering_routes",
+    ) as post, mock.patch.object(
+        transports.VmwareEngineRestInterceptor,
+        "pre_list_private_connection_peering_routes",
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = vmwareengine.ListPrivateConnectionPeeringRoutesRequest.pb(
+            vmwareengine.ListPrivateConnectionPeeringRoutesRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = (
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse.to_json(
+                vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+            )
+        )
+
+        request = vmwareengine.ListPrivateConnectionPeeringRoutesRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+
+        client.list_private_connection_peering_routes(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_list_private_connection_peering_routes_rest_bad_request(
+    transport: str = "rest",
+    request_type=vmwareengine.ListPrivateConnectionPeeringRoutesRequest,
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {
+        "parent": "projects/sample1/locations/sample2/privateConnections/sample3"
+    }
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_private_connection_peering_routes(request)
+
+
+def test_list_private_connection_peering_routes_rest_flattened():
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {
+            "parent": "projects/sample1/locations/sample2/privateConnections/sample3"
+        }
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            parent="parent_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = vmwareengine.ListPrivateConnectionPeeringRoutesResponse.pb(
+            return_value
+        )
+        json_return_value = json_format.MessageToJson(pb_return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.list_private_connection_peering_routes(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v1/{parent=projects/*/locations/*/privateConnections/*}/peeringRoutes"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_list_private_connection_peering_routes_rest_flattened_error(
+    transport: str = "rest",
+):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_private_connection_peering_routes(
+            vmwareengine.ListPrivateConnectionPeeringRoutesRequest(),
+            parent="parent_value",
+        )
+
+
+def test_list_private_connection_peering_routes_rest_pager(transport: str = "rest"):
+    client = VmwareEngineClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # TODO(kbandes): remove this mock unless there's a good reason for it.
+        # with mock.patch.object(path_template, 'transcode') as transcode:
+        # Set the response as a series of pages
+        response = (
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="abc",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[],
+                next_page_token="def",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+                next_page_token="ghi",
+            ),
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse(
+                peering_routes=[
+                    vmwareengine_resources.PeeringRoute(),
+                    vmwareengine_resources.PeeringRoute(),
+                ],
+            ),
+        )
+        # Two responses for two calls
+        response = response + response
+
+        # Wrap the values into proper Response objs
+        response = tuple(
+            vmwareengine.ListPrivateConnectionPeeringRoutesResponse.to_json(x)
+            for x in response
+        )
+        return_values = tuple(Response() for i in response)
+        for return_val, response_val in zip(return_values, response):
+            return_val._content = response_val.encode("UTF-8")
+            return_val.status_code = 200
+        req.side_effect = return_values
+
+        sample_request = {
+            "parent": "projects/sample1/locations/sample2/privateConnections/sample3"
+        }
+
+        pager = client.list_private_connection_peering_routes(request=sample_request)
+
+        results = list(pager)
+        assert len(results) == 6
+        assert all(isinstance(i, vmwareengine_resources.PeeringRoute) for i in results)
+
+        pages = list(
+            client.list_private_connection_peering_routes(request=sample_request).pages
+        )
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.VmwareEngineGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = VmwareEngineClient(
@@ -19559,14 +24573,16 @@
         "undelete_private_cloud",
         "list_clusters",
         "get_cluster",
         "create_cluster",
         "update_cluster",
         "delete_cluster",
         "list_subnets",
+        "get_subnet",
+        "update_subnet",
         "list_node_types",
         "get_node_type",
         "show_nsx_credentials",
         "show_vcenter_credentials",
         "reset_nsx_credentials",
         "reset_vcenter_credentials",
         "create_hcx_activation_key",
@@ -19578,14 +24594,20 @@
         "update_network_policy",
         "delete_network_policy",
         "create_vmware_engine_network",
         "update_vmware_engine_network",
         "delete_vmware_engine_network",
         "get_vmware_engine_network",
         "list_vmware_engine_networks",
+        "create_private_connection",
+        "get_private_connection",
+        "list_private_connections",
+        "update_private_connection",
+        "delete_private_connection",
+        "list_private_connection_peering_routes",
         "set_iam_policy",
         "get_iam_policy",
         "test_iam_permissions",
         "get_location",
         "list_locations",
         "get_operation",
         "delete_operation",
@@ -19899,14 +24921,20 @@
     assert session1 != session2
     session1 = client1.transport.delete_cluster._session
     session2 = client2.transport.delete_cluster._session
     assert session1 != session2
     session1 = client1.transport.list_subnets._session
     session2 = client2.transport.list_subnets._session
     assert session1 != session2
+    session1 = client1.transport.get_subnet._session
+    session2 = client2.transport.get_subnet._session
+    assert session1 != session2
+    session1 = client1.transport.update_subnet._session
+    session2 = client2.transport.update_subnet._session
+    assert session1 != session2
     session1 = client1.transport.list_node_types._session
     session2 = client2.transport.list_node_types._session
     assert session1 != session2
     session1 = client1.transport.get_node_type._session
     session2 = client2.transport.get_node_type._session
     assert session1 != session2
     session1 = client1.transport.show_nsx_credentials._session
@@ -19956,14 +24984,32 @@
     assert session1 != session2
     session1 = client1.transport.get_vmware_engine_network._session
     session2 = client2.transport.get_vmware_engine_network._session
     assert session1 != session2
     session1 = client1.transport.list_vmware_engine_networks._session
     session2 = client2.transport.list_vmware_engine_networks._session
     assert session1 != session2
+    session1 = client1.transport.create_private_connection._session
+    session2 = client2.transport.create_private_connection._session
+    assert session1 != session2
+    session1 = client1.transport.get_private_connection._session
+    session2 = client2.transport.get_private_connection._session
+    assert session1 != session2
+    session1 = client1.transport.list_private_connections._session
+    session2 = client2.transport.list_private_connections._session
+    assert session1 != session2
+    session1 = client1.transport.update_private_connection._session
+    session2 = client2.transport.update_private_connection._session
+    assert session1 != session2
+    session1 = client1.transport.delete_private_connection._session
+    session2 = client2.transport.delete_private_connection._session
+    assert session1 != session2
+    session1 = client1.transport.list_private_connection_peering_routes._session
+    session2 = client2.transport.list_private_connection_peering_routes._session
+    assert session1 != session2
 
 
 def test_vmware_engine_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.VmwareEngineGrpcTransport(
@@ -20273,166 +25319,194 @@
     path = VmwareEngineClient.private_cloud_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_private_cloud_path(path)
     assert expected == actual
 
 
-def test_subnet_path():
+def test_private_connection_path():
     project = "whelk"
     location = "octopus"
-    private_cloud = "oyster"
-    subnet = "nudibranch"
+    private_connection = "oyster"
+    expected = "projects/{project}/locations/{location}/privateConnections/{private_connection}".format(
+        project=project,
+        location=location,
+        private_connection=private_connection,
+    )
+    actual = VmwareEngineClient.private_connection_path(
+        project, location, private_connection
+    )
+    assert expected == actual
+
+
+def test_parse_private_connection_path():
+    expected = {
+        "project": "nudibranch",
+        "location": "cuttlefish",
+        "private_connection": "mussel",
+    }
+    path = VmwareEngineClient.private_connection_path(**expected)
+
+    # Check that the path construction is reversible.
+    actual = VmwareEngineClient.parse_private_connection_path(path)
+    assert expected == actual
+
+
+def test_subnet_path():
+    project = "winkle"
+    location = "nautilus"
+    private_cloud = "scallop"
+    subnet = "abalone"
     expected = "projects/{project}/locations/{location}/privateClouds/{private_cloud}/subnets/{subnet}".format(
         project=project,
         location=location,
         private_cloud=private_cloud,
         subnet=subnet,
     )
     actual = VmwareEngineClient.subnet_path(project, location, private_cloud, subnet)
     assert expected == actual
 
 
 def test_parse_subnet_path():
     expected = {
-        "project": "cuttlefish",
-        "location": "mussel",
-        "private_cloud": "winkle",
-        "subnet": "nautilus",
+        "project": "squid",
+        "location": "clam",
+        "private_cloud": "whelk",
+        "subnet": "octopus",
     }
     path = VmwareEngineClient.subnet_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_subnet_path(path)
     assert expected == actual
 
 
 def test_vmware_engine_network_path():
-    project = "scallop"
-    location = "abalone"
-    vmware_engine_network = "squid"
+    project = "oyster"
+    location = "nudibranch"
+    vmware_engine_network = "cuttlefish"
     expected = "projects/{project}/locations/{location}/vmwareEngineNetworks/{vmware_engine_network}".format(
         project=project,
         location=location,
         vmware_engine_network=vmware_engine_network,
     )
     actual = VmwareEngineClient.vmware_engine_network_path(
         project, location, vmware_engine_network
     )
     assert expected == actual
 
 
 def test_parse_vmware_engine_network_path():
     expected = {
-        "project": "clam",
-        "location": "whelk",
-        "vmware_engine_network": "octopus",
+        "project": "mussel",
+        "location": "winkle",
+        "vmware_engine_network": "nautilus",
     }
     path = VmwareEngineClient.vmware_engine_network_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_vmware_engine_network_path(path)
     assert expected == actual
 
 
 def test_common_billing_account_path():
-    billing_account = "oyster"
+    billing_account = "scallop"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = VmwareEngineClient.common_billing_account_path(billing_account)
     assert expected == actual
 
 
 def test_parse_common_billing_account_path():
     expected = {
-        "billing_account": "nudibranch",
+        "billing_account": "abalone",
     }
     path = VmwareEngineClient.common_billing_account_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
-    folder = "cuttlefish"
+    folder = "squid"
     expected = "folders/{folder}".format(
         folder=folder,
     )
     actual = VmwareEngineClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
-        "folder": "mussel",
+        "folder": "clam",
     }
     path = VmwareEngineClient.common_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
-    organization = "winkle"
+    organization = "whelk"
     expected = "organizations/{organization}".format(
         organization=organization,
     )
     actual = VmwareEngineClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
-        "organization": "nautilus",
+        "organization": "octopus",
     }
     path = VmwareEngineClient.common_organization_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
-    project = "scallop"
+    project = "oyster"
     expected = "projects/{project}".format(
         project=project,
     )
     actual = VmwareEngineClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
-        "project": "abalone",
+        "project": "nudibranch",
     }
     path = VmwareEngineClient.common_project_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_common_project_path(path)
     assert expected == actual
 
 
 def test_common_location_path():
-    project = "squid"
-    location = "clam"
+    project = "cuttlefish"
+    location = "mussel"
     expected = "projects/{project}/locations/{location}".format(
         project=project,
         location=location,
     )
     actual = VmwareEngineClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
-        "project": "whelk",
-        "location": "octopus",
+        "project": "winkle",
+        "location": "nautilus",
     }
     path = VmwareEngineClient.common_location_path(**expected)
 
     # Check that the path construction is reversible.
     actual = VmwareEngineClient.parse_common_location_path(path)
     assert expected == actual
```

