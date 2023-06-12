# Comparing `tmp/floating-window-framework-0.0.3.tar.gz` & `tmp/floating-window-framework-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floating-window-framework-0.0.3.tar", last modified: Mon Jun 12 10:59:10 2023, max compression
+gzip compressed data, was "floating-window-framework-0.0.4.tar", last modified: Mon Jun 12 11:07:48 2023, max compression
```

## Comparing `floating-window-framework-0.0.3.tar` & `floating-window-framework-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:59:10.130823 floating-window-framework-0.0.3/
--rw-r--r--   0 attai     (1000) attai     (1000)     1070 2023-06-12 10:09:18.000000 floating-window-framework-0.0.3/LICENSE
--rw-r--r--   0 attai     (1000) attai     (1000)     3415 2023-06-12 10:59:10.130823 floating-window-framework-0.0.3/PKG-INFO
--rw-r--r--   0 attai     (1000) attai     (1000)     2907 2023-06-12 10:53:42.000000 floating-window-framework-0.0.3/README.md
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:59:10.130823 floating-window-framework-0.0.3/floating_window_framework.egg-info/
--rw-r--r--   0 attai     (1000) attai     (1000)     3415 2023-06-12 10:59:10.000000 floating-window-framework-0.0.3/floating_window_framework.egg-info/PKG-INFO
--rw-r--r--   0 attai     (1000) attai     (1000)      348 2023-06-12 10:59:10.000000 floating-window-framework-0.0.3/floating_window_framework.egg-info/SOURCES.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        1 2023-06-12 10:59:10.000000 floating-window-framework-0.0.3/floating_window_framework.egg-info/dependency_links.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        8 2023-06-12 10:59:10.000000 floating-window-framework-0.0.3/floating_window_framework.egg-info/requires.txt
--rw-r--r--   0 attai     (1000) attai     (1000)        4 2023-06-12 10:59:10.000000 floating-window-framework-0.0.3/floating_window_framework.egg-info/top_level.txt
-drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 10:59:10.130823 floating-window-framework-0.0.3/fwf/
--rw-r--r--   0 attai     (1000) attai     (1000)      115 2023-06-12 10:35:10.000000 floating-window-framework-0.0.3/fwf/__init__.py
--rw-r--r--   0 attai     (1000) attai     (1000)     1787 2023-06-12 10:36:50.000000 floating-window-framework-0.0.3/fwf/base_app.py
--rw-r--r--   0 attai     (1000) attai     (1000)     2407 2023-06-12 10:34:21.000000 floating-window-framework-0.0.3/fwf/component.py
--rw-r--r--   0 attai     (1000) attai     (1000)      527 2023-06-12 10:34:19.000000 floating-window-framework-0.0.3/fwf/keybindings.py
--rw-r--r--   0 attai     (1000) attai     (1000)       79 2023-06-12 10:59:10.134156 floating-window-framework-0.0.3/setup.cfg
--rw-r--r--   0 attai     (1000) attai     (1000)      905 2023-06-12 10:58:26.000000 floating-window-framework-0.0.3/setup.py
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/
+-rw-r--r--   0 attai     (1000) attai     (1000)     1070 2023-06-12 10:09:18.000000 floating-window-framework-0.0.4/LICENSE
+-rw-r--r--   0 attai     (1000) attai     (1000)     3554 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/PKG-INFO
+-rw-r--r--   0 attai     (1000) attai     (1000)     3046 2023-06-12 11:05:54.000000 floating-window-framework-0.0.4/README.md
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/floating_window_framework.egg-info/
+-rw-r--r--   0 attai     (1000) attai     (1000)     3554 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/PKG-INFO
+-rw-r--r--   0 attai     (1000) attai     (1000)      348 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        1 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        8 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/requires.txt
+-rw-r--r--   0 attai     (1000) attai     (1000)        4 2023-06-12 11:07:48.000000 floating-window-framework-0.0.4/floating_window_framework.egg-info/top_level.txt
+drwxr-xr-x   0 attai     (1000) attai     (1000)        0 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/fwf/
+-rw-r--r--   0 attai     (1000) attai     (1000)      115 2023-06-12 10:35:10.000000 floating-window-framework-0.0.4/fwf/__init__.py
+-rw-r--r--   0 attai     (1000) attai     (1000)     1787 2023-06-12 10:36:50.000000 floating-window-framework-0.0.4/fwf/base_app.py
+-rw-r--r--   0 attai     (1000) attai     (1000)     2407 2023-06-12 10:34:21.000000 floating-window-framework-0.0.4/fwf/component.py
+-rw-r--r--   0 attai     (1000) attai     (1000)      527 2023-06-12 10:34:19.000000 floating-window-framework-0.0.4/fwf/keybindings.py
+-rw-r--r--   0 attai     (1000) attai     (1000)       79 2023-06-12 11:07:48.936050 floating-window-framework-0.0.4/setup.cfg
+-rw-r--r--   0 attai     (1000) attai     (1000)      905 2023-06-12 11:05:49.000000 floating-window-framework-0.0.4/setup.py
```

### Comparing `floating-window-framework-0.0.3/LICENSE` & `floating-window-framework-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.3/PKG-INFO` & `floating-window-framework-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: floating-window-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for building floating window applications.
 Home-page: https://github.com/youssef-attai/fwf
 Author: Youssef Atta'i
 Author-email: youssefgalalnazem@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fwf
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/youssef-attai/fwf/blob/main/LICENSE)
 
 fwf (Floating Window Framework) is a powerful Python framework built on top of Tkinter. It allows users to create highly configurable, keyboard-driven graphical user interfaces (GUIs) that are ideal for scratchpad-style applications. With this framework, you can easily build custom alternatives to the scratchpads used with i3 or create your own keyboard-centric applications.
 
 ## Features
 
 - Keyboard-driven: The framework is designed to provide a Vim-like experience, making it highly efficient for keyboard users. It supports customizable keybindings, allowing you to create your own keyboard shortcuts for various actions.
 - Configurability: The framework offers extensive configuration options, enabling you to customize the behavior, appearance, and keybindings of your GUI applications. It provides flexibility to adapt the framework to your specific needs.
