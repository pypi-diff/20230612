# Comparing `tmp/pm20_3-0.1.tar.gz` & `tmp/pm20_3-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm20_3-0.1.tar", last modified: Mon Jun 12 18:19:30 2023, max compression
+gzip compressed data, was "pm20_3-0.2.tar", last modified: Mon Jun 12 18:32:23 2023, max compression
```

## Comparing `pm20_3-0.1.tar` & `pm20_3-0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:19:30.028755 pm20_3-0.1/
--rw-rw-rw-   0        0        0      993 2023-06-12 18:19:30.028755 pm20_3-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 18:19:30.028755 pm20_3-0.1/pm20_3/
--rw-rw-rw-   0        0        0       37 2023-06-12 16:30:23.669995 pm20_3-0.1/pm20_3/__init__.py
--rw-rw-rw-   0        0        0     1591 2023-06-12 17:03:09.939809 pm20_3-0.1/pm20_3/questions.py
--rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1883 2023-06-12 18:01:25.878051 pm20_3-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:32:23.014044 pm20_3-0.2/
+-rw-rw-rw-   0        0        0      993 2023-06-12 18:32:23.014044 pm20_3-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 18:32:23.014044 pm20_3-0.2/pm20_3/
+-rw-rw-rw-   0        0        0       37 2023-06-12 16:30:23.669995 pm20_3-0.2/pm20_3/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-06-12 18:30:45.253599 pm20_3-0.2/pm20_3/questions.py
+-rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1883 2023-06-12 18:31:15.458788 pm20_3-0.2/setup.py
```

### Comparing `pm20_3-0.1/PKG-INFO` & `pm20_3-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pm20_3
-Version: 0.1
+Version: 0.2
 Summary: For cheating again..
 Home-page: http://www.fa.ru/Pages/Home.aspx
 Author: Anatoliy Nesterov
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `pm20_3-0.1/setup.py` & `pm20_3-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='pm20_3',  # How you named your package folder (MyLib)
     packages=['pm20_3'],  # Chose the same as "name"
-    version='0.1',  # Start with a small number and increase it with every change you make
+    version='0.2',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='For cheating again..',  # Give a short description about your library
     author='Anatoliy Nesterov',  # Type in your name
     author_email='your.email@domain.com',  # Type in your E-Mail
     url='http://www.fa.ru/Pages/Home.aspx',  # Provide either the link to your github or to your website
     download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     keywords=['CHEATING'],  # Keywords that define your package best
```

