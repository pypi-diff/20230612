# Comparing `tmp/yplib-0.2.2.tar.gz` & `tmp/yplib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.2.2.tar", last modified: Mon Jun 12 07:06:00 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.3.tar", last modified: Mon Jun 12 07:43:57 2023, max compression
```

## Comparing `yplib-0.2.2.tar` & `yplib-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:06:00.828449 yplib-0.2.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-12 07:06:00.828137 yplib-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 07:06:00.828449 yplib-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-12 07:05:48.000000 yplib-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:06:00.825281 yplib-0.2.2/yplib/
--rw-rw-rw-   0        0        0    14292 2023-06-12 07:04:18.000000 yplib-0.2.2/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.2/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:06:00.827239 yplib-0.2.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 07:43:57.443023 yplib-0.2.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-12 07:43:57.442676 yplib-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:43:57.443446 yplib-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-12 07:43:39.000000 yplib-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:43:57.439447 yplib-0.2.3/yplib/
+-rw-rw-rw-   0        0        0    15364 2023-06-12 07:42:15.000000 yplib-0.2.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.3/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:43:57.441917 yplib-0.2.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.2.2/LICENSE` & `yplib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.2.2/PKG-INFO` & `yplib-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.2
+Version: 0.2.3
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.2.2/setup.py` & `yplib-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.2.2",
+  version="0.2.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.2.2/yplib/__init__.py` & `yplib-0.2.3/yplib/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import datetime
 
 import xlrd
 import xlwt
 import time
 import re
 # import random
+import hashlib
 from yplib.line_stack_temp import line_stack_temp_html
 
 
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
@@ -118,14 +119,24 @@
 def get_file_name(file_name, suffix='.txt'):
     return str(file_name) \
         + '_' + datetime.today().strftime('%Y%m%d_%H%M%S') \
         + '_' + uuid_random()[0:5] \
         + suffix
 
 
+def do_md5(data='do_md5'):
+    return hashlib.md5(data.encode(encoding='UTF-8')).hexdigest()
+
+
+def do_sha256(data='do_sha256'):
+    h = hashlib.sha256()
+    h.update(data.encode('utf-8'))
+    return h.hexdigest()
+
+
 def uuid_random(length=32):
     r = uuid.uuid4().hex
     while len(r) < length:
         r += uuid.uuid4().hex
     return r[0:length]
 
 
@@ -219,14 +230,27 @@
     if can_use_json(data):
         s = json.dumps(data)
     else:
         s = str(data)
     return s
 
 
+# 根据json的key排序,用于签名
+def sort_by_json_key(data):
+    key_list = list()
+    for one_data in data:
+        key_list.append(one_data)
+    key_list.sort()
+    result = ''
+    for one_data in key_list:
+        result += one_data + '=' + data[one_data] + '&'
+    if len(result) > 0:
+        return result[0: len(result) - 1]
+
+
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前,行后的空格
 def to_list(file_name='a.txt', sheet_index=0):
     data_list = list()
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
         book = xlrd.open_workbook(file_name)  # 打开一个excel
         sheet = book.sheet_by_index(sheet_index)  # 根据顺序获取sheet
@@ -438,7 +462,27 @@
 # print(to_datetime('2019-09-08 12'))
 # print(to_datetime('2019-09-08 12:13'))
 # print(to_datetime('2019-09-08 12:13:14'))
 # print(to_datetime('2019-09-08 12:13:14.789'))
 # print(to_datetime(1686537485))
 # print(to_datetime(1686537484467))
 # print(to_datetime(datetime.today()))
+#
+# print(do_md5())
+# print(do_md5())
+# print(do_md5('yangpu'))
+# print(do_md5('yangpu12'))
+#
+# log_msg = ''
+# headers = {'Content-Type': 'application/json;charset=utf-8'}
+# data = {}
+# data['merchantId'] = "merchantId"
+# data['currency'] = "IDR"
+# data['accType'] = "payout"
+# data['version'] = "1.0"
+# sign = sort_by_json_key(data)
+# print(sign)
+# hash = hashlib.sha256()
+# hash.update(sign.encode('utf-8'))
+# data['sign'] = hash.hexdigest()
+#
+# print(data)
```

### Comparing `yplib-0.2.2/yplib/line_stack_temp.py` & `yplib-0.2.3/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.2/yplib.egg-info/PKG-INFO` & `yplib-0.2.3/yplib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.2
+Version: 0.2.3
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

