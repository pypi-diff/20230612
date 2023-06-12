# Comparing `tmp/perftester-0.6.2.tar.gz` & `tmp/perftester-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perftester-0.6.2.tar", last modified: Sat Jun  3 03:59:12 2023, max compression
+gzip compressed data, was "perftester-0.6.3.tar", last modified: Mon Jun 12 10:47:18 2023, max compression
```

## Comparing `perftester-0.6.2.tar` & `perftester-0.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-03 03:59:12.560365 perftester-0.6.2/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1063 2023-06-03 01:55:57.000000 perftester-0.6.2/LICENSE
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-03 03:59:12.559367 perftester-0.6.2/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28074 2023-06-03 01:55:57.000000 perftester-0.6.2/README.md
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-03 03:59:12.517082 perftester-0.6.2/perftester/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      285 2023-06-03 02:47:03.000000 perftester-0.6.2/perftester/__init__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5212 2023-06-03 02:47:03.000000 perftester-0.6.2/perftester/__main__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    33545 2023-06-03 02:47:06.000000 perftester-0.6.2/perftester/perftester.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-03 03:59:12.556364 perftester-0.6.2/perftester.egg-info/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      303 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/SOURCES.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/dependency_links.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/entry_points.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/requires.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-06-03 03:59:12.000000 perftester-0.6.2/perftester.egg-info/top_level.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-03 03:59:12.561678 perftester-0.6.2/setup.cfg
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      917 2023-06-03 02:50:31.000000 perftester-0.6.2/setup.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-12 10:47:18.526709 perftester-0.6.3/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1063 2023-06-03 01:55:57.000000 perftester-0.6.3/LICENSE
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-12 10:47:18.525710 perftester-0.6.3/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    28074 2023-06-03 01:55:57.000000 perftester-0.6.3/README.md
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-12 10:47:18.486144 perftester-0.6.3/perftester/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      307 2023-06-11 02:27:34.000000 perftester-0.6.3/perftester/__init__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     5212 2023-06-03 02:47:03.000000 perftester-0.6.3/perftester/__main__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    34428 2023-06-12 10:45:09.000000 perftester-0.6.3/perftester/perftester.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-12 10:47:18.521714 perftester-0.6.3/perftester.egg-info/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    32823 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      303 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       57 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/entry_points.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       61 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/requires.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       11 2023-06-12 10:47:18.000000 perftester-0.6.3/perftester.egg-info/top_level.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-12 10:47:18.527709 perftester-0.6.3/setup.cfg
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      917 2023-06-11 02:17:46.000000 perftester-0.6.3/setup.py
```

### Comparing `perftester-0.6.2/LICENSE` & `perftester-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `perftester-0.6.2/PKG-INFO` & `perftester-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.2
+Version: 0.6.3
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
```

### Comparing `perftester-0.6.2/README.md` & `perftester-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `perftester-0.6.2/perftester/__main__.py` & `perftester-0.6.3/perftester/__main__.py`

 * *Files identical despite different names*

### Comparing `perftester-0.6.2/perftester/perftester.py` & `perftester-0.6.3/perftester/perftester.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 call of a function. That way, the user can define tests without worrying of
 different settings: while the "number" argument in timeit functions affects
 the results, it does not so in perftester.
 
 Remember that all lambda functions are stored as anonymous functions,
 without a name. Hence it's better to avoid using lambdas in perftester.
 
+WARNING: Unlike memory_profiler.memory_usage(), which reports memory in MiB,
+perftester provides data in MB. That way, the data from 
+memory_profiler.memory_usage() and pympler.asizeof.asizeof() are provided in
+the same units. If you want to recalculate the data to MiB, you can divide the
+memory by perftester.MiB_TO_MB_FACTOR.
+
 For the sake of pretty-printing the benchmarks, perftester comes with a pp
 function, which rounds all numbers to four significant digits and prints
 the object using pprint.pprint:
 >>> import perftester as pt
 >>> pt.pp([2.1212, 2.93135])
 [2.121, 2.931]
 
@@ -38,24 +44,27 @@
 from collections.abc import Callable
 from easycheck import (
     check_argument,
     check_if,
     check_if_not,
     check_instance,
     check_if_paths_exist,
-    assert_instance,
+    assert_instance, # required for doctests
 )
 from functools import wraps
 from memory_profiler import memory_usage
 from pathlib import Path
 from pprint import pprint
 from pympler.asizeof import asizeof
 from statistics import mean
 
 
+MiB_TO_MB_FACTOR = 1.048576
+
+
 class CLIPathError(Exception):
     """Exception class to be used for the CLI perftester app."""
 
 
 class LogFilePathError(Exception):
     """Exception class to be used when incorrect path is provided for a log file."""
 
