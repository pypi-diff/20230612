# Comparing `tmp/pm20_3-0.2.tar.gz` & `tmp/pm20_3-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm20_3-0.2.tar", last modified: Mon Jun 12 18:32:23 2023, max compression
+gzip compressed data, was "pm20_3-0.3.tar", last modified: Mon Jun 12 18:39:12 2023, max compression
```

## Comparing `pm20_3-0.2.tar` & `pm20_3-0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:32:23.014044 pm20_3-0.2/
--rw-rw-rw-   0        0        0      993 2023-06-12 18:32:23.014044 pm20_3-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 18:32:23.014044 pm20_3-0.2/pm20_3/
--rw-rw-rw-   0        0        0       37 2023-06-12 16:30:23.669995 pm20_3-0.2/pm20_3/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-06-12 18:30:45.253599 pm20_3-0.2/pm20_3/questions.py
--rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1883 2023-06-12 18:31:15.458788 pm20_3-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:39:12.623762 pm20_3-0.3/
+-rw-rw-rw-   0        0        0      993 2023-06-12 18:39:12.624735 pm20_3-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 18:39:12.623762 pm20_3-0.3/pm20_3/
+-rw-rw-rw-   0        0        0       37 2023-06-12 16:30:23.669995 pm20_3-0.3/pm20_3/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-06-12 18:30:45.253599 pm20_3-0.3/pm20_3/questions.py
+-rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2023-06-12 18:38:19.837998 pm20_3-0.3/setup.py
```

### Comparing `pm20_3-0.2/PKG-INFO` & `pm20_3-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pm20_3
-Version: 0.2
+Version: 0.3
 Summary: For cheating again..
 Home-page: http://www.fa.ru/Pages/Home.aspx
 Author: Anatoliy Nesterov
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `pm20_3-0.2/pm20_3/questions.py` & `pm20_3-0.3/pm20_3/questions.py`

 * *Files identical despite different names*

### Comparing `pm20_3-0.2/setup.py` & `pm20_3-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='pm20_3',  # How you named your package folder (MyLib)
     packages=['pm20_3'],  # Chose the same as "name"
-    version='0.2',  # Start with a small number and increase it with every change you make
+    version='0.3',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='For cheating again..',  # Give a short description about your library
     author='Anatoliy Nesterov',  # Type in your name
     author_email='your.email@domain.com',  # Type in your E-Mail
     url='http://www.fa.ru/Pages/Home.aspx',  # Provide either the link to your github or to your website
     download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     keywords=['CHEATING'],  # Keywords that define your package best
@@ -28,8 +28,9 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
+    include_package_data=True
 )
```

