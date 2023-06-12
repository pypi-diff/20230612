# Comparing `tmp/wbpUItools-0.1.9.tar.gz` & `tmp/wbpUItools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpUItools-0.1.9.tar", last modified: Tue May  2 10:33:21 2023, max compression
+gzip compressed data, was "wbpUItools-0.2.0.tar", last modified: Mon Jun 12 14:02:28 2023, max compression
```

## Comparing `wbpUItools-0.1.9.tar` & `wbpUItools-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.698206 wbpUItools-0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.689955 wbpUItools-0.1.9/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.693622 wbpUItools-0.1.9/Lib/wbpUItools/
--rw-rw-rw-   0 root         (0) root         (0)     4917 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.696372 wbpUItools-0.1.9/Lib/wbpUItools/control/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3383 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/checkAllListBox.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     5762 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPickerUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.698206 wbpUItools-0.1.9/Lib/wbpUItools/dialog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1815 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/checkListDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPickerUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1568 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStrings.py
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStringsUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.695455 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2039 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2039 2023-05-02 10:33:21.698206 wbpUItools-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-02 10:33:21.699123 wbpUItools-0.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:02:28.512589 wbpUItools-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:02:28.509589 wbpUItools-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:02:28.510589 wbpUItools-0.2.0/Lib/wbpUItools/
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:02:28.511588 wbpUItools-0.2.0/Lib/wbpUItools/control/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3410 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/control/checkAllListBox.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/control/panelItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5762 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/control/panelItemPickerUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:02:28.512589 wbpUItools-0.2.0/Lib/wbpUItools/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/dialog/checkListDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogItemPickerUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogTwoStrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogTwoStringsUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 14:02:28.511588 wbpUItools-0.2.0/Lib/wbpUItools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-06-12 14:02:28.000000 wbpUItools-0.2.0/Lib/wbpUItools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      705 2023-06-12 14:02:28.000000 wbpUItools-0.2.0/Lib/wbpUItools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 14:02:28.000000 wbpUItools-0.2.0/Lib/wbpUItools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-12 14:02:28.000000 wbpUItools-0.2.0/Lib/wbpUItools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 14:02:28.000000 wbpUItools-0.2.0/Lib/wbpUItools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-12 14:02:28.000000 wbpUItools-0.2.0/Lib/wbpUItools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-06-12 14:02:28.512589 wbpUItools-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-06-12 14:02:28.513589 wbpUItools-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 14:02:27.000000 wbpUItools-0.2.0/setup.py
```

### Comparing `wbpUItools-0.1.9/LICENSE` & `wbpUItools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/__init__.py` & `wbpUItools-0.2.0/Lib/wbpUItools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from .dialog.checkListDialogUI import CheckListDialogUI
 from .dialog.dialogItemPicker import DialogItemPicker
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 
 
 def AskString(message: str, value: str = "", title: str = "") -> Optional[str]:
     app: App = wx.GetApp()
     return wx.GetTextFromUser(
         message,
         caption=title or app.AppDisplayName,
```

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/control/checkAllListBox.py` & `wbpUItools-0.2.0/Lib/wbpUItools/control/checkAllListBox.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 class CheckAllListBox(wx.Panel):
     """
     Drop-In replacement for wx.CheckListBox with additional "Check All" option
     """
     def __init__(
         self,
         parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
+        id:int=wx.ID_ANY,
+        pos:wx.Point=wx.DefaultPosition,
+        size:wx.Size=wx.DefaultSize,
         choices=None,
-        style=wx.TAB_TRAVERSAL,
+        style:int=wx.TAB_TRAVERSAL,
         validator=wx.DefaultValidator,
-        name="AlphaCheckListBox",
+        name:str="CheckAllListBox",
     ):
         wx.Panel.__init__(
             self, parent, id=id, pos=pos, size=size, style=wx.TAB_TRAVERSAL, name=name
         )
 
         sizer = wx.BoxSizer(wx.VERTICAL)
```

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPicker.py` & `wbpUItools-0.2.0/Lib/wbpUItools/control/panelItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPickerUI.py` & `wbpUItools-0.2.0/Lib/wbpUItools/control/panelItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/dialog/checkListDialogUI.py` & `wbpUItools-0.2.0/Lib/wbpUItools/dialog/checkListDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPicker.py` & `wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPickerUI.py` & `wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStrings.py` & `wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogTwoStrings.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStringsUI.py` & `wbpUItools-0.2.0/Lib/wbpUItools/dialog/dialogTwoStringsUI.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools.egg-info/PKG-INFO` & `wbpUItools-0.2.0/Lib/wbpUItools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpUItools
-Version: 0.1.9
+Version: 0.2.0
 Summary: UI tools for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUItools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUItools/-/issues
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
 
 # wbpUItools
 
 UI tools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
```

### Comparing `wbpUItools-0.1.9/Lib/wbpUItools.egg-info/SOURCES.txt` & `wbpUItools-0.2.0/Lib/wbpUItools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/PKG-INFO` & `wbpUItools-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: wbpUItools
-Version: 0.1.9
+Version: 0.2.0
 Summary: UI tools for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUItools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUItools/-/issues
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
 
 # wbpUItools
 
 UI tools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
```

### Comparing `wbpUItools-0.1.9/README.md` & `wbpUItools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.9/setup.cfg` & `wbpUItools-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

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
 
@@ -31,51 +31,53 @@
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
 wbbase.plugin = uitools = wbpUItools
 
 [tox:tox]
-min_version = 4.5
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

