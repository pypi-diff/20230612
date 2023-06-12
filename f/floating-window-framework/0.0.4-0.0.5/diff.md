# Comparing `tmp/floating-window-framework-0.0.4.tar.gz` & `tmp/floating-window-framework-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floating-window-framework-0.0.4.tar", last modified: Mon Jun 12 11:07:48 2023, max compression
+gzip compressed data, was "floating-window-framework-0.0.5.tar", last modified: Mon Jun 12 11:11:32 2023, max compression
```

## Comparing `floating-window-framework-0.0.4.tar` & `floating-window-framework-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/
--rw-r--r--   0 attai     (1000) attai     (1000)     1070 2023-06-12 10:09:18.000000 floating-window-framework-0.0.4/LICENSE
--rw-r--r--   0 attai     (1000) attai     (1000)     3554 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/PKG-INFO
--rw-r--r--   0 attai     (1000) attai     (1000)     3046 2023-06-12 11:05:54.000000 floating-window-framework-0.0.4/README.md
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/floating_window_framework.egg-info/
--rw-r--r--   0 attai     (1000) attai     (1000)     3554 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/PKG-INFO
--rw-r--r--   0 attai     (1000) attai     (1000)      348 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/SOURCES.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        1 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/dependency_links.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        8 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/requires.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        4 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/top_level.txt
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/fwf/
--rw-r--r--   0 attai     (1000) attai     (1000)      115 2023-06-12 10:35:10.000000 floating-window-framework-0.0.4/fwf/__init__.py
--rw-r--r--   0 attai     (1000) attai     (1000)     1787 2023-06-12 10:36:50.000000 floating-window-framework-0.0.4/fwf/base_app.py
--rw-r--r--   0 attai     (1000) attai     (1000)     2407 2023-06-12 10:34:21.000000 floating-window-framework-0.0.4/fwf/component.py
--rw-r--r--   0 attai     (1000) attai     (1000)      527 2023-06-12 10:34:19.000000 floating-window-framework-0.0.4/fwf/keybindings.py
--rw-r--r--   0 attai     (1000) attai     (1000)       79 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/setup.cfg
--rw-r--r--   0 attai     (1000) attai     (1000)      905 2023-06-12 11:05:49.000000 floating-window-framework-0.0.4/setup.py
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:11:32.722403 floating-window-framework-0.0.5/
+-rw-r--r--   0 attai     (1000) attai     (1000)     1070 2023-06-12 10:09:18.000000 floating-window-framework-0.0.5/LICENSE
+-rw-r--r--   0 attai     (1000) attai     (1000)     3590 2023-06-12 11:11:32.722403 floating-window-framework-0.0.5/PKG-INFO
+-rw-r--r--   0 attai     (1000) attai     (1000)     3082 2023-06-12 11:10:09.000000 floating-window-framework-0.0.5/README.md
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:11:32.722403 floating-window-framework-0.0.5/floating_window_framework.egg-info/
+-rw-r--r--   0 attai     (1000) attai     (1000)     3590 2023-06-12 11:11:32.000000 floating-window-framework-0.0.5/floating_window_framework.egg-info/PKG-INFO
+-rw-r--r--   0 attai     (1000) attai     (1000)      348 2023-06-12 11:11:32.000000 floating-window-framework-0.0.5/floating_window_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        1 2023-06-12 11:11:32.000000 floating-window-framework-0.0.5/floating_window_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        8 2023-06-12 11:11:32.000000 floating-window-framework-0.0.5/floating_window_framework.egg-info/requires.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        4 2023-06-12 11:11:32.000000 floating-window-framework-0.0.5/floating_window_framework.egg-info/top_level.txt
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:11:32.722403 floating-window-framework-0.0.5/fwf/
+-rw-r--r--   0 attai     (1000) attai     (1000)      115 2023-06-12 10:35:10.000000 floating-window-framework-0.0.5/fwf/__init__.py
+-rw-r--r--   0 attai     (1000) attai     (1000)     1787 2023-06-12 10:36:50.000000 floating-window-framework-0.0.5/fwf/base_app.py
+-rw-r--r--   0 attai     (1000) attai     (1000)     2407 2023-06-12 10:34:21.000000 floating-window-framework-0.0.5/fwf/component.py
+-rw-r--r--   0 attai     (1000) attai     (1000)      527 2023-06-12 10:34:19.000000 floating-window-framework-0.0.5/fwf/keybindings.py
+-rw-r--r--   0 attai     (1000) attai     (1000)       79 2023-06-12 11:11:32.722403 floating-window-framework-0.0.5/setup.cfg
+-rw-r--r--   0 attai     (1000) attai     (1000)      905 2023-06-12 11:11:32.000000 floating-window-framework-0.0.5/setup.py
```

### Comparing `floating-window-framework-0.0.4/LICENSE` & `floating-window-framework-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.4/PKG-INFO` & `floating-window-framework-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floating-window-framework
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for building floating window applications.
 Home-page: https://github.com/youssef-attai/fwf
 Author: Youssef Atta'i
 Author-email: youssefgalalnazem@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -45,14 +45,15 @@
 4. Override the `setup_keybindings` method to add your custom keybindings:
    ```python
    class YourCustomApp(BaseApp):
     def __init__(self):
         super().__init__()
 
     def setup_keybindings(self):
+        super().setup_keybindings()
         self.keybindings.add('h', self.hello)
 
     def hello(self):
         print("Hello, World!")
    ```
 
 5. Run your application by instantiating your subclass and calling the `run()` method:
```

### Comparing `floating-window-framework-0.0.4/README.md` & `floating-window-framework-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 4. Override the `setup_keybindings` method to add your custom keybindings:
    ```python
    class YourCustomApp(BaseApp):
     def __init__(self):
         super().__init__()
 
     def setup_keybindings(self):
+        super().setup_keybindings()
         self.keybindings.add('h', self.hello)
 
     def hello(self):
         print("Hello, World!")
    ```
 
 5. Run your application by instantiating your subclass and calling the `run()` method:
```

### Comparing `floating-window-framework-0.0.4/floating_window_framework.egg-info/PKG-INFO` & `floating-window-framework-0.0.5/floating_window_framework.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floating-window-framework
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for building floating window applications.
 Home-page: https://github.com/youssef-attai/fwf
 Author: Youssef Atta'i
 Author-email: youssefgalalnazem@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -45,14 +45,15 @@
 4. Override the `setup_keybindings` method to add your custom keybindings:
    ```python
    class YourCustomApp(BaseApp):
     def __init__(self):
         super().__init__()
 
     def setup_keybindings(self):
+        super().setup_keybindings()
         self.keybindings.add('h', self.hello)
 
     def hello(self):
         print("Hello, World!")
    ```
 
 5. Run your application by instantiating your subclass and calling the `run()` method:
```

### Comparing `floating-window-framework-0.0.4/fwf/base_app.py` & `floating-window-framework-0.0.5/fwf/base_app.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.4/fwf/component.py` & `floating-window-framework-0.0.5/fwf/component.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.4/fwf/keybindings.py` & `floating-window-framework-0.0.5/fwf/keybindings.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.4/setup.py` & `floating-window-framework-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='floating-window-framework',
-    version='0.0.4',
+    version='0.0.5',
     description='A framework for building floating window applications.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Youssef Atta'i",
     author_email='youssefgalalnazem@gmail.com',
     url='https://github.com/youssef-attai/fwf',
     packages=['fwf'],
```

