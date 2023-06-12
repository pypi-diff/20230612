# Comparing `tmp/ddgmail-0.1.0.tar.gz` & `tmp/ddgmail-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddgmail-0.1.0.tar", last modified: Mon Jun 12 15:38:25 2023, max compression
+gzip compressed data, was "ddgmail-0.1.1.tar", last modified: Mon Jun 12 15:39:48 2023, max compression
```

## Comparing `ddgmail-0.1.0.tar` & `ddgmail-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 15:38:25.761646 ddgmail-0.1.0/
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.0/.gitignore
--rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.0/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.0/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)      484 2023-06-12 15:38:25.761646 ddgmail-0.1.0/PKG-INFO
--rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.0/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 15:38:25.761646 ddgmail-0.1.0/ddgmail.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      484 2023-06-12 15:38:25.000000 ddgmail-0.1.0/ddgmail.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      256 2023-06-12 15:38:25.000000 ddgmail-0.1.0/ddgmail.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 15:38:25.000000 ddgmail-0.1.0/ddgmail.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-12 15:38:25.000000 ddgmail-0.1.0/ddgmail.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2023-06-12 15:38:25.000000 ddgmail-0.1.0/ddgmail.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-12 15:38:25.000000 ddgmail-0.1.0/ddgmail.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4160 2023-06-12 15:36:16.000000 ddgmail-0.1.0/ddgmail.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 15:38:25.761646 ddgmail-0.1.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1179 2023-06-12 15:38:17.000000 ddgmail-0.1.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 15:39:48.518304 ddgmail-0.1.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.1/.gitignore
+-rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.1/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.1/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 15:39:48.518304 ddgmail-0.1.1/PKG-INFO
+-rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.1/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 15:39:48.518304 ddgmail-0.1.1/ddgmail.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 15:39:48.000000 ddgmail-0.1.1/ddgmail.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      256 2023-06-12 15:39:48.000000 ddgmail-0.1.1/ddgmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 15:39:48.000000 ddgmail-0.1.1/ddgmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-12 15:39:48.000000 ddgmail-0.1.1/ddgmail.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2023-06-12 15:39:48.000000 ddgmail-0.1.1/ddgmail.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-12 15:39:48.000000 ddgmail-0.1.1/ddgmail.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     4160 2023-06-12 15:36:16.000000 ddgmail-0.1.1/ddgmail.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 15:39:48.518304 ddgmail-0.1.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1126 2023-06-12 15:39:42.000000 ddgmail-0.1.1/setup.py
```

### Comparing `ddgmail-0.1.0/.gitignore` & `ddgmail-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.0/LICENSE` & `ddgmail-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.0/ddgmail.py` & `ddgmail-0.1.1/ddgmail.py`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.0/setup.py` & `ddgmail-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 # This conditional isn't necessary, but it provides better error messages to
 # people who try to install this package with older versions of setuptools.
 if parse_version(setuptools_version) < parse_version(min_setuptools_version):
     raise RuntimeError(f"setuptools {min_setuptools_version}+ is required")
 
 setup(
     name="ddgmail",
-    version="0.1.0",
+    version="0.1.1",
     py_modules=["ddgmail"],
-    license='GNU General Public License v3 (GPLv3)',
     author='rany',
     author_email='ranygh@riseup.net',
     url='https://github.com/rany2/ddgmail',
     description="A command line tool to use DuckDuckGo's E-mail forwarding service",
     install_requires=[
         "Click",
         f"setuptools>={min_setuptools_version}",
```

