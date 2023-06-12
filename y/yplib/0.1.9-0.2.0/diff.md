# Comparing `tmp/yplib-0.1.9.tar.gz` & `tmp/yplib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.1.9.tar", last modified: Fri Jun  9 07:59:35 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.0.tar", last modified: Mon Jun 12 01:20:45 2023, max compression
```

## Comparing `yplib-0.1.9.tar` & `yplib-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 07:59:35.690467 yplib-0.1.9/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-09 07:59:35.690155 yplib-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 07:59:35.690999 yplib-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-09 07:59:17.000000 yplib-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:59:35.686970 yplib-0.1.9/yplib/
--rw-rw-rw-   0        0        0     9490 2023-06-09 07:58:57.000000 yplib-0.1.9/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.1.9/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-09 07:59:35.689643 yplib-0.1.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 07:59:35.000000 yplib-0.1.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 01:20:45.593160 yplib-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-12 01:20:45.592717 yplib-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 01:20:45.593160 yplib-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-12 01:18:40.000000 yplib-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:20:45.588903 yplib-0.2.0/yplib/
+-rw-rw-rw-   0        0        0    11653 2023-06-12 01:18:04.000000 yplib-0.2.0/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.0/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:20:45.591516 yplib-0.2.0/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.1.9/LICENSE` & `yplib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.1.9/PKG-INFO` & `yplib-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.9
+Version: 0.2.0
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.1.9/setup.py` & `yplib-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.1.9",
+  version="0.2.0",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.1.9/yplib/__init__.py` & `yplib-0.2.0/yplib/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import os
 import uuid
 from datetime import datetime
 
 import xlrd
 import xlwt
+import re
 # import random
 from yplib.line_stack_temp import line_stack_temp_html
 
 
 # 记录日志, 如果是对象会转化为 json
 def log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
         a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
@@ -32,14 +33,77 @@
 # 将 log 数据, 写入到文件
 def log_to_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     lo = log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
     list_to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True)
 
 
+# 将 log 数据, 写入到固定文件中
+def log_to_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+               a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
+    lo = log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
+    list_to_txt([lo], file_name, 'log', True)
+
+
+# 将下划线命名转成驼峰命名
+# 例如 : user_id -> userId
+# 例如 : USER_ID -> userId
+def to_hump(a1=''):
+    if a1 == '':
+        return a1
+    a1 = a1.lower()
+    words = a1.split('_')
+    r = ""
+    for w in words:
+        r += w.capitalize()
+    return r[0].lower() + r[1:]
+
+
+def to_hump_more(a1='', a2='', a3='', a4='', a5=''):
+    if a1 == '':
+        return a1
+    elif a2 == '':
+        return to_hump(a1)
+    elif a3 == '':
+        return to_hump(a1), to_hump(a2)
+    elif a4 == '':
+        return to_hump(a1), to_hump(a2), to_hump(a3)
+    elif a5 == '':
+        return to_hump(a1), to_hump(a2), to_hump(a3), to_hump(a4)
+    return to_hump(a1), to_hump(a2), to_hump(a3), to_hump(a4), to_hump(a5)
+
+
+# 将驼峰命名转成下划线命名
+# 例如 : userId -> user_id
+def to_underline(a1=''):
+    if a1 == '':
+        return a1
+    r = ''
+    for char in a1:
+        if char.isupper():
+            r += '_' + char.lower()
+        else:
+            r += char
+    return r
+
+
+def to_underline_more(a1='', a2='', a3='', a4='', a5=''):
+    if a1 == '':
+        return a1
+    elif a2 == '':
+        return to_underline(a1)
+    elif a3 == '':
+        return to_underline(a1), to_underline(a2)
+    elif a4 == '':
+        return to_underline(a1), to_underline(a2), to_underline(a3)
+    elif a5 == '':
+        return to_underline(a1), to_underline(a2), to_underline(a3), to_underline(a4)
+    return to_underline(a1), to_underline(a2), to_underline(a3), to_underline(a4), to_underline(a5)
+
+
 # 是否能用 json
 def can_use_json(data):
     if isinstance(data, dict) or isinstance(data, list) or isinstance(data, tuple) or isinstance(data, set):
         return True
     return False
 
 
@@ -77,15 +141,15 @@
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def list_to_txt(list_data, file_name, file_path='data', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
-    if fixed_name is False:
+    if fixed_name:
         file_name = file_name + suffix
     else:
         file_name = get_file_name(file_name, suffix)
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
     text_file = open(file_name_path, 'a', encoding='utf-8')
@@ -274,7 +338,18 @@
 
 # log_to_file(1)
 # log_to_file(12)
 # log_to_file('yangpu')
 # print(str_to_int('yan123gpu'))
 # print(str_to_float('yan123gpu'))
 # print(str_to_float('yan123g.12pu'))
+
+#
+# print(to_hump('user_id'))
+# print(to_hump('USER_ID'))
+# print(to_hump('userId'))
+# print(to_hump('user'))
+# print(to_hump(''))
+
+# print(to_hump_more('userId'))
+
+# print(to_underline('userId'))
```

### Comparing `yplib-0.1.9/yplib/line_stack_temp.py` & `yplib-0.2.0/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.1.9/yplib.egg-info/PKG-INFO` & `yplib-0.2.0/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.1.9
+Version: 0.2.0
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

