# Comparing `tmp/baysalt_christmas-0.1.7.6.tar.gz` & `tmp/baysalt_christmas-0.1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.6.tar", last modified: Thu Jun  8 02:22:41 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.7.tar", last modified: Mon Jun 12 03:13:47 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.6.tar` & `baysalt_christmas-0.1.7.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.559088 baysalt_christmas-0.1.7.6/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.6/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.6/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-08 02:22:41.558935 baysalt_christmas-0.1.7.6/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.6/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.548994 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.552525 baysalt_christmas-0.1.7.6/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.7.6/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.6/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.6/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.6/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.6/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.557653 baysalt_christmas-0.1.7.6/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.558569 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.6/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.6/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.6/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.6/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-08 02:22:41.559146 baysalt_christmas-0.1.7.6/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-08 02:22:36.000000 baysalt_christmas-0.1.7.6/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.331713 baysalt_christmas-0.1.7.7/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.7/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.7/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-12 03:13:47.331570 baysalt_christmas-0.1.7.7/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.7/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.327005 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-12 03:13:47.000000 baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.328921 baysalt_christmas-0.1.7.7/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.7.7/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.7/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.7/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.7/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.7/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.330181 baysalt_christmas-0.1.7.7/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-12 03:13:47.331207 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.7/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.7/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.7.7/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.7/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.7/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-12 03:13:47.331772 baysalt_christmas-0.1.7.7/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-12 03:13:42.000000 baysalt_christmas-0.1.7.7/setup.py
```

### Comparing `baysalt_christmas-0.1.7.6/.DS_Store` & `baysalt_christmas-0.1.7.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/PKG-INFO` & `baysalt_christmas-0.1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.6
+Version: 0.1.7.7
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.6/README.md` & `baysalt_christmas-0.1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.6
+Version: 0.1.7.7
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.7/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/Blogging.py` & `baysalt_christmas-0.1.7.7/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.7/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/commonCode.py` & `baysalt_christmas-0.1.7.7/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/cprintf.py` & `baysalt_christmas-0.1.7.7/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.7/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.7/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.7/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.7/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.7/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/processBar.py` & `baysalt_christmas-0.1.7.7/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/christmas/read_conf.py` & `baysalt_christmas-0.1.7.7/christmas/read_conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 			# 去除空格和注释
 			line = line.strip()
 			if line.startswith('#'):
 				continue
 			if line == '':
 				continue
 
-			key, value = line.split('=')
+			key, value = line.split('=', maxsplit=1)
 			key = key.strip()
 			value = value.strip()
 			value = value.split('#')[0].strip().strip("'").strip('"')
 			value = split_path(value)
 			[key, value] = char_fill_dic(key, value)
 			if value == '':
 				value = None
@@ -64,28 +64,32 @@
 		_str = [x for x in _str if x.strip()]
 		try:
 			for i in range(len(_str)):
 				if is_number(_str[i]):
 					_str[i] = float(_str[i])
 				else:
 					tmp_1 = _str[i].strip().split(':')
-					_str[i] = np.arange(float(tmp_1[0]), float(tmp_1[2]) + float(tmp_1[1]), float(tmp_1[1])).tolist()
+					_str[i] = np.arange(float(tmp_1[0]), float(tmp_1[2]) + float(tmp_1[1]), float(tmp_1[1])).tolist() # [1:1,120]
 			_str = flatten_list(_str, [])
 
 		except ValueError:
 			try:
 				if type(_str[0]) == str:
 					_str = [_str[i].replace('[', '').replace(']', '').split() for i in range(len(_str))]
 					with contextlib.suppress(ValueError):
 						_str = [float(x) for _str in _str for x in _str]  # ['1', '2', '3'] -> [1, 2, 3]
 					with contextlib.suppress(TypeError):
 						_str = [x.strip("'").strip('"') for _str in _str for x in _str]  # [["'hs'"], ["'t02'"]] -> ['hs', 't02']
 			except IndexError:
 				for i in range(len(_str)):
 					_str[i] = _str[i].strip().strip("'").strip('"')
+		except IndexError: # [1,120]
+			_str = _str[0].strip().strip("'").strip('"')
+			tmp_1 = _str.split(':')
+			_str = np.arange(float(tmp_1[0]),float(tmp_1[1])+1).tolist() # [1:1,120]
 	elif _str.startswith('{'):
 		# "{'KK' :'sds', 'YY' : 'asd'}" ->  {'KK' :'sds', 'YY' : 'asd'}
 		_str = _str[1:-1].split(',')
 		_str = {i.split(':')[0].strip().strip("'").strip('"'): i.split(':')[1].strip().strip("'").strip('"') for i in _str}
 	elif _str.startswith("'") or _str.startswith('"'):
 		_str = _str.strip().strip("'").strip('"')
 	elif is_number(_str):
```

### Comparing `baysalt_christmas-0.1.7.6/christmas/server_info.py` & `baysalt_christmas-0.1.7.7/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.6/setup.py` & `baysalt_christmas-0.1.7.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.6",
+    version="0.1.7.7",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

