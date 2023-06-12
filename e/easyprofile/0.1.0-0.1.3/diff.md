# Comparing `tmp/easyprofile-0.1.0.tar.gz` & `tmp/easyprofile-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyprofile-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "easyprofile-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `easyprofile-0.1.0.tar` & `easyprofile-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-05-23 00:06:38.657308 easyprofile-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3249 2023-05-24 11:18:41.678737 easyprofile-0.1.0/README.md
--rw-r--r--   0        0        0     4065 2023-06-09 13:15:57.554758 easyprofile-0.1.0/easyprofile.py
--rw-r--r--   0        0        0      532 2023-05-24 11:23:53.275865 easyprofile-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 easyprofile-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 07:26:10.246984 easyprofile-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     3415 2023-06-12 07:26:10.246984 easyprofile-0.1.3/README.md
+-rw-r--r--   0        0        0     4169 2023-06-12 07:26:10.246984 easyprofile-0.1.3/easyprofile.py
+-rw-r--r--   0        0        0      532 2023-06-12 07:26:10.246984 easyprofile-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 easyprofile-0.1.3/PKG-INFO
```

### Comparing `easyprofile-0.1.0/LICENSE.txt` & `easyprofile-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyprofile-0.1.0/README.md` & `easyprofile-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -98,20 +98,26 @@
 event `<event>` is encountered, with a signature of `frame, arg`.
 
 ```py
 >>> class MyProfile(easyprofile.BaseProfile):
 ...     def __init__(self, arg, *, kwarg):
 ...         print(f'MyProfile: init, {arg=}, {kwarg=}')
 ...
+...     def _attach(self, frame, arg):
+...         print('MyProfile: attached')
+...
+...     def _detach(self, frame, arg):
+...         print('MyProfile: detached')
+...
 ...     def _call(self, frame, arg):
 ...         print('MyProfile: function called')
-... 
+...
 ...     def _return(self, frame, arg):
 ...         print('MyProfile: function returned')
-... 
+...
 ...     # profile C extension calls using the same methods
 ...     _c_call = _call
 ...     _c_return = _return
 ...
 
 ```
