# Comparing `tmp/djsm-0.0.1.tar.gz` & `tmp/djsm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsm-0.0.1.tar", last modified: Sun Jun 11 22:05:12 2023, max compression
+gzip compressed data, was "djsm-0.0.2.tar", last modified: Sun Jun 11 22:49:31 2023, max compression
```

## Comparing `djsm-0.0.1.tar` & `djsm-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 22:05:12.016867 djsm-0.0.1/
--rw-rw-rw-   0        0        0     1104 2023-06-04 21:28:33.000000 djsm-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    12496 2023-06-11 22:05:12.010868 djsm-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    11652 2023-06-11 22:00:56.000000 djsm-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 22:05:11.909866 djsm-0.0.1/djsm/
--rw-rw-rw-   0        0        0      625 2023-06-11 21:51:55.000000 djsm-0.0.1/djsm/__init__.py
--rw-rw-rw-   0        0        0     7999 2023-06-10 07:29:05.000000 djsm-0.0.1/djsm/crypt.py
--rw-rw-rw-   0        0        0     7337 2023-06-09 21:21:42.000000 djsm-0.0.1/djsm/jcrypt.py
--rw-rw-rw-   0        0        0    14305 2023-06-11 21:46:36.000000 djsm-0.0.1/djsm/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-11 22:05:11.999872 djsm-0.0.1/djsm.egg-info/
--rw-rw-rw-   0        0        0    12496 2023-06-11 22:05:11.000000 djsm-0.0.1/djsm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-11 22:05:11.000000 djsm-0.0.1/djsm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 22:05:11.000000 djsm-0.0.1/djsm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-11 22:05:11.000000 djsm-0.0.1/djsm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-11 22:05:11.000000 djsm-0.0.1/djsm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1041 2023-06-11 22:03:26.000000 djsm-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 22:05:12.017868 djsm-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 22:49:31.397903 djsm-0.0.2/
+-rw-rw-rw-   0        0        0     1104 2023-06-04 21:28:33.000000 djsm-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    13029 2023-06-11 22:49:31.392865 djsm-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12185 2023-06-11 22:46:37.000000 djsm-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 22:49:31.275296 djsm-0.0.2/djsm/
+-rw-rw-rw-   0        0        0      625 2023-06-11 22:47:50.000000 djsm-0.0.2/djsm/__init__.py
+-rw-rw-rw-   0        0        0     7999 2023-06-10 07:29:05.000000 djsm-0.0.2/djsm/crypt.py
+-rw-rw-rw-   0        0        0     7337 2023-06-09 21:21:42.000000 djsm-0.0.2/djsm/jcrypt.py
+-rw-rw-rw-   0        0        0    14305 2023-06-11 21:46:36.000000 djsm-0.0.2/djsm/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:49:31.386858 djsm-0.0.2/djsm.egg-info/
+-rw-rw-rw-   0        0        0    13029 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1041 2023-06-11 22:47:43.000000 djsm-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 22:49:31.398900 djsm-0.0.2/setup.cfg
```

### Comparing `djsm-0.0.1/LICENSE` & `djsm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djsm-0.0.1/PKG-INFO` & `djsm-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.0.1
+Version: 0.0.2
 Summary: DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
@@ -32,24 +32,48 @@
 
 ```bash
 pip install djsm
 ```
 
 * Initial setup:
 
-Copy this into a .env file in your project (adjust as needed)
+Copy this into a .env file just outside your project (adjust as needed)
 
 ```.env
 DJSM_SECRETS_FILE_PATH = ".hidden_folder/pathtofile/secrets_file.json"
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
 DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
 ```
 
+Your project structure should look like this:
+
+```bash
+├── my_project
+│   ├── my_project
+|   |   ├── __init__.py
+|   |   ├── settings.py
+|   |   ├── urls.py
+|   |   └── wsgi.py
+|   |
+│   ├── my_app
+|       ├── __init__.py 
+|       ├── admin.py
+|       ├── apps.py
+|       ├── models.py
+|       ├── tests.py
+|       └── views.py                 
+├── venv
+├── .env
+├── .gitignore
+├── manage.py
+└── requirements.txt
+```
+
 * Import the package in your Django project
 
 In settings.py
 
 ```python
 import djsm
 ```
