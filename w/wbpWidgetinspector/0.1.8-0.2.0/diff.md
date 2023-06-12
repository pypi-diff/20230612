# Comparing `tmp/wbpWidgetinspector-0.1.8.tar.gz` & `tmp/wbpWidgetinspector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpWidgetinspector-0.1.8.tar", last modified: Tue May  2 11:11:49 2023, max compression
+gzip compressed data, was "wbpWidgetinspector-0.2.0.tar", last modified: Mon Jun 12 14:28:29 2023, max compression
```

## Comparing `wbpWidgetinspector-0.1.8.tar` & `wbpWidgetinspector-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.050387 wbpWidgetinspector-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.046387 wbpWidgetinspector-0.1.8/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.048387 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector/
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.050387 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1853 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1853 2023-05-02 11:11:49.050387 wbpWidgetinspector-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2171 2023-05-02 11:11:49.051387 wbpWidgetinspector-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:28:29.792670 wbpWidgetinspector-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 14:28:28.000000 wbpWidgetinspector-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:28:29.790670 wbpWidgetinspector-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:28:29.791670 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector/
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-06-12 14:28:28.000000 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:28:29.792670 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-12 14:28:29.000000 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-12 14:28:29.000000 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 14:28:29.000000 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-12 14:28:29.000000 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 14:28:29.000000 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-12 14:28:29.000000 wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-12 14:28:29.792670 wbpWidgetinspector-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-12 14:28:28.000000 wbpWidgetinspector-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-06-12 14:28:29.793670 wbpWidgetinspector-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 14:28:28.000000 wbpWidgetinspector-0.2.0/setup.py
```

### Comparing `wbpWidgetinspector-0.1.8/LICENSE` & `wbpWidgetinspector-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector/__init__.py` & `wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import wx
 from wx.lib.inspection import InspectionTool
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.1.8"
+__version__ = "0.2.0"
 
 
 class WidgetInspector:
     def __init__(self, alt=True, cmd=True, shift=False, keyCode=ord("I")):
         self._alt = alt
         self._cmd = cmd
         self._shift = shift
```

### Comparing `wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/PKG-INFO` & `wbpWidgetinspector-0.2.0/Lib/wbpWidgetinspector.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wbpWidgetinspector
-Version: 0.1.8
+Version: 0.2.0
 Summary: Itegrate Widgetinspector in Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpwidgetinspector/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector/-/issues
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
```

### Comparing `wbpWidgetinspector-0.1.8/PKG-INFO` & `wbpWidgetinspector-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wbpWidgetinspector
-Version: 0.1.8
+Version: 0.2.0
 Summary: Itegrate Widgetinspector in Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpwidgetinspector/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector/-/issues
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
```

### Comparing `wbpWidgetinspector-0.1.8/setup.cfg` & `wbpWidgetinspector-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.8
+current_version = 0.2.0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -27,15 +27,15 @@
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
@@ -50,15 +50,15 @@
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	wbBase>=0.1.56
+	wbBase>=0.2
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = widgetinspector = wbpWidgetinspector
```

