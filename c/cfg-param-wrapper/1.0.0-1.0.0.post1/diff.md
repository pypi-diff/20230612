# Comparing `tmp/cfg-param-wrapper-1.0.0.tar.gz` & `tmp/cfg-param-wrapper-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-param-wrapper-1.0.0.tar", last modified: Sun Jun 11 22:35:30 2023, max compression
+gzip compressed data, was "cfg-param-wrapper-1.0.0.post1.tar", last modified: Sun Jun 11 22:38:01 2023, max compression
```

## Comparing `cfg-param-wrapper-1.0.0.tar` & `cfg-param-wrapper-1.0.0.post1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:35:30.208790 cfg-param-wrapper-1.0.0/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-param-wrapper-1.0.0/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1736 2023-06-11 22:35:30.208790 cfg-param-wrapper-1.0.0/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      877 2023-06-11 22:34:05.000000 cfg-param-wrapper-1.0.0/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      984 2023-06-11 22:34:17.000000 cfg-param-wrapper-1.0.0/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-11 22:35:30.208790 cfg-param-wrapper-1.0.0/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:35:30.208790 cfg-param-wrapper-1.0.0/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:35:30.208790 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/argparse_config.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2888 2023-06-11 22:35:08.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/cfg_dict.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2263 2023-06-11 22:35:07.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/function_config_wrapper.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 18:09:29.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/save_handlers.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:35:30.208790 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1736 2023-06-11 22:35:30.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      453 2023-06-11 22:35:30.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-11 22:35:30.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-11 22:35:30.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper.egg-info/requires.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       18 2023-06-11 22:35:30.000000 cfg-param-wrapper-1.0.0/src/cfg_param_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-param-wrapper-1.0.0.post1/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1585 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      746 2023-06-11 22:36:59.000000 cfg-param-wrapper-1.0.0.post1/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      959 2023-06-11 22:37:48.000000 cfg-param-wrapper-1.0.0.post1/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/argparse_config.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2888 2023-06-11 22:35:08.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/cfg_dict.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2263 2023-06-11 22:35:07.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/function_config_wrapper.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 18:09:29.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/save_handlers.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-11 22:38:01.124001 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1585 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      453 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/requires.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       18 2023-06-11 22:38:01.000000 cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/top_level.txt
```

### Comparing `cfg-param-wrapper-1.0.0/LICENSE` & `cfg-param-wrapper-1.0.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0/PKG-INFO` & `cfg-param-wrapper-1.0.0.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cfg-param-wrapper
-Version: 1.0.0
-Summary: A package designed to simplify configurable defaults from argparse.
+Version: 1.0.0.post1
+Summary: A package designed to simplify defaults.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
 ## Installation
 
 ```bash
 # from pypi:
-pip install cfg-argparser
+pip install cfg-param-wrapper
 
 # from github:
-git clone "https://github.com/zeptofine/cfg-argparser"
-cd cfg-argparser
+git clone "https://github.com/zeptofine/cfg-param-wrapper"
+cd cfg-param-wrapper
 pip install -e .
 
 ```
 
 ## Example
 
 ```python
@@ -46,11 +46,7 @@
     return f"{s} is {'real' if is_real else 'fake'}"
 
 if __name__ == "__main__":
   print(test_function("We"))
   cfg['s'] = "us"
   print(test_function()) # Linters hate him!
 ```
-
-## Compatibilty
-
-This was mainly tested on 3.9 and 3.10, but it should work from 3.6 onwards. i can't test earlier versions for some reason.
```

### Comparing `cfg-param-wrapper-1.0.0/README.md` & `cfg-param-wrapper-1.0.0.post1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
 ## Installation
 
 ```bash
 # from pypi:
-pip install cfg-argparser
+pip install cfg-param-wrapper
 
 # from github:
-git clone "https://github.com/zeptofine/cfg-argparser"
-cd cfg-argparser
+git clone "https://github.com/zeptofine/cfg-param-wrapper"
+cd cfg-param-wrapper
 pip install -e .
 
 ```
 
 ## Example
 
 ```python
@@ -25,12 +25,8 @@
 def test_function(s: str, is_real: bool = True): # I'd advise only wrapping functions all having default methods
     return f"{s} is {'real' if is_real else 'fake'}"
 
 if __name__ == "__main__":
   print(test_function("We"))
   cfg['s'] = "us"
   print(test_function()) # Linters hate him!
-```
-
-## Compatibilty
-
-This was mainly tested on 3.9 and 3.10, but it should work from 3.6 onwards. i can't test earlier versions for some reason.
+```
```

### Comparing `cfg-param-wrapper-1.0.0/pyproject.toml` & `cfg-param-wrapper-1.0.0.post1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-param-wrapper"
-version = "1.0.0"
+version = "1.0.0-1"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
-description = "A package designed to simplify configurable defaults from argparse."
+description = "A package designed to simplify defaults."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/argparse_config.py` & `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/argparse_config.py`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/cfg_dict.py` & `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/cfg_dict.py`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/function_config_wrapper.py` & `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/function_config_wrapper.py`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0/src/cfg_param_wrapper/save_handlers.py` & `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper/save_handlers.py`

 * *Files identical despite different names*

### Comparing `cfg-param-wrapper-1.0.0/src/cfg_param_wrapper.egg-info/PKG-INFO` & `cfg-param-wrapper-1.0.0.post1/src/cfg_param_wrapper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cfg-param-wrapper
-Version: 1.0.0
-Summary: A package designed to simplify configurable defaults from argparse.
+Version: 1.0.0.post1
+Summary: A package designed to simplify defaults.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 
 a config wrapper I made. It's made to wrap simple functions, and intercept configurations in tandem with a CfgDict object.
 
 ## Installation
 
 ```bash
 # from pypi:
-pip install cfg-argparser
+pip install cfg-param-wrapper
 
 # from github:
-git clone "https://github.com/zeptofine/cfg-argparser"
-cd cfg-argparser
+git clone "https://github.com/zeptofine/cfg-param-wrapper"
+cd cfg-param-wrapper
 pip install -e .
 
 ```
 
 ## Example
 
 ```python
@@ -46,11 +46,7 @@
     return f"{s} is {'real' if is_real else 'fake'}"
 
 if __name__ == "__main__":
   print(test_function("We"))
   cfg['s'] = "us"
   print(test_function()) # Linters hate him!
 ```
-
-## Compatibilty
-
-This was mainly tested on 3.9 and 3.10, but it should work from 3.6 onwards. i can't test earlier versions for some reason.
```