@@ -57,17 +57,17 @@
 
 5. Run your application by instantiating your subclass and calling the `run()` method:
    ```python
    app = YourCustomApp()
    app.run()
    ```
 
-For more details and examples, please refer to the [example](./example/) provided.
+For more details and examples, please refer to the [example](https://github.com/youssef-attai/fwf/blob/main/example/) provided.
 
 ## Contributing
 
 Contributions are welcome! If you find any issues, have suggestions, or want to contribute new features or improvements, please feel free to open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/youssef-attai/fwf/blob/main/LICENSE) file for more information.
```

### Comparing `floating-window-framework-0.0.3/README.md` & `floating-window-framework-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # fwf
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/youssef-attai/fwf/blob/main/LICENSE)
 
 fwf (Floating Window Framework) is a powerful Python framework built on top of Tkinter. It allows users to create highly configurable, keyboard-driven graphical user interfaces (GUIs) that are ideal for scratchpad-style applications. With this framework, you can easily build custom alternatives to the scratchpads used with i3 or create your own keyboard-centric applications.
 
 ## Features
 
 - Keyboard-driven: The framework is designed to provide a Vim-like experience, making it highly efficient for keyboard users. It supports customizable keybindings, allowing you to create your own keyboard shortcuts for various actions.
 - Configurability: The framework offers extensive configuration options, enabling you to customize the behavior, appearance, and keybindings of your GUI applications. It provides flexibility to adapt the framework to your specific needs.
@@ -43,17 +43,17 @@
 
 5. Run your application by instantiating your subclass and calling the `run()` method:
    ```python
    app = YourCustomApp()
    app.run()
    ```
 
-For more details and examples, please refer to the [example](./example/) provided.
+For more details and examples, please refer to the [example](https://github.com/youssef-attai/fwf/blob/main/example/) provided.
 
 ## Contributing
 
 Contributions are welcome! If you find any issues, have suggestions, or want to contribute new features or improvements, please feel free to open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/youssef-attai/fwf/blob/main/LICENSE) file for more information.
```

### Comparing `floating-window-framework-0.0.3/floating_window_framework.egg-info/PKG-INFO` & `floating-window-framework-0.0.4/floating_window_framework.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: floating-window-framework
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for building floating window applications.
 Home-page: https://github.com/youssef-attai/fwf
 Author: Youssef Atta'i
 Author-email: youssefgalalnazem@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fwf
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/youssef-attai/fwf/blob/main/LICENSE)
 
 fwf (Floating Window Framework) is a powerful Python framework built on top of Tkinter. It allows users to create highly configurable, keyboard-driven graphical user interfaces (GUIs) that are ideal for scratchpad-style applications. With this framework, you can easily build custom alternatives to the scratchpads used with i3 or create your own keyboard-centric applications.
 
 ## Features
 
 - Keyboard-driven: The framework is designed to provide a Vim-like experience, making it highly efficient for keyboard users. It supports customizable keybindings, allowing you to create your own keyboard shortcuts for various actions.
 - Configurability: The framework offers extensive configuration options, enabling you to customize the behavior, appearance, and keybindings of your GUI applications. It provides flexibility to adapt the framework to your specific needs.
@@ -57,17 +57,17 @@
 
 5. Run your application by instantiating your subclass and calling the `run()` method:
    ```python
    app = YourCustomApp()
    app.run()
    ```
 
-For more details and examples, please refer to the [example](./example/) provided.
+For more details and examples, please refer to the [example](https://github.com/youssef-attai/fwf/blob/main/example/) provided.
 
 ## Contributing
 
 Contributions are welcome! If you find any issues, have suggestions, or want to contribute new features or improvements, please feel free to open an issue or submit a pull request.
 
 ## License
 
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/youssef-attai/fwf/blob/main/LICENSE) file for more information.
```

### Comparing `floating-window-framework-0.0.3/fwf/base_app.py` & `floating-window-framework-0.0.4/fwf/base_app.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.3/fwf/component.py` & `floating-window-framework-0.0.4/fwf/component.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.3/fwf/keybindings.py` & `floating-window-framework-0.0.4/fwf/keybindings.py`

 * *Files identical despite different names*

### Comparing `floating-window-framework-0.0.3/setup.py` & `floating-window-framework-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='floating-window-framework',
-    version='0.0.3',
+    version='0.0.4',
     description='A framework for building floating window applications.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Youssef Atta'i",
     author_email='youssefgalalnazem@gmail.com',
     url='https://github.com/youssef-attai/fwf',
     packages=['fwf'],
```

