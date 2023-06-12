# Comparing `tmp/yplib-0.2.3.tar.gz` & `tmp/yplib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.2.3.tar", last modified: Mon Jun 12 07:43:57 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.4.tar", last modified: Mon Jun 12 07:50:36 2023, max compression
```

## Comparing `yplib-0.2.3.tar` & `yplib-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:43:57.443023 yplib-0.2.3/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-12 07:43:57.442676 yplib-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 07:43:57.443446 yplib-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-12 07:43:39.000000 yplib-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:43:57.439447 yplib-0.2.3/yplib/
--rw-rw-rw-   0        0        0    15364 2023-06-12 07:42:15.000000 yplib-0.2.3/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.3/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:43:57.441917 yplib-0.2.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 07:43:57.000000 yplib-0.2.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 07:50:36.944774 yplib-0.2.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-12 07:50:36.944774 yplib-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:50:36.944774 yplib-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-12 07:50:15.000000 yplib-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:50:36.941955 yplib-0.2.4/yplib/
+-rw-rw-rw-   0        0        0    15370 2023-06-12 07:49:32.000000 yplib-0.2.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.4/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:50:36.944774 yplib-0.2.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 07:50:36.000000 yplib-0.2.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.2.3/LICENSE` & `yplib-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.2.3/PKG-INFO` & `yplib-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.3
+Version: 0.2.4
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.2.3/setup.py` & `yplib-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.2.3",
+  version="0.2.4",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.2.3/yplib/__init__.py` & `yplib-0.2.4/yplib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     to_txt([lo], datetime.today().strftime('%Y-%m-%d'), 'log', True)
 
 
 # 将 log 数据, 写入到固定文件中
 def to_log_txt(file_name, a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
                a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20=''):
     lo = to_log(a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20)
-    to_txt([lo], file_name, 'txt', True)
+    to_txt([lo], file_name, 'log', True)
 
 
 # 将下划线命名转成驼峰命名
 # 例如 : user_id -> userId
 # 例如 : USER_ID -> userId
 def to_hump(a1=''):
     if a1 == '':
@@ -195,15 +195,15 @@
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # list_data : 数组数据, 也可以不是数组
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
-def to_txt(list_data, file_name='data', file_path='txt', fixed_name=False, suffix='.txt'):
+def to_txt(list_data, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     if fixed_name:
         file_name = file_name + suffix
     else:
@@ -218,15 +218,15 @@
         for one in list_data:
             text_file.write(to_str(one) + '\n')
     text_file.close()
     return file_name_path
 
 
 # 将 list 中的数据写入到固定的文件中,自己设置文件后缀
-def to_txt_data(list_data, file_name):
+def to_txt_data(list_data, file_name='data'):
     return to_txt(list_data, file_name, 'data', True)
 
 
 def to_str(data):
     if can_use_json(data):
         s = json.dumps(data)
     else:
```

### Comparing `yplib-0.2.3/yplib/line_stack_temp.py` & `yplib-0.2.4/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.3/yplib.egg-info/PKG-INFO` & `yplib-0.2.4/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.3
+Version: 0.2.4
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

