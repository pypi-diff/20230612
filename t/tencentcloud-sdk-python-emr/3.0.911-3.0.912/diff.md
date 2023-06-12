# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.911.tar", last modified: Fri Jun  9 02:19:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.912.tar", last modified: Mon Jun 12 03:03:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.911.tar` & `tencentcloud-sdk-python-emr-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    27330 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    13996 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260148 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:19:00.000000 tencentcloud-sdk-python-emr-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    27330 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    13996 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   262109 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:03:22.000000 tencentcloud-sdk-python-emr-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:03:23.000000 tencentcloud-sdk-python-emr-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-emr-3.0.911/README.rst` & `tencentcloud-sdk-python-emr-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.911/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.912/tencentcloud/emr/v20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6197,30 +6197,36 @@
         :param InstanceId: 集群ID
         :type InstanceId: str
         :param OpType: 操作类型，当前支持
 <li>StartService：启动服务</li>
 <li>StopService：停止服务</li>
 <li>StartMonitor：退出维护</li>
 <li>StopMonitor：进入维护</li>
-
+<li>RestartService：重启服务</li>
         :type OpType: str
         :param OpScope: 操作范围
         :type OpScope: :class:`tencentcloud.emr.v20190103.models.OpScope`
+        :param StrategyConfig: 操作策略
+        :type StrategyConfig: :class:`tencentcloud.emr.v20190103.models.StrategyConfig`
         """
         self.InstanceId = None
         self.OpType = None
         self.OpScope = None
+        self.StrategyConfig = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.OpType = params.get("OpType")
         if params.get("OpScope") is not None:
             self.OpScope = OpScope()
             self.OpScope._deserialize(params.get("OpScope"))
+        if params.get("StrategyConfig") is not None:
+            self.StrategyConfig = StrategyConfig()
+            self.StrategyConfig._deserialize(params.get("StrategyConfig"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6277,14 +6283,55 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class StrategyConfig(AbstractModel):
+    """重启/停止/启动服务/监控的配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RollingRestartSwitch: 0:关闭滚动重启
+1:开启滚动启动
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RollingRestartSwitch: int
+        :param BatchSize: 滚动重启每批次的重启数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BatchSize: int
+        :param TimeWait: 滚动重启每批停止等待时间 ,最大重启台数为 99999 台，最大间隔为 5 分钟 单位是秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TimeWait: int
+        :param DealOnFail: 操作失败处理策略，0:失败阻塞, 1:失败自动跳过
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DealOnFail: int
+        """
+        self.RollingRestartSwitch = None
+        self.BatchSize = None
+        self.TimeWait = None
+        self.DealOnFail = None
+
+
+    def _deserialize(self, params):
+        self.RollingRestartSwitch = params.get("RollingRestartSwitch")
+        self.BatchSize = params.get("BatchSize")
+        self.TimeWait = params.get("TimeWait")
+        self.DealOnFail = params.get("DealOnFail")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class SubnetInfo(AbstractModel):
     """子网信息
 
     """
```

### Comparing `tencentcloud-sdk-python-emr-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.912/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.911/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.912/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.911/setup.py` & `tencentcloud-sdk-python-emr-3.0.912/setup.py`

 * *Files identical despite different names*

