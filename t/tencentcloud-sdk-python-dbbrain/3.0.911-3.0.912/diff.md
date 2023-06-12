# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.911.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.912.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.911.tar", last modified: Fri Jun  9 02:17:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.912.tar", last modified: Mon Jun 12 03:01:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.911.tar` & `tencentcloud-sdk-python-dbbrain-3.0.912.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    48612 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   183066 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   111420 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-09 02:17:31.000000 tencentcloud-sdk-python-dbbrain-3.0.911/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    48612 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185526 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114440 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-12 03:01:45.000000 tencentcloud-sdk-python-dbbrain-3.0.912/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-12 03:01:46.000000 tencentcloud-sdk-python-dbbrain-3.0.912/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.912/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2596,30 +2596,43 @@
 
     def __init__(self):
         r"""
         :param TotalCount: 来源地址数目。
         :type TotalCount: int
         :param Items: 各来源地址的慢日志占比详情列表。
         :type Items: list of SlowLogHost
+        :param UserNameItems: 各来源用户名的慢日志占比详情列表。
+        :type UserNameItems: list of SlowLogUser
+        :param UserTotalCount: 来源用户数目。
+        :type UserTotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.Items = None
+        self.UserNameItems = None
+        self.UserTotalCount = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.TotalCount = params.get("TotalCount")
         if params.get("Items") is not None:
             self.Items = []
             for item in params.get("Items"):
                 obj = SlowLogHost()
                 obj._deserialize(item)
                 self.Items.append(obj)
+        if params.get("UserNameItems") is not None:
+            self.UserNameItems = []
+            for item in params.get("UserNameItems"):
+                obj = SlowLogUser()
+                obj._deserialize(item)
+                self.UserNameItems.append(obj)
+        self.UserTotalCount = params.get("UserTotalCount")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeSlowLogsRequest(AbstractModel):
     """DescribeSlowLogs请求参数结构体
 
     """
@@ -3641,22 +3654,28 @@
         :type IsSupported: bool
         :param SecAuditStatus: 实例安全审计日志开启状态：ON： 安全审计开启；OFF： 未开启安全审计。
         :type SecAuditStatus: str
         :param AuditPolicyStatus: 实例审计日志开启状态，ALL_AUDIT： 开启全审计；RULE_AUDIT： 开启规则审计；UNBOUND： 未开启审计。
         :type AuditPolicyStatus: str
         :param AuditRunningStatus: 实例审计日志运行状态：normal： 运行中； paused： 欠费暂停。
         :type AuditRunningStatus: str
-        :param InternalVip: 内网vip
+        :param InternalVip: 内网vip。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InternalVip: str
-        :param InternalVport: 内网port
+        :param InternalVport: 内网port。
 注意：此字段可能返回 null，表示取不到有效值。
         :type InternalVport: int
-        :param CreateTime: 创建时间
+        :param CreateTime: 创建时间。
         :type CreateTime: str
+        :param ClusterId: 所属集群ID（仅对集群数据库产品该字段非空，如TDSQL-C）。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param ClusterName: 所属集群名称（仅对集群数据库产品该字段非空，如TDSQL-C）。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterName: str
         """
         self.InstanceId = None
         self.InstanceName = None
         self.Region = None
         self.HealthScore = None
         self.Product = None
         self.EventCount = None
@@ -3681,14 +3700,16 @@
         self.IsSupported = None
         self.SecAuditStatus = None
         self.AuditPolicyStatus = None
         self.AuditRunningStatus = None
         self.InternalVip = None
         self.InternalVport = None
         self.CreateTime = None
+        self.ClusterId = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.Region = params.get("Region")
         self.HealthScore = params.get("HealthScore")
@@ -3717,14 +3738,16 @@
         self.IsSupported = params.get("IsSupported")
         self.SecAuditStatus = params.get("SecAuditStatus")
         self.AuditPolicyStatus = params.get("AuditPolicyStatus")
         self.AuditRunningStatus = params.get("AuditRunningStatus")
         self.InternalVip = params.get("InternalVip")
         self.InternalVport = params.get("InternalVport")
         self.CreateTime = params.get("CreateTime")
+        self.ClusterId = params.get("ClusterId")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4257,32 +4280,40 @@
         :type ExpireTime: int
         :param Length: key内存大小，单位Byte。
         :type Length: int
         :param ItemCount: 元素个数。
         :type ItemCount: int
         :param MaxElementSize: 最大元素长度。
         :type MaxElementSize: int
+        :param AveElementSize: 平均元素长度。
+        :type AveElementSize: int
+        :param ShardId: 所属分片序号。
+        :type ShardId: str
         """
         self.Key = None
         self.Type = None
         self.Encoding = None
         self.ExpireTime = None
         self.Length = None
         self.ItemCount = None
         self.MaxElementSize = None
+        self.AveElementSize = None
+        self.ShardId = None
 
 
     def _deserialize(self, params):
         self.Key = params.get("Key")
         self.Type = params.get("Type")
         self.Encoding = params.get("Encoding")
         self.ExpireTime = params.get("ExpireTime")
         self.Length = params.get("Length")
         self.ItemCount = params.get("ItemCount")
         self.MaxElementSize = params.get("MaxElementSize")
+        self.AveElementSize = params.get("AveElementSize")
+        self.ShardId = params.get("ShardId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4890,14 +4921,46 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SlowLogUser(AbstractModel):
+    """慢日志来源用户详情。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 来源用户名。
+        :type UserName: str
+        :param Ratio: 该来源用户名的慢日志数目占总数目的比例，单位%。
+        :type Ratio: float
+        :param Count: 该来源用户名的慢日志数目。
+        :type Count: int
+        """
+        self.UserName = None
+        self.Ratio = None
+        self.Count = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.Ratio = params.get("Ratio")
+        self.Count = params.get("Count")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class Table(AbstractModel):
     """表结构。
 
     """
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/dbbrain/v20191016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1425,30 +1425,43 @@
 
     def __init__(self):
         r"""
         :param TotalCount: 来源地址数目。
         :type TotalCount: int
         :param Items: 各来源地址的慢日志占比详情列表。
         :type Items: list of SlowLogHost
