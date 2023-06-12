# Comparing `tmp/flask_signing-0.1.0.tar.gz` & `tmp/flask_signing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.1.0.tar", last modified: Mon Jun 12 15:47:20 2023, max compression
+gzip compressed data, was "flask_signing-0.2.0.tar", last modified: Mon Jun 12 20:08:18 2023, max compression
```

## Comparing `flask_signing-0.1.0.tar` & `flask_signing-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 15:47:20.948574 flask_signing-0.1.0/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.1.0/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)      690 2023-06-12 15:47:20.948574 flask_signing-0.1.0/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     2478 2023-06-12 15:27:23.000000 flask_signing-0.1.0/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 15:47:20.948574 flask_signing-0.1.0/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)     8156 2023-06-12 14:37:45.000000 flask_signing-0.1.0/flask_signing/__init__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 15:47:20.948574 flask_signing-0.1.0/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)      690 2023-06-12 15:47:20.000000 flask_signing-0.1.0/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      264 2023-06-12 15:47:20.000000 flask_signing-0.1.0/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-12 15:47:20.000000 flask_signing-0.1.0/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-12 15:47:20.000000 flask_signing-0.1.0/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-12 15:47:20.000000 flask_signing-0.1.0/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-12 15:47:20.948574 flask_signing-0.1.0/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)      869 2023-06-12 15:47:08.000000 flask_signing-0.1.0/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 15:47:20.948574 flask_signing-0.1.0/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     2996 2023-06-12 14:35:39.000000 flask_signing-0.1.0/tests/test_flask_signing.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.172595 flask_signing-0.2.0/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.2.0/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)      690 2023-06-12 20:08:18.172595 flask_signing-0.2.0/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2736 2023-06-12 15:59:14.000000 flask_signing-0.2.0/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.168594 flask_signing-0.2.0/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     8210 2023-06-12 20:07:03.000000 flask_signing-0.2.0/flask_signing/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.168594 flask_signing-0.2.0/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)      690 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      264 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-12 20:08:18.172595 flask_signing-0.2.0/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)      869 2023-06-12 20:07:00.000000 flask_signing-0.2.0/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.172595 flask_signing-0.2.0/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2996 2023-06-12 14:35:39.000000 flask_signing-0.2.0/tests/test_flask_signing.py
```

### Comparing `flask_signing-0.1.0/LICENSE` & `flask_signing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.1.0/PKG-INFO` & `flask_signing-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_signing
-Version: 0.1.0
+Version: 0.2.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask_signing-0.1.0/README.md` & `flask_signing-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
+[![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
 
 ## Flask-Signing
 a signing key extension for flask
```

### Comparing `flask_signing-0.1.0/flask_signing/__init__.py` & `flask_signing-0.2.0/flask_signing/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
 from flask_sqlalchemy import SQLAlchemy
-
+from typing import Union, List, Dict, Any
 
 class Signatures:
     """
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
     """
 
@@ -177,33 +177,41 @@
                 expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
 
             self._model = Signing
 
         return self._model
 
 
-    # def get_model(self):
-    #     class Signing(self.db.Model):
+    def query_keys(self, active:bool=None, scope:str=None, email:str=None) -> Union[List[Dict[str, Any]], bool]:
+        """
+        Query signing keys by active status, scope, and email.
 
-    #         """
-    #         The Signing class represents the Signing table in the database.
+        This function returns a list of signing keys that match the provided parameters.
+        If no keys are found, it returns False.
 
-    #         Each instance of this class represents a row of data in the database table.
+        Args:
+            active (bool, optional): The active status of the signing keys. Defaults to None.
+            scope (str, optional): The scope of the signing keys. Defaults to None.
+            email (str, optional): The email associated with the signing keys. Defaults to None.
 
-    #         Attributes:
-    #             signature (str): The primary key of the Signing table. This field is unique for each entry.
-    #             email (str): The email associated with a specific signing key.
-    #             scope (str): The scope within which the key is valid.
-    #             active (bool): The status of the signing key. If True, the key is active.
-    #             timestamp (datetime): The date and time when the signing key was created.
-    #             expiration (datetime): The date and time when the signing key is set to expire.
-    #         """
-    #         __tablename__ = 'signing'
-    #         signature = self.db.Column(self.db.String, primary_key=True) 
-    #         email = self.db.Column(self.db.String(100))
-    #         scope = self.db.Column(self.db.String(100))
-    #         active = self.db.Column(self.db.Boolean)
-    #         timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
-    #         expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
+        Returns:
+            Union[List[Dict[str, Any]], bool]: A list of dictionaries where each dictionary contains the details of a signing key,
+            or False if no keys are found.
+        """
 
-    #     return Signing
+        Signing = self.get_model()
+
+        query = Signing.query
+
+        if active is not None:
+            query = query.filter(Signing.active == active)
+        if scope:
+            query = query.filter(Signing.scope == scope)
+        if email:
+            query = query.filter(Signing.email == email)
+
+        result = query.all()
+
+        if not result:
+            return False
 
+        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in result]
```

### Comparing `flask_signing-0.1.0/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.2.0/flask_signing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-signing
-Version: 0.1.0
+Version: 0.2.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flask_signing-0.1.0/setup.py` & `flask_signing-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flask_signing',
-    version='0.1.0',
+    version='0.2.0',
     url='https://github.com/signebedi/Flask-Signing',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     description='a signing key extension for flask',
     packages=find_packages(),  
     install_requires=[
         'Flask<3.0.0',
```

### Comparing `flask_signing-0.1.0/tests/test_flask_signing.py` & `flask_signing-0.2.0/tests/test_flask_signing.py`

 * *Files identical despite different names*