@@ -284,15 +293,15 @@
         Returns:
             float: the minimum maximum memory usage over time across all runs.
         """
         memory_results = [
             memory_usage((self.benchmark_function, (), {}))
             for _ in range(self.defaults["memory"]["repeat"])
         ]
-        self.memory_benchmark = min(max(r) for r in memory_results)
+        self.memory_benchmark = MiB_TO_MB_FACTOR * min(max(r) for r in memory_results)
 
     def set_defaults(
         self, which, number=None, repeat=None, Number=None, Repeat=None
     ):
         """Change the default settings.
 
         Beware! This does not change particular settings for a particular test,
@@ -604,14 +613,17 @@
     a limit for a relative test (against a function defined in the config);
     then use raw_limit=None. But you can also use both at the same time, and
     the tests passes only when both the raw and the relative tests pass.
 
     When you use Repeat, it has a higher priority than the corresponding
     setting from config.settings, and it will be used. This is used in this
     single call only, and so it does not overwrite the config settings.
+    
+    WARNING: Unlike memory_profiler.memory_usage(), which reports memory in MiB,
+    perftester provides data in MB.
 
     Args:
         func (Callable): the tested function.
         raw_limit (float): raw limit for the test. It is the maximum memory
             that the function can use; if it's exceeded, the test does not pass.
         relative_limit (float): relative limit for the test. It is used for
             relative testing (against a standard function defined in the
@@ -698,14 +710,17 @@
     be added to config.settings.
 
     When you use Repeat, it has a higher priority than the corresponding
     setting from config.settings, and it will be used. This is used in this
     single call only, and so it does not overwrite the config settings.
 
     The function returns a dict that you can pretty-print using function pp().
+    
+    WARNING: Unlike memory_profiler.memory_usage(), which reports memory in MiB,
+    perftester provides data in MB.
 
     Args:
         func (Callable): a function (or a callable) to run benchmarks for
         Repeat (int): a repeat setting, overwriting (for this function call)
             the setting in config.settings[func]["memory"]["repeat"]
         *args, **kwargs: arguments passed to func
 
@@ -720,30 +735,41 @@
     """
     check_instance(func, Callable, message="Argument func must be a callable.")
     _add_func_to_config(func)
 
     n = Repeat or config.settings[func]["memory"]["repeat"]
 
     try:
-        memory_results = [memory_usage((func, args, kwargs)) for i in range(n)]
+        memory_results = [
+            memory_usage((func, args, kwargs))
+            for i in range(n)
+        ]
     except Exception as e:
         raise FunctionError(
             f"The tested function raised {type(e).__name__}: {str(e)}"
         )
 
-    memory_results_mean = [mean(this_result) for this_result in memory_results]
+    for i, result in enumerate(memory_results):
+        for j, _ in enumerate(result):
+            memory_results[i][j] *= MiB_TO_MB_FACTOR
+
+    memory_results_mean = [
+        mean(this_result)
+        for this_result in memory_results
+    ]
     memory_results_max = [max(this_result) for this_result in memory_results]
     overall_mean = mean(memory_results_mean)
     # We take the min of the max values
     overall_max = min(memory_results_max)
 
     relative_results = copy.deepcopy(memory_results)
     for i, result in enumerate(relative_results):
         for j, r in enumerate(result):
             relative_results[i][j] = r / config.memory_benchmark
+            
     return {
         "raw_results": memory_results,
         "relative_results": relative_results,
         "mean_result_per_run": memory_results_mean,
         "max_result_per_run": memory_results_max,
         "max_result_per_run_relative": [
             r / config.memory_benchmark for r in memory_results_max
```

### Comparing `perftester-0.6.2/perftester.egg-info/PKG-INFO` & `perftester-0.6.3/perftester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perftester
-Version: 0.6.2
+Version: 0.6.3
 Summary: Lightweight performance testing in Python
 Home-page: https://github.com/nyggus/perftester
 Author: Nyggus
 Author-email: nyggus@gmail.com
 License: UNKNOWN
 Description: # `perftester`: Lightweight performance testing of Python functions
```

### Comparing `perftester-0.6.2/setup.py` & `perftester-0.6.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 extras_requirements = {
     "dev": ["wheel", "black"],
 }
 
 setuptools.setup(
     name="perftester",
-    version="0.6.2",
+    version="0.6.3",
     author="Nyggus",
     author_email="nyggus@gmail.com",
     description="Lightweight performance testing in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyggus/perftester",
     packages=setuptools.find_packages(),
```

