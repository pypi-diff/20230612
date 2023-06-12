# Comparing `tmp/vedro-jj-0.1.1.tar.gz` & `tmp/vedro-jj-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-jj-0.1.1.tar", last modified: Wed Nov 16 16:24:20 2022, max compression
+gzip compressed data, was "vedro-jj-0.2.0.tar", last modified: Mon Jun 12 17:51:23 2023, max compression
```

## Comparing `vedro-jj-0.1.1.tar` & `vedro-jj-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:24:20.492986 vedro-jj-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-16 16:23:49.000000 vedro-jj-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-11-16 16:24:20.496986 vedro-jj-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-11-16 16:23:49.000000 vedro-jj-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-11-16 16:24:20.496986 vedro-jj-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-11-16 16:23:49.000000 vedro-jj-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:24:20.492986 vedro-jj-0.1.1/vedro_jj/
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-16 16:23:49.000000 vedro-jj-0.1.1/vedro_jj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-11-16 16:23:49.000000 vedro-jj-0.1.1/vedro_jj/_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2022-11-16 16:23:49.000000 vedro-jj-0.1.1/vedro_jj/_remote_mock.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 16:23:49.000000 vedro-jj-0.1.1/vedro_jj/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 16:24:20.492986 vedro-jj-0.1.1/vedro_jj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2098 2022-11-16 16:24:20.000000 vedro-jj-0.1.1/vedro_jj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-16 16:24:20.000000 vedro-jj-0.1.1/vedro_jj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 16:24:20.000000 vedro-jj-0.1.1/vedro_jj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-16 16:24:20.000000 vedro-jj-0.1.1/vedro_jj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-16 16:24:20.000000 vedro-jj-0.1.1/vedro_jj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:23.529235 vedro-jj-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-12 17:51:23.529235 vedro-jj-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-12 17:51:23.529235 vedro-jj-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:23.529235 vedro-jj-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/tests/test_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:23.529235 vedro-jj-0.2.0/vedro_jj/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/vedro_jj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/vedro_jj/_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/vedro_jj/_vedro_jj.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:07.000000 vedro-jj-0.2.0/vedro_jj/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:51:23.529235 vedro-jj-0.2.0/vedro_jj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-12 17:51:23.000000 vedro-jj-0.2.0/vedro_jj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-12 17:51:23.000000 vedro-jj-0.2.0/vedro_jj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:51:23.000000 vedro-jj-0.2.0/vedro_jj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 17:51:23.000000 vedro-jj-0.2.0/vedro_jj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 17:51:23.000000 vedro-jj-0.2.0/vedro_jj.egg-info/top_level.txt
```

### Comparing `vedro-jj-0.1.1/LICENSE` & `vedro-jj-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-jj-0.1.1/PKG-INFO` & `vedro-jj-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,97 @@
 Metadata-Version: 2.1
 Name: vedro-jj