@@ -60,15 +84,15 @@
 python manage.py runserver
 ```
 
 If everything was setup successfully, you should see "Setup OK!" on the terminal.
 
 ## Usage
 
-Before starting, a '.env' file as to be created somewhere in the django project directory(preferably the root directory).
+Before starting, a '.env' file as to be created just outside the django project directory.
 In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
 SECRETS_FILE_PATH = ".secrets/pathtofile/secrets.json"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djsm-0.0.1/README.md` & `djsm-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,48 @@
 
 ```bash
 pip install djsm
 ```
 
 * Initial setup:
 
-Copy this into a .env file in your project (adjust as needed)
+Copy this into a .env file just outside your project (adjust as needed)
 
 ```.env
 DJSM_SECRETS_FILE_PATH = ".hidden_folder/pathtofile/secrets_file.json"
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
 DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
 ```
 
+Your project structure should look like this:
+
+```bash
+├── my_project
+│   ├── my_project
+|   |   ├── __init__.py
+|   |   ├── settings.py
+|   |   ├── urls.py
+|   |   └── wsgi.py
+|   |
+│   ├── my_app
+|       ├── __init__.py 
+|       ├── admin.py
+|       ├── apps.py
+|       ├── models.py
+|       ├── tests.py
+|       └── views.py                 
+├── venv
+├── .env
+├── .gitignore
+├── manage.py
+└── requirements.txt
+```
+
 * Import the package in your Django project
 
 In settings.py
 
 ```python
 import djsm
 ```
@@ -41,15 +65,15 @@
 python manage.py runserver
 ```
 
 If everything was setup successfully, you should see "Setup OK!" on the terminal.
 
 ## Usage
 
-Before starting, a '.env' file as to be created somewhere in the django project directory(preferably the root directory).
+Before starting, a '.env' file as to be created just outside the django project directory.
 In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
 SECRETS_FILE_PATH = ".secrets/pathtofile/secrets.json"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djsm-0.0.1/djsm/__init__.py` & `djsm-0.0.2/djsm/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 djsm - Django JSON Secrets Manager
 ==================================
 djsm helps create, store, retrieve, update and manage secrets in Django
 
 LICENSE: MIT
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "ti-oluwa"
 __license__ = "MIT"
 
 import os
 import sys
 
 from .manager import DjangoJSONSecretManager as DJSM
```

### Comparing `djsm-0.0.1/djsm/crypt.py` & `djsm-0.0.2/djsm/crypt.py`

 * *Files identical despite different names*

### Comparing `djsm-0.0.1/djsm/jcrypt.py` & `djsm-0.0.2/djsm/jcrypt.py`

 * *Files identical despite different names*

### Comparing `djsm-0.0.1/djsm/manager.py` & `djsm-0.0.2/djsm/manager.py`

 * *Files identical despite different names*

### Comparing `djsm-0.0.1/djsm.egg-info/PKG-INFO` & `djsm-0.0.2/djsm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.0.1
+Version: 0.0.2
 Summary: DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
@@ -32,24 +32,48 @@
 
 ```bash
 pip install djsm
 ```
 
 * Initial setup:
 
-Copy this into a .env file in your project (adjust as needed)
+Copy this into a .env file just outside your project (adjust as needed)
 
 ```.env
 DJSM_SECRETS_FILE_PATH = ".hidden_folder/pathtofile/secrets_file.json"
 
 # NOT MANDATORY
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
 DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
 ```
 
+Your project structure should look like this:
+
+```bash
+├── my_project
+│   ├── my_project
+|   |   ├── __init__.py
+|   |   ├── settings.py
+|   |   ├── urls.py
+|   |   └── wsgi.py
+|   |
+│   ├── my_app
+|       ├── __init__.py 
+|       ├── admin.py
+|       ├── apps.py
+|       ├── models.py
+|       ├── tests.py
+|       └── views.py                 
+├── venv
+├── .env
+├── .gitignore
+├── manage.py
+└── requirements.txt
+```
+
 * Import the package in your Django project
 
 In settings.py
 
 ```python
 import djsm
 ```
@@ -60,15 +84,15 @@
 python manage.py runserver
 ```
 
 If everything was setup successfully, you should see "Setup OK!" on the terminal.
 
 ## Usage
 
-Before starting, a '.env' file as to be created somewhere in the django project directory(preferably the root directory).
+Before starting, a '.env' file as to be created just outside the django project directory.
 In the file, the following should be added;
 
 * **`DJSM_SECRETS_FILE_PATH`** -> Path(preferably absolute) to file where all secrets will be stored.
 Example:
 
 ```.env
 SECRETS_FILE_PATH = ".secrets/pathtofile/secrets.json"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djsm-0.0.1/pyproject.toml` & `djsm-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djsm"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project."
```

