# Comparing `tmp/djsm-0.0.2.tar.gz` & `tmp/djsm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsm-0.0.2.tar", last modified: Sun Jun 11 22:49:31 2023, max compression
+gzip compressed data, was "djsm-0.0.3.tar", last modified: Mon Jun 12 07:57:11 2023, max compression
```

## Comparing `djsm-0.0.2.tar` & `djsm-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 22:49:31.397903 djsm-0.0.2/
--rw-rw-rw-   0        0        0     1104 2023-06-04 21:28:33.000000 djsm-0.0.2/LICENSE
--rw-rw-rw-   0        0        0    13029 2023-06-11 22:49:31.392865 djsm-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    12185 2023-06-11 22:46:37.000000 djsm-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 22:49:31.275296 djsm-0.0.2/djsm/
--rw-rw-rw-   0        0        0      625 2023-06-11 22:47:50.000000 djsm-0.0.2/djsm/__init__.py
--rw-rw-rw-   0        0        0     7999 2023-06-10 07:29:05.000000 djsm-0.0.2/djsm/crypt.py
--rw-rw-rw-   0        0        0     7337 2023-06-09 21:21:42.000000 djsm-0.0.2/djsm/jcrypt.py
--rw-rw-rw-   0        0        0    14305 2023-06-11 21:46:36.000000 djsm-0.0.2/djsm/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-11 22:49:31.386858 djsm-0.0.2/djsm.egg-info/
--rw-rw-rw-   0        0        0    13029 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-11 22:49:31.000000 djsm-0.0.2/djsm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1041 2023-06-11 22:47:43.000000 djsm-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 22:49:31.398900 djsm-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 07:57:11.667058 djsm-0.0.3/
+-rw-rw-rw-   0        0        0     1104 2023-06-04 21:28:33.000000 djsm-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0    12942 2023-06-12 07:57:11.661066 djsm-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12098 2023-06-12 07:42:42.000000 djsm-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 07:57:11.517455 djsm-0.0.3/djsm/
+-rw-rw-rw-   0        0        0      625 2023-06-12 07:55:20.000000 djsm-0.0.3/djsm/__init__.py
+-rw-rw-rw-   0        0        0     7999 2023-06-10 07:29:05.000000 djsm-0.0.3/djsm/crypt.py
+-rw-rw-rw-   0        0        0     7337 2023-06-09 21:21:42.000000 djsm-0.0.3/djsm/jcrypt.py
+-rw-rw-rw-   0        0        0    14349 2023-06-12 07:54:36.000000 djsm-0.0.3/djsm/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:57:11.656037 djsm-0.0.3/djsm.egg-info/
+-rw-rw-rw-   0        0        0    12942 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-12 07:57:11.000000 djsm-0.0.3/djsm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1041 2023-06-12 07:55:11.000000 djsm-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:57:11.668064 djsm-0.0.3/setup.cfg
```

### Comparing `djsm-0.0.2/LICENSE` & `djsm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djsm-0.0.2/PKG-INFO` & `djsm-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.0.2
+Version: 0.0.3
 Summary: DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DJSM - Django JSON Secrets Manager
 
 ## What is DJSM?
 
