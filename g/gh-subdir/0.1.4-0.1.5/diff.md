# Comparing `tmp/gh_subdir-0.1.4.tar.gz` & `tmp/gh_subdir-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_subdir-0.1.4.tar", last modified: Mon Jun 12 06:50:02 2023, max compression
+gzip compressed data, was "gh_subdir-0.1.5.tar", last modified: Mon Jun 12 06:54:03 2023, max compression
```

## Comparing `gh_subdir-0.1.4.tar` & `gh_subdir-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 06:50:02.488655 gh_subdir-0.1.4/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.4/LICENSE
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1636 2023-06-12 06:50:02.489691 gh_subdir-0.1.4/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      887 2023-06-12 06:08:12.000000 gh_subdir-0.1.4/README.md
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 06:50:02.470353 gh_subdir-0.1.4/gh_subdir.egg-info/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1636 2023-06-12 06:50:02.000000 gh_subdir-0.1.4/gh_subdir.egg-info/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      233 2023-06-12 06:50:02.000000 gh_subdir-0.1.4/gh_subdir.egg-info/SOURCES.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 06:50:02.000000 gh_subdir-0.1.4/gh_subdir.egg-info/dependency_links.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 06:50:02.000000 gh_subdir-0.1.4/gh_subdir.egg-info/requires.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        4 2023-06-12 06:50:02.000000 gh_subdir-0.1.4/gh_subdir.egg-info/top_level.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 06:50:02.496689 gh_subdir-0.1.4/setup.cfg
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      796 2023-06-12 06:47:42.000000 gh_subdir-0.1.4/setup.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 06:50:02.487406 gh_subdir-0.1.4/src/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       34 2023-06-12 06:41:55.000000 gh_subdir-0.1.4/src/__init__.py
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 06:14:11.000000 gh_subdir-0.1.4/src/gh_subdir.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 06:54:03.478775 gh_subdir-0.1.5/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.5/LICENSE
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1636 2023-06-12 06:54:03.478775 gh_subdir-0.1.5/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      887 2023-06-12 06:08:12.000000 gh_subdir-0.1.5/README.md
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 06:54:03.469762 gh_subdir-0.1.5/gh_subdir.egg-info/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1636 2023-06-12 06:54:03.000000 gh_subdir-0.1.5/gh_subdir.egg-info/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      233 2023-06-12 06:54:03.000000 gh_subdir-0.1.5/gh_subdir.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 06:54:03.000000 gh_subdir-0.1.5/gh_subdir.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 06:54:03.000000 gh_subdir-0.1.5/gh_subdir.egg-info/requires.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        4 2023-06-12 06:54:03.000000 gh_subdir-0.1.5/gh_subdir.egg-info/top_level.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 06:54:03.486786 gh_subdir-0.1.5/setup.cfg
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      796 2023-06-12 06:54:00.000000 gh_subdir-0.1.5/setup.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 06:54:03.475777 gh_subdir-0.1.5/src/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       34 2023-06-12 06:41:55.000000 gh_subdir-0.1.5/src/__init__.py
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 06:14:11.000000 gh_subdir-0.1.5/src/gh_subdir.py
```

### Comparing `gh_subdir-0.1.4/LICENSE` & `gh_subdir-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.4/PKG-INFO` & `gh_subdir-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_subdir
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh-subdir-py
         Python module to install a subfolder of a github repo instead of the entire repo.
```

### Comparing `gh_subdir-0.1.4/README.md` & `gh_subdir-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.4/gh_subdir.egg-info/PKG-INFO` & `gh_subdir-0.1.5/gh_subdir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-subdir
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh-subdir-py
         Python module to install a subfolder of a github repo instead of the entire repo.
```

### Comparing `gh_subdir-0.1.4/setup.py` & `gh_subdir-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gh_subdir',
-    version='0.1.4',
+    version='0.1.5',
     description='A Python module for installing GitHub subdirectories.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Reece Vela',
     author_email='reecevela@outlook.com',
     url='https://github.com/reecevela/gh-subdir-py',
     packages=find_packages(),
```

### Comparing `gh_subdir-0.1.4/src/gh_subdir.py` & `gh_subdir-0.1.5/src/gh_subdir.py`

 * *Files identical despite different names*

