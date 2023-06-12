# Comparing `tmp/yatrash-0.1.2.tar.gz` & `tmp/yatrash-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yatrash-0.1.2.tar", last modified: Sat Jun 23 15:17:22 2018, max compression
+gzip compressed data, was "yatrash-0.1.3.tar", last modified: Mon Jun 12 04:32:30 2023, max compression
```

## Comparing `yatrash-0.1.2.tar` & `yatrash-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2018-06-23 15:17:22.000000 yatrash-0.1.2/
--rw-r--r--   0 sam       (1000) sam       (1000)     1041 2018-06-23 15:17:04.000000 yatrash-0.1.2/README.md
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2018-06-23 15:17:22.000000 yatrash-0.1.2/yatrash/
--rw-r--r--   0 sam       (1000) sam       (1000)      166 2018-06-22 23:55:13.000000 yatrash-0.1.2/yatrash/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)       48 2018-06-22 23:55:17.000000 yatrash-0.1.2/yatrash/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1766 2018-06-22 23:22:59.000000 yatrash-0.1.2/yatrash/trash.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1502 2018-06-23 05:40:23.000000 yatrash-0.1.2/yatrash/main.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2109 2018-06-23 15:17:22.000000 yatrash-0.1.2/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)       38 2018-06-23 15:17:22.000000 yatrash-0.1.2/setup.cfg
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2018-06-23 15:17:22.000000 yatrash-0.1.2/script/
--rwxr-xr-x   0 sam       (1000) sam       (1000)      189 2018-06-22 23:41:19.000000 yatrash-0.1.2/script/trash
--rw-r--r--   0 sam       (1000) sam       (1000)      955 2018-06-23 15:17:19.000000 yatrash-0.1.2/setup.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2018-06-23 15:17:22.000000 yatrash-0.1.2/yatrash.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     2109 2018-06-23 15:17:22.000000 yatrash-0.1.2/yatrash.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2018-06-23 15:17:22.000000 yatrash-0.1.2/yatrash.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)      262 2018-06-23 15:17:22.000000 yatrash-0.1.2/yatrash.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       49 2018-06-23 15:17:22.000000 yatrash-0.1.2/yatrash.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        8 2018-06-23 15:17:22.000000 yatrash-0.1.2/yatrash.egg-info/top_level.txt
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 04:32:30.036093 yatrash-0.1.3/
+-rw-rw-r--   0 sam       (1000) sam       (1000)    35149 2023-06-12 04:01:11.000000 yatrash-0.1.3/LICENSE
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1627 2023-06-12 04:32:30.036093 yatrash-0.1.3/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1041 2023-06-12 04:30:16.000000 yatrash-0.1.3/README.md
+-rw-rw-r--   0 sam       (1000) sam       (1000)       38 2023-06-12 04:32:30.036093 yatrash-0.1.3/setup.cfg
+-rw-rw-r--   0 sam       (1000) sam       (1000)      969 2023-06-12 04:32:14.000000 yatrash-0.1.3/setup.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 04:32:30.036093 yatrash-0.1.3/yatrash/
+-rw-rw-r--   0 sam       (1000) sam       (1000)       48 2023-06-12 04:01:11.000000 yatrash-0.1.3/yatrash/__init__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)      166 2023-06-12 04:01:11.000000 yatrash-0.1.3/yatrash/__main__.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1502 2023-06-12 04:01:11.000000 yatrash-0.1.3/yatrash/main.py
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1766 2023-06-12 04:01:11.000000 yatrash-0.1.3/yatrash/trash.py
+drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2023-06-12 04:32:30.036093 yatrash-0.1.3/yatrash.egg-info/
+-rw-rw-r--   0 sam       (1000) sam       (1000)     1627 2023-06-12 04:32:30.000000 yatrash-0.1.3/yatrash.egg-info/PKG-INFO
+-rw-rw-r--   0 sam       (1000) sam       (1000)      257 2023-06-12 04:32:30.000000 yatrash-0.1.3/yatrash.egg-info/SOURCES.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        1 2023-06-12 04:32:30.000000 yatrash-0.1.3/yatrash.egg-info/dependency_links.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)       48 2023-06-12 04:32:30.000000 yatrash-0.1.3/yatrash.egg-info/entry_points.txt
+-rw-rw-r--   0 sam       (1000) sam       (1000)        8 2023-06-12 04:32:30.000000 yatrash-0.1.3/yatrash.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yatrash-0.1.2/README.md` & `yatrash-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `yatrash-0.1.2/yatrash/trash.py` & `yatrash-0.1.3/yatrash/trash.py`

 * *Files identical despite different names*

