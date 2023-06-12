# Comparing `tmp/std.algorithm-1.1.4.tar.gz` & `tmp/std.algorithm-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std.algorithm-1.1.4.tar", last modified: Sun Jun  4 15:21:33 2023, max compression
+gzip compressed data, was "std.algorithm-1.1.5.tar", last modified: Mon Jun 12 08:50:00 2023, max compression
```

## Comparing `std.algorithm-1.1.4.tar` & `std.algorithm-1.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.416764 std.algorithm-1.1.4/
--rw-rw-rw-   0        0        0      324 2023-06-04 15:21:33.416764 std.algorithm-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       47 2022-10-07 01:09:45.000000 std.algorithm-1.1.4/README.md
--rw-rw-rw-   0        0        0      312 2023-06-04 15:21:33.417790 std.algorithm-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-02-19 07:05:31.000000 std.algorithm-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.388840 std.algorithm-1.1.4/std/
--rw-rw-rw-   0        0        0    14485 2023-06-03 18:41:19.000000 std.algorithm-1.1.4/std/MySQL.py
--rw-rw-rw-   0        0        0    20805 2023-05-31 15:05:36.000000 std.algorithm-1.1.4/std/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-18 14:54:44.000000 std.algorithm-1.1.4/std/combinatorics.py
--rw-rw-rw-   0        0        0     2819 2023-05-14 09:54:42.000000 std.algorithm-1.1.4/std/data.py
--rw-rw-rw-   0        0        0      214 2022-10-12 06:19:30.000000 std.algorithm-1.1.4/std/error.py
--rw-rw-rw-   0        0        0     8504 2023-05-14 09:57:03.000000 std.algorithm-1.1.4/std/file.py
--rw-rw-rw-   0        0        0     1754 2023-03-04 02:50:47.000000 std.algorithm-1.1.4/std/http.py
--rw-rw-rw-   0        0        0    39618 2023-05-24 14:34:06.000000 std.algorithm-1.1.4/std/keras.py
-drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.414798 std.algorithm-1.1.4/std/lib/
--rw-rw-rw-   0        0        0  2220528 2022-10-22 04:21:48.000000 std.algorithm-1.1.4/std/lib/eigen.dll
--rw-rw-rw-   0        0        0    12858 2022-11-01 16:38:35.000000 std.algorithm-1.1.4/std/nlp.py
--rw-rw-rw-   0        0        0       89 2023-03-11 01:48:50.000000 std.algorithm-1.1.4/std/regexp.py
--rw-rw-rw-   0        0        0      770 2022-10-12 05:55:17.000000 std.algorithm-1.1.4/std/search.py
--rw-rw-rw-   0        0        0    19454 2023-03-11 01:48:50.000000 std.algorithm-1.1.4/std/sets.py
--rw-rw-rw-   0        0        0     1162 2022-10-07 01:27:48.000000 std.algorithm-1.1.4/std/tree.py
--rw-rw-rw-   0        0        0      443 2023-03-17 14:49:04.000000 std.algorithm-1.1.4/std/unicode.py
--rw-rw-rw-   0        0        0    35286 2023-02-05 04:04:59.000000 std.algorithm-1.1.4/std/xml.py
-drwxrwxrwx   0        0        0        0 2023-06-04 15:21:33.394823 std.algorithm-1.1.4/std.algorithm.egg-info/
--rw-rw-rw-   0        0        0      324 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-04 15:21:33.000000 std.algorithm-1.1.4/std.algorithm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 08:50:00.819171 std.algorithm-1.1.5/
+-rw-rw-rw-   0        0        0      324 2023-06-12 08:50:00.819171 std.algorithm-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2022-10-13 00:41:19.000000 std.algorithm-1.1.5/README.md
+-rw-rw-rw-   0        0        0      312 2023-06-12 08:50:00.820170 std.algorithm-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-03-01 06:13:36.000000 std.algorithm-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:50:00.802775 std.algorithm-1.1.5/std/
+-rw-rw-rw-   0        0        0    14485 2023-06-05 00:56:34.000000 std.algorithm-1.1.5/std/MySQL.py
+-rw-rw-rw-   0        0        0    20878 2023-06-09 00:47:00.000000 std.algorithm-1.1.5/std/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-19 00:57:44.000000 std.algorithm-1.1.5/std/combinatorics.py
+-rw-rw-rw-   0        0        0     2819 2023-05-15 01:39:31.000000 std.algorithm-1.1.5/std/data.py
+-rw-rw-rw-   0        0        0      202 2022-10-13 00:41:19.000000 std.algorithm-1.1.5/std/error.py
+-rw-rw-rw-   0        0        0     8575 2023-06-06 01:16:49.000000 std.algorithm-1.1.5/std/file.py
+-rw-rw-rw-   0        0        0     1754 2023-03-01 06:13:03.000000 std.algorithm-1.1.5/std/http.py
+-rw-rw-rw-   0        0        0    39618 2023-05-24 03:29:48.000000 std.algorithm-1.1.5/std/keras.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:50:00.815170 std.algorithm-1.1.5/std/lib/
+-rw-rw-rw-   0        0        0  2220528 2022-10-21 02:36:11.000000 std.algorithm-1.1.5/std/lib/eigen.dll
+-rw-rw-rw-   0        0        0    13748 2023-06-12 07:38:44.000000 std.algorithm-1.1.5/std/nlp.py
+-rw-rw-rw-   0        0        0       89 2023-03-07 01:03:31.000000 std.algorithm-1.1.5/std/regexp.py
+-rw-rw-rw-   0        0        0      740 2022-10-13 00:41:19.000000 std.algorithm-1.1.5/std/search.py
+-rw-rw-rw-   0        0        0    19454 2023-03-08 09:05:45.000000 std.algorithm-1.1.5/std/sets.py
+-rw-rw-rw-   0        0        0     1162 2022-10-13 00:41:19.000000 std.algorithm-1.1.5/std/tree.py
+-rw-rw-rw-   0        0        0      443 2023-03-16 02:15:53.000000 std.algorithm-1.1.5/std/unicode.py
+-rw-rw-rw-   0        0        0    35286 2023-02-02 07:42:54.000000 std.algorithm-1.1.5/std/xml.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:50:00.812770 std.algorithm-1.1.5/std.algorithm.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-06-12 08:50:00.000000 std.algorithm-1.1.5/std.algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-06-12 08:50:00.000000 std.algorithm-1.1.5/std.algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 08:50:00.000000 std.algorithm-1.1.5/std.algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 08:50:00.000000 std.algorithm-1.1.5/std.algorithm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-12 08:50:00.000000 std.algorithm-1.1.5/std.algorithm.egg-info/top_level.txt
```

### Comparing `std.algorithm-1.1.4/std/MySQL.py` & `std.algorithm-1.1.5/std/MySQL.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/__init__.py` & `std.algorithm-1.1.5/std/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os, json, time, queue, inspect, functools, sys, signal
 from _collections import defaultdict
 from enum import Enum, unique
