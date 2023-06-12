# Comparing `tmp/wbpLoglist-0.1.5.tar.gz` & `tmp/wbpLoglist-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpLoglist-0.1.5.tar", last modified: Sun Apr 23 01:37:11 2023, max compression
+gzip compressed data, was "wbpLoglist-0.2.0.tar", last modified: Mon Jun 12 11:23:48 2023, max compression
```

## Comparing `wbpLoglist-0.1.5.tar` & `wbpLoglist-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.957045 wbpLoglist-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.952045 wbpLoglist-0.1.5/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.955045 wbpLoglist-0.1.5/Lib/wbpLoglist/
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/Lib/wbpLoglist/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5700 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/Lib/wbpLoglist/loglistwin.py
--rw-rw-rw-   0 root         (0) root         (0)     1262 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/Lib/wbpLoglist/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 01:37:11.957045 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1967 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-23 01:37:11.000000 wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1967 2023-04-23 01:37:11.957045 wbpLoglist-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2094 2023-04-23 01:37:11.958045 wbpLoglist-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-23 01:37:10.000000 wbpLoglist-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:23:48.296779 wbpLoglist-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 11:23:47.000000 wbpLoglist-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:23:48.293779 wbpLoglist-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:23:48.294779 wbpLoglist-0.2.0/Lib/wbpLoglist/
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-12 11:23:47.000000 wbpLoglist-0.2.0/Lib/wbpLoglist/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5700 2023-06-12 11:23:47.000000 wbpLoglist-0.2.0/Lib/wbpLoglist/loglistwin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-06-12 11:23:47.000000 wbpLoglist-0.2.0/Lib/wbpLoglist/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:23:48.296779 wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-06-12 11:23:48.000000 wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      352 2023-06-12 11:23:48.000000 wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:23:48.000000 wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 11:23:48.000000 wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 11:23:48.000000 wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 11:23:48.000000 wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-06-12 11:23:48.296779 wbpLoglist-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-12 11:23:47.000000 wbpLoglist-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-06-12 11:23:48.296779 wbpLoglist-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 11:23:47.000000 wbpLoglist-0.2.0/setup.py
```

### Comparing `wbpLoglist-0.1.5/LICENSE` & `wbpLoglist-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpLoglist-0.1.5/Lib/wbpLoglist/__init__.py` & `wbpLoglist-0.2.0/Lib/wbpLoglist/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .preferences import LogListPreferences, name
 
 if TYPE_CHECKING:
     from wbBase.application import App
     from wbBase.dialog.preferences import PreferencesPageBase
     from wx import aui
 
-__version__ = "0.1.5"
+__version__ = "0.2.0"
 
 
 #: Panels provided by the wbpLoglist plugin.
 panels: List[Tuple[type[wx.Window], aui.AuiPaneInfo]] = [logListPanel]
 
 #: Preference pages provided by the wbpLoglist plugin.
 preferencepages: List[type[PreferencesPageBase]] = [LogListPreferences]
```

### Comparing `wbpLoglist-0.1.5/Lib/wbpLoglist/loglistwin.py` & `wbpLoglist-0.2.0/Lib/wbpLoglist/loglistwin.py`

 * *Files identical despite different names*

### Comparing `wbpLoglist-0.1.5/Lib/wbpLoglist/preferences.py` & `wbpLoglist-0.2.0/Lib/wbpLoglist/preferences.py`

 * *Files identical despite different names*

### Comparing `wbpLoglist-0.1.5/Lib/wbpLoglist.egg-info/PKG-INFO` & `wbpLoglist-0.2.0/Lib/wbpLoglist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpLoglist
-Version: 0.1.5
+Version: 0.2.0
 Summary: Log list panel panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbploglist
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbploglist
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbploglist/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbploglist/-/issues
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
 
 # wbpLoglist
 
 Loglist plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpLoglist-0.1.5/PKG-INFO` & `wbpLoglist-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpLoglist
-Version: 0.1.5
+Version: 0.2.0
 Summary: Log list panel panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbploglist
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbploglist
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbploglist/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbploglist/-/issues
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
 
 # wbpLoglist
 
 Loglist plugin for [Workbench](https://pypi.org/project/wbBase/) applications
```

### Comparing `wbpLoglist-0.1.5/setup.cfg` & `wbpLoglist-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.5
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
 wbbase.plugin = loglist = wbpLoglist
 
 [bumpversion:file:Lib/wbpLoglist/__init__.py]
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

