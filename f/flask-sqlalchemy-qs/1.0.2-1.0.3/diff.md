# Comparing `tmp/flask_sqlalchemy_qs-1.0.2.tar.gz` & `tmp/flask_sqlalchemy_qs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_sqlalchemy_qs-1.0.2.tar", last modified: Thu Jun  8 22:49:08 2023, max compression
+gzip compressed data, was "flask_sqlalchemy_qs-1.0.3.tar", last modified: Mon Jun 12 19:00:57 2023, max compression
```

## Comparing `flask_sqlalchemy_qs-1.0.2.tar` & `flask_sqlalchemy_qs-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-08 22:49:08.808504 flask_sqlalchemy_qs-1.0.2/
--rw-r--r--   0 marco      (501) staff       (20)     1083 2023-06-08 22:48:59.000000 flask_sqlalchemy_qs-1.0.2/LICENSE
--rw-r--r--   0 marco      (501) staff       (20)     5953 2023-06-08 22:49:08.808365 flask_sqlalchemy_qs-1.0.2/PKG-INFO
--rw-r--r--   0 marco      (501) staff       (20)     5384 2023-06-08 22:48:58.000000 flask_sqlalchemy_qs-1.0.2/README.md
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-08 22:49:08.807224 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs/
--rw-r--r--   0 marco      (501) staff       (20)      118 2023-06-06 17:53:38.000000 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs/__init__.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-08 22:49:08.807793 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs.egg-info/
--rw-r--r--   0 marco      (501) staff       (20)     5953 2023-06-08 22:49:08.000000 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs.egg-info/PKG-INFO
--rw-r--r--   0 marco      (501) staff       (20)      342 2023-06-08 22:49:08.000000 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs.egg-info/SOURCES.txt
--rw-r--r--   0 marco      (501) staff       (20)        1 2023-06-08 22:49:08.000000 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs.egg-info/dependency_links.txt
--rw-r--r--   0 marco      (501) staff       (20)       79 2023-06-08 22:49:08.000000 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs.egg-info/requires.txt
--rw-r--r--   0 marco      (501) staff       (20)       20 2023-06-08 22:49:08.000000 flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs.egg-info/top_level.txt
--rw-r--r--   0 marco      (501) staff       (20)       38 2023-06-08 22:49:08.808548 flask_sqlalchemy_qs-1.0.2/setup.cfg
--rw-r--r--   0 marco      (501) staff       (20)      923 2023-06-08 22:48:57.000000 flask_sqlalchemy_qs-1.0.2/setup.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-08 22:49:08.808153 flask_sqlalchemy_qs-1.0.2/tests/
--rw-r--r--   0 marco      (501) staff       (20)      722 2023-06-07 23:48:33.000000 flask_sqlalchemy_qs-1.0.2/tests/test_integration.py
--rw-r--r--   0 marco      (501) staff       (20)     6043 2023-06-06 04:36:10.000000 flask_sqlalchemy_qs-1.0.2/tests/test_qs_parser.py
--rw-r--r--   0 marco      (501) staff       (20)     6772 2023-06-06 14:10:19.000000 flask_sqlalchemy_qs-1.0.2/tests/test_query.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.699725 flask_sqlalchemy_qs-1.0.3/
+-rw-r--r--   0 marco      (501) staff       (20)     1083 2023-06-08 22:48:59.000000 flask_sqlalchemy_qs-1.0.3/LICENSE
+-rw-r--r--   0 marco      (501) staff       (20)     5953 2023-06-12 19:00:57.699610 flask_sqlalchemy_qs-1.0.3/PKG-INFO
+-rw-r--r--   0 marco      (501) staff       (20)     5384 2023-06-12 17:46:16.000000 flask_sqlalchemy_qs-1.0.3/README.md
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.697407 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/
+-rw-r--r--   0 marco      (501) staff       (20)      118 2023-06-06 17:53:38.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/__init__.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.698321 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/qs_parser/
+-rw-r--r--   0 marco      (501) staff       (20)     3683 2023-06-07 23:35:08.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/qs_parser/main.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.698544 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/
+-rw-r--r--   0 marco      (501) staff       (20)      770 2023-06-12 17:46:23.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/constants.py
+-rw-r--r--   0 marco      (501) staff       (20)     8695 2023-06-12 17:46:54.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/model.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.698216 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/
+-rw-r--r--   0 marco      (501) staff       (20)     5953 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/PKG-INFO
+-rw-r--r--   0 marco      (501) staff       (20)      454 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/SOURCES.txt
+-rw-r--r--   0 marco      (501) staff       (20)        1 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/dependency_links.txt
+-rw-r--r--   0 marco      (501) staff       (20)       79 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/requires.txt
+-rw-r--r--   0 marco      (501) staff       (20)       20 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/top_level.txt
+-rw-r--r--   0 marco      (501) staff       (20)       38 2023-06-12 19:00:57.699761 flask_sqlalchemy_qs-1.0.3/setup.cfg
+-rw-r--r--   0 marco      (501) staff       (20)      985 2023-06-12 18:59:42.000000 flask_sqlalchemy_qs-1.0.3/setup.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.699272 flask_sqlalchemy_qs-1.0.3/tests/
+-rw-r--r--   0 marco      (501) staff       (20)      722 2023-06-07 23:48:33.000000 flask_sqlalchemy_qs-1.0.3/tests/test_integration.py
+-rw-r--r--   0 marco      (501) staff       (20)     6043 2023-06-06 04:36:10.000000 flask_sqlalchemy_qs-1.0.3/tests/test_qs_parser.py
+-rw-r--r--   0 marco      (501) staff       (20)     6772 2023-06-06 14:10:19.000000 flask_sqlalchemy_qs-1.0.3/tests/test_query.py
```

### Comparing `flask_sqlalchemy_qs-1.0.2/LICENSE` & `flask_sqlalchemy_qs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_qs-1.0.2/PKG-INFO` & `flask_sqlalchemy_qs-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_sqlalchemy_qs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate and manipulatew SQLAlchemy filters and sorts from query strings in the URL
 Home-page: https://github.com/marcogil93/flask-sqlalchemy-qs
 Author: Marco Gil
 Author-email: marcogil93@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -179,15 +179,15 @@
 
   results = query.all()
 
   ...
 ```
 
 ## Version
-1.0.2
+1.0.3
 
 ## Requirements 
 SQLALCHEMYSQLAlchemy~=2.0
 
 flask~=2.2
 
 flask-sqlalchemy~=3.0
```