-DJSM is a light weight Python module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project. It provides a simple interface to access the secrets in a JSON file. DJSM uses Fernet encryption combined with RSA encryption to keep secrets secure.
+DJSM is a light weight Python module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project. DJSM uses Fernet encryption combined with RSA encryption to keep secrets secure.
 
 [View Project on PyPI](https://pypi.org/project/djsm/)
 
 
 ## Installation and Quick Setup
 
 * Install the package using pip
@@ -45,33 +45,38 @@
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
 DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
 ```
 
 Your project structure should look like this:
 
 ```bash
-├── my_project
-│   ├── my_project
-|   |   ├── __init__.py
-|   |   ├── settings.py
-|   |   ├── urls.py
-|   |   └── wsgi.py
+
+|-- my_project
+|   |-- my_project
+|   |   |-- __init__.py
+|   |   |-- settings.py
+|   |   |-- urls.py
+|   |   |-- wsgi.py
+|   |
+|   |-- my_app
+|   |   |-- __init__.py
+|   |   |-- admin.py
+|   |   |-- apps.py
+|   |   |-- models.py
+|   |   |-- tests.py
+|   |   |-- views.py
 |   |
-│   ├── my_app
-|       ├── __init__.py 
-|       ├── admin.py
-|       ├── apps.py
-|       ├── models.py
-|       ├── tests.py
-|       └── views.py                 
-├── venv
-├── .env
-├── .gitignore
-├── manage.py
-└── requirements.txt
+|   |-- db.sqlite3
+|   |-- manage.py
+|
+|-- venv
+|-- .env
+|-- .gitignore
+|-- requirements.py
+
 ```
 
 * Import the package in your Django project
 
 In settings.py
 
 ```python
@@ -216,19 +221,19 @@
 # update secrets
 new_secret = {"DB_PASSWORD": "new_db_password"}
 djsm.update_secrets(new_secret)
 
 # write secrets to a file
 path_to_secret_file = ".secrets/pathtofile/secrets.json"
 new_secret = {"API_KEY": "api_key"}
-djsm.write_secret(new_secret, path_to_secret_file, overwrite=True, encrypt=True)
+djsm.write_secrets(new_secret, path_to_secret_file, overwrite=True, encrypt=True)
 
 # load secrets from a file
 path_to_secret_file = ".secrets/pathtofile/secrets.json"
-secrets = djsm.load_secret(path_to_secret_file, decrypt=True)
+secrets = djsm.load_secrets(path_to_secret_file, decrypt=True)
 
 # encrypt a secret
 secret = {"API_KEY": "api_key"}
 encrypted_secret = djsm.encrypt(secret)
 
 # decrypt a secret
 decrypted_secret = djsm.decrypt(encrypted_secret)
@@ -272,15 +277,16 @@
 # Get key strings
 fernet_key_str, rsa_pub_key_str, rsa_priv_key_str = Crypt.generate_key_as_str()
 
 # Instantiating a Crypt object from keys
 crypt = Crypt(fernet_key, rsa_pub_key, rsa_priv_key, hash_algorithm="SHA-256")
 
 # Instantiating a Crypt object from key strings
-crypt = Crypt.from_str(fernet_key_str, rsa_pub_key_str, rsa_priv_key_str, hash_algorithm="SHA-256")
+crypt = Crypt.from_str(fernet_key_str, rsa_pub_key_str, rsa_priv_key_str, encoding: str = 'utf-8')
+crypt.hash_algorithm = "SHA-256"
 text = 'Text I want to keep secret.'
 
 # Encrypt text
 cipher_text = crypt.encrypt(text)
 print(cipher_text)
 
 # decrypt text
@@ -356,13 +362,14 @@
 
 #### NOTE: DJSM just provides an added layer of security in managing secrets in your application. It has not been tested to be completely attack proof
 
 ### CREDITS
 
 * [python-dotenv](https://pypi.org/project/python-dotenv/)
 * [cryptography](https://pypi.org/project/cryptography/)
+* [rsa](https://pypi.org/project/rsa/)
 
 #### Contributors and feedbacks are welcome. For feedbacks, please open an issue or contact me at tioluwa.dev@gmail.com or on twitter [@ti_oluwa_](https://twitter.com/ti_oluwa_)
 
 #### To contribute, please fork the repo and submit a pull request
 
 #### If you find this module useful, please consider giving it a star. Thanks!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `djsm-0.0.2/README.md` & `djsm-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # DJSM - Django JSON Secrets Manager
 
 ## What is DJSM?
 
-DJSM is a light weight Python module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project. It provides a simple interface to access the secrets in a JSON file. DJSM uses Fernet encryption combined with RSA encryption to keep secrets secure.
+DJSM is a light weight Python module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project. DJSM uses Fernet encryption combined with RSA encryption to keep secrets secure.
 
 [View Project on PyPI](https://pypi.org/project/djsm/)
 
 
 ## Installation and Quick Setup
 
 * Install the package using pip
@@ -26,33 +26,38 @@
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
 DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
 ```
 
 Your project structure should look like this:
 
 ```bash
-├── my_project
-│   ├── my_project
-|   |   ├── __init__.py
-|   |   ├── settings.py
-|   |   ├── urls.py
-|   |   └── wsgi.py
+
+|-- my_project
+|   |-- my_project
+|   |   |-- __init__.py
+|   |   |-- settings.py
+|   |   |-- urls.py
+|   |   |-- wsgi.py
+|   |
+|   |-- my_app
+|   |   |-- __init__.py
+|   |   |-- admin.py
+|   |   |-- apps.py
+|   |   |-- models.py
+|   |   |-- tests.py
+|   |   |-- views.py
 |   |
-│   ├── my_app
-|       ├── __init__.py 
-|       ├── admin.py
-|       ├── apps.py
-|       ├── models.py
-|       ├── tests.py
-|       └── views.py                 
-├── venv
-├── .env
-├── .gitignore
-├── manage.py
-└── requirements.txt
+|   |-- db.sqlite3
+|   |-- manage.py
+|
+|-- venv
+|-- .env
+|-- .gitignore
+|-- requirements.py
+
 ```
 
 * Import the package in your Django project
 
 In settings.py
 
 ```python
@@ -197,19 +202,19 @@
 # update secrets
 new_secret = {"DB_PASSWORD": "new_db_password"}
 djsm.update_secrets(new_secret)
 
 # write secrets to a file
 path_to_secret_file = ".secrets/pathtofile/secrets.json"
 new_secret = {"API_KEY": "api_key"}
-djsm.write_secret(new_secret, path_to_secret_file, overwrite=True, encrypt=True)
+djsm.write_secrets(new_secret, path_to_secret_file, overwrite=True, encrypt=True)
 
 # load secrets from a file
 path_to_secret_file = ".secrets/pathtofile/secrets.json"
-secrets = djsm.load_secret(path_to_secret_file, decrypt=True)
+secrets = djsm.load_secrets(path_to_secret_file, decrypt=True)
 
 # encrypt a secret
 secret = {"API_KEY": "api_key"}
 encrypted_secret = djsm.encrypt(secret)
 
 # decrypt a secret
 decrypted_secret = djsm.decrypt(encrypted_secret)
@@ -253,15 +258,16 @@
 # Get key strings
 fernet_key_str, rsa_pub_key_str, rsa_priv_key_str = Crypt.generate_key_as_str()
 
 # Instantiating a Crypt object from keys
 crypt = Crypt(fernet_key, rsa_pub_key, rsa_priv_key, hash_algorithm="SHA-256")
 
 # Instantiating a Crypt object from key strings
-crypt = Crypt.from_str(fernet_key_str, rsa_pub_key_str, rsa_priv_key_str, hash_algorithm="SHA-256")
+crypt = Crypt.from_str(fernet_key_str, rsa_pub_key_str, rsa_priv_key_str, encoding: str = 'utf-8')
+crypt.hash_algorithm = "SHA-256"
 text = 'Text I want to keep secret.'
 
 # Encrypt text
 cipher_text = crypt.encrypt(text)
 print(cipher_text)
 
 # decrypt text
@@ -337,13 +343,14 @@
 
 #### NOTE: DJSM just provides an added layer of security in managing secrets in your application. It has not been tested to be completely attack proof
 
 ### CREDITS
 
 * [python-dotenv](https://pypi.org/project/python-dotenv/)
 * [cryptography](https://pypi.org/project/cryptography/)
+* [rsa](https://pypi.org/project/rsa/)
 
 #### Contributors and feedbacks are welcome. For feedbacks, please open an issue or contact me at tioluwa.dev@gmail.com or on twitter [@ti_oluwa_](https://twitter.com/ti_oluwa_)
 
 #### To contribute, please fork the repo and submit a pull request
 
 #### If you find this module useful, please consider giving it a star. Thanks!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `djsm-0.0.2/djsm/__init__.py` & `djsm-0.0.3/djsm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 djsm - Django JSON Secrets Manager
 ==================================
 djsm helps create, store, retrieve, update and manage secrets in Django
 
 LICENSE: MIT
 """
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __author__ = "ti-oluwa"
 __license__ = "MIT"
 
 import os
 import sys
 
 from .manager import DjangoJSONSecretManager as DJSM
```

### Comparing `djsm-0.0.2/djsm/crypt.py` & `djsm-0.0.3/djsm/crypt.py`

 * *Files identical despite different names*

### Comparing `djsm-0.0.2/djsm/jcrypt.py` & `djsm-0.0.3/djsm/jcrypt.py`

 * *Files identical despite different names*

### Comparing `djsm-0.0.2/djsm/manager.py` & `djsm-0.0.3/djsm/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from bs4_web_scraper.file_handler import FileHandler
 import bs4_web_scraper
 import warnings
 from dotenv import load_dotenv, find_dotenv, dotenv_values
 import string
 import random
+from time import sleep
 
 from .jcrypt import JSONCrypt
 
 
 SECRET_KEY_ALLOWED_CHARS = string.ascii_letters + string.digits + string.punctuation
 
 env_variables = [
@@ -205,15 +206,17 @@
         for key, value in env_file_dict.items():
             line = f'{key} = "{value}"\n'
             env_file_handler.write_to_file(line, write_mode='a+')
         return env_file_handler.close_file()
 
 
     def change_crypt_keys(self):
-        """Change the encryption keys"""
+        """
+        Change the encryption keys
+        """
         # Get existing secrets
         secret_key = self.load_secrets(self.__django_secret_key_file_path, decrypt=True) if self.__django_secret_key_file_path else {}
         secrets = self.load_secrets(self.__path_to_secret_file, decrypt=True)
 
         # Delete fernet and rsa public keys in JSON file - Just delete the cryptkeys.json file
         FileHandler(self.__path_to_key_file).delete_file()
         # Delete crypt key in .env file
```

### Comparing `djsm-0.0.2/djsm.egg-info/PKG-INFO` & `djsm-0.0.3/djsm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsm
-Version: 0.0.2
+Version: 0.0.3
 Summary: DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project.
 Author-email: ti-oluwa <tioluwa.dev@gmail.com>
 Maintainer-email: ti-oluwa <tioluwa.dev@gmail.com>
 Project-URL: Homepage, https://github.com/ti-oluwa/djsm
 Project-URL: Bug Tracker, https://github.com/ti-oluwa/djsm/issues
 Project-URL: Repository, https://github.com/ti-oluwa/djsm
 Keywords: Django,Django Secrets Encryption
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DJSM - Django JSON Secrets Manager
 
 ## What is DJSM?
 
-DJSM is a light weight Python module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project. It provides a simple interface to access the secrets in a JSON file. DJSM uses Fernet encryption combined with RSA encryption to keep secrets secure.
+DJSM is a light weight Python module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project. DJSM uses Fernet encryption combined with RSA encryption to keep secrets secure.
 
 [View Project on PyPI](https://pypi.org/project/djsm/)
 
 
 ## Installation and Quick Setup
 
 * Install the package using pip
@@ -45,33 +45,38 @@
 DJSM_SECRET_KEY_NAME = "__secret_key_name__"
 DJSM_SECRET_KEY_FILE_PATH = ".hidden_folder/pathtofile/secret_key_file.json"
 ```
 
 Your project structure should look like this:
 
 ```bash
-├── my_project
-│   ├── my_project
-|   |   ├── __init__.py
-|   |   ├── settings.py
-|   |   ├── urls.py
-|   |   └── wsgi.py
+
+|-- my_project
+|   |-- my_project
+|   |   |-- __init__.py
+|   |   |-- settings.py
+|   |   |-- urls.py
+|   |   |-- wsgi.py
+|   |
+|   |-- my_app
+|   |   |-- __init__.py
+|   |   |-- admin.py
+|   |   |-- apps.py
+|   |   |-- models.py
+|   |   |-- tests.py
+|   |   |-- views.py
 |   |
-│   ├── my_app
-|       ├── __init__.py 
-|       ├── admin.py
-|       ├── apps.py
-|       ├── models.py
-|       ├── tests.py
-|       └── views.py                 
-├── venv
-├── .env
-├── .gitignore
-├── manage.py
-└── requirements.txt
+|   |-- db.sqlite3
+|   |-- manage.py
+|
+|-- venv
+|-- .env
+|-- .gitignore
+|-- requirements.py
+
 ```
 
 * Import the package in your Django project
 
 In settings.py
 
 ```python
@@ -216,19 +221,19 @@
 # update secrets
 new_secret = {"DB_PASSWORD": "new_db_password"}
 djsm.update_secrets(new_secret)
 
 # write secrets to a file
 path_to_secret_file = ".secrets/pathtofile/secrets.json"
 new_secret = {"API_KEY": "api_key"}
-djsm.write_secret(new_secret, path_to_secret_file, overwrite=True, encrypt=True)
+djsm.write_secrets(new_secret, path_to_secret_file, overwrite=True, encrypt=True)
 
 # load secrets from a file
 path_to_secret_file = ".secrets/pathtofile/secrets.json"
-secrets = djsm.load_secret(path_to_secret_file, decrypt=True)
+secrets = djsm.load_secrets(path_to_secret_file, decrypt=True)
 
 # encrypt a secret
 secret = {"API_KEY": "api_key"}
 encrypted_secret = djsm.encrypt(secret)
 
 # decrypt a secret
 decrypted_secret = djsm.decrypt(encrypted_secret)
@@ -272,15 +277,16 @@
 # Get key strings
 fernet_key_str, rsa_pub_key_str, rsa_priv_key_str = Crypt.generate_key_as_str()
 
 # Instantiating a Crypt object from keys
 crypt = Crypt(fernet_key, rsa_pub_key, rsa_priv_key, hash_algorithm="SHA-256")
 
 # Instantiating a Crypt object from key strings
-crypt = Crypt.from_str(fernet_key_str, rsa_pub_key_str, rsa_priv_key_str, hash_algorithm="SHA-256")
+crypt = Crypt.from_str(fernet_key_str, rsa_pub_key_str, rsa_priv_key_str, encoding: str = 'utf-8')
+crypt.hash_algorithm = "SHA-256"
 text = 'Text I want to keep secret.'
 
 # Encrypt text
 cipher_text = crypt.encrypt(text)
 print(cipher_text)
 
 # decrypt text
@@ -356,13 +362,14 @@
 
 #### NOTE: DJSM just provides an added layer of security in managing secrets in your application. It has not been tested to be completely attack proof
 
 ### CREDITS
 
 * [python-dotenv](https://pypi.org/project/python-dotenv/)
 * [cryptography](https://pypi.org/project/cryptography/)
+* [rsa](https://pypi.org/project/rsa/)
 
 #### Contributors and feedbacks are welcome. For feedbacks, please open an issue or contact me at tioluwa.dev@gmail.com or on twitter [@ti_oluwa_](https://twitter.com/ti_oluwa_)
 
 #### To contribute, please fork the repo and submit a pull request
 
 #### If you find this module useful, please consider giving it a star. Thanks!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `djsm-0.0.2/pyproject.toml` & `djsm-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djsm"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "DJSM is a light weight module that allows you to store secrets encrypted in a JSON file and access them easily in your Django project."
```

