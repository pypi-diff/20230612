# Comparing `tmp/gh_subdir-0.1.8.tar.gz` & `tmp/gh_subdir-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_subdir-0.1.8.tar", last modified: Mon Jun 12 07:15:09 2023, max compression
+gzip compressed data, was "gh_subdir-0.1.9.tar", last modified: Mon Jun 12 07:27:41 2023, max compression
```

## Comparing `gh_subdir-0.1.8.tar` & `gh_subdir-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:15:09.448517 gh_subdir-0.1.8/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.8/LICENSE
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:15:09.448517 gh_subdir-0.1.8/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      884 2023-06-12 07:01:01.000000 gh_subdir-0.1.8/README.md
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 07:15:09.458514 gh_subdir-0.1.8/setup.cfg
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      831 2023-06-12 07:14:58.000000 gh_subdir-0.1.8/setup.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:15:09.374179 gh_subdir-0.1.8/src/
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:15:09.391985 gh_subdir-0.1.8/src/gh_subdir/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:14:42.000000 gh_subdir-0.1.8/src/gh_subdir/__init__.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:15:09.445512 gh_subdir-0.1.8/src/gh_subdir/installer/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:14:16.000000 gh_subdir-0.1.8/src/gh_subdir/installer/__init__.py
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 06:14:11.000000 gh_subdir-0.1.8/src/gh_subdir/installer/gh_subdir.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:15:09.440514 gh_subdir-0.1.8/src/gh_subdir.egg-info/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:15:09.000000 gh_subdir-0.1.8/src/gh_subdir.egg-info/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      319 2023-06-12 07:15:09.000000 gh_subdir-0.1.8/src/gh_subdir.egg-info/SOURCES.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:15:09.000000 gh_subdir-0.1.8/src/gh_subdir.egg-info/dependency_links.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 07:15:09.000000 gh_subdir-0.1.8/src/gh_subdir.egg-info/requires.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       10 2023-06-12 07:15:09.000000 gh_subdir-0.1.8/src/gh_subdir.egg-info/top_level.txt
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:27:41.794398 gh_subdir-0.1.9/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.9/LICENSE
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:27:41.794398 gh_subdir-0.1.9/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      884 2023-06-12 07:01:01.000000 gh_subdir-0.1.9/README.md
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 07:27:41.804408 gh_subdir-0.1.9/setup.cfg
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      831 2023-06-12 07:27:30.000000 gh_subdir-0.1.9/setup.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:27:41.738179 gh_subdir-0.1.9/src/
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:27:41.765848 gh_subdir-0.1.9/src/gh_subdir/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       38 2023-06-12 07:25:25.000000 gh_subdir-0.1.9/src/gh_subdir/__init__.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:27:41.791398 gh_subdir-0.1.9/src/gh_subdir/tools/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:14:16.000000 gh_subdir-0.1.9/src/gh_subdir/tools/__init__.py
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 07:19:43.000000 gh_subdir-0.1.9/src/gh_subdir/tools/gh_subdir.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:27:41.781849 gh_subdir-0.1.9/src/gh_subdir.egg-info/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:27:41.000000 gh_subdir-0.1.9/src/gh_subdir.egg-info/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      311 2023-06-12 07:27:41.000000 gh_subdir-0.1.9/src/gh_subdir.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:27:41.000000 gh_subdir-0.1.9/src/gh_subdir.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 07:27:41.000000 gh_subdir-0.1.9/src/gh_subdir.egg-info/requires.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       10 2023-06-12 07:27:41.000000 gh_subdir-0.1.9/src/gh_subdir.egg-info/top_level.txt
```

### Comparing `gh_subdir-0.1.8/LICENSE` & `gh_subdir-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.8/PKG-INFO` & `gh_subdir-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_subdir
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
```

### Comparing `gh_subdir-0.1.8/README.md` & `gh_subdir-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.8/setup.py` & `gh_subdir-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gh_subdir',
-    version='0.1.8',
+    version='0.1.9',
     description='A Python module for installing GitHub subdirectories.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Reece Vela',
     author_email='reecevela@outlook.com',
     url='https://github.com/reecevela/gh-subdir-py',
     packages=find_packages('src'),
```

### Comparing `gh_subdir-0.1.8/src/gh_subdir/installer/gh_subdir.py` & `gh_subdir-0.1.9/src/gh_subdir/tools/gh_subdir.py`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.8/src/gh_subdir.egg-info/PKG-INFO` & `gh_subdir-0.1.9/src/gh_subdir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-subdir
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
```

