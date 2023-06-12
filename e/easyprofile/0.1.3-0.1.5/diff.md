# Comparing `tmp/easyprofile-0.1.3.tar.gz` & `tmp/easyprofile-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyprofile-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "easyprofile-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `easyprofile-0.1.3.tar` & `easyprofile-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-06-12 07:26:10.246984 easyprofile-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     3415 2023-06-12 07:26:10.246984 easyprofile-0.1.3/README.md
--rw-r--r--   0        0        0     4169 2023-06-12 07:26:10.246984 easyprofile-0.1.3/easyprofile.py
--rw-r--r--   0        0        0      532 2023-06-12 07:26:10.246984 easyprofile-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 easyprofile-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 07:35:33.679124 easyprofile-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     3415 2023-06-12 07:35:33.679124 easyprofile-0.1.5/README.md
+-rw-r--r--   0        0        0     4610 2023-06-12 07:35:33.679124 easyprofile-0.1.5/easyprofile.py
+-rw-r--r--   0        0        0      532 2023-06-12 07:35:33.679124 easyprofile-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 easyprofile-0.1.5/PKG-INFO
```

### Comparing `easyprofile-0.1.3/LICENSE.txt` & `easyprofile-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easyprofile-0.1.3/README.md` & `easyprofile-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `easyprofile-0.1.3/easyprofile.py` & `easyprofile-0.1.5/easyprofile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''Easy context-based profiling with logging support'''
 
 from __future__ import annotations
 
-__version__ = '0.1.3'
+__version__ = '0.1.5'
 
 __all__ = (
     'BaseProfile',
     'LogProfile',
     'ignore',
     'ignored',
     'log',
@@ -31,14 +31,29 @@
     for u in ['B', 'K', 'M', 'G', 'T', 'P']:
         if x < 1000:
             break
         x /= 1000
     return f'{x:.3f}'[:5] + u
 
 
+def ftd(time: float | None) -> str:
+    '''Format time difference.'''
+    if time is None:
+        return '--:--:--.------'
+    td = timedelta(seconds=time)
+    mm, ss = divmod(td.seconds, 60)
+    hh, mm = divmod(mm, 60)
+    uu = td.microseconds
+    if td.days:
+        dd = f'{td.days} day{"s" if abs(td.days) != 1 else ""}, '
+    else:
+        dd = ''
+    return f'{dd}{hh:02d}:{mm:02d}:{ss:02d}.{uu:06d}'
+
+
 def fname(frame):
     '''Return the function name from a frame.'''
     name = frame.f_code.co_name
     try:
         qualname = frame.f_code.co_qualname
     except AttributeError:
         qualname = name
@@ -130,33 +145,31 @@
         self.counts[hash(obj)] = perf_counter()
 
     def __stop(self, obj: Any) -> float:
         count = perf_counter()
         return count - self.counts.pop(hash(obj), count)
 
     def __log(self, time: float, name: str) -> None:
-        parr = []
-        if time > 0:
-            parr += [f'{timedelta(seconds=time)!s}']
+        line = []
         if tracemalloc.is_tracing():
-            mem, peak = tracemalloc.get_traced_memory()
-            parr += [f'{fnb(mem)}', f'{fnb(peak)}']
-        if parr:
-            prof = '[' + ' - '.join(parr) + ']'
-        else:
-            prof = ''
-        self.log(f'{prof} {name}')
+            current, peak = tracemalloc.get_traced_memory()
+            line.append(f'[{fnb(current)} / {fnb(peak)}]')
+        line.append('>' if time is None else '<')
+        line.append(name)
+        if time is not None:
+            line.append(f'[{ftd(time)}]')
+        self.log(' '.join(line))
 
     def _call(self, frame: FrameType, arg: Any) -> None:
-        self.__start(frame)
+        self.__log(self.__start(frame), fname(frame))
 
     def _return(self, frame: FrameType, arg: Any) -> None:
         self.__log(self.__stop(frame), fname(frame))
 
     def _c_call(self, frame: FrameType, arg: Any) -> None:
-        self.__start(arg)
+        self.__log(self.__start(arg), cname(arg))
 
     def _c_return(self, frame: FrameType, arg: Any) -> None:
         self.__log(self.__stop(arg), cname(arg))
 
 
 log = LogProfile.profile
```

### Comparing `easyprofile-0.1.3/pyproject.toml` & `easyprofile-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easyprofile-0.1.3/PKG-INFO` & `easyprofile-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyprofile
-Version: 0.1.3
+Version: 0.1.5
 Summary: Easy context-based profiling with logging support
 Author-email: Nicolas Tessore <n.tessore@ucl.ac.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Homepage, https://github.com/ntessore/easyprofile
 Project-URL: Issues, https://github.com/ntessore/easyprofile/issues
```

