# Comparing `tmp/w3multicall-0.0.1.tar.gz` & `tmp/w3multicall-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3multicall-0.0.1.tar", last modified: Mon Jun 12 15:03:48 2023, max compression
+gzip compressed data, was "w3multicall-0.1.0.tar", last modified: Mon Jun 12 15:11:45 2023, max compression
```

## Comparing `w3multicall-0.0.1.tar` & `w3multicall-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:03:48.254165 w3multicall-0.0.1/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.0.1/LICENSE
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5237 2023-06-12 15:03:48.254165 w3multicall-0.0.1/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3529 2023-06-12 14:55:00.000000 w3multicall-0.0.1/README.md
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-12 15:02:51.000000 w3multicall-0.0.1/pyproject.toml
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-12 15:03:48.254165 w3multicall-0.0.1/setup.cfg
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:03:48.254165 w3multicall-0.0.1/src/
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:03:48.254165 w3multicall-0.0.1/src/w3multicall.egg-info/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5237 2023-06-12 15:03:48.000000 w3multicall-0.0.1/src/w3multicall.egg-info/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      389 2023-06-12 15:03:48.000000 w3multicall-0.0.1/src/w3multicall.egg-info/SOURCES.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-12 15:03:48.000000 w3multicall-0.0.1/src/w3multicall.egg-info/dependency_links.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-12 15:03:48.000000 w3multicall-0.0.1/src/w3multicall.egg-info/requires.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       14 2023-06-12 15:03:48.000000 w3multicall-0.0.1/src/w3multicall.egg-info/top_level.txt
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:03:48.254165 w3multicall-0.0.1/src/web3multicall/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.0.1/src/web3multicall/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5624 2023-06-12 13:12:08.000000 w3multicall-0.0.1/src/web3multicall/multicall.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:03:48.254165 w3multicall-0.0.1/src/web3multicall/threading/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.0.1/src/web3multicall/threading/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     6221 2023-06-12 14:51:33.000000 w3multicall-0.0.1/src/web3multicall/threading/w3multicall_executor.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.1.0/LICENSE
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5221 2023-06-12 15:11:45.979601 w3multicall-0.1.0/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3513 2023-06-12 15:08:40.000000 w3multicall-0.1.0/README.md
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-12 15:11:39.000000 w3multicall-0.1.0/pyproject.toml
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-12 15:11:45.979601 w3multicall-0.1.0/setup.cfg
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/w3multicall/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.1.0/src/w3multicall/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5624 2023-06-12 13:12:08.000000 w3multicall-0.1.0/src/w3multicall/multicall.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/w3multicall/threading/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.1.0/src/w3multicall/threading/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     6207 2023-06-12 15:07:37.000000 w3multicall-0.1.0/src/w3multicall/threading/w3multicall_executor.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/w3multicall.egg-info/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5221 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      381 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/SOURCES.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/dependency_links.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/requires.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/top_level.txt
```

### Comparing `w3multicall-0.0.1/LICENSE` & `w3multicall-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `w3multicall-0.0.1/PKG-INFO` & `w3multicall-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -32,23 +32,23 @@
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![Pypi_repo](https://img.shields.io/pypi/v/web3multicall?style=flat-square)](https://pypi.org/project/web3multicall/)
-[![GitHub license](https://img.shields.io/github/license/0rtis/web3multicall.svg?style=flat-square)](https://github.com/0rtis/web3multicall/blob/master/LICENSE)
+[![Pypi_repo](https://img.shields.io/pypi/v/w3multicall?style=flat-square)](https://pypi.org/project/w3multicall/)
+[![GitHub license](https://img.shields.io/github/license/0rtis/w3multicall.svg?style=flat-square)](https://github.com/0rtis/w3multicall/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
 [![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
 
 
-Install with `pip install web3multicall`
+Install with `pip install w3multicall`
 
-https://pypi.org/project/web3multicall/
+https://pypi.org/project/w3multicall/
 
 
 **Want to support this project ? You can help us by:**
 - Delegating AVAX to our Avalanche node **NodeID-4btZGj8TmrycK22kwgBK5wJEFighAFWiZ**
 - Making a donation to **0xA68fBfa3E0c86D1f3fF071853df6DAe8753095E2**
 
 
@@ -62,15 +62,15 @@
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into one.
 
 # Simple Multicall
 
 ```
 from web3 import Web3
