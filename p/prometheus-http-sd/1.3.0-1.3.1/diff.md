# Comparing `tmp/prometheus_http_sd-1.3.0.tar.gz` & `tmp/prometheus_http_sd-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_http_sd-1.3.0.tar", max compression
+gzip compressed data, was "prometheus_http_sd-1.3.1.tar", max compression
```

## Comparing `prometheus_http_sd-1.3.0.tar` & `prometheus_http_sd-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-31 03:52:46.087086 prometheus_http_sd-1.3.0/LICENSE
--rw-r--r--   0        0        0    11097 2023-05-31 03:52:46.087086 prometheus_http_sd-1.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/__init__.py
--rw-r--r--   0        0        0     3774 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/app.py
--rw-r--r--   0        0        0     2398 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/cli.py
--rw-r--r--   0        0        0      110 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/config.py
--rw-r--r--   0        0        0       45 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/const.py
--rw-r--r--   0        0        0     7349 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/decorator.py
--rw-r--r--   0        0        0        0 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/exceptions.py
--rw-r--r--   0        0        0     1165 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/mem_perf.py
--rw-r--r--   0        0        0     5019 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/sd.py
--rw-r--r--   0        0        0      147 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/targets.py
--rw-r--r--   0        0        0     1148 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/templates/admin.html
--rw-r--r--   0        0        0     2118 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/validate.py
--rw-r--r--   0        0        0       18 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/prometheus_http_sd/version.py
--rw-r--r--   0        0        0      648 2023-05-31 03:52:46.095086 prometheus_http_sd-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 prometheus_http_sd-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 10:34:04.994293 prometheus_http_sd-1.3.1/LICENSE
+-rw-r--r--   0        0        0    11329 2023-06-12 10:34:04.994293 prometheus_http_sd-1.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/__init__.py
+-rw-r--r--   0        0        0     3774 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/app.py
+-rw-r--r--   0        0        0     2868 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/cli.py
+-rw-r--r--   0        0        0      110 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/config.py
+-rw-r--r--   0        0        0       45 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/const.py
+-rw-r--r--   0        0        0     8286 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/decorator.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/exceptions.py
+-rw-r--r--   0        0        0     1165 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/mem_perf.py
+-rw-r--r--   0        0        0     5019 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/sd.py
+-rw-r--r--   0        0        0      147 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/targets.py
+-rw-r--r--   0        0        0     1148 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/templates/admin.html
+-rw-r--r--   0        0        0     2118 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/validate.py
+-rw-r--r--   0        0        0       18 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/prometheus_http_sd/version.py
+-rw-r--r--   0        0        0      648 2023-06-12 10:34:05.002293 prometheus_http_sd-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12098 1970-01-01 00:00:00.000000 prometheus_http_sd-1.3.1/PKG-INFO
```

### Comparing `prometheus_http_sd-1.3.0/LICENSE` & `prometheus_http_sd-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.0/README.md` & `prometheus_http_sd-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 - [Installation](#installation)
 - [Usage](#usage)
   - [The Python Target Generator](#the-python-target-generator)
   - [Python Target Generator Cache and Throttle](#python-target-generator-cache-and-throttle)
   - [Manage prometheus-http-sd by systemd](#manage-prometheus-http-sd-by-systemd)
   - [Admin Page](#admin-page)
   - [Serve under a different root path](#serve-under-a-different-root-path)
+  - [Sentry APM](#sentry-apm)
 - [Define your targets](#define-your-targets)
   - [Your target generator](#your-target-generator)
   - [The Target Path](#the-target-path)
   - [Overwriting `job_name` labels](#overwriting-job_name-labels)
   - [Check and Validate your Targets](#check-and-validate-your-targets)
   - [Script Dependencies](#script-dependencies)
 - [Update Your Scripts](#update-your-scripts)
@@ -36,14 +37,15 @@
   counting the targets;
 - You can monitoring your target generator via `/metrics`, see
   [metrics](./docs/metrics.txt);
 - Admin page to list all target paths;
 - Auto reload when generator or targets changed;
 - Support managing targets in a hierarchy way;
 - Throttle parallel execution and cache the result for Python script;
+- Support Sentry APM.
 
 ## Installation
 
 ```shell
 pip install prometheus-http-sd
 ```
 
@@ -202,14 +204,21 @@
 }
 ```
 
 Then you need to tell prometheus_http_sd to serve all HTTP requests under this
 path, by using the `--url_prefix /http_sd` cli option, (or `-r /http_sd` for
 short).
 
+### Sentry APM
+
+You can use the option `--sentry-url <you-sentry-url>` (or `-s <your-sentry-url>`)
+to enable Sentry APM.
+
+The Exception from user's script will be sent to Sentry.
+
 ## Define your targets
 
 ### Your target generator
 
 Please see the [Usage](#usage) to know how to define your generator.
 
 ### The Target Path
```

### Comparing `prometheus_http_sd-1.3.0/prometheus_http_sd/app.py` & `prometheus_http_sd-1.3.1/prometheus_http_sd/app.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.0/prometheus_http_sd/decorator.py` & `prometheus_http_sd-1.3.1/prometheus_http_sd/decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import time
 import heapq
 import traceback
 import threading
 
 from prometheus_client import Gauge, Counter, Histogram
 
@@ -26,15 +27,15 @@
 _collection_run_interval = Histogram(
     "http_sd_garbage_collection_run_interval_seconds_bucket",
     "The interval of two garbage collection run.",
     ["name"],
 )
 
 
-class WrapTargetException(Exception):
+class CachedScriptException(Exception):
     """Raised when user's function raises an exception."""
 
     def __init__(self, message, exception_type="Exception", traceback=[]):
         traceback = "".join(traceback)
         super().__init__(
             self,
             f"""this is a cached exception,
@@ -49,17 +50,19 @@
 
 
 class TimeoutDecorator:
     def __init__(
         self,
         timeout=None,
         cache_time=0,
+        cache_exception_time=0,
         name="",
         garbage_collection_interval=5,
         garbage_collection_count=30,
+        copy_response=False,
     ):
         """
         Use threading and cache to store the function result.
 
         Garbage Collection time complexity:
             worse: O(nlogn)
             average in every operation: O(logn)
@@ -67,31 +70,38 @@
         Parameters
         ----------
         timeout: int
             function timeout. if exceed, raise TimeoutException (in sec).
         cache_time: int
             after function return normally,
                 how long should we cache the result (in sec).
+        cache_exception_time: int
+            after function return incorrectly,
+                how long should we cache the exception (in sec).
         name: str
             prometheus_client metrics prefix
         garbage_collection_count: int
             garbage collection threshold
         garbage_collection_interval: int
             the second to avoid collection too often.
+        copy_response: bool
+            use copy.deepcopy on the response from the target function.
 
         Returns
         -------
         TimeoutDecorator
             decorator class.
         """
         self.timeout = timeout
         self.cache_time = cache_time
+        self.cache_exception_time = cache_exception_time
         self.name = name
         self.garbage_collection_interval = garbage_collection_interval
         self.garbage_collection_count = garbage_collection_count
+        self.copy_response = copy_response
 
         self.thread_cache = {}
         self.cache_lock = threading.Lock()
         self.heap = []
         self.heap_lock = threading.Lock()
         self.garbage_collection_timestamp = 0
         self.garbage_collection_lock = threading.Lock()
@@ -120,14 +130,18 @@
             if _key in worked_keys:
                 continue
             worked_keys[_key] = True
             with self.cache_lock:
                 if _key not in self.thread_cache:
                     continue
                 if self.is_expired(self.thread_cache[_key]):
+                    if "traceback" in self.thread_cache[_key]:
+                        traceback.clear_frames(
+                            self.thread_cache[_key]["traceback"],
+                        )
                     del self.thread_cache[_key]
                     _collected_total.labels(name=self.name).inc(1)
         _heap_cache_count.labels(
             name=self.name,
         ).set(len(self.heap))
         _thread_cache_count.labels(
             name=self.name,
@@ -148,29 +162,35 @@
 
     def __call__(self, function):
         def wrapper(*arg, **kwargs):
             cache = {
                 "thread": None,
                 "error": None,
                 "response": None,
-                "traceback": [],
                 "expired_timestamp": float("inf"),
             }
 
             def target_function(key):
                 try:
-                    cache["response"] = function(*arg, **kwargs)
+                    if self.copy_response:
+                        cache["response"] = copy.deepcopy(
+                            function(*arg, **kwargs),
+                        )
+                    else:
+                        cache["response"] = function(*arg, **kwargs)
                     cache["expired_timestamp"] = time.time() + self.cache_time
                 except Exception as e:
                     cache["error"] = {
                         "message": str(e),
                         "error_type": type(e).__name__,
-                        "traceback": traceback.format_tb(e.__traceback__),
+                        "traceback": e.__traceback__,
                     }
-                    cache["expired_timestamp"] = 0
+                    cache["expired_timestamp"] = (
+                        time.time() + self.cache_exception_time
+                    )
                 with self.heap_lock:
                     heapq.heappush(
                         self.heap,
                         (
                             cache["expired_timestamp"],
                             key,
                         ),
@@ -209,15 +229,15 @@
                 finally:
                     self.garbage_collection_lock.release()
             if cache["thread"].is_alive():
                 raise TimeoutException("target function timeout!")
             if cache["error"]:
                 e = cache["error"]
                 # avoid duplicated append the traceback
-                raise WrapTargetException(
+                raise CachedScriptException(
                     e["message"],
                     e["error_type"],
-                    e["traceback"],
-                )
-            return cache["response"]
+                    traceback.format_tb(e["traceback"]),
+                ).with_traceback(e["traceback"])
+            return copy.deepcopy(cache["response"])
 
         return wrapper
```

### Comparing `prometheus_http_sd-1.3.0/prometheus_http_sd/mem_perf.py` & `prometheus_http_sd-1.3.1/prometheus_http_sd/mem_perf.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.0/prometheus_http_sd/sd.py` & `prometheus_http_sd-1.3.1/prometheus_http_sd/sd.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.0/prometheus_http_sd/templates/admin.html` & `prometheus_http_sd-1.3.1/prometheus_http_sd/templates/admin.html`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.0/prometheus_http_sd/validate.py` & `prometheus_http_sd-1.3.1/prometheus_http_sd/validate.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.3.0/pyproject.toml` & `prometheus_http_sd-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-http-sd"
-version = "1.3.0"
+version = "1.3.1"
 description = "Prometheus HTTP SD framework."
 authors = ["laixintao <laixintaoo@gmail.com>"]
 readme = 'README.md'
 homepage = "https://python-poetry.org://github.com/laixintao/prometheus-http-sd"
 
 
 [tool.poetry.dependencies]
@@ -15,15 +15,15 @@
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.3.0"]
+requires = ["poetry-core>=1.3.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.scripts]
 prometheus-http-sd = 'prometheus_http_sd.cli:main'
```

### Comparing `prometheus_http_sd-1.3.0/PKG-INFO` & `prometheus_http_sd-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-http-sd
-Version: 1.3.0
+Version: 1.3.1
 Summary: Prometheus HTTP SD framework.
 Home-page: https://python-poetry.org://github.com/laixintao/prometheus-http-sd
 Author: laixintao
 Author-email: laixintaoo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -32,14 +32,15 @@
 - [Installation](#installation)
 - [Usage](#usage)
   - [The Python Target Generator](#the-python-target-generator)
   - [Python Target Generator Cache and Throttle](#python-target-generator-cache-and-throttle)
   - [Manage prometheus-http-sd by systemd](#manage-prometheus-http-sd-by-systemd)
   - [Admin Page](#admin-page)
   - [Serve under a different root path](#serve-under-a-different-root-path)
+  - [Sentry APM](#sentry-apm)
 - [Define your targets](#define-your-targets)
   - [Your target generator](#your-target-generator)
   - [The Target Path](#the-target-path)
   - [Overwriting `job_name` labels](#overwriting-job_name-labels)
   - [Check and Validate your Targets](#check-and-validate-your-targets)
   - [Script Dependencies](#script-dependencies)
 - [Update Your Scripts](#update-your-scripts)
@@ -56,14 +57,15 @@
   counting the targets;
 - You can monitoring your target generator via `/metrics`, see
   [metrics](./docs/metrics.txt);
 - Admin page to list all target paths;
 - Auto reload when generator or targets changed;
 - Support managing targets in a hierarchy way;
 - Throttle parallel execution and cache the result for Python script;
+- Support Sentry APM.
 
 ## Installation
 
 ```shell
 pip install prometheus-http-sd
 ```
 
@@ -222,14 +224,21 @@
 }
 ```
 
 Then you need to tell prometheus_http_sd to serve all HTTP requests under this
 path, by using the `--url_prefix /http_sd` cli option, (or `-r /http_sd` for
 short).
 
+### Sentry APM
+
+You can use the option `--sentry-url <you-sentry-url>` (or `-s <your-sentry-url>`)
+to enable Sentry APM.
+
+The Exception from user's script will be sent to Sentry.
+
 ## Define your targets
 
 ### Your target generator
 
 Please see the [Usage](#usage) to know how to define your generator.
 
 ### The Target Path
```