-
+from types import FunctionType, GeneratorType
 
 def is_Windows():
     return os.sep == '\\'
 
     
 # is Linux System
 def is_Linux():
@@ -102,15 +102,14 @@
         eol_convert(fileName)
 
 def cstring(s):
     return bytes(s, 'utf8')
 
 
 def json_encode(data, utf8=False, indent=None):
-    from types import FunctionType
     if isinstance(data, FunctionType):
 
         def func(*args, **kwargs): 
             return json_encode(data(*args, **kwargs), utf8=utf8, indent=indent)
         
         func.__name__ = data.__name__
         return func 
@@ -666,14 +665,16 @@
     for i in range(0, len(listOfElement), batch_size):
         batches[index] = listOfElement[i: min(i + batch_size, len(listOfElement))]
         index += 1
     return batches
 
 
 def is_same(list):
+    if isinstance(list, GeneratorType):
+        list = [*list]
     for i in range(1, len(list)):
         if list[i] != list[i - 1]:
             return False
                         
     return True
```

### Comparing `std.algorithm-1.1.4/std/combinatorics.py` & `std.algorithm-1.1.5/std/combinatorics.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/data.py` & `std.algorithm-1.1.5/std/data.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/file.py` & `std.algorithm-1.1.5/std/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,20 @@
     if not os.path.exists(basedir):
         os.makedirs(basedir)
 
 
 class Text:
 
     def __init__(self, path, encoding="utf-8", **kwargs):
+        mode = kwargs.get('mode') or "r+" if os.path.isfile(path) else "w+"
         try:
-            self.file = open(path, "r+" if os.path.isfile(path) else "w+", encoding=encoding)
-        except PermissionError: 
-            self.file = open(path, "r", encoding=encoding)
+            self.file = open(path, mode=mode, encoding=encoding)
+        except PermissionError as e:
+            print("error message printed in std.file:", e)
+            exit(0)
         except FileNotFoundError:
             createNewFile(path)
             self.file = open(path, "w+", encoding=encoding)
 
         self.rewind()
         
         if kwargs.get('strip'):
```

### Comparing `std.algorithm-1.1.4/std/http.py` & `std.algorithm-1.1.5/std/http.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/keras.py` & `std.algorithm-1.1.5/std/keras.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/lib/eigen.dll` & `std.algorithm-1.1.5/std/lib/eigen.dll`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/nlp.py` & `std.algorithm-1.1.5/std/nlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,7 +300,49 @@
         msg = 'pos tag count and token text count are not equal, token {}, pos tag {}'
         if pos_tag_count != new_token_count:
             raise Exception(msg.format(new_token_count, pos_tag_count))
         else:
             for token, pos_tag in zip(new_tokens, pos_tags):
                 token['pos_tag'] = pos_tag
     return new_tokens
+
+
+import regex as re
+
+def detect_language(text):
+    cn = 0
+    en = 0
+    for ch in text:
+        if re.compile('\p{Letter}').match(ch):
+            if re.compile('\p{Han}').fullmatch(ch):
+                cn += 2
+            else:
+                en += 1    
+
+        elif re.compile('\p{Number}').match(ch):
+            if ord(ch) > 256:
+                cn += 2
+            else:
+                en += 1
+
+        elif re.compile('\p{Punctuation}').match(ch):
+            if ord(ch) > 256:
+                cn += 2
+            else:
+                en += 1
+
+        elif re.compile('\p{Symbol}').match(ch):
+            ...
+        elif re.compile('\p{Separator}').match(ch):
+            ...
+        elif re.compile('\p{Mark}').match(ch):
+            ...
+        else:
+            ...
+            
+    if cn > en:
+        return 'cn'
+
+    if en > cn:
+        return 'en'
+    
+    return 'en'
```

### Comparing `std.algorithm-1.1.4/std/sets.py` & `std.algorithm-1.1.5/std/sets.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/tree.py` & `std.algorithm-1.1.5/std/tree.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.4/std/xml.py` & `std.algorithm-1.1.5/std/xml.py`

 * *Files identical despite different names*

