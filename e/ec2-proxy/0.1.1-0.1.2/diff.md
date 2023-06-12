# Comparing `tmp/ec2_proxy-0.1.1.tar.gz` & `tmp/ec2_proxy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2_proxy-0.1.1.tar", last modified: Fri Jun  2 08:40:20 2023, max compression
+gzip compressed data, was "ec2_proxy-0.1.2.tar", last modified: Mon Jun 12 00:32:42 2023, max compression
```

## Comparing `ec2_proxy-0.1.1.tar` & `ec2_proxy-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.233797 ec2_proxy-0.1.1/
--rw-rw-rw-   0        0        0     3670 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-06-02 08:40:17.000000 ec2_proxy-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0      599 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      252 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1851 2023-06-02 08:40:20.234803 ec2_proxy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      965 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.208786 ec2_proxy-0.1.1/docs/
--rw-rw-rw-   0        0        0      630 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0     4963 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/history.rst
--rw-rw-rw-   0        0        0      314 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     1173 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/installation.rst
--rwxrwxrwx   0        0        0      807 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/readme.rst
--rw-rw-rw-   0        0        0       80 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.212792 ec2_proxy-0.1.1/ec2_proxy/
--rw-rw-rw-   0        0        0      174 2023-06-02 08:40:13.000000 ec2_proxy-0.1.1/ec2_proxy/__init__.py
--rw-rw-rw-   0        0        0     4964 2023-06-02 06:46:49.000000 ec2_proxy-0.1.1/ec2_proxy/ec2_proxy.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.229786 ec2_proxy-0.1.1/ec2_proxy.egg-info/
--rw-rw-rw-   0        0        0     1851 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 06:44:25.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-06-02 08:40:20.000000 ec2_proxy-0.1.1/ec2_proxy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      404 2023-06-02 08:40:20.236796 ec2_proxy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1368 2023-06-02 08:40:10.000000 ec2_proxy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:40:20.232800 ec2_proxy-0.1.1/tests/
--rw-rw-rw-   0        0        0       40 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      418 2023-06-02 06:40:47.000000 ec2_proxy-0.1.1/tests/test_ec2_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:32:42.703882 ec2_proxy-0.1.2/
+-rw-rw-rw-   0        0        0     3670 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       29 2023-06-12 00:32:39.000000 ec2_proxy-0.1.2/HISTORY.rst
+-rw-rw-rw-   0        0        0      599 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-06-12 00:17:33.000000 ec2_proxy-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2735 2023-06-12 00:32:42.703882 ec2_proxy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1897 2023-06-12 00:23:46.000000 ec2_proxy-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 00:32:42.677809 ec2_proxy-0.1.2/docs/
+-rw-rw-rw-   0        0        0      630 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/Makefile
+-rw-rw-rw-   0        0        0     4963 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/history.rst
+-rw-rw-rw-   0        0        0      314 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1173 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      807 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       80 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 00:32:42.681823 ec2_proxy-0.1.2/ec2_proxy/
+-rw-rw-rw-   0        0        0      174 2023-06-12 00:11:15.000000 ec2_proxy-0.1.2/ec2_proxy/__init__.py
+-rw-rw-rw-   0        0        0     4964 2023-06-02 06:46:49.000000 ec2_proxy-0.1.2/ec2_proxy/ec2_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:32:42.699405 ec2_proxy-0.1.2/ec2_proxy.egg-info/
+-rw-rw-rw-   0        0        0     2735 2023-06-12 00:32:42.000000 ec2_proxy-0.1.2/ec2_proxy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-06-12 00:32:42.000000 ec2_proxy-0.1.2/ec2_proxy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 00:32:42.000000 ec2_proxy-0.1.2/ec2_proxy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 06:44:25.000000 ec2_proxy-0.1.2/ec2_proxy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-12 00:32:42.000000 ec2_proxy-0.1.2/ec2_proxy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      703 2023-06-12 00:08:16.000000 ec2_proxy-0.1.2/proxy_setup.md
+-rw-rw-rw-   0        0        0      404 2023-06-12 00:32:42.705827 ec2_proxy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2023-06-12 00:25:28.000000 ec2_proxy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 00:32:42.702842 ec2_proxy-0.1.2/tests/
+-rw-rw-rw-   0        0        0       40 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-06-02 06:40:47.000000 ec2_proxy-0.1.2/tests/test_ec2_proxy.py
```

### Comparing `ec2_proxy-0.1.1/CONTRIBUTING.rst` & `ec2_proxy-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.1/LICENSE` & `ec2_proxy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.1/PKG-INFO` & `ec2_proxy-0.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ec2_proxy
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package provides ability to use amazon aws as proxy with everchanging IP.
 Home-page: https://github.com/AG4lyf/ec2_proxy
 Author: Suraj Bhari
 Author-email: surajbhari159@gmail.com
 License: Apache Software License 2.0
 Keywords: ec2_proxy
 Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
