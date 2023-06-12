# Comparing `tmp/amis_python-1.0.8.post1.tar.gz` & `tmp/amis_python-1.0.8.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amis_python-1.0.8.post1.tar", max compression
+gzip compressed data, was "amis_python-1.0.8.post2.tar", max compression
```

## Comparing `amis_python-1.0.8.post1.tar` & `amis_python-1.0.8.post2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11356 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/LICENSE
--rw-r--r--   0        0        0     1434 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/README.md
--rw-r--r--   0        0        0      227 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/__init__.py
--rw-r--r--   0        0        0   179505 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/components.py
--rw-r--r--   0        0        0     1287 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/constants.py
--rw-r--r--   0        0        0     6859 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/templates/app.jinja2
--rw-r--r--   0        0        0     1621 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/templates/page.jinja2
--rw-r--r--   0        0        0     5918 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/amis/types.py
--rw-r--r--   0        0        0      766 2023-06-11 14:29:49.097075 amis_python-1.0.8.post1/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 amis_python-1.0.8.post1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/LICENSE
+-rw-r--r--   0        0        0     1434 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/README.md
+-rw-r--r--   0        0        0      227 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/amis/__init__.py
+-rw-r--r--   0        0        0   179505 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/amis/components.py
+-rw-r--r--   0        0        0     1287 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/amis/constants.py
+-rw-r--r--   0        0        0     6859 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/amis/templates/app.jinja2
+-rw-r--r--   0        0        0     1621 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/amis/templates/page.jinja2
+-rw-r--r--   0        0        0     5918 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/amis/types.py
+-rw-r--r--   0        0        0      766 2023-06-12 14:44:14.688905 amis_python-1.0.8.post2/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 amis_python-1.0.8.post2/PKG-INFO
```

### Comparing `amis_python-1.0.8.post1/LICENSE` & `amis_python-1.0.8.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8.post1/README.md` & `amis_python-1.0.8.post2/README.md`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8.post1/amis/components.py` & `amis_python-1.0.8.post2/amis/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     """Header 区域 dom 类名"""
     initApi: API = None
     """Page 用来获取初始数据的 api。返回的数据可以整个 page 级别使用。"""
     initFetch: bool = True
     """是否起始拉取 initApi"""
     initFetchOn: Expression = None
     """是否起始拉取 initApi, 通过表达式配置"""
-    interval: int = 3000
+    interval: int = None
     """刷新时间(最小 1000)"""
     silentPolling: bool = False
     """配置刷新时是否显示加载动画"""
     stopAutoRefreshWhen: Expression = ""
     """通过表达式来配置停止刷新的条件"""
     pullRefresh: dict = {"disabled": True}
     """下拉刷新配置（仅用于移动端）"""
@@ -3680,15 +3680,15 @@
     """设置过滤器，当该表单提交后，会把数据带给当前 mode 刷新列表。"""
     filterTogglable: bool = False
     """是否可显隐过滤器"""
     filterDefaultVisible: bool = True
     """设置过滤器默认是否可见。"""
     initFetch: bool = True
     """是否初始化的时候拉取数据, 只针对有 filter 的情况, 没有 filter 初始都会拉取数据"""
-    interval: int = 3000
+    interval: int = None
     """刷新时间(最低 1000)"""
     silentPolling: bool = False
     """配置刷新时是否隐藏加载动画"""
     stopAutoRefreshWhen: str = ""
     """通过表达式来配置停止刷新的条件"""
     stopAutoRefreshWhenModalIsOpen: bool = False
     """当有弹框时关闭自动刷新，关闭弹框又恢复"""
@@ -4945,15 +4945,15 @@
     """任务列表"""
     checkApi: API = None
     """返回任务列表，返回的数据请参考 items。"""
     submitApi: API = None
     """提交任务使用的 API"""
     reSubmitApi: API = None
     """如果任务失败，且可以重试，提交的时候会使用此 API"""
-    interval: int = 3000
+    interval: int = None
     """当有任务进行中，会每隔一段时间再次检测，而时间间隔就是通过此项配置，默认 3s。"""
     taskNameLabel: str = "任务名称"
     """任务名称列说明"""
     operationLabel: str = "操作"
     """操作列说明"""
     statusLabel: str = "状态"
     """状态列说明"""
```

### Comparing `amis_python-1.0.8.post1/amis/constants.py` & `amis_python-1.0.8.post2/amis/constants.py`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8.post1/amis/templates/app.jinja2` & `amis_python-1.0.8.post2/amis/templates/app.jinja2`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8.post1/amis/templates/page.jinja2` & `amis_python-1.0.8.post2/amis/templates/page.jinja2`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8.post1/amis/types.py` & `amis_python-1.0.8.post2/amis/types.py`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.8.post1/pyproject.toml` & `amis_python-1.0.8.post2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amis-python"
-version = "1.0.8post1"
+version = "1.0.8post2"
 description = "基于百度amis前端框架的python pydantic模型封装。"
 authors = ["惜月 <277073121@qq.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["amis"]
 homepage = "https://github.com/CMHopeSunshine/amis-py"
 repository = "https://github.com/CMHopeSunshine/amis-py"
```

### Comparing `amis_python-1.0.8.post1/PKG-INFO` & `amis_python-1.0.8.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amis-python
-Version: 1.0.8.post1
+Version: 1.0.8.post2
 Summary: 基于百度amis前端框架的python pydantic模型封装。
 Home-page: https://github.com/CMHopeSunshine/amis-py
 License: Apache-2.0
 Keywords: amis
 Author: 惜月
 Author-email: 277073121@qq.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amis-python Version: 1.0.8.post1 Summary:
+Metadata-Version: 2.1 Name: amis-python Version: 1.0.8.post2 Summary:
 åºäºç¾åº¦amisåç«¯æ¡æ¶çpython pydanticæ¨¡åå°è£ã Home-page: https:
 //github.com/CMHopeSunshine/amis-py License: Apache-2.0 Keywords: amis Author:
 ææ Author-email: 277073121@qq.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

