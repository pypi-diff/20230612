# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.911.tar", last modified: Fri Jun  9 02:23:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.912.tar", last modified: Mon Jun 12 03:08:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.911.tar` & `tencentcloud-sdk-python-mps-3.0.912.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)    90653 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)   820599 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:23:23.000000 tencentcloud-sdk-python-mps-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)    99031 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   836509 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:08:03.000000 tencentcloud-sdk-python-mps-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mps-3.0.911/README.rst` & `tencentcloud-sdk-python-mps-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/mps_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,83 @@
 
 class MpsClient(AbstractClient):
     _apiVersion = '2019-06-12'
     _endpoint = 'mps.tencentcloudapi.com'
     _service = 'mps'
 
 
+    def BatchDeleteStreamLinkFlow(self, request):
+        """批量删除媒体传输流。
+
+        :param request: Request instance for BatchDeleteStreamLinkFlow.
+        :type request: :class:`tencentcloud.mps.v20190612.models.BatchDeleteStreamLinkFlowRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.BatchDeleteStreamLinkFlowResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("BatchDeleteStreamLinkFlow", params, headers=headers)
+            response = json.loads(body)
+            model = models.BatchDeleteStreamLinkFlowResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def BatchStartStreamLinkFlow(self, request):
+        """批量启动媒体传输流。
+
+        :param request: Request instance for BatchStartStreamLinkFlow.
+        :type request: :class:`tencentcloud.mps.v20190612.models.BatchStartStreamLinkFlowRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.BatchStartStreamLinkFlowResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("BatchStartStreamLinkFlow", params, headers=headers)
+            response = json.loads(body)
+            model = models.BatchStartStreamLinkFlowResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def BatchStopStreamLinkFlow(self, request):
+        """批量停止媒体传输流。
+
+        :param request: Request instance for BatchStopStreamLinkFlow.
+        :type request: :class:`tencentcloud.mps.v20190612.models.BatchStopStreamLinkFlowRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.BatchStopStreamLinkFlowResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("BatchStopStreamLinkFlow", params, headers=headers)
+            response = json.loads(body)
+            model = models.BatchStopStreamLinkFlowResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateAIAnalysisTemplate(self, request):
         """创建用户自定义内容分析模板，数量上限：50。
 
         :param request: Request instance for CreateAIAnalysisTemplate.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateAIAnalysisTemplateRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.CreateAIAnalysisTemplateResponse`
 
@@ -263,14 +332,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateStreamLinkEvent(self, request):
+        """创建媒体传输的事件Event。
+
+        :param request: Request instance for CreateStreamLinkEvent.
+        :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkEventRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateStreamLinkEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateStreamLinkEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateStreamLinkFlow(self, request):
         """创建媒体传输的传输流配置。
 
         :param request: Request instance for CreateStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkFlowRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkFlowResponse`
 
@@ -667,14 +759,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteStreamLinkEvent(self, request):
+        """删除媒体传输的事件配置。
+
+        :param request: Request instance for DeleteStreamLinkEvent.
+        :type request: :class:`tencentcloud.mps.v20190612.models.DeleteStreamLinkEventRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.DeleteStreamLinkEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteStreamLinkEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteStreamLinkEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteStreamLinkFlow(self, request):
         """删除媒体传输的传输流配置。
 
         :param request: Request instance for DeleteStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.DeleteStreamLinkFlowRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.DeleteStreamLinkFlowResponse`
 