### Comparing `yatrash-0.1.2/yatrash/main.py` & `yatrash-0.1.3/yatrash/main.py`

 * *Files identical despite different names*

### Comparing `yatrash-0.1.2/PKG-INFO` & `yatrash-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,55 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: yatrash
-Version: 0.1.2
+Version: 0.1.3
 Summary: Safely move files into a trash can instead of `rm`.
 Home-page: https://github.com/charmoniumQ/yatrash/
 Author: Samuel Grayson
 Author-email: sam@samgrayson.me
-License: UNKNOWN
-Description: yatrash
-        =======
-        
-        Safely move files into a trash can instead of ``rm``.
-        
-        OS Independent, as long as your OS supports Python’s ``pathlib`` and
-        ``shutil``.
-        
-        Now living on `Github <https://github.com/charmoniumQ/yatrash/>`__
-        
-        Detailed usage
-        --------------
-        
-        ::
-        
-           $ trash --help
-           usage: __main__.py [-h] [--trash-dir TRASH_DIR]
-                              [trash_files [trash_files ...]]
-        
-           ...
-           see the real --help for more
-        
-        Why do we need another trash utility?
-        -------------------------------------
-        
-        This is mostly for self-educational purposes.
-        
-        If you actually want a trash utility, see
-        `trash-cli <https://pypi.org/project/trash-cli/>`__ which implements the
-        `xdg trash
-        specification <http://www.ramendik.ru/docs/trashspec.html>`__, so it
-        will play nicely with your Desktop’s trash and other tools. It also
-        features more utilities, such as recover.
-        
-        Origin
-        ------
-        
-        -  `CodeReview <https://gist.github.com/charmoniumQ/0c5fe34dbb5b3905440a3b06c4f60634>`__
-        -  `Github
-           Gist <https://codereview.stackexchange.com/questions/188842/safely-trash-instead-of-rm>`__
-        -  `Github
-           Repository <https://codereview.stackexchange.com/questions/188842/safely-trash-instead-of-rm>`__
-           (current home)
-        
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# yatrash
+Safely move files into a trash can instead of `rm`.
+
+OS Independent, as long as your OS supports Python's `pathlib` and `shutil`.
+
+Now living on [Github][5]
+
+## Detailed usage
+
+```
+$ trash --help
+usage: __main__.py [-h] [--trash-dir TRASH_DIR]
+                   [trash_files [trash_files ...]]
+
+...
+see the real --help for more
+```
+
+## Why do we need another trash utility?
+
+This is mostly for self-educational purposes.
+
+If you actually want a trash utility, see [trash-cli][1] which
+implements the [xdg trash specification][2], so it will play nicely
+with your Desktop's trash and other tools. It also features more
+utilities, such as recover.
+
+## Origin
+
+- [CodeReview][3]
+- [Github Gist][4]
+- [Github Repository][4] (current home)
+
+[1]: https://pypi.org/project/trash-cli/
+[2]: http://www.ramendik.ru/docs/trashspec.html
+[3]: https://gist.github.com/charmoniumQ/0c5fe34dbb5b3905440a3b06c4f60634
+[4]: https://codereview.stackexchange.com/questions/188842/safely-trash-instead-of-rm
+[5]: https://github.com/charmoniumQ/yatrash/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yatrash-0.1.2/setup.py` & `yatrash-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 #!/usr/bin/env python3
 
-import pypandoc
+import pathlib
 from setuptools import setup, find_packages
 