-from web3multicall.multicall import W3Multicall
+from w3multicall.multicall import W3Multicall
 
 w3 = Web3(Web3.HTTPProvider(rpc))
 
 w3_multicall = W3Multicall(w3)
 
 w3_multicall.add(W3Multicall.Call(
     '0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48',  # USDC contract address
@@ -91,15 +91,15 @@
 ```
 w3_pool = W3Pool([
         W3(Web3(Web3.HTTPProvider('https://eth-rpc.gateway.pokt.network')), 5),
         W3(Web3(Web3.HTTPProvider('https://ethereum.publicnode.com')), 5),
         W3(Web3(Web3.HTTPProvider('https://rpc.flashbots.net/')), 5)
     ], logger)
 
-executor = Web3MulticallExecutor(w3_pool, processes=len(w3_pool.w3s))
+executor = W3MulticallExecutor(w3_pool, processes=len(w3_pool.w3s))
 
 bayc_futures = []
 azuki_futures = []
 moonbird_futures = []
 for i in range(1, 10):
 
     bayc_futures.append(executor.submit(W3Multicall.Call(
```

### Comparing `w3multicall-0.0.1/README.md` & `w3multicall-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
-[![Pypi_repo](https://img.shields.io/pypi/v/web3multicall?style=flat-square)](https://pypi.org/project/web3multicall/)
-[![GitHub license](https://img.shields.io/github/license/0rtis/web3multicall.svg?style=flat-square)](https://github.com/0rtis/web3multicall/blob/master/LICENSE)
+[![Pypi_repo](https://img.shields.io/pypi/v/w3multicall?style=flat-square)](https://pypi.org/project/w3multicall/)
+[![GitHub license](https://img.shields.io/github/license/0rtis/w3multicall.svg?style=flat-square)](https://github.com/0rtis/w3multicall/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
 [![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
 
 
-Install with `pip install web3multicall`
+Install with `pip install w3multicall`
 
-https://pypi.org/project/web3multicall/
+https://pypi.org/project/w3multicall/
 
 
 **Want to support this project ? You can help us by:**
 - Delegating AVAX to our Avalanche node **NodeID-4btZGj8TmrycK22kwgBK5wJEFighAFWiZ**
 - Making a donation to **0xA68fBfa3E0c86D1f3fF071853df6DAe8753095E2**
 
 
@@ -25,15 +25,15 @@
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into one.
 
 # Simple Multicall
 
 ```
 from web3 import Web3
-from web3multicall.multicall import W3Multicall
+from w3multicall.multicall import W3Multicall
 
 w3 = Web3(Web3.HTTPProvider(rpc))
 
 w3_multicall = W3Multicall(w3)
 
 w3_multicall.add(W3Multicall.Call(
     '0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48',  # USDC contract address
@@ -54,15 +54,15 @@
 ```
 w3_pool = W3Pool([
         W3(Web3(Web3.HTTPProvider('https://eth-rpc.gateway.pokt.network')), 5),
         W3(Web3(Web3.HTTPProvider('https://ethereum.publicnode.com')), 5),
         W3(Web3(Web3.HTTPProvider('https://rpc.flashbots.net/')), 5)
     ], logger)
 
-executor = Web3MulticallExecutor(w3_pool, processes=len(w3_pool.w3s))
+executor = W3MulticallExecutor(w3_pool, processes=len(w3_pool.w3s))
 
 bayc_futures = []
 azuki_futures = []
 moonbird_futures = []
 for i in range(1, 10):
 
     bayc_futures.append(executor.submit(W3Multicall.Call(
```

### Comparing `w3multicall-0.0.1/pyproject.toml` & `w3multicall-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=57"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "w3multicall"
 description = "Python interface and utilities for Solidity multicall contract"
 authors = [{name = "Ortis", email = "ortis@ortis.io"}]
-version = "0.0.1"
+version = "0.1.0"
 readme = "README.md"
 keywords = ["blockchain", "web3", "etherum", "solidity"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `w3multicall-0.0.1/setup.cfg` & `w3multicall-0.1.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = w3multicall
-version = 0.0.1
+version = 0.1.0
 author = Ortis
 author_email = ortis@ortis.io
 description = Python interface and utilities for Solidity multicall contract
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0rtis/w3multicall
 project_urls =
```

### Comparing `w3multicall-0.0.1/src/w3multicall.egg-info/PKG-INFO` & `w3multicall-0.1.0/src/w3multicall.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -32,23 +32,23 @@
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-[![Pypi_repo](https://img.shields.io/pypi/v/web3multicall?style=flat-square)](https://pypi.org/project/web3multicall/)
-[![GitHub license](https://img.shields.io/github/license/0rtis/web3multicall.svg?style=flat-square)](https://github.com/0rtis/web3multicall/blob/master/LICENSE)
+[![Pypi_repo](https://img.shields.io/pypi/v/w3multicall?style=flat-square)](https://pypi.org/project/w3multicall/)
+[![GitHub license](https://img.shields.io/github/license/0rtis/w3multicall.svg?style=flat-square)](https://github.com/0rtis/w3multicall/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
 [![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
 
 
-Install with `pip install web3multicall`
+Install with `pip install w3multicall`
 
-https://pypi.org/project/web3multicall/
+https://pypi.org/project/w3multicall/
 
 
 **Want to support this project ? You can help us by:**
 - Delegating AVAX to our Avalanche node **NodeID-4btZGj8TmrycK22kwgBK5wJEFighAFWiZ**
 - Making a donation to **0xA68fBfa3E0c86D1f3fF071853df6DAe8753095E2**
 
 
@@ -62,15 +62,15 @@
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into one.
 
 # Simple Multicall
 
 ```
 from web3 import Web3
-from web3multicall.multicall import W3Multicall
+from w3multicall.multicall import W3Multicall
 
 w3 = Web3(Web3.HTTPProvider(rpc))
 
 w3_multicall = W3Multicall(w3)
 
 w3_multicall.add(W3Multicall.Call(
     '0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48',  # USDC contract address
@@ -91,15 +91,15 @@
 ```
 w3_pool = W3Pool([
         W3(Web3(Web3.HTTPProvider('https://eth-rpc.gateway.pokt.network')), 5),
         W3(Web3(Web3.HTTPProvider('https://ethereum.publicnode.com')), 5),
         W3(Web3(Web3.HTTPProvider('https://rpc.flashbots.net/')), 5)
     ], logger)
 
-executor = Web3MulticallExecutor(w3_pool, processes=len(w3_pool.w3s))
+executor = W3MulticallExecutor(w3_pool, processes=len(w3_pool.w3s))
 
 bayc_futures = []
 azuki_futures = []
 moonbird_futures = []
 for i in range(1, 10):
 
     bayc_futures.append(executor.submit(W3Multicall.Call(
```

### Comparing `w3multicall-0.0.1/src/web3multicall/multicall.py` & `w3multicall-0.1.0/src/w3multicall/multicall.py`

 * *Files identical despite different names*

### Comparing `w3multicall-0.0.1/src/web3multicall/threading/w3multicall_executor.py` & `w3multicall-0.1.0/src/w3multicall/threading/w3multicall_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 time.sleep(sleep)
             self.logger.debug("Using {}".format(next_available))
             return next_available.use()
         else:
             return None
 
 
-class Web3MulticallExecutor:
+class W3MulticallExecutor:
 
     class Task:
         def __init__(self):
             self.sync = threading.Condition()
             self.creation_time = time.time()
             self.w3_calls: Dict[int, W3Multicall.Call] = {}
             self.w3_results = None
@@ -89,34 +89,34 @@
                 if self.exception is not None:
                     raise self.exception
                 if self.w3_results is None or key not in self.w3_results:
                     raise Exception("Results not available or invalid key")
                 return self.w3_results[key]
 
     class Future:
-        def __init__(self, task: 'Web3MulticallExecutor.Task', call_key: int):
+        def __init__(self, task: 'W3MulticallExecutor.Task', call_key: int):
             self.task = task
             self.call_key = call_key
 
         def get(self):
             return self.task.get(self.call_key)
 
     def __init__(self, w3_pool: W3Pool, processes: int, multicall_contract_address = '0xcA11bde05977b3631167028862bE2a173976CA11', batch_max_size: int = 20, tick_duration: float = 0.05, logger: Union[logging.Logger, None] = None):
         self.w3_pool = w3_pool
         self.processes = processes
         self.multicall_contract_address = multicall_contract_address
         self.batch_max_size = batch_max_size
         self.tick_duration = tick_duration
         self.logger = logger
-        self.pending_task: Union[Web3MulticallExecutor.Task, None] = None
+        self.pending_task: Union[W3MulticallExecutor.Task, None] = None
         self.lock = threading.RLock()
 
         def thread_pool_initializer():
             t = threading.current_thread()
-            t.name = 'Web3MulticallExecutor-{}'.format(t.name)
+            t.name = 'W3MulticallExecutor-{}'.format(t.name)
 
         self.thread_pool = ThreadPool(processes=processes, initializer=thread_pool_initializer)
         threading.Thread(target=self.__loop, daemon=True).start()
 
     def __loop(self):
         while True:
             self.__check_pending_task()
@@ -127,15 +127,15 @@
             if self.pending_task is not None and (time.time() >= self.pending_task.creation_time + self.tick_duration or len(self.pending_task.w3_calls) >= self.batch_max_size):
                 if self.logger is not None:
                     self.logger.debug("Triggering task {}".format(self.pending_task))
                 task = self.pending_task
                 self.pending_task = None
                 self.thread_pool.apply_async(func=self.__execute, args=(task, ))
 
-    def __execute(self, task: 'Web3MulticallExecutor.Task'):
+    def __execute(self, task: 'W3MulticallExecutor.Task'):
         if self.logger is not None:
             self.logger.debug("Executing task {}".format(task))
         w3m = W3Multicall(self.w3_pool.use(), self.multicall_contract_address)
         for k in task.w3_calls:
             w3m.add(task.w3_calls[k])
         with task.sync:
             try:
@@ -153,17 +153,17 @@
                 task.sync.notify_all()
         if self.logger is not None:
             self.logger.debug("Task {} completed".format(task))
 
     def submit(self, call: W3Multicall.Call) -> Future:
         with self.lock:
             if self.pending_task is None:
-                self.pending_task = Web3MulticallExecutor.Task()
+                self.pending_task = W3MulticallExecutor.Task()
             call_key = len(self.pending_task.w3_calls)
             self.pending_task.w3_calls[call_key] = call
             task = self.pending_task
             self.__check_pending_task()
-            return Web3MulticallExecutor.Future(task, call_key)
+            return W3MulticallExecutor.Future(task, call_key)
 
     def cancel_pending(self):
         with self.lock:
             self.pending_task = None
```

