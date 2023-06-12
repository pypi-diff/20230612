# Comparing `tmp/justpass-me-django-3.0.5b1.tar.gz` & `tmp/justpass-me-django-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justpass-me-django-3.0.5b1.tar", last modified: Fri Jun  9 14:03:31 2023, max compression
+gzip compressed data, was "justpass-me-django-3.1.0.tar", last modified: Mon Jun 12 18:56:59 2023, max compression
```

## Comparing `justpass-me-django-3.0.5b1.tar` & `justpass-me-django-3.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4911 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3648 2023-05-18 19:36:39.000000 justpass-me-django-3.0.5b1/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4911 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      456 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 16:54:06.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       58 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-06-09 14:03:30.000000 justpass-me-django-3.0.5b1/justpass_me_django.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/justpassme/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7896 2023-06-09 13:58:06.000000 justpass-me-django-3.0.5b1/justpassme/OIDC_CLIENT.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/admin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/apps.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-15 17:40:25.000000 justpass-me-django-3.0.5b1/justpassme/helpers.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-15 17:54:17.000000 justpass-me-django-3.0.5b1/justpassme/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 16:53:18.000000 justpass-me-django-3.0.5b1/justpassme/utils.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-15 17:42:22.000000 justpass-me-django-3.0.5b1/justpassme/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1690 2023-06-09 14:03:23.000000 justpass-me-django-3.0.5b1/setup-3.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-06-09 14:03:31.061977 justpass-me-django-3.0.5b1/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1690 2023-06-09 14:03:23.000000 justpass-me-django-3.0.5b1/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-12 18:56:59.466025 justpass-me-django-3.1.0/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 16:53:18.000000 justpass-me-django-3.1.0/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4902 2023-06-12 18:56:59.466025 justpass-me-django-3.1.0/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3648 2023-05-18 19:36:39.000000 justpass-me-django-3.1.0/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-12 18:56:59.465025 justpass-me-django-3.1.0/justpass_me_django.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4902 2023-06-12 18:56:59.000000 justpass-me-django-3.1.0/justpass_me_django.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      456 2023-06-12 18:56:59.000000 justpass-me-django-3.1.0/justpass_me_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-06-12 18:56:59.000000 justpass-me-django-3.1.0/justpass_me_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 16:54:06.000000 justpass-me-django-3.1.0/justpass_me_django.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       58 2023-06-12 18:56:59.000000 justpass-me-django-3.1.0/justpass_me_django.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-06-12 18:56:59.000000 justpass-me-django-3.1.0/justpass_me_django.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-06-12 18:56:59.466025 justpass-me-django-3.1.0/justpassme/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     7896 2023-06-09 13:58:06.000000 justpass-me-django-3.1.0/justpassme/OIDC_CLIENT.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 16:53:18.000000 justpass-me-django-3.1.0/justpassme/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 16:53:18.000000 justpass-me-django-3.1.0/justpassme/admin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 16:53:18.000000 justpass-me-django-3.1.0/justpassme/apps.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1096 2023-05-15 17:40:25.000000 justpass-me-django-3.1.0/justpassme/helpers.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      672 2023-05-15 17:54:17.000000 justpass-me-django-3.1.0/justpassme/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 16:53:18.000000 justpass-me-django-3.1.0/justpassme/utils.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      968 2023-05-15 17:42:22.000000 justpass-me-django-3.1.0/justpassme/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1688 2023-06-12 18:49:07.000000 justpass-me-django-3.1.0/setup-3.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-06-12 18:56:59.466025 justpass-me-django-3.1.0/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1688 2023-06-12 18:49:07.000000 justpass-me-django-3.1.0/setup.py
```

### Comparing `justpass-me-django-3.0.5b1/LICENSE` & `justpass-me-django-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.5b1/PKG-INFO` & `justpass-me-django-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.5b1
+Version: 3.1.0
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
+Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
-Download-URL: https://github.com/justpass-me/justpass-me-django
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -140,9 +139,7 @@
 
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
-
-
```

### Comparing `justpass-me-django-3.0.5b1/README.md` & `justpass-me-django-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.5b1/justpass_me_django.egg-info/PKG-INFO` & `justpass-me-django-3.1.0/justpass_me_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 3.0.5b1
+Version: 3.1.0
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
+Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
-Download-URL: https://github.com/justpass-me/justpass-me-django
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -140,9 +139,7 @@
 
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
-
-
```

### Comparing `justpass-me-django-3.0.5b1/justpassme/OIDC_CLIENT.py` & `justpass-me-django-3.1.0/justpassme/OIDC_CLIENT.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.5b1/justpassme/helpers.py` & `justpass-me-django-3.1.0/justpassme/helpers.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.5b1/justpassme/urls.py` & `justpass-me-django-3.1.0/justpassme/urls.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.5b1/justpassme/views.py` & `justpass-me-django-3.1.0/justpassme/views.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-3.0.5b1/setup-3.py` & `justpass-me-django-3.1.0/setup-3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='justpass-me-django',
-    version='3.0.5b1',
+    version='3.1.0',
     description='Django Integration with JustPass.me',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='JustPassMe',
     author_email = 'sameh@justpass.me',
     url = 'https://github.com/justpass-me/justpass-me-django',
     download_url='https://github.com/justpass-me/justpass-me-django',
@@ -19,16 +19,16 @@
         'mozilla-django-oidc==3.0.0',
         'python-jose==3.3.0'
       ],
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False, # because we're including static files
     classifiers=[
-        #"Development Status :: 5 - Production/Stable",
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
+        #"Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
```

### Comparing `justpass-me-django-3.0.5b1/setup.py` & `justpass-me-django-3.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='justpass-me-django',
-    version='3.0.5b1',
+    version='3.1.0',
     description='Django Integration with JustPass.me',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='JustPassMe',
     author_email = 'sameh@justpass.me',
     url = 'https://github.com/justpass-me/justpass-me-django',
     download_url='https://github.com/justpass-me/justpass-me-django',
@@ -19,16 +19,16 @@
         'mozilla-django-oidc==3.0.0',
         'python-jose==3.3.0'
       ],
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False, # because we're including static files
     classifiers=[
-        #"Development Status :: 5 - Production/Stable",
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
+        #"Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
```