@@ -1081,14 +1196,83 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeStreamLinkEvent(self, request):
+        """查询媒体传输事件的配置信息。
+
+        :param request: Request instance for DescribeStreamLinkEvent.
+        :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeStreamLinkEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeStreamLinkEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeStreamLinkEventAttachedFlows(self, request):
+        """查询媒体传输事件关联的所有媒体输入流的配置信息。
+
+        :param request: Request instance for DescribeStreamLinkEventAttachedFlows.
+        :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventAttachedFlowsRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventAttachedFlowsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeStreamLinkEventAttachedFlows", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeStreamLinkEventAttachedFlowsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeStreamLinkEvents(self, request):
+        """批量查询媒体传输事件的配置信息。
+
+        :param request: Request instance for DescribeStreamLinkEvents.
+        :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventsRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkEventsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeStreamLinkEvents", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeStreamLinkEventsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeStreamLinkFlow(self, request):
         """查询媒体输入流的配置信息。
 
         :param request: Request instance for DescribeStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.DescribeStreamLinkFlowResponse`
 
@@ -1800,14 +1984,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyStreamLinkEvent(self, request):
+        """修改媒体传输的事件配置信息。
+
+        :param request: Request instance for ModifyStreamLinkEvent.
+        :type request: :class:`tencentcloud.mps.v20190612.models.ModifyStreamLinkEventRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.ModifyStreamLinkEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyStreamLinkEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyStreamLinkEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyStreamLinkFlow(self, request):
         """修改媒体传输的传输流配置信息。
 
         :param request: Request instance for ModifyStreamLinkFlow.
         :type request: :class:`tencentcloud.mps.v20190612.models.ModifyStreamLinkFlowRequest`
```

### Comparing `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.911/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.912/tencentcloud/mps/v20190612/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4493,14 +4493,149 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BatchDeleteStreamLinkFlowRequest(AbstractModel):
+    """BatchDeleteStreamLinkFlow请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventId: EventId。
+        :type EventId: str
+        :param FlowIds: Event关联的流Id数组，如果不传默认删除Event下面的所有媒体传输流。
+        :type FlowIds: list of str
+        """
+        self.EventId = None
+        self.FlowIds = None
+
+
+    def _deserialize(self, params):
+        self.EventId = params.get("EventId")
+        self.FlowIds = params.get("FlowIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BatchDeleteStreamLinkFlowResponse(AbstractModel):
+    """BatchDeleteStreamLinkFlow返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class BatchStartStreamLinkFlowRequest(AbstractModel):
+    """BatchStartStreamLinkFlow请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventId: EventId。
+        :type EventId: str
+        :param FlowIds: Event关联的流Id数组，如果不传默认启动Event下面的所有媒体传输流。
+        :type FlowIds: list of str
+        """
+        self.EventId = None
+        self.FlowIds = None
+
+
+    def _deserialize(self, params):
+        self.EventId = params.get("EventId")
+        self.FlowIds = params.get("FlowIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BatchStartStreamLinkFlowResponse(AbstractModel):
+    """BatchStartStreamLinkFlow返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class BatchStopStreamLinkFlowRequest(AbstractModel):
+    """BatchStopStreamLinkFlow请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventId: EventId。
+        :type EventId: str
+        :param FlowIds: 流Id，如果不传默认停止Event下所有的媒体传输流。
+        :type FlowIds: list of str
+        """
+        self.EventId = None
+        self.FlowIds = None
+
+
+    def _deserialize(self, params):
+        self.EventId = params.get("EventId")
+        self.FlowIds = params.get("FlowIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BatchStopStreamLinkFlowResponse(AbstractModel):
+    """BatchStopStreamLinkFlow返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ClassificationConfigureInfo(AbstractModel):
     """智能分类任务控制参数
 
     """
 
     def __init__(self):
         r"""
@@ -6194,14 +6329,65 @@
 
 
     def _deserialize(self, params):
         self.Definition = params.get("Definition")
         self.RequestId = params.get("RequestId")
 
 
+class CreateStreamLinkEventRequest(AbstractModel):
+    """CreateStreamLinkEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventName: 事件名称。
+        :type EventName: str
+        :param Description: 事件描述。
+        :type Description: str
+        """
+        self.EventName = None
+        self.Description = None
+
+
+    def _deserialize(self, params):
+        self.EventName = params.get("EventName")
+        self.Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateStreamLinkEventResponse(AbstractModel):
+    """CreateStreamLinkEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Info: 创建的Event信息。
+        :type Info: :class:`tencentcloud.mps.v20190612.models.DescribeEvent`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Info = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Info") is not None:
+            self.Info = DescribeEvent()
+            self.Info._deserialize(params.get("Info"))
+        self.RequestId = params.get("RequestId")
+
+
 class CreateStreamLinkFlowRequest(AbstractModel):
     """CreateStreamLinkFlow请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7123,14 +7309,55 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DeleteStreamLinkEventRequest(AbstractModel):
+    """DeleteStreamLinkEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventId: 媒体传输事件Id，删除前需要保证该Event关联的所有Flow都已经删除。
+        :type EventId: str
+        """
+        self.EventId = None
+
+
+    def _deserialize(self, params):
+        self.EventId = params.get("EventId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteStreamLinkEventResponse(AbstractModel):
+    """DeleteStreamLinkEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteStreamLinkFlowRequest(AbstractModel):
     """DeleteStreamLinkFlow请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7713,14 +7940,66 @@
             for item in params.get("ContentReviewTemplateSet"):
                 obj = ContentReviewTemplateItem()
                 obj._deserialize(item)
                 self.ContentReviewTemplateSet.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeEvent(AbstractModel):
+    """查询Event的配置信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventName: Event的名称。
+        :type EventName: str
+        :param EventId: Event的Id，唯一标识一个event。
+        :type EventId: str
+        :param CreateTime: Event创建时间，格式为yyyy-MM-ddTHH:mm:ssZ。
+        :type CreateTime: str
+        :param Description: Event的描述。
+        :type Description: str
+        :param Status: Event的状态信息
+0：未运行
+1：运行中
+        :type Status: int
+        :param AttachedFlowGroup: Event关联的Flow列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AttachedFlowGroup: list of DescribeFlowId
+        """
+        self.EventName = None
+        self.EventId = None
+        self.CreateTime = None
+        self.Description = None
+        self.Status = None
+        self.AttachedFlowGroup = None
+
+
+    def _deserialize(self, params):
+        self.EventName = params.get("EventName")
+        self.EventId = params.get("EventId")
+        self.CreateTime = params.get("CreateTime")
+        self.Description = params.get("Description")
+        self.Status = params.get("Status")
+        if params.get("AttachedFlowGroup") is not None:
+            self.AttachedFlowGroup = []
+            for item in params.get("AttachedFlowGroup"):
+                obj = DescribeFlowId()
+                obj._deserialize(item)
+                self.AttachedFlowGroup.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeFlow(AbstractModel):
     """查询Flow的配置信息。
 
     """
 
     def __init__(self):
         r"""
@@ -7776,14 +8055,42 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DescribeFlowId(AbstractModel):
+    """Event管理的Flow列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: FlowId，唯一标识一个flow。
+        :type FlowId: str
+        :param Region: flow所在的区域名称。
+        :type Region: str
+        """
+        self.FlowId = None
+        self.Region = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class DescribeHLSPullSourceAddress(AbstractModel):
     """查询输入的HLS配置信息。
 
     """
 
     def __init__(self):
         r"""
@@ -9039,14 +9346,193 @@
 
 
     def _deserialize(self, params):
         self.Status = params.get("Status")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeStreamLinkEventAttachedFlowsRequest(AbstractModel):
+    """DescribeStreamLinkEventAttachedFlows请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventId: EventId。
+        :type EventId: str
+        :param PageNum: 当前页数，默认1。
+        :type PageNum: int
+        :param PageSize: 每页大小，默认10。
+        :type PageSize: int
+        """
+        self.EventId = None
+        self.PageNum = None
+        self.PageSize = None
+
+
+    def _deserialize(self, params):
+        self.EventId = params.get("EventId")
+        self.PageNum = params.get("PageNum")
+        self.PageSize = params.get("PageSize")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeStreamLinkEventAttachedFlowsResponse(AbstractModel):
+    """DescribeStreamLinkEventAttachedFlows返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Infos: 流的配置信息列表。
+        :type Infos: list of DescribeFlow
+        :param TotalNum: 总数量。
+        :type TotalNum: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Infos = None
+        self.TotalNum = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Infos") is not None:
+            self.Infos = []
+            for item in params.get("Infos"):
+                obj = DescribeFlow()
+                obj._deserialize(item)
+                self.Infos.append(obj)
+        self.TotalNum = params.get("TotalNum")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeStreamLinkEventRequest(AbstractModel):
+    """DescribeStreamLinkEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventId: 媒体传输事件ID。
+        :type EventId: str
+        """
+        self.EventId = None
+
+
+    def _deserialize(self, params):
+        self.EventId = params.get("EventId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeStreamLinkEventResponse(AbstractModel):
+    """DescribeStreamLinkEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Info: 媒体传输事件的配置信息。
+        :type Info: :class:`tencentcloud.mps.v20190612.models.DescribeEvent`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Info = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Info") is not None:
+            self.Info = DescribeEvent()
+            self.Info._deserialize(params.get("Info"))
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeStreamLinkEventsRequest(AbstractModel):
+    """DescribeStreamLinkEvents请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PageNum: 当前页数，默认1。
+        :type PageNum: int
+        :param PageSize: 每页大小，默认10。
+        :type PageSize: int
+        """
+        self.PageNum = None
+        self.PageSize = None
+
+
+    def _deserialize(self, params):
+        self.PageNum = params.get("PageNum")
+        self.PageSize = params.get("PageSize")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeStreamLinkEventsResponse(AbstractModel):
+    """DescribeStreamLinkEvents返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Infos: 媒体传输事件的配置信息列表。
+        :type Infos: list of DescribeEvent
+        :param PageNum: 当前页数。
+        :type PageNum: int
+        :param PageSize: 每页大小。
+        :type PageSize: int
+        :param TotalNum: 总数量。
+        :type TotalNum: int
+        :param TotalPage: 总页数。
+        :type TotalPage: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Infos = None
+        self.PageNum = None
+        self.PageSize = None
+        self.TotalNum = None
+        self.TotalPage = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Infos") is not None:
+            self.Infos = []
+            for item in params.get("Infos"):
+                obj = DescribeEvent()
+                obj._deserialize(item)
+                self.Infos.append(obj)
+        self.PageNum = params.get("PageNum")
+        self.PageSize = params.get("PageSize")
+        self.TotalNum = params.get("TotalNum")
+        self.TotalPage = params.get("TotalPage")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeStreamLinkFlowLogsRequest(AbstractModel):
     """DescribeStreamLinkFlowLogs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -15422,14 +15908,63 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class ModifyStreamLinkEventRequest(AbstractModel):
+    """ModifyStreamLinkEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EventId: 媒体传输事件Event Id。
+        :type EventId: str
+        :param EventName: 需要修改的事件名称。
+        :type EventName: str
+        :param Description: Event的描述信息。
+        :type Description: str
+        """
+        self.EventId = None
+        self.EventName = None
+        self.Description = None
+
+
+    def _deserialize(self, params):
+        self.EventId = params.get("EventId")
+        self.EventName = params.get("EventName")
+        self.Description = params.get("Description")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyStreamLinkEventResponse(AbstractModel):
+    """ModifyStreamLinkEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-mps-3.0.911/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.912/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.911/setup.py` & `tencentcloud-sdk-python-mps-3.0.912/setup.py`

 * *Files identical despite different names*

