# Comparing `tmp/wbpNamespace-0.1.9.tar.gz` & `tmp/wbpNamespace-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpNamespace-0.1.9.tar", last modified: Tue May  2 10:59:31 2023, max compression
+gzip compressed data, was "wbpNamespace-0.2.0.tar", last modified: Mon Jun 12 11:51:46 2023, max compression
```

## Comparing `wbpNamespace-0.1.9.tar` & `wbpNamespace-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:59:31.119617 wbpNamespace-0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-02 10:59:29.000000 wbpNamespace-0.1.9/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:59:31.115616 wbpNamespace-0.1.9/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:59:31.117616 wbpNamespace-0.1.9/Lib/wbpNamespace/
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-05-02 10:59:29.000000 wbpNamespace-0.1.9/Lib/wbpNamespace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-05-02 10:59:29.000000 wbpNamespace-0.1.9/Lib/wbpNamespace/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1719 2023-05-02 10:59:29.000000 wbpNamespace-0.1.9/Lib/wbpNamespace/control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:59:31.119617 wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-02 10:59:31.000000 wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-02 10:59:31.000000 wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 10:59:31.000000 wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-02 10:59:31.000000 wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 10:59:31.000000 wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-02 10:59:31.000000 wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-02 10:59:31.119617 wbpNamespace-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-02 10:59:29.000000 wbpNamespace-0.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2109 2023-05-02 10:59:31.120617 wbpNamespace-0.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 10:59:29.000000 wbpNamespace-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:46.166940 wbpNamespace-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-12 11:51:44.000000 wbpNamespace-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:46.164940 wbpNamespace-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:46.165940 wbpNamespace-0.2.0/Lib/wbpNamespace/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-06-12 11:51:44.000000 wbpNamespace-0.2.0/Lib/wbpNamespace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-06-12 11:51:44.000000 wbpNamespace-0.2.0/Lib/wbpNamespace/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2023-06-12 11:51:44.000000 wbpNamespace-0.2.0/Lib/wbpNamespace/control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:51:46.166940 wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-06-12 11:51:46.000000 wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-12 11:51:46.000000 wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:51:46.000000 wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-12 11:51:46.000000 wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 11:51:46.000000 wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 11:51:46.000000 wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-06-12 11:51:46.167940 wbpNamespace-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-12 11:51:44.000000 wbpNamespace-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2023-06-12 11:51:46.167940 wbpNamespace-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 11:51:44.000000 wbpNamespace-0.2.0/setup.py
```

### Comparing `wbpNamespace-0.1.9/LICENSE` & `wbpNamespace-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpNamespace-0.1.9/Lib/wbpNamespace/config.py` & `wbpNamespace-0.2.0/Lib/wbpNamespace/config.py`

 * *Files identical despite different names*

### Comparing `wbpNamespace-0.1.9/Lib/wbpNamespace/control.py` & `wbpNamespace-0.2.0/Lib/wbpNamespace/control.py`

 * *Files identical despite different names*

### Comparing `wbpNamespace-0.1.9/Lib/wbpNamespace.egg-info/PKG-INFO` & `wbpNamespace-0.2.0/Lib/wbpNamespace.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpNamespace
-Version: 0.1.9
+Version: 0.2.0
 Summary: Namespace panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpnamespace/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpNamespace
 
 Namespace plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpNamespace-0.1.9/PKG-INFO` & `wbpNamespace-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpNamespace
-Version: 0.1.9
+Version: 0.2.0
 Summary: Namespace panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpnamespace/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpnamespace/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpNamespace
 
 Namespace plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpNamespace-0.1.9/README.md` & `wbpNamespace-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wbpNamespace-0.1.9/setup.cfg` & `wbpNamespace-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.9
+current_version = 0.2.0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -27,55 +27,57 @@
 	OSX
 	POSIX
 keywords = 
 	workbench
 	wxPython
 	GUI
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Environment :: MacOS X :: Cocoa
 	Environment :: Win32 (MS Windows)
 	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.8,<3.11
+python_requires = >=3.8
 install_requires = 
-	wbBase>=0.1.56
+	wbBase>=0.2
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = namespace = wbpNamespace
 
 [bumpversion:file:Lib/wbpNamespace/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.5
+min_version = 4.6
 env_list = 
 	py38
 	py39
 	py310
+	py311
 
 [testenv]
 deps = 
 	pytest
 	pytest-cov
 	coverage
 commands =
```

