# Comparing `tmp/wbpShell-0.1.7.tar.gz` & `tmp/wbpShell-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpShell-0.1.7.tar", last modified: Sun Apr 23 04:07:30 2023, max compression
+gzip compressed data, was "wbpShell-0.2.0.tar", last modified: Mon Jun 12 13:44:07 2023, max compression
```

## Comparing `wbpShell-0.1.7.tar` & `wbpShell-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.874070 wbpShell-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-23 04:07:28.000000 wbpShell-0.1.7/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.870070 wbpShell-0.1.7/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.873070 wbpShell-0.1.7/Lib/wbpShell/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-23 04:07:28.000000 wbpShell-0.1.7/Lib/wbpShell/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-04-23 04:07:28.000000 wbpShell-0.1.7/Lib/wbpShell/preferences.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-23 04:07:28.000000 wbpShell-0.1.7/Lib/wbpShell/shellwin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 04:07:30.874070 wbpShell-0.1.7/Lib/wbpShell.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1935 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-23 04:07:30.000000 wbpShell-0.1.7/Lib/wbpShell.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1935 2023-04-23 04:07:30.875070 wbpShell-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-04-23 04:07:28.000000 wbpShell-0.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2063 2023-04-23 04:07:30.876070 wbpShell-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-23 04:07:28.000000 wbpShell-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:44:07.381276 wbpShell-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-12 13:44:06.000000 wbpShell-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:44:07.379276 wbpShell-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:44:07.380276 wbpShell-0.2.0/Lib/wbpShell/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-12 13:44:06.000000 wbpShell-0.2.0/Lib/wbpShell/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-06-12 13:44:06.000000 wbpShell-0.2.0/Lib/wbpShell/preferences.py
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-06-12 13:44:06.000000 wbpShell-0.2.0/Lib/wbpShell/shellwin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:44:07.381276 wbpShell-0.2.0/Lib/wbpShell.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-12 13:44:07.000000 wbpShell-0.2.0/Lib/wbpShell.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-12 13:44:07.000000 wbpShell-0.2.0/Lib/wbpShell.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 13:44:07.000000 wbpShell-0.2.0/Lib/wbpShell.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-12 13:44:07.000000 wbpShell-0.2.0/Lib/wbpShell.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 13:44:07.000000 wbpShell-0.2.0/Lib/wbpShell.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-12 13:44:07.000000 wbpShell-0.2.0/Lib/wbpShell.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-12 13:44:07.381276 wbpShell-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-06-12 13:44:06.000000 wbpShell-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-06-12 13:44:07.381276 wbpShell-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 13:44:06.000000 wbpShell-0.2.0/setup.py
```

### Comparing `wbpShell-0.1.7/LICENSE` & `wbpShell-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpShell-0.1.7/Lib/wbpShell/preferences.py` & `wbpShell-0.2.0/Lib/wbpShell/preferences.py`

 * *Files identical despite different names*

### Comparing `wbpShell-0.1.7/Lib/wbpShell/shellwin.py` & `wbpShell-0.2.0/Lib/wbpShell/shellwin.py`

 * *Files identical despite different names*

### Comparing `wbpShell-0.1.7/Lib/wbpShell.egg-info/PKG-INFO` & `wbpShell-0.2.0/Lib/wbpShell.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpShell
-Version: 0.1.7
+Version: 0.2.0
 Summary: Shell panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpshell
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpshell
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpshell
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpshell/-/issues
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
 
 # wbpShell
 
 Shell plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpShell-0.1.7/PKG-INFO` & `wbpShell-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpShell
-Version: 0.1.7
+Version: 0.2.0
 Summary: Shell panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpshell
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpshell
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpshell
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpshell/-/issues
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
 
 # wbpShell
 
 Shell plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpShell-0.1.7/setup.cfg` & `wbpShell-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.7
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
-	wbBase>=0.1.54
+	wbBase>=0.2
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = shell = wbpShell
 
 [bumpversion:file:Lib/wbpShell/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.4
+min_version = 4.6
 env_list = 
 	py38
 	py39
-	py10
+	py310
+	py311
 
 [testenv]
 deps = 
 	pytest
 	pytest-cov
 	coverage
 commands =
```

