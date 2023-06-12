# Comparing `tmp/djangolazy-0.3.0.tar.gz` & `tmp/djangolazy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangolazy-0.3.0.tar", last modified: Sun Jun 11 17:52:43 2023, max compression
+gzip compressed data, was "djangolazy-0.4.0.tar", last modified: Mon Jun 12 16:05:04 2023, max compression
```

## Comparing `djangolazy-0.3.0.tar` & `djangolazy-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 17:52:43.828822 djangolazy-0.3.0/
--rw-rw-rw-   0        0        0     1077 2023-06-11 14:29:04.000000 djangolazy-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      936 2023-06-11 17:52:43.829824 djangolazy-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-06-11 15:21:19.000000 djangolazy-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 17:52:43.769831 djangolazy-0.3.0/djangolazy/
--rw-rw-rw-   0        0        0       64 2023-06-11 17:52:33.000000 djangolazy-0.3.0/djangolazy/__init__.py
--rw-rw-rw-   0        0        0     7016 2023-06-11 16:14:30.000000 djangolazy-0.3.0/djangolazy/__main__.py
--rw-rw-rw-   0        0        0     9769 2023-06-11 16:16:16.000000 djangolazy-0.3.0/djangolazy/setupscript.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:52:43.818824 djangolazy-0.3.0/djangolazy.egg-info/
--rw-rw-rw-   0        0        0      936 2023-06-11 17:52:43.000000 djangolazy-0.3.0/djangolazy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-11 17:52:43.000000 djangolazy-0.3.0/djangolazy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 17:52:43.000000 djangolazy-0.3.0/djangolazy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-11 17:52:43.000000 djangolazy-0.3.0/djangolazy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 17:52:43.000000 djangolazy-0.3.0/djangolazy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-11 17:52:43.832823 djangolazy-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1924 2023-06-11 17:52:23.000000 djangolazy-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:05:04.523115 djangolazy-0.4.0/
+-rw-rw-rw-   0        0        0     1077 2023-06-11 14:29:04.000000 djangolazy-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1105 2023-06-12 16:05:04.523115 djangolazy-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-06-11 15:21:19.000000 djangolazy-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 16:05:04.457114 djangolazy-0.4.0/djangolazy/
+-rw-rw-rw-   0        0        0    16491 2023-06-12 15:45:39.000000 djangolazy-0.4.0/djangolazy/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-06-12 15:38:39.000000 djangolazy-0.4.0/djangolazy/__main__.py
+-rw-rw-rw-   0        0        0       21 2023-06-12 16:00:25.000000 djangolazy-0.4.0/djangolazy/version.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:05:04.513117 djangolazy-0.4.0/djangolazy.egg-info/
+-rw-rw-rw-   0        0        0     1105 2023-06-12 16:05:03.000000 djangolazy-0.4.0/djangolazy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-06-12 16:05:04.000000 djangolazy-0.4.0/djangolazy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:05:03.000000 djangolazy-0.4.0/djangolazy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-12 16:05:03.000000 djangolazy-0.4.0/djangolazy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-12 16:05:03.000000 djangolazy-0.4.0/djangolazy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-12 16:05:03.000000 djangolazy-0.4.0/djangolazy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 16:05:03.000000 djangolazy-0.4.0/djangolazy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 16:05:04.527114 djangolazy-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2031 2023-06-12 15:21:40.000000 djangolazy-0.4.0/setup.py
```

### Comparing `djangolazy-0.3.0/LICENSE.txt` & `djangolazy-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangolazy-0.3.0/PKG-INFO` & `djangolazy-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: djangolazy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Script for initial django project setup
 Home-page: https://github.com/IshuSinghSE
-Download-URL: https://github.com/IshuSinghSE/djangolazy/archive/refs/tags/v.0.1.0.tar.gz
+Download-URL: https://github.com/IshuSinghSE/djangolazy/archive/refs/tags/v.0.4.0.tar.gz
 Author:  Ishu Singh
 Author-email: ishu.111636@gmail.com
 License: MIT
 Keywords: django,setup,autosetup,setupscript
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # scripts
 
 Script for initial django project setup
```

### Comparing `djangolazy-0.3.0/djangolazy.egg-info/PKG-INFO` & `djangolazy-0.4.0/djangolazy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: djangolazy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Script for initial django project setup
 Home-page: https://github.com/IshuSinghSE
-Download-URL: https://github.com/IshuSinghSE/djangolazy/archive/refs/tags/v.0.1.0.tar.gz
+Download-URL: https://github.com/IshuSinghSE/djangolazy/archive/refs/tags/v.0.4.0.tar.gz
 Author:  Ishu Singh
 Author-email: ishu.111636@gmail.com
 License: MIT
 Keywords: django,setup,autosetup,setupscript
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # scripts
 
 Script for initial django project setup
```

### Comparing `djangolazy-0.3.0/setup.py` & `djangolazy-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,44 @@
-from distutils.core import setup
+from setuptools import setup
+from djangolazy.version import __version__ as version
+
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
   name = 'djangolazy',         # How you named your package folder (MyLib)
   packages = ['djangolazy'],   # Chose the same as "name"
-  version = '0.3.0',      # Start with a small number and increase it with every change you make
+  version = version,      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Script for initial django project setup',   # Give a short description about your library
   long_description = long_description,
   long_description_content_type = "text/markdown",
   author = ' Ishu Singh',                   # Type in your name
   author_email = 'ishu.111636@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/IshuSinghSE',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/IshuSinghSE/djangolazy/archive/refs/tags/v.0.1.0.tar.gz',    # I explain this later on
+  download_url = f'https://github.com/IshuSinghSE/djangolazy/archive/refs/tags/v.{version}.tar.gz',    # I explain this later on
   keywords = ['django', 'setup', 'autosetup','setupscript'],   # Keywords that define your package best
-  install_requires=[            # I get to this in a second
+  python_requires= '>=3.7',
+  entry_points={
+    'console_scripts':[
+                'djangolazy =  djangolazy:main',
+                   ],},
+  install_requires=[
             'urllib3',
             ],
   classifiers=[
-    'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-    'Intended Audience :: Developers',      # Define that your audience are developers
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',   # Again, pick a license
-    'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
-    'Programming Language :: Python :: 3.4',
-    'Programming Language :: Python :: 3.5',
-    'Programming Language :: Python :: 3.6',
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Natural Language :: English',
+    'Operating System :: Microsoft :: Windows',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
   ],
-)
+  include_package_data=True,
+      zip_safe=False
+)
```