-Version: 0.1.1
-Home-page: https://github.com/nikitanovosibirsk/vedro-jj
+Version: 0.2.0
+Home-page: https://github.com/vedro-universe/vedro-jj
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: GitHub, https://github.com/vedro-universe/vedro-jj
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vedro-jj
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-jj/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-jj)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-jj/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-jj)
 [![PyPI](https://img.shields.io/pypi/v/vedro-jj.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-jj?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-jj.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 
+[Vedro](https://vedro.io/) + [jj](https://pypi.org/project/jj/)
+
 ## Installation
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager as follows:
+
+```shell
+$ vedro plugin install vedro-jj
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-jj
 ```
 
-### 2. Enable plugin
+2. Next, activate the plugin in your `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
 import vedro_jj
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class RemoteMock(vedro_jj.RemoteMock):
+        class VedroJJ(vedro_jj.VedroJJ):
             enabled = True
 ```
 
+</p>
+</details>
+
 ## Usage
 
 ```python
-# ./scenarios/get_users.py
+import httpx
 import jj
 import vedro
-from httpx import AsyncClient
 from jj.mock import mocked
 
 class Scenario(vedro.Scenario):
     subject = "get users"
 
     def given(self):
         self.mock_matcher = jj.match("GET", "/users")
         self.mock_response = jj.Response(json=[])
 
-    async def when(self):
-        async with mocked(self.mock_matcher, self.mock_response):
-            async with AsyncClient() as client:
-                self.response = await client.get("http://localhost:8080/users")
+    def when(self):
+        with mocked(self.mock_matcher, self.mock_response):
+            self.response = httpx.get("http://localhost:8080/users")
 
     def then(self):
         assert self.response.status_code == 200
         assert self.response.json() == []
 ```
 
 ```shell
```

### Comparing `vedro-jj-0.1.1/README.md` & `vedro-jj-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,79 @@
 # vedro-jj
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-jj/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-jj)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-jj/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-jj)
 [![PyPI](https://img.shields.io/pypi/v/vedro-jj.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-jj?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-jj.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 
+[Vedro](https://vedro.io/) + [jj](https://pypi.org/project/jj/)
+
 ## Installation
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager as follows:
+
+```shell
+$ vedro plugin install vedro-jj
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-jj
 ```
 
-### 2. Enable plugin
+2. Next, activate the plugin in your `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
 import vedro_jj
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class RemoteMock(vedro_jj.RemoteMock):
+        class VedroJJ(vedro_jj.VedroJJ):
             enabled = True
 ```
 
+</p>
+</details>
+
 ## Usage
 
 ```python
-# ./scenarios/get_users.py
+import httpx
 import jj
 import vedro
-from httpx import AsyncClient
 from jj.mock import mocked
 
 class Scenario(vedro.Scenario):
     subject = "get users"
 
     def given(self):
         self.mock_matcher = jj.match("GET", "/users")
         self.mock_response = jj.Response(json=[])
 
-    async def when(self):
-        async with mocked(self.mock_matcher, self.mock_response):
-            async with AsyncClient() as client:
-                self.response = await client.get("http://localhost:8080/users")
+    def when(self):
+        with mocked(self.mock_matcher, self.mock_response):
+            self.response = httpx.get("http://localhost:8080/users")
 
     def then(self):
         assert self.response.status_code == 200
         assert self.response.json() == []
 ```
 
 ```shell
```

### Comparing `vedro-jj-0.1.1/setup.cfg` & `vedro-jj-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.2.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-jj-0.1.1/setup.py` & `vedro-jj-0.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-import pipfile
 from setuptools import find_packages, setup
 
 
 def find_required():
-    pf = pipfile.load()
-    return [f"{key}{val}" for key, val in pf.data["default"].items()]
+    with open("requirements.txt") as f:
+        return f.read().splitlines()
 
 
 def find_dev_required():
-    pf = pipfile.load()
-    return [key for key, _ in pf.data["develop"].items()]
+    with open("requirements-dev.txt") as f:
+        return f.read().splitlines()
 
 
 setup(
     name="vedro-jj",
-    version="0.1.1",
+    version="0.2.0",
     description="",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
-    url="https://github.com/nikitanovosibirsk/vedro-jj",
+    url="https://github.com/vedro-universe/vedro-jj",
+    project_urls={
+        "GitHub": "https://github.com/vedro-universe/vedro-jj",
+    },
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_jj": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
```

### Comparing `vedro-jj-0.1.1/vedro_jj/_interceptor.py` & `vedro-jj-0.2.0/vedro_jj/_interceptor.py`

 * *Files identical despite different names*

### Comparing `vedro-jj-0.1.1/vedro_jj/_remote_mock.py` & `vedro-jj-0.2.0/vedro_jj/_vedro_jj.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from jj.runners import AppRunner
 from jj.servers import Server
 from vedro.core import Dispatcher, Plugin, PluginConfig
 from vedro.events import CleanupEvent, StartupEvent
 
 from ._interceptor import Interceptor, InterceptorType
 
-__all__ = ("RemoteMock", "RemoteMockPlugin", "interceptor",)
+__all__ = ("VedroJJ", "VedroJJPlugin", "interceptor",)
 
 
 _interceptors: List[InterceptorType] = []
 
 
 def interceptor(fn: InterceptorType) -> InterceptorType:
     _interceptors.append(fn)
@@ -28,16 +28,16 @@
 
 
 @Interceptor(_interceptors)
 class _Mock(Mock):
     pass
 
 
-class RemoteMockPlugin(Plugin):
-    def __init__(self, config: Type["RemoteMock"]) -> None:
+class VedroJJPlugin(Plugin):
+    def __init__(self, config: Type["VedroJJ"]) -> None:
         super().__init__(config)
         self._host = config.host
         self._port = config.port
         self._threaded = config.threaded
         self._server: Union[Server, None] = None
         self._task: Union["Task[Any]", None] = None
         self._thread: Union[Thread, None] = None
@@ -82,16 +82,16 @@
             self._thread = None
 
         if self._task:
             await self._task
             self._task = None
 
 
-class RemoteMock(PluginConfig):
-    plugin = RemoteMockPlugin
+class VedroJJ(PluginConfig):
+    plugin = VedroJJPlugin
 
     host: str = "0.0.0.0"
     port: int = 8080
 
     # Start mock in a separate thread
     # Mandatory if blocking calls are used
     threaded: bool = True
```

### Comparing `vedro-jj-0.1.1/vedro_jj.egg-info/PKG-INFO` & `vedro-jj-0.2.0/vedro_jj.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,97 @@
 Metadata-Version: 2.1
 Name: vedro-jj
-Version: 0.1.1
-Home-page: https://github.com/nikitanovosibirsk/vedro-jj
+Version: 0.2.0
+Home-page: https://github.com/vedro-universe/vedro-jj
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
+Project-URL: GitHub, https://github.com/vedro-universe/vedro-jj
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # vedro-jj
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-jj/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-jj)
+[![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-jj/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-jj)
 [![PyPI](https://img.shields.io/pypi/v/vedro-jj.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-jj?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-jj.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-jj/)
 
+[Vedro](https://vedro.io/) + [jj](https://pypi.org/project/jj/)
+
 ## Installation
 
-### 1. Install package
+<details open>
+<summary>Quick</summary>
+<p>
+
+For a quick installation, you can use a plugin manager as follows:
+
+```shell
+$ vedro plugin install vedro-jj
+```
+
+</p>
+</details>
+
+<details>
+<summary>Manual</summary>
+<p>
+
+To install manually, follow these steps:
+
+1. Install the package using pip:
 
 ```shell
 $ pip3 install vedro-jj
 ```
 
-### 2. Enable plugin
+2. Next, activate the plugin in your `vedro.cfg.py` configuration file:
 
 ```python
 # ./vedro.cfg.py
 import vedro
 import vedro_jj
 
 class Config(vedro.Config):
 
     class Plugins(vedro.Config.Plugins):
 
-        class RemoteMock(vedro_jj.RemoteMock):
+        class VedroJJ(vedro_jj.VedroJJ):
             enabled = True
 ```
 
+</p>
+</details>
+
 ## Usage
 
 ```python
-# ./scenarios/get_users.py
+import httpx
 import jj
 import vedro
-from httpx import AsyncClient
 from jj.mock import mocked
 
 class Scenario(vedro.Scenario):
     subject = "get users"
 
     def given(self):
         self.mock_matcher = jj.match("GET", "/users")
         self.mock_response = jj.Response(json=[])
 
-    async def when(self):
-        async with mocked(self.mock_matcher, self.mock_response):
-            async with AsyncClient() as client:
-                self.response = await client.get("http://localhost:8080/users")
+    def when(self):
+        with mocked(self.mock_matcher, self.mock_response):
+            self.response = httpx.get("http://localhost:8080/users")
 
     def then(self):
         assert self.response.status_code == 200
         assert self.response.json() == []
 ```
 
 ```shell
```

