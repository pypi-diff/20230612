# Comparing `tmp/yplib-0.2.0.tar.gz` & `tmp/yplib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.2.0.tar", last modified: Mon Jun 12 01:20:45 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.1.tar", last modified: Mon Jun 12 02:00:51 2023, max compression
```

## Comparing `yplib-0.2.0.tar` & `yplib-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 01:20:45.593160 yplib-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-12 01:20:45.592717 yplib-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 01:20:45.593160 yplib-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-12 01:18:40.000000 yplib-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 01:20:45.588903 yplib-0.2.0/yplib/
--rw-rw-rw-   0        0        0    11653 2023-06-12 01:18:04.000000 yplib-0.2.0/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.0/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 01:20:45.591516 yplib-0.2.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 01:20:45.000000 yplib-0.2.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:51.247445 yplib-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-12 02:00:51.246943 yplib-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 02:00:51.247944 yplib-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-12 02:00:27.000000 yplib-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:51.242162 yplib-0.2.1/yplib/
+-rw-rw-rw-   0        0        0    12346 2023-06-12 01:59:50.000000 yplib-0.2.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.1/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:00:51.245912 yplib-0.2.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 02:00:51.000000 yplib-0.2.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.2.0/LICENSE` & `yplib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.2.0/PKG-INFO` & `yplib-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.0
+Version: 0.2.1
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.2.0/setup.py` & `yplib-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.2.0",
+  version="0.2.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.2.0/yplib/__init__.py` & `yplib-0.2.1/yplib/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import xlwt
 import re
 # import random
 from yplib.line_stack_temp import line_stack_temp_html
 
 
 # 记录日志, 如果是对象会转化为 json
-def log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
-        a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
+def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+           a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10,
          a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ''
     for one in l:
         if can_use_json(one):
             o = json.dumps(one)
         else:
@@ -27,25 +27,25 @@
             d = d + ' ' + o
     lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + d
     print(lo)
     return lo
 
 
 # 将 log 数据, 写入到文件
-def log_to_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+def to_log_file(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                 a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
-    lo = log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    list_to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True)
+    lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
+    to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True)
 
 
 # 将 log 数据, 写入到固定文件中
-def log_to_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
+def to_log_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
-    lo = log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    list_to_txt([lo], file_name, 'log', True)
+    lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
+    to_txt([lo], file_name, 'txt', True)
 
 
 # 将下划线命名转成驼峰命名
 # 例如 : user_id -> userId
 # 例如 : USER_ID -> userId
 def to_hump(a1=''):
     if a1 == '':
@@ -113,38 +113,53 @@
         os.mkdir(file_name)
 
 
 # 获得文件名称
 def get_file_name(file_name, suffix='.txt'):
     return str(file_name) \
         + '_' + datetime.today().strftime('%Y%m%d_%H%M%S') \
-        + '_' + str(uuid.uuid4().hex).replace('-', '')[0:5] \
+        + '_' + uuid_random()[0:5] \
         + suffix
 
 
+def uuid_random(length=32):
+    r = uuid.uuid4().hex
+    while len(r) < length:
+        r += uuid.uuid4().hex
+    return r[0:length]
+
+
 # 去掉 str 中的 非数字字符, 然后, 再转化为 int
-def str_to_int(s):
+def to_int(s):
     if s is None or s == '':
         return 0
-    return int(''.join(filter(lambda ch: ch in '0123456789', s)))
+    if isinstance(s, float):
+        return int(s)
+    s = ''.join(filter(lambda ch: ch in '0123456789', str(s)))
+    if s == '':
+        return 0
+    return int(s)
 
 
 # 去掉 str 中的 非数字字符, 然后, 再转化为 float
-def str_to_float(s):
+def to_float(s):
     if s is None or s == '':
         return 0.0