+        :param UserNameItems: 各来源用户名的慢日志占比详情列表。
+        :type UserNameItems: list of SlowLogUser
+        :param UserTotalCount: 来源用户数目。
+        :type UserTotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TotalCount = None
         self.Items = None
+        self.UserNameItems = None
+        self.UserTotalCount = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.TotalCount = params.get("TotalCount")
         if params.get("Items") is not None:
             self.Items = []
             for item in params.get("Items"):
                 obj = SlowLogHost()
                 obj._deserialize(item)
                 self.Items.append(obj)
+        if params.get("UserNameItems") is not None:
+            self.UserNameItems = []
+            for item in params.get("UserNameItems"):
+                obj = SlowLogUser()
+                obj._deserialize(item)
+                self.UserNameItems.append(obj)
+        self.UserTotalCount = params.get("UserTotalCount")
         self.RequestId = params.get("RequestId")
 
 
 class DescribeTopSpaceSchemaTimeSeriesRequest(AbstractModel):
     """DescribeTopSpaceSchemaTimeSeries请求参数结构体
 
     """
@@ -2138,22 +2151,27 @@
 
     def __init__(self):
         r"""
         :param DailyInspection: 数据库巡检开关, Yes/No。
         :type DailyInspection: str
         :param OverviewDisplay: 实例概览开关，Yes/No。
         :type OverviewDisplay: str
+        :param KeyDelimiters: redis大key分析的自定义分割符，仅redis使用
+注意：此字段可能返回 null，表示取不到有效值。
+        :type KeyDelimiters: list of str
         """
         self.DailyInspection = None
         self.OverviewDisplay = None
+        self.KeyDelimiters = None
 
 
     def _deserialize(self, params):
         self.DailyInspection = params.get("DailyInspection")
         self.OverviewDisplay = params.get("OverviewDisplay")
+        self.KeyDelimiters = params.get("KeyDelimiters")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2218,14 +2236,28 @@
         :type IsSupported: bool
         :param SecAuditStatus: 实例安全审计日志开启状态：ON： 安全审计开启；OFF： 未开启安全审计。
         :type SecAuditStatus: str
         :param AuditPolicyStatus: 实例审计日志开启状态，ALL_AUDIT： 开启全审计；RULE_AUDIT： 开启规则审计；UNBOUND： 未开启审计。
         :type AuditPolicyStatus: str
         :param AuditRunningStatus: 实例审计日志运行状态：normal： 运行中； paused： 欠费暂停。
         :type AuditRunningStatus: str
+        :param InternalVip: 内网vip。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InternalVip: str
+        :param InternalVport: 内网port。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InternalVport: int
+        :param CreateTime: 创建时间。
+        :type CreateTime: str
+        :param ClusterId: 所属集群ID（仅对集群数据库产品该字段非空，如TDSQL-C）。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param ClusterName: 所属集群名称（仅对集群数据库产品该字段非空，如TDSQL-C）。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterName: str
         """
         self.InstanceId = None
         self.InstanceName = None
         self.Region = None
         self.HealthScore = None
         self.Product = None
         self.EventCount = None
@@ -2247,14 +2279,19 @@
         self.UniqVpcId = None
         self.InstanceConf = None
         self.DeadlineTime = None
         self.IsSupported = None
         self.SecAuditStatus = None
         self.AuditPolicyStatus = None
         self.AuditRunningStatus = None
+        self.InternalVip = None
+        self.InternalVport = None
+        self.CreateTime = None
+        self.ClusterId = None
+        self.ClusterName = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.Region = params.get("Region")
         self.HealthScore = params.get("HealthScore")
@@ -2280,14 +2317,19 @@
             self.InstanceConf = InstanceConfs()
             self.InstanceConf._deserialize(params.get("InstanceConf"))
         self.DeadlineTime = params.get("DeadlineTime")
         self.IsSupported = params.get("IsSupported")
         self.SecAuditStatus = params.get("SecAuditStatus")
         self.AuditPolicyStatus = params.get("AuditPolicyStatus")
         self.AuditRunningStatus = params.get("AuditRunningStatus")
+        self.InternalVip = params.get("InternalVip")
+        self.InternalVport = params.get("InternalVport")
+        self.CreateTime = params.get("CreateTime")
+        self.ClusterId = params.get("ClusterId")
+        self.ClusterName = params.get("ClusterName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2988,14 +3030,46 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SlowLogUser(AbstractModel):
+    """慢日志来源用户详情。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 来源用户名。
+        :type UserName: str
+        :param Ratio: 该来源用户名的慢日志数目占总数目的比例，单位%。
+        :type Ratio: float
+        :param Count: 该来源用户名的慢日志数目。
+        :type Count: int
+        """
+        self.UserName = None
+        self.Ratio = None
+        self.Count = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.Ratio = params.get("Ratio")
+        self.Count = params.get("Count")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class TableSpaceData(AbstractModel):
     """库表空间统计数据。
 
     """
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.912/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.912/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.911
+Version: 3.0.912
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.911/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.912/setup.py`

 * *Files identical despite different names*