```

### Comparing `easyprofile-0.1.0/easyprofile.py` & `easyprofile-0.1.3/easyprofile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''Easy context-based profiling with logging support'''
 
 from __future__ import annotations
 
-__version__ = '0.1.0'
+__version__ = '0.1.3'
 
 __all__ = (
     'BaseProfile',
     'LogProfile',
     'ignore',
     'ignored',
     'log',
     'profile',
 )
 
 import tracemalloc
-from sys import getprofile, setprofile
 from datetime import timedelta
+from sys import getprofile, setprofile
 from time import perf_counter
 from types import FrameType
 from typing import Any, Callable
 
 ProfileType = Callable[[FrameType, str, Any], Any]
 
 PROFILE_IGNORE = set()
@@ -31,14 +31,38 @@
     for u in ['B', 'K', 'M', 'G', 'T', 'P']:
         if x < 1000:
             break
         x /= 1000
     return f'{x:.3f}'[:5] + u
 
 
+def fname(frame):
+    '''Return the function name from a frame.'''
+    name = frame.f_code.co_name
+    try:
+        qualname = frame.f_code.co_qualname
+    except AttributeError:
+        qualname = name
+    if qualname.endswith(name):
+        name = qualname
+    return name
+
+
+def cname(func):
+    '''Return the function name from a C function.'''
+    name = func.__name__
+    try:
+        qualname = func.__qualname__
+    except AttributeError:
+        qualname = name
+    if qualname.endswith(name):
+        name = qualname
+    return name
+
+
 def ignored(func):
     '''Mark a function as ignored by the profiler.'''
     PROFILE_IGNORE.add(func.__code__)
     return func
 
 
 class profile:
@@ -65,26 +89,23 @@
                         else:
                             in_scope = frame.f_back is scope
 
                         if in_scope and frame.f_code not in PROFILE_IGNORE:
                             func(frame, event, arg)
 
                     setprofile(prof)
-                    func(scope, 'attach', None)
         else:
             trap = None
 
         self.stack.append(getprofile())
         setprofile(trap)
         return func
 
     @ignored
     def __exit__(self, *args: Any) -> None:
-        if self.func is not None:
-            self.func(None, 'detach', None)
         setprofile(self.stack.pop())
 
 
 ignore = profile(None)
 
 
 class BaseProfile:
@@ -99,58 +120,43 @@
             handler(frame, arg)
 
 
 class LogProfile(BaseProfile):
 
     def __init__(self, log: Callable[[str], Any]) -> None:
         self.log = log
-        self.counts: dict[FrameType, float] = {}
-        self.frame: FrameType | None = None
+        self.counts: dict[int, float] = {}
 
-    def _attach(self, frame: FrameType, arg: Any) -> None:
-        self.frame = frame
+    def __start(self, obj: Any) -> None:
+        self.counts[hash(obj)] = perf_counter()
 
-    def _detach(self, frame: FrameType, arg: Any) -> None:
-        self.frame = None
-
-    def _call(self, frame: FrameType, arg: Any) -> None:
-        self.counts[frame] = perf_counter()
-
-    def _return(self, frame: FrameType, arg: Any) -> None:
+    def __stop(self, obj: Any) -> float:
         count = perf_counter()
-        delta = count - self.counts.get(frame, count)
-
-        names = []
-        f: FrameType | None = frame
-        while f:
-            name = f.f_code.co_name
-            try:
-                qualname = f.f_code.co_qualname
-            except AttributeError:
-                qualname = name
-            if qualname.endswith(name):
-                name = qualname
-            names.append(name)
-            if f == self.frame:
-                break
-            f = f.f_back
-        name = ' > '.join(names[-2::-1])
+        return count - self.counts.pop(hash(obj), count)
 
+    def __log(self, time: float, name: str) -> None:
         parr = []
-        if delta > 0:
-            parr += [f'{timedelta(seconds=delta)!s}']
+        if time > 0:
+            parr += [f'{timedelta(seconds=time)!s}']
         if tracemalloc.is_tracing():
             mem, peak = tracemalloc.get_traced_memory()
             parr += [f'{fnb(mem)}', f'{fnb(peak)}']
-
         if parr:
             prof = '[' + ' - '.join(parr) + ']'
         else:
             prof = ''
-
         self.log(f'{prof} {name}')
 
-    _c_call = _call
-    _c_return = _return
+    def _call(self, frame: FrameType, arg: Any) -> None:
+        self.__start(frame)
+
+    def _return(self, frame: FrameType, arg: Any) -> None:
+        self.__log(self.__stop(frame), fname(frame))
+
+    def _c_call(self, frame: FrameType, arg: Any) -> None:
+        self.__start(arg)
+
+    def _c_return(self, frame: FrameType, arg: Any) -> None:
+        self.__log(self.__stop(arg), cname(arg))
 
 
 log = LogProfile.profile
```

### Comparing `easyprofile-0.1.0/pyproject.toml` & `easyprofile-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyprofile-0.1.0/PKG-INFO` & `easyprofile-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyprofile
-Version: 0.1.0
+Version: 0.1.3
 Summary: Easy context-based profiling with logging support
 Author-email: Nicolas Tessore <n.tessore@ucl.ac.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Homepage, https://github.com/ntessore/easyprofile
 Project-URL: Issues, https://github.com/ntessore/easyprofile/issues
@@ -109,20 +109,26 @@
 event `<event>` is encountered, with a signature of `frame, arg`.
 
 ```py
 >>> class MyProfile(easyprofile.BaseProfile):
 ...     def __init__(self, arg, *, kwarg):
 ...         print(f'MyProfile: init, {arg=}, {kwarg=}')
 ...
+...     def _attach(self, frame, arg):
+...         print('MyProfile: attached')
+...
+...     def _detach(self, frame, arg):
+...         print('MyProfile: detached')
+...
 ...     def _call(self, frame, arg):
 ...         print('MyProfile: function called')
-... 
+...
 ...     def _return(self, frame, arg):
 ...         print('MyProfile: function returned')
-... 
+...
 ...     # profile C extension calls using the same methods
 ...     _c_call = _call
 ...     _c_return = _return
 ...
 
 ```
```