-    return float(''.join(filter(lambda ch: ch in '0123456789.', s)))
+    s = ''.join(filter(lambda ch: ch in '0123456789.', str(s)))
+    if s == '':
+        return 0.0
+    return float(s)
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # list_data : 数组数据
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
-def list_to_txt(list_data, file_name, file_path='data', fixed_name=False, suffix='.txt'):
+def to_txt(list_data, file_name, file_path='data', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     if fixed_name:
         file_name = file_name + suffix
     else:
@@ -160,29 +175,41 @@
             s = str(one)
         text_file.write(s + '\n')
     text_file.close()
     return file_name_path
 
 
 # 将 list 中的数据写入到固定的文件中,自己设置文件后缀
-def list_to_txt_fixed_file_name(list_data, file_name):
-    return list_to_txt(list_data, file_name, '', True)
+def to_txt_file_name(list_data, file_name):
+    return to_txt(list_data, file_name, '', True)
 
 
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前,行后的空格
-def txt_to_list(file_name):
+def to_list(file_name='a.txt', sheet_index=0):
+    data_list = list()
+    # excel 表格解析成 list 数据
+    if file_name.endswith('.xls') or file_name.endswith('.xlsx'):
+        book = xlrd.open_workbook(file_name)  # 打开一个excel
+        sheet = book.sheet_by_index(sheet_index)  # 根据顺序获取sheet
+        for i in range(sheet.nrows):  # 0 1 2 3 4 5
+            rows = sheet.row_values(i)
+            row_data = []
+            for j in range(len(rows)):
+                row_data.append(str(rows[j]).strip())
+            data_list.append(row_data)
+        return data_list
+    # 普通文件的解析
     file = open(file_name, 'r', encoding='utf-8')
-    data_all = list()
     for line in file.readlines():
         line = line.strip()
-        data_all.append(line)
-    return data_all
+        data_list.append(line)
+    return data_list
 
 
-def list_to_excel(list_data, file_name, file_path='data'):
+def to_excel(list_data, file_name, file_path='excel'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     # 2. 创建Excel工作薄
     myWorkbook = xlwt.Workbook()
     # 3. 添加Excel工作表
@@ -209,28 +236,14 @@
             mySheet.write(m, n, s)  # 写入A3，数值等于1
         m += 1
     # 5. 保存
     # myWorkbook.save('5002200.xls')
     myWorkbook.save(file_path + '/' + get_file_name(file_name, '.xls'))
 
 
-# 将 excel 文件读取到 list 中, 单元格中的空格自动过滤掉了
-def excel_to_list(file_name, sheet_index=0):
-    book = xlrd.open_workbook(file_name)  # 打开一个excel
-    sheet = book.sheet_by_index(sheet_index)  # 根据顺序获取sheet
-    data_list = list()
-    for i in range(sheet.nrows):  # 0 1 2 3 4 5
-        rows = sheet.row_values(i)
-        row_data = []
-        for j in range(len(rows)):
-            row_data.append(str(rows[j]).strip())
-        data_list.append(row_data)
-    return data_list
-
-
 # 将数据整理成折线图
 # x轴数据 : x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y轴数据 : y_list = [
 #             {
 #                 name: 'Email',
 #                 selected: False,
 #                 data: [120, 132, 101, 134, 90, 230, 210],
@@ -267,19 +280,19 @@
     legend_selected = {}
     for y_one in y_list:
         legend_data.append(y_one['name'])
         if 'selected' in y_one:
             legend_selected[y_one['name']] = 'false'
     legend = "data : " + str(legend_data) + ", selected : " + str(legend_selected)
     # {
-    #                 name: 'Email',
-    #                 type: 'line',
-    #                 stack: 'Total',
-    #                 data: [120, 132, 101, 134, 90, 230, 210],
-    #             }
+    #     name: 'Email',
+    #     type: 'line',
+    #     stack: 'Total',
+    #     data: [120, 132, 101, 134, 90, 230, 210],
+    # }
     series = []
     for y_one in y_list:
         y_one['type'] = 'line'
         y_one['stack'] = 'Total'
         series.append(y_one)
 
     one_line = html_list_one
@@ -289,36 +302,38 @@
         # ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
         one_line = one_line.replace(x_list_html, str(x_list))
     if legend_html in one_line:
         one_line = one_line.replace(legend_html, str(legend))
     if series_html in one_line:
         one_line = one_line.replace(series_html, str(series))
     r_list.append(one_line)
-    list_to_txt(r_list, str(chart_name), 'html', False, '.html')
+    to_txt(r_list, str(chart_name), 'html', False, '.html')
+
 
-# list_to_txt([1,2,3], 'p')
-# list_to_txt_fixed_file_name([1,2,3], 'p')
+# to_txt([1,2,3], 'p')
+# to_txt_file_name([1,2,3], 'p')
 #
 #
-# li = txt_to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230609_081711_78ff6.txt')
+# li = to_list('D:\code\python3\packaging_tutorial\yplib\data\p_20230612_095450_34779.txt')
 #
-# print(log())
+# to_log()
 #
-# log()
-# log(1)
-# log(1, 2)
-# log(1, 2, [1, 2])
-# log(1, 2, [{'a': 2}])
+# to_log()
+# to_log(1)
+# to_log(1, 2)
+# to_log(1, 2, [1, 2])
+# to_log_file(1, 2, [{'a': 2}])
+# to_log_txt('1.txt', 1, 2, [{'a': 2}])
 #
 # x_list = ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
 # y_list = json.loads(
 #     '[{"name":"Email","data":[120,132,101,134,90,230,210]},{"name":"Union Ads","data":[220,182,191,234,290,330,310]},{"name":"Video Ads","data":[150,232,201,154,190,330,410]},{"name":"Direct","data":[320,332,301,334,390,330,320]},{"name":"Search Engine","data":[820,932,901,934,1290,1330,1320]}]')
 #
 
-#
+# 将 list 转化成 图表的例子
 # x_list = []
 # y_list = []
 # # x 轴有 100 个
 # # 100 个横坐标
 # for i in range(100):
 #     x_list.append(i)
 #
@@ -349,7 +364,28 @@
 # print(to_hump('userId'))
 # print(to_hump('user'))
 # print(to_hump(''))
 
 # print(to_hump_more('userId'))
 
 # print(to_underline('userId'))
+
+
+# print(uuid_random(5))
+# print(uuid_random(10))
+# print(uuid_random())
+# print(uuid_random(32))
+# print(uuid_random(64))
+# print(uuid_random(128))
+# print(uuid_random(127))
+# print(uuid_random(129))
+
+
+# print(to_int('a'))
+# print(to_int(2))
+# print(to_int(2.2))
+# print(to_int(2.2))
+
+# print(to_float('a'))
+# print(to_float(2))
+# print(to_float(2.2))
+# print(to_float(2.24))
```

### Comparing `yplib-0.2.0/yplib/line_stack_temp.py` & `yplib-0.2.1/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.0/yplib.egg-info/PKG-INFO` & `yplib-0.2.1/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.0
+Version: 0.2.1
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

