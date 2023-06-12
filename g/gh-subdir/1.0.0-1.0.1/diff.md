# Comparing `tmp/gh_subdir-1.0.0.tar.gz` & `tmp/gh_subdir-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_subdir-1.0.0.tar", last modified: Mon Jun 12 07:39:03 2023, max compression
+gzip compressed data, was "gh_subdir-1.0.1.tar", last modified: Mon Jun 12 07:41:10 2023, max compression
```

## Comparing `gh_subdir-1.0.0.tar` & `gh_subdir-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:39:03.851584 gh_subdir-1.0.0/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-1.0.0/LICENSE
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1771 2023-06-12 07:39:03.852586 gh_subdir-1.0.0/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      959 2023-06-12 07:36:26.000000 gh_subdir-1.0.0/README.md
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 07:39:03.863218 gh_subdir-1.0.0/setup.cfg
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      831 2023-06-12 07:38:43.000000 gh_subdir-1.0.0/setup.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:39:03.800450 gh_subdir-1.0.0/src/
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:39:03.826828 gh_subdir-1.0.0/src/gh_subdir/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       38 2023-06-12 07:25:25.000000 gh_subdir-1.0.0/src/gh_subdir/__init__.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:39:03.848563 gh_subdir-1.0.0/src/gh_subdir/tools/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:14:16.000000 gh_subdir-1.0.0/src/gh_subdir/tools/__init__.py
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 07:19:43.000000 gh_subdir-1.0.0/src/gh_subdir/tools/gh_subdir.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:39:03.843567 gh_subdir-1.0.0/src/gh_subdir.egg-info/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1771 2023-06-12 07:39:03.000000 gh_subdir-1.0.0/src/gh_subdir.egg-info/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      311 2023-06-12 07:39:03.000000 gh_subdir-1.0.0/src/gh_subdir.egg-info/SOURCES.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:39:03.000000 gh_subdir-1.0.0/src/gh_subdir.egg-info/dependency_links.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 07:39:03.000000 gh_subdir-1.0.0/src/gh_subdir.egg-info/requires.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       10 2023-06-12 07:39:03.000000 gh_subdir-1.0.0/src/gh_subdir.egg-info/top_level.txt
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.962072 gh_subdir-1.0.1/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-1.0.1/LICENSE
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1815 2023-06-12 07:41:10.963072 gh_subdir-1.0.1/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1003 2023-06-12 07:40:36.000000 gh_subdir-1.0.1/README.md
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 07:41:10.971096 gh_subdir-1.0.1/setup.cfg
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      831 2023-06-12 07:41:06.000000 gh_subdir-1.0.1/setup.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.915398 gh_subdir-1.0.1/src/
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.938827 gh_subdir-1.0.1/src/gh_subdir/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       38 2023-06-12 07:25:25.000000 gh_subdir-1.0.1/src/gh_subdir/__init__.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.960075 gh_subdir-1.0.1/src/gh_subdir/tools/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:14:16.000000 gh_subdir-1.0.1/src/gh_subdir/tools/__init__.py
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 07:19:43.000000 gh_subdir-1.0.1/src/gh_subdir/tools/gh_subdir.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:41:10.954073 gh_subdir-1.0.1/src/gh_subdir.egg-info/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1815 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      311 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/requires.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       10 2023-06-12 07:41:10.000000 gh_subdir-1.0.1/src/gh_subdir.egg-info/top_level.txt
```

### Comparing `gh_subdir-1.0.0/LICENSE` & `gh_subdir-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_subdir-1.0.0/PKG-INFO` & `gh_subdir-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_subdir
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
@@ -36,15 +36,15 @@
         
         create_subfolder: 
         - If True, the files will be installed in a subfolder with the same name as the subfolder path. 
         - If False, the files will be installed in the same directory as the python file.
         
         ## Contributors
         
-        Reece Vela
+        Reece Vela  - [Github](https://github.com/reecevela)  
         Others welcome!
 Keywords: github directory download python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gh_subdir-1.0.0/README.md` & `gh_subdir-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,9 +28,9 @@
 
 create_subfolder: 
 - If True, the files will be installed in a subfolder with the same name as the subfolder path. 
 - If False, the files will be installed in the same directory as the python file.
 
 ## Contributors
 
-Reece Vela
+Reece Vela  - [Github](https://github.com/reecevela)  
 Others welcome!
```

### Comparing `gh_subdir-1.0.0/setup.py` & `gh_subdir-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gh_subdir',
-    version='1.0.0',
+    version='1.0.1',
     description='A Python module for installing GitHub subdirectories.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Reece Vela',
     author_email='reecevela@outlook.com',
     url='https://github.com/reecevela/gh-subdir-py',
     packages=find_packages('src'),
```

### Comparing `gh_subdir-1.0.0/src/gh_subdir/tools/gh_subdir.py` & `gh_subdir-1.0.1/src/gh_subdir/tools/gh_subdir.py`

 * *Files identical despite different names*

### Comparing `gh_subdir-1.0.0/src/gh_subdir.egg-info/PKG-INFO` & `gh_subdir-1.0.1/src/gh_subdir.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-subdir
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
@@ -36,15 +36,15 @@
         
         create_subfolder: 
         - If True, the files will be installed in a subfolder with the same name as the subfolder path. 
         - If False, the files will be installed in the same directory as the python file.
         
         ## Contributors
         
-        Reece Vela
+        Reece Vela  - [Github](https://github.com/reecevela)  
         Others welcome!
 Keywords: github directory download python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