### Comparing `flask_sqlalchemy_qs-1.0.2/README.md` & `flask_sqlalchemy_qs-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
   results = query.all()
 
   ...
 ```
 
 ## Version
-1.0.2
+1.0.3
 
 ## Requirements 
 SQLALCHEMYSQLAlchemy~=2.0
 
 flask~=2.2
 
 flask-sqlalchemy~=3.0
```

### Comparing `flask_sqlalchemy_qs-1.0.2/flask_sqlalchemy_qs.egg-info/PKG-INFO` & `flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-sqlalchemy-qs
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate and manipulatew SQLAlchemy filters and sorts from query strings in the URL
 Home-page: https://github.com/marcogil93/flask-sqlalchemy-qs
 Author: Marco Gil
 Author-email: marcogil93@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -179,15 +179,15 @@
 
   results = query.all()
 
   ...
 ```
 
 ## Version
-1.0.2
+1.0.3
 
 ## Requirements 
 SQLALCHEMYSQLAlchemy~=2.0
 
 flask~=2.2
 
 flask-sqlalchemy~=3.0
```

### Comparing `flask_sqlalchemy_qs-1.0.2/setup.py` & `flask_sqlalchemy_qs-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flask_sqlalchemy_qs",
-    version="1.0.2",
+    version="1.0.3",
     description="Generate and manipulatew SQLAlchemy filters and sorts from query strings in the URL",
-    packages=["flask_sqlalchemy_qs"],
+    packages=["flask_sqlalchemy_qs", "flask_sqlalchemy_qs.qs_parser", "flask_sqlalchemy_qs.query"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marcogil93/flask-sqlalchemy-qs",
     author="Marco Gil",
     author_email="marcogil93@gmail.com",
     license="MIT",
     classifiers=[
```

### Comparing `flask_sqlalchemy_qs-1.0.2/tests/test_integration.py` & `flask_sqlalchemy_qs-1.0.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_qs-1.0.2/tests/test_qs_parser.py` & `flask_sqlalchemy_qs-1.0.3/tests/test_qs_parser.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_qs-1.0.2/tests/test_query.py` & `flask_sqlalchemy_qs-1.0.3/tests/test_query.py`

 * *Files identical despite different names*

