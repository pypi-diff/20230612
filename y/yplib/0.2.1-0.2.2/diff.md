# Comparing `tmp/yplib-0.2.1.tar.gz` & `tmp/yplib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.2.1.tar", last modified: Mon Jun 12 02:00:51 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.2.tar", last modified: Mon Jun 12 07:06:00 2023, max compression
```

## Comparing `yplib-0.2.1.tar` & `yplib-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 02:00:51.247445 yplib-0.2.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-12 02:00:51.246943 yplib-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 02:00:51.247944 yplib-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-12 02:00:27.000000 yplib-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:00:51.242162 yplib-0.2.1/yplib/
--rw-rw-rw-   0        0        0    12346 2023-06-12 01:59:50.000000 yplib-0.2.1/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.1/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:00:51.245912 yplib-0.2.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 07:06:00.828449 yplib-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-12 07:06:00.828137 yplib-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:06:00.828449 yplib-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-12 07:05:48.000000 yplib-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:06:00.825281 yplib-0.2.2/yplib/
+-rw-rw-rw-   0        0        0    14292 2023-06-12 07:04:18.000000 yplib-0.2.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.2/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:06:00.827239 yplib-0.2.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 07:06:00.000000 yplib-0.2.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.2.1/LICENSE` & `yplib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.2.1/PKG-INFO` & `yplib-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.1
+Version: 0.2.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.2.1/setup.py` & `yplib-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.2.1",
+  version="0.2.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.2.1/yplib/__init__.py` & `yplib-0.2.2/yplib/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import os
 import uuid
 from datetime import datetime
 
 import xlrd
 import xlwt
+import time
 import re
 # import random
 from yplib.line_stack_temp import line_stack_temp_html
 
 
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
@@ -146,45 +147,84 @@
         return 0.0
     s = ''.join(filter(lambda ch: ch in '0123456789.', str(s)))
     if s == '':
         return 0.0
     return float(s)
 
 
+def to_datetime(s=None, return_str=False):
+    if s is None or s == '':
+        return datetime.today()
+    s = str(s)
+    r = datetime.today()
+    if re.match("^\\d{4}$", s):
+        r = datetime.strptime(s, "%Y")
+    if re.match("^\\d{4}-\\d{1,2}$", s):
+        r = datetime.strptime(s, "%Y-%m")
+    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2}$", s):
+        r = datetime.strptime(s, "%Y-%m-%d")
+    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}$", s):
+        r = datetime.strptime(s, "%Y-%m-%d %H")
+    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}$", s):
+        r = datetime.strptime(s, "%Y-%m-%d %H:%M")
+    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}:\\d{1,2}$", s):
+        r = datetime.strptime(s, "%Y-%m-%d %H:%M:%S")
+    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}:\\d{1,2}.\\d{1,9}$", s):
+        r = datetime.strptime(s.split('.')[0], "%Y-%m-%d %H:%M:%S")
+    if re.match("^\\d{1,13}$", s):
+        s_int = int(s)
+        if len(s) > 10:
+            s_int = int(s_int / 1000)
+        time_arr = time.localtime(s_int)
+        time_str = time.strftime("%Y-%m-%d %H:%M:%S", time_arr)
+        r = datetime.strptime(time_str, "%Y-%m-%d %H:%M:%S")
+
+    if return_str:
+        return str(r)
+    return r
+
+
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
-# list_data : 数组数据
+# list_data : 数组数据, 也可以不是数组
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
-def to_txt(list_data, file_name, file_path='data', fixed_name=False, suffix='.txt'):
+def to_txt(list_data, file_name='data', file_path='txt', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     if fixed_name:
         file_name = file_name + suffix
     else:
         file_name = get_file_name(file_name, suffix)
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
     text_file = open(file_name_path, 'a', encoding='utf-8')
-    for one in list_data:
-        if can_use_json(one):
-            s = json.dumps(one)
-        else:
-            s = str(one)
-        text_file.write(s + '\n')
+    if isinstance(list_data, list) is False:
+        text_file.write(to_str(list_data) + '\n')
+    else:
+        for one in list_data:
+            text_file.write(to_str(one) + '\n')
     text_file.close()
     return file_name_path
 
 
 # 将 list 中的数据写入到固定的文件中,自己设置文件后缀
-def to_txt_file_name(list_data, file_name):
-    return to_txt(list_data, file_name, '', True)
+def to_txt_data(list_data, file_name):
+    return to_txt(list_data, file_name, 'data', True)
+
+
+def to_str(data):
+    if can_use_json(data):
+        s = json.dumps(data)
+    else:
+        s = str(data)
+    return s
 
 
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前,行后的空格
 def to_list(file_name='a.txt', sheet_index=0):
     data_list = list()
     # excel 表格解析成 list 数据
     if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
@@ -304,29 +344,32 @@
     if legend_html in one_line:
         one_line = one_line.replace(legend_html, str(legend))
     if series_html in one_line:
         one_line = one_line.replace(series_html, str(series))
     r_list.append(one_line)
     to_txt(r_list, str(chart_name), 'html', False, '.html')
 
-
 # to_txt([1,2,3], 'p')
 # to_txt_file_name([1,2,3], 'p')
 #
 #
 # li = to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230612_095450_34779.txt')
 #
 # to_log()
 #
 # to_log()
 # to_log(1)
 # to_log(1, 2)
 # to_log(1, 2, [1, 2])
 # to_log_file(1, 2, [{'a': 2}])
 # to_log_txt('1.txt', 1, 2, [{'a': 2}])
+# to_txt([{'a': 2}])
+# to_txt_data('yangpu', 1)
+# to_txt_data('yangpu1', 1)
+# to_txt_data('yangpu12', 1)
 #
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 
 # 将 list 转化成 图表的例子
@@ -385,7 +428,17 @@
 # print(to_int(2.2))
 # print(to_int(2.2))
 
 # print(to_float('a'))
 # print(to_float(2))
 # print(to_float(2.2))
 # print(to_float(2.24))
+
+# print(to_datetime('2019-09'))
+# print(to_datetime('2019-09-08'))
+# print(to_datetime('2019-09-08 12'))
+# print(to_datetime('2019-09-08 12:13'))
+# print(to_datetime('2019-09-08 12:13:14'))
+# print(to_datetime('2019-09-08 12:13:14.789'))
+# print(to_datetime(1686537485))
+# print(to_datetime(1686537484467))
+# print(to_datetime(datetime.today()))
```

### Comparing `yplib-0.2.1/yplib/line_stack_temp.py` & `yplib-0.2.2/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.1/yplib.egg-info/PKG-INFO` & `yplib-0.2.2/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.1
+Version: 0.2.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

