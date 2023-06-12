# Comparing `tmp/gh_subdir-0.1.6.tar.gz` & `tmp/gh_subdir-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_subdir-0.1.6.tar", last modified: Mon Jun 12 07:01:34 2023, max compression
+gzip compressed data, was "gh_subdir-0.1.7.tar", last modified: Mon Jun 12 07:07:18 2023, max compression
```

## Comparing `gh_subdir-0.1.6.tar` & `gh_subdir-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:01:34.513813 gh_subdir-0.1.6/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.6/LICENSE
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:01:34.513813 gh_subdir-0.1.6/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      884 2023-06-12 07:01:01.000000 gh_subdir-0.1.6/README.md
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:01:34.505778 gh_subdir-0.1.6/gh_subdir.egg-info/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:01:34.000000 gh_subdir-0.1.6/gh_subdir.egg-info/PKG-INFO
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      233 2023-06-12 07:01:34.000000 gh_subdir-0.1.6/gh_subdir.egg-info/SOURCES.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:01:34.000000 gh_subdir-0.1.6/gh_subdir.egg-info/dependency_links.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 07:01:34.000000 gh_subdir-0.1.6/gh_subdir.egg-info/requires.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        4 2023-06-12 07:01:34.000000 gh_subdir-0.1.6/gh_subdir.egg-info/top_level.txt
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 07:01:34.522187 gh_subdir-0.1.6/setup.cfg
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      796 2023-06-12 07:01:06.000000 gh_subdir-0.1.6/setup.py
-drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:01:34.511781 gh_subdir-0.1.6/src/
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       34 2023-06-12 06:41:55.000000 gh_subdir-0.1.6/src/__init__.py
--rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1968 2023-06-12 06:14:11.000000 gh_subdir-0.1.6/src/gh_subdir.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:07:18.952886 gh_subdir-0.1.7/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)    35823 2023-06-12 04:39:33.000000 gh_subdir-0.1.7/LICENSE
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:07:18.952886 gh_subdir-0.1.7/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      884 2023-06-12 07:01:01.000000 gh_subdir-0.1.7/README.md
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)       74 2023-06-12 07:07:18.960892 gh_subdir-0.1.7/setup.cfg
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      831 2023-06-12 07:07:04.000000 gh_subdir-0.1.7/setup.py
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:07:18.915502 gh_subdir-0.1.7/src/
+drwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        0 2023-06-12 07:07:18.950934 gh_subdir-0.1.7/src/gh_subdir.egg-info/
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)     1633 2023-06-12 07:07:18.000000 gh_subdir-0.1.7/src/gh_subdir.egg-info/PKG-INFO
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)      220 2023-06-12 07:07:18.000000 gh_subdir-0.1.7/src/gh_subdir.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:07:18.000000 gh_subdir-0.1.7/src/gh_subdir.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        9 2023-06-12 07:07:18.000000 gh_subdir-0.1.7/src/gh_subdir.egg-info/requires.txt
+-rwxrwxrwx   0 rlvela    (1000) rlvela    (1000)        1 2023-06-12 07:07:18.000000 gh_subdir-0.1.7/src/gh_subdir.egg-info/top_level.txt
```

### Comparing `gh_subdir-0.1.6/LICENSE` & `gh_subdir-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.6/PKG-INFO` & `gh_subdir-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_subdir
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
```

### Comparing `gh_subdir-0.1.6/README.md` & `gh_subdir-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gh_subdir-0.1.6/gh_subdir.egg-info/PKG-INFO` & `gh_subdir-0.1.7/src/gh_subdir.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh-subdir
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python module for installing GitHub subdirectories.
 Home-page: https://github.com/reecevela/gh-subdir-py
 Author: Reece Vela
 Author-email: reecevela@outlook.com
 License: GPLv3
 Description: # gh_subdir
         Python module to install a subfolder of a github repo instead of the entire repo.
```

