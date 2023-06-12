# Comparing `tmp/wbpTextedit-0.1.6.tar.gz` & `tmp/wbpTextedit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpTextedit-0.1.6.tar", last modified: Tue May  2 10:27:52 2023, max compression
+gzip compressed data, was "wbpTextedit-0.2.0.tar", last modified: Mon Jun 12 13:53:47 2023, max compression
```

## Comparing `wbpTextedit-0.1.6.tar` & `wbpTextedit-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.316700 wbpTextedit-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.309700 wbpTextedit-0.1.6/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.313700 wbpTextedit-0.1.6/Lib/wbpTextedit/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3641 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7646 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/control.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.316700 wbpTextedit-0.1.6/Lib/wbpTextedit/template/
--rw-rw-rw-   0 root         (0) root         (0)     4999 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/ini.py
--rw-rw-rw-   0 root         (0) root         (0)     4858 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/python.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/xml.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/view.py
--rw-rw-rw-   0 root         (0) root         (0)     1395 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/window.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.315700 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2082 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2082 2023-05-02 10:27:52.316700 wbpTextedit-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-05-02 10:27:52.317700 wbpTextedit-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:53:47.940589 wbpTextedit-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:53:47.937590 wbpTextedit-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:53:47.939589 wbpTextedit-0.2.0/Lib/wbpTextedit/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3641 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7646 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/control.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:53:47.940589 wbpTextedit-0.2.0/Lib/wbpTextedit/template/
+-rw-rw-rw-   0 root         (0) root         (0)     4999 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/template/ini.py
+-rw-rw-rw-   0 root         (0) root         (0)     4858 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/template/python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/template/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/view.py
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/Lib/wbpTextedit/window.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 13:53:47.940589 wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-12 13:53:47.000000 wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-12 13:53:47.000000 wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 13:53:47.000000 wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-12 13:53:47.000000 wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 13:53:47.000000 wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 13:53:47.000000 wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-12 13:53:47.940589 wbpTextedit-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-06-12 13:53:47.941589 wbpTextedit-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-12 13:53:46.000000 wbpTextedit-0.2.0/setup.py
```

### Comparing `wbpTextedit-0.1.6/LICENSE` & `wbpTextedit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/__init__.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .template import PlainTextTemplate
 from .config import TextEditPreferences, PlainTextPreferences
 from .template.python import PythonTextTemplate, PythonTextPreferences
 from .template.xml import XMLTextTemplate, XMLTextPreferences
 from .template.ini import IniTextTemplate, IniTextPreferences
 
 
-__version__ = "0.1.6"
+__version__ = "0.2.0"
 
 doctemplates = (PlainTextTemplate, PythonTextTemplate, XMLTextTemplate, IniTextTemplate)
 
 preferencepages = (
     TextEditPreferences,
     PlainTextPreferences,
     PythonTextPreferences,
```

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/config.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/config.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/control.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/control.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/template/__init__.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/template/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/template/ini.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/template/ini.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/template/python.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/template/python.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/template/xml.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/template/xml.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/view.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/view.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit/window.py` & `wbpTextedit-0.2.0/Lib/wbpTextedit/window.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/PKG-INFO` & `wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: wbpTextedit
-Version: 0.1.6
+Version: 0.2.0
 Summary: Text editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbptextedit
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbptextedit
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbptextedit
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbptextedit/-/issues
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
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/SOURCES.txt` & `wbpTextedit-0.2.0/Lib/wbpTextedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/PKG-INFO` & `wbpTextedit-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: wbpTextedit
-Version: 0.1.6
+Version: 0.2.0
 Summary: Text editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbptextedit
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbptextedit
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbptextedit
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbptextedit/-/issues
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
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wbpTextedit-0.1.6/README.md` & `wbpTextedit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.6/setup.cfg` & `wbpTextedit-0.2.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.6
+current_version = 0.2.0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -31,50 +31,52 @@
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
 	Intended Audience :: Developers
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	wbBase>=0.1.52
+	wbBase>=0.2
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = textedit = wbpTextedit
 
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