-long_description = pypandoc.convert('README.md', 'rst')
-
 description = 'Safely move files into a trash can instead of `rm`.'
 
 classifiers='''
 Natural Language :: English
 Environment :: Console
 License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Operating System :: OS Independent
 Programming Language :: Python :: 3.6
 Topic :: Utilities
 '''
 
 setup(
     name='yatrash',
-    version='0.1.2',
+    version='0.1.3',
     description=description,
     author='Samuel Grayson',
     author_email='sam@samgrayson.me',
     url='https://github.com/charmoniumQ/yatrash/',
     packages=find_packages(),
-    long_description=long_description,
+    long_description=pathlib.Path("README.md").read_text(),
+    long_description_content_type="text/markdown",
     python_requires='>=3.6.0',
     entry_points = {
         "console_scripts": [
             'trash = yatrash.__main__:main',
         ],
     },
     classifiers=[classifier.strip()
```

### Comparing `yatrash-0.1.2/yatrash.egg-info/PKG-INFO` & `yatrash-0.1.3/yatrash.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,55 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: yatrash
-Version: 0.1.2
+Version: 0.1.3
 Summary: Safely move files into a trash can instead of `rm`.
 Home-page: https://github.com/charmoniumQ/yatrash/
 Author: Samuel Grayson
 Author-email: sam@samgrayson.me
-License: UNKNOWN
-Description: yatrash
-        =======
-        
-        Safely move files into a trash can instead of ``rm``.
-        
-        OS Independent, as long as your OS supports Python’s ``pathlib`` and
-        ``shutil``.
-        
-        Now living on `Github <https://github.com/charmoniumQ/yatrash/>`__
-        
-        Detailed usage
-        --------------
-        
-        ::
-        
-           $ trash --help
-           usage: __main__.py [-h] [--trash-dir TRASH_DIR]
-                              [trash_files [trash_files ...]]
-        
-           ...
-           see the real --help for more
-        
-        Why do we need another trash utility?
-        -------------------------------------
-        
-        This is mostly for self-educational purposes.
-        
-        If you actually want a trash utility, see
-        `trash-cli <https://pypi.org/project/trash-cli/>`__ which implements the
-        `xdg trash
-        specification <http://www.ramendik.ru/docs/trashspec.html>`__, so it
-        will play nicely with your Desktop’s trash and other tools. It also
-        features more utilities, such as recover.
-        
-        Origin
-        ------
-        
-        -  `CodeReview <https://gist.github.com/charmoniumQ/0c5fe34dbb5b3905440a3b06c4f60634>`__
-        -  `Github
-           Gist <https://codereview.stackexchange.com/questions/188842/safely-trash-instead-of-rm>`__
-        -  `Github
-           Repository <https://codereview.stackexchange.com/questions/188842/safely-trash-instead-of-rm>`__
-           (current home)
-        
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# yatrash
+Safely move files into a trash can instead of `rm`.
+
+OS Independent, as long as your OS supports Python's `pathlib` and `shutil`.
+
+Now living on [Github][5]
+
+## Detailed usage
+
+```
+$ trash --help
+usage: __main__.py [-h] [--trash-dir TRASH_DIR]
+                   [trash_files [trash_files ...]]
+
+...
+see the real --help for more
+```
+
+## Why do we need another trash utility?
+
+This is mostly for self-educational purposes.
+
+If you actually want a trash utility, see [trash-cli][1] which
+implements the [xdg trash specification][2], so it will play nicely
+with your Desktop's trash and other tools. It also features more
+utilities, such as recover.
+
+## Origin
+
+- [CodeReview][3]
+- [Github Gist][4]
+- [Github Repository][4] (current home)
+
+[1]: https://pypi.org/project/trash-cli/
+[2]: http://www.ramendik.ru/docs/trashspec.html
+[3]: https://gist.github.com/charmoniumQ/0c5fe34dbb5b3905440a3b06c4f60634
+[4]: https://codereview.stackexchange.com/questions/188842/safely-trash-instead-of-rm
+[5]: https://github.com/charmoniumQ/yatrash/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