@@ -21,50 +21,72 @@
 
 =========
 EC2 Proxy
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/ec2_proxy.svg
-        :target: https://pypi.python.org/pypi/ec2_proxy
+   :target: https://pypi.python.org/pypi/ec2_proxy
 
 .. image:: https://img.shields.io/travis/AG4lyf/ec2_proxy.svg
-        :target: https://travis-ci.com/AG4lyf/ec2_proxy
+   :target: https://travis-ci.com/AG4lyf/ec2_proxy
 
 .. image:: https://readthedocs.org/projects/ec2-proxy/badge/?version=latest
-        :target: https://ec2-proxy.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
+   :target: https://ec2-proxy.readthedocs.io/en/latest/?version=latest
+   :alt: Documentation Status
 
 
-
-
-This package provides ability to use amazon aws as proxy with everchanging IP.
+This package provides the ability to use Amazon AWS as a proxy with ever-changing IP.
 
 
 * Free software: Apache Software License 2.0
 * Documentation: https://ec2-proxy.readthedocs.io.
 
+Install a Proxy Server
+======================
+Read `Setup </proxy_setup.md>`__ for instructions on how to install a proxy server on an EC2 instance.
+
+
+How to Use
+==========
+1. Install the package:
+      pip install ec2_proxy
+
+2. Create an AWS account and obtain the access key and secret key from `Here <https://us-east-1.console.aws.amazon.com/iamv2/home?region=us-east-1#/security_credentials/access-key-wizard>`__.
+
 
-Features
---------
+There are 2 ways to use this package:
 
-* TODO
+Way #1 - Use it with the credentials that are present in your `.aws` folder in your home directory
 
-Credits
--------
+.. code-block:: python
 
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+      from ec2_proxy import TProxy
 
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+      tp = TProxy(<instance_id_here>)
+      ip = tp.start()
+      print(ip)
+
+Way #2 - Use it with the credentials that you will pass at runtime
+
+.. code-block:: python
+
+      from ec2_proxy import TProxy
+      from botocore.config import Config
+      import boto3
+
+      region = 'us-west-2'
+      access_key_id = 'YOUR_ACCESS_KEY_ID'
+      secret_access_key = 'YOUR_SECRET_ACCESS_KEY'
+
+      ec2 = boto3.client('ec2', region_name=region, aws_access_key_id=access_key_id, aws_secret_access_key=secret_access_key)
+      tp = TProxy(<instance_id_here>, ec2=ec2)
+      ip = tp.start()
+      print(ip)
 
 
 =======
 History
 =======
 
-0.1.0 (2023-06-02)
-------------------
-
-* First release on PyPI.
```

### Comparing `ec2_proxy-0.1.1/docs/Makefile` & `ec2_proxy-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.1/docs/conf.py` & `ec2_proxy-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.1/docs/installation.rst` & `ec2_proxy-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.1/docs/make.bat` & `ec2_proxy-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.1/ec2_proxy/ec2_proxy.py` & `ec2_proxy-0.1.2/ec2_proxy/ec2_proxy.py`

 * *Files identical despite different names*

### Comparing `ec2_proxy-0.1.1/setup.py` & `ec2_proxy-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 test_requirements = [ ]
 
 setup(
     author="Suraj Bhari",
     author_email='surajbhari159@gmail.com',
     python_requires='>=3.6',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Information Technology',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='ec2_proxy',
     name='ec2_proxy',
     packages=find_packages(include=['ec2_proxy', 'ec2_proxy.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/AG4lyf/ec2_proxy',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

