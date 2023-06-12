# Comparing `tmp/pytest-runtime-yoyo-1.0.0.tar.gz` & `tmp/pytest-runtime-yoyo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-runtime-yoyo-1.0.0.tar", last modified: Mon Jun 12 03:38:26 2023, max compression
+gzip compressed data, was "dist\pytest-runtime-yoyo-1.0.1.tar", last modified: Mon Jun 12 07:19:02 2023, max compression
```

## Comparing `pytest-runtime-yoyo-1.0.0.tar` & `pytest-runtime-yoyo-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 03:38:26.527118 pytest-runtime-yoyo-1.0.0/
--rw-rw-rw-   0        0        0     4379 2023-06-12 03:38:26.526125 pytest-runtime-yoyo-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3874 2023-06-12 03:38:09.000000 pytest-runtime-yoyo-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-12 03:38:26.527118 pytest-runtime-yoyo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-06-12 03:29:14.000000 pytest-runtime-yoyo-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:38:26.512156 pytest-runtime-yoyo-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 03:38:26.516148 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo/
--rw-rw-rw-   0        0        0        0 2023-06-12 02:17:20.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo/__init__.py
--rw-rw-rw-   0        0        0     1622 2023-06-12 03:33:44.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo/plugin.py
-drwxrwxrwx   0        0        0        0 2023-06-12 03:38:26.525124 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/
--rw-rw-rw-   0        0        0     4379 2023-06-12 03:38:26.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-06-12 03:38:26.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 03:38:26.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-12 03:38:26.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-06-12 03:38:26.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-12 03:38:26.000000 pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 07:19:02.637505 pytest-runtime-yoyo-1.0.1/
+-rw-rw-rw-   0        0        0     4379 2023-06-12 07:19:02.636511 pytest-runtime-yoyo-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3874 2023-06-12 03:38:09.000000 pytest-runtime-yoyo-1.0.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:19:02.637505 pytest-runtime-yoyo-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-06-12 07:18:55.000000 pytest-runtime-yoyo-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:19:02.620558 pytest-runtime-yoyo-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 07:19:02.626536 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo/
+-rw-rw-rw-   0        0        0        0 2023-06-12 02:17:20.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     1629 2023-06-12 07:18:45.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo/plugin.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:19:02.635510 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/
+-rw-rw-rw-   0        0        0     4379 2023-06-12 07:19:02.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-06-12 07:19:02.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:19:02.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-12 07:19:02.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-12 07:19:02.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-12 07:19:02.000000 pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-runtime-yoyo-1.0.0/PKG-INFO` & `pytest-runtime-yoyo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-runtime-yoyo
-Version: 1.0.0
+Version: 1.0.1
 Summary: run case mark timeout
 Home-page: https://gitee.com/yoyoketang/pytest-runtime-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-runtime,pytest-runtime-yoyo
 Classifier: Framework :: Pytest
```

### Comparing `pytest-runtime-yoyo-1.0.0/README.rst` & `pytest-runtime-yoyo-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-runtime-yoyo-1.0.0/setup.py` & `pytest-runtime-yoyo-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-runtime-yoyo',
     url='https://gitee.com/yoyoketang/pytest-runtime-yoyo',
-    version='v1.0.0',
+    version='v1.0.1',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='run case mark timeout',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_runtime_yoyo"],
     classifiers=[
```

### Comparing `pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo/plugin.py` & `pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         if isinstance(item.parent, Module):
             # 父类是 Module
             own_markers = item.__dict__['own_markers'] or item.parent.__dict__['own_markers']
         else:
             # 父类是 Class
             own_markers = item.__dict__['own_markers'] or item.parent.__dict__['own_markers'] or item.parent.parent.__dict__['own_markers']
         run_time_mark = [mark.__dict__['args'][0] for mark in own_markers if mark.__dict__.get('name') == 'runtime']
-        run_time_args = run_time_mark[0] if run_time_mark else config_run_time
+        run_time_args = float(run_time_mark[0]) if run_time_mark else config_run_time
         if run_time_args and report.duration > run_time_args:
             report.outcome = "failed"
 
 
 def pytest_addoption(parser):   # noqa
     parser.addini('runtime', default=None, help='run case timeout...')
     parser.addoption(
```

### Comparing `pytest-runtime-yoyo-1.0.0/src/pytest_runtime_yoyo.egg-info/PKG-INFO` & `pytest-runtime-yoyo-1.0.1/src/pytest_runtime_yoyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-runtime-yoyo
-Version: 1.0.0
+Version: 1.0.1
 Summary: run case mark timeout
 Home-page: https://gitee.com/yoyoketang/pytest-runtime-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-runtime,pytest-runtime-yoyo
 Classifier: Framework :: Pytest
```

