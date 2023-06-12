# Comparing `tmp/wbpFilebrowser-0.1.6.tar.gz` & `tmp/wbpFilebrowser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpFilebrowser-0.1.6.tar", last modified: Sat Apr 22 14:54:06 2023, max compression
+gzip compressed data, was "wbpFilebrowser-0.2.1.tar", last modified: Mon Jun 12 10:51:22 2023, max compression
```

## Comparing `wbpFilebrowser-0.1.6.tar` & `wbpFilebrowser-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.207555 wbpFilebrowser-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.202555 wbpFilebrowser-0.1.6/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.204555 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6619 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/dirtreewindow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.206555 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2015 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2015 2023-04-22 14:54:06.207555 wbpFilebrowser-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2138 2023-04-22 14:54:06.208555 wbpFilebrowser-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:51:22.060686 wbpFilebrowser-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 10:51:20.000000 wbpFilebrowser-0.2.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:51:22.058686 wbpFilebrowser-0.2.1/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:51:22.059687 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser/
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-12 10:51:20.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2023-06-12 10:51:20.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser/dirtreewindow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:51:22.060686 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-12 10:51:22.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-12 10:51:22.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 10:51:22.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-12 10:51:22.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 10:51:22.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-12 10:51:22.000000 wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-12 10:51:22.060686 wbpFilebrowser-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-12 10:51:20.000000 wbpFilebrowser-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2023-06-12 10:51:22.060686 wbpFilebrowser-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 10:51:20.000000 wbpFilebrowser-0.2.1/setup.py
```

### Comparing `wbpFilebrowser-0.1.6/LICENSE` & `wbpFilebrowser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/dirtreewindow.py` & `wbpFilebrowser-0.2.1/Lib/wbpFilebrowser/dirtreewindow.py`

 * *Files identical despite different names*

### Comparing `wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/PKG-INFO` & `wbpFilebrowser-0.2.1/Lib/wbpFilebrowser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpFilebrowser
-Version: 0.1.6
+Version: 0.2.1
 Summary: File browser panel panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfilebrowser/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser/-/issues
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
 
 # wbpFilebrowser
 
 Filebrowser plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpFilebrowser-0.1.6/PKG-INFO` & `wbpFilebrowser-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpFilebrowser
-Version: 0.1.6
+Version: 0.2.1
 Summary: File browser panel panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfilebrowser/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser/-/issues
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
 
 # wbpFilebrowser
 
 Filebrowser plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpFilebrowser-0.1.6/README.md` & `wbpFilebrowser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wbpFilebrowser-0.1.6/setup.cfg` & `wbpFilebrowser-0.2.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.6
+current_version = 0.2.1
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
-	wbBase>=0.1.53
+	wbBase>=0.2
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = filebrowser = wbpFilebrowser
 
 [bumpversion:file:Lib/wbpFilebrowser/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.4
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

