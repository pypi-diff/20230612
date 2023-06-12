# Comparing `tmp/fonttoolsWB-0.1.4.tar.gz` & `tmp/fonttoolsWB-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fonttoolsWB-0.1.4.tar", last modified: Thu May  4 11:53:52 2023, max compression
+gzip compressed data, was "fonttoolsWB-0.2.0.tar", last modified: Mon Jun 12 15:42:34 2023, max compression
```

## Comparing `fonttoolsWB-0.1.4.tar` & `fonttoolsWB-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.952935 fonttoolsWB-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.946934 fonttoolsWB-0.1.4/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.949934 fonttoolsWB-0.1.4/Lib/fonttoolsWB/
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.952935 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/application.yml
--rw-rw-rw-   0 root         (0) root         (0)     2379 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/firstRun.py
--rw-rw-rw-   0 root         (0) root         (0)     9767 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/splashscreen.png
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB/gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:53:52.951934 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-04 11:53:52.000000 fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-04 11:53:52.952935 fonttoolsWB-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2379 2023-05-04 11:53:52.953935 fonttoolsWB-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-04 11:53:51.000000 fonttoolsWB-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.765546 fonttoolsWB-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.761546 fonttoolsWB-0.2.0/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.763546 fonttoolsWB-0.2.0/Lib/fonttoolsWB/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.765546 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/application.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/firstRun.py
+-rw-rw-rw-   0 root         (0) root         (0)     9767 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/splashscreen.png
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB/gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 15:42:34.764546 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-12 15:42:34.000000 fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-12 15:42:34.765546 fonttoolsWB-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-06-12 15:42:34.766546 fonttoolsWB-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 15:42:33.000000 fonttoolsWB-0.2.0/setup.py
```

### Comparing `fonttoolsWB-0.1.4/LICENSE` & `fonttoolsWB-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/application.yml` & `fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/application.yml`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/firstRun.py` & `fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/firstRun.py`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.4/Lib/fonttoolsWB/data/splashscreen.png` & `fonttoolsWB-0.2.0/Lib/fonttoolsWB/data/splashscreen.png`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.4/Lib/fonttoolsWB.egg-info/PKG-INFO` & `fonttoolsWB-0.2.0/Lib/fonttoolsWB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.1.4
+Version: 0.2.0
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
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
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # fonttoolsWB
 
 ## FontTools Workbench
```

### Comparing `fonttoolsWB-0.1.4/PKG-INFO` & `fonttoolsWB-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: fonttoolsWB
-Version: 0.1.4
+Version: 0.2.0
 Summary: FontTools WorkBench - Edit OpenType fonts as XML.
 Home-page: https://gitlab.com/workbench2/fonttoolsWB
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/fonttoolsWB
 Project-URL: Documentation, https://workbench2.gitlab.io/fonttoolsWB
 Project-URL: Tracker, https://gitlab.com/workbench2/fonttoolsWB/-/issues
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
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # fonttoolsWB
 
 ## FontTools Workbench
```

### Comparing `fonttoolsWB-0.1.4/README.md` & `fonttoolsWB-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fonttoolsWB-0.1.4/setup.cfg` & `fonttoolsWB-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.4
+current_version = 0.2.0
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -31,69 +31,71 @@
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
 	Intended Audience :: End Users/Desktop
 	Topic :: Text Processing :: Fonts
 	Topic :: Multimedia :: Graphics
 
 [options]
 packages = find:
 package_dir = 
 	=Lib
-python_requires = >=3.8,<3.11
+python_requires = >=3.8
 install_requires = 
-	wbBase>=0.1.58
-	wbpFonttools>=0.1.9
-	wbpLoglist>=0.1.5
-	wbpOutput>=0.1.9
-	wbpShell>=0.1.7
-	wbpTextedit>=0.1.6
-	wbpUItools>=0.1.9
+	wbBase>=0.2
+	wbpFonttools>=0.2
+	wbpLoglist>=0.2
+	wbpOutput>=0.2
+	wbpShell>=0.2
+	wbpTextedit>=0.2
+	wbpUItools>=0.2
 
 [options.extras_require]
 develop = 
-	wbpNamespace>=0.1.9
-	wbpWidgetinspector>=0.1.8
+	wbpNamespace>=0.2
+	wbpWidgetinspector>=0.2
 
 [options.packages.find]
 where = Lib
 
 [options.package_data]
 fonttoolsWB.data = 
 	splashscreen.png
 	application.yml
 
 [options.entry_points]
 console_scripts = ftwb = fonttoolsWB.gui:main
 gui_scripts = fonttoolswb = fonttoolsWB.gui:main
 
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

