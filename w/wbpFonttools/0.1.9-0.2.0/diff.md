# Comparing `tmp/wbpFonttools-0.1.9.tar.gz` & `tmp/wbpFonttools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpFonttools-0.1.9.tar", last modified: Tue May  2 09:59:55 2023, max compression
+gzip compressed data, was "wbpFonttools-0.2.0.tar", last modified: Mon Jun 12 15:12:31 2023, max compression
```

## Comparing `wbpFonttools-0.1.9.tar` & `wbpFonttools-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.894666 wbpFonttools-0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.887666 wbpFonttools-0.1.9/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.892666 wbpFonttools-0.1.9/Lib/wbpFonttools/
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6779 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/control.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3277 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/template.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/view.py
--rw-rw-rw-   0 root         (0) root         (0)    12103 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/window.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/windowUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.894666 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2323 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2323 2023-05-02 09:59:55.894666 wbpFonttools-0.1.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-05-02 09:59:55.895666 wbpFonttools-0.1.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.855611 wbpFonttools-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.852611 wbpFonttools-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.854611 wbpFonttools-0.2.0/Lib/wbpFonttools/
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6779 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/control.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    12103 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/window.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/Lib/wbpFonttools/windowUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:12:31.855611 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      594 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-12 15:12:31.000000 wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-12 15:12:31.856611 wbpFonttools-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-06-12 15:12:31.856611 wbpFonttools-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 15:12:30.000000 wbpFonttools-0.2.0/setup.py
```

### Comparing `wbpFonttools-0.1.9/LICENSE` & `wbpFonttools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/__init__.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     WebFont_WOFF_2_Template,
     WebFont_WOFF_Template,
 )
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 
 
 def CurrentFont() -> Optional[TTFont]:
     """
     Get the currently active font
     """
     app: App = wx.GetApp()
```

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/config.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/config.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/control.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/control.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/dialog.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/dialog.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/document.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,17 +68,20 @@
     def __repr__(self):
         return f'<TTFont object: "{self.document.printableName}">'
 
     def save(self, file, reorderTables=True):
         TTFontBase.save(self, file, reorderTables)
         self._modifiedTables = set()
 
-    def updateUI(self):
+    def updateUI(self, table:Optional[str]=None):
         if hasattr(self, "document"):
-            self.document.UpdateAllViews(self.document, ("refresh",))
+            if table:
+                self.document.UpdateAllViews(self.document, ("modify", table))
+            else:
+                self.document.UpdateAllViews(self.document, ("refresh",))
 
 
 class FontToolsDocument(Document):
     binaryData = True
     canReload = True
 
     def __init__(self, template: FontToolsTemplate):
```

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/selectFontsDialogUI.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/template.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/template.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/tools.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/tools.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/view.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/view.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/window.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/window.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools/windowUI.py` & `wbpFonttools-0.2.0/Lib/wbpFonttools/windowUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/PKG-INFO` & `wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.1.9
+Version: 0.2.0
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
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
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpFonttools
 
 FontTools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
```

### Comparing `wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/SOURCES.txt` & `wbpFonttools-0.2.0/Lib/wbpFonttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/PKG-INFO` & `wbpFonttools-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.1.9
+Version: 0.2.0
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
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
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpFonttools
 
 FontTools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
```

### Comparing `wbpFonttools-0.1.9/README.md` & `wbpFonttools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.9/setup.cfg` & `wbpFonttools-0.2.0/setup.cfg`

 * *Files 4% similar despite different names*

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
 
@@ -27,58 +27,60 @@
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
 	Topic :: Text Processing :: Fonts
 	Topic :: Multimedia :: Graphics
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.8,<3.11
+python_requires = >=3.8
 install_requires = 
-	wbBase>=0.1.56
-	fonttools[ufo,lxml,woff,unicode,interpolatable,plot,symfont]>=4.39.3
+	wbBase>=0.2
+	fonttools[ufo,lxml,woff,unicode,interpolatable,plot,symfont]>=4.39.4
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = fonttools = wbpFonttools
 
 [bumpversion:file:Lib/wbpFonttools/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
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

