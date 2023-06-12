# Comparing `tmp/django-splash-1.2.1.tar.gz` & `tmp/django-splash-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-splash-1.2.1.tar", last modified: Thu Jan 27 10:16:08 2022, max compression
+gzip compressed data, was "django-splash-1.3.0.tar", last modified: Mon Jun 12 13:19:48 2023, max compression
```

## Comparing `django-splash-1.2.1.tar` & `django-splash-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 10:16:08.733327 django-splash-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-01-27 10:16:04.000000 django-splash-1.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-01-27 10:16:04.000000 django-splash-1.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10177 2022-01-27 10:16:04.000000 django-splash-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-01-27 10:16:04.000000 django-splash-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-01-27 10:16:08.733327 django-splash-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-01-27 10:16:04.000000 django-splash-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 10:16:08.733327 django-splash-1.2.1/django_splash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-01-27 10:16:08.000000 django-splash-1.2.1/django_splash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-01-27 10:16:08.000000 django-splash-1.2.1/django_splash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 10:16:08.000000 django-splash-1.2.1/django_splash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 10:16:08.000000 django-splash-1.2.1/django_splash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-27 10:16:08.000000 django-splash-1.2.1/django_splash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-27 10:16:08.000000 django-splash-1.2.1/django_splash.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 10:16:08.733327 django-splash-1.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-01-27 10:16:04.000000 django-splash-1.2.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-01-27 10:16:08.733327 django-splash-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-01-27 10:16:04.000000 django-splash-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 10:16:08.733327 django-splash-1.2.1/splash/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-01-27 10:16:04.000000 django-splash-1.2.1/splash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-01-27 10:16:04.000000 django-splash-1.2.1/splash/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-01-27 10:16:04.000000 django-splash-1.2.1/splash/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 10:16:08.733327 django-splash-1.2.1/splash/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-01-27 10:16:04.000000 django-splash-1.2.1/splash/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-27 10:16:04.000000 django-splash-1.2.1/splash/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-01-27 10:16:04.000000 django-splash-1.2.1/splash/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:48.158086 django-splash-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-12 13:19:41.000000 django-splash-1.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-06-12 13:19:41.000000 django-splash-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10177 2023-06-12 13:19:41.000000 django-splash-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-06-12 13:19:41.000000 django-splash-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4959 2023-06-12 13:19:48.158086 django-splash-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3108 2023-06-12 13:19:41.000000 django-splash-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:48.158086 django-splash-1.3.0/django_splash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4959 2023-06-12 13:19:48.000000 django-splash-1.3.0/django_splash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-06-12 13:19:48.000000 django-splash-1.3.0/django_splash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 13:19:48.000000 django-splash-1.3.0/django_splash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 13:19:48.000000 django-splash-1.3.0/django_splash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-12 13:19:48.000000 django-splash-1.3.0/django_splash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-12 13:19:48.000000 django-splash-1.3.0/django_splash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:48.158086 django-splash-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-12 13:19:41.000000 django-splash-1.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-06-12 13:19:48.158086 django-splash-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-12 13:19:41.000000 django-splash-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:48.158086 django-splash-1.3.0/splash/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-12 13:19:41.000000 django-splash-1.3.0/splash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-06-12 13:19:41.000000 django-splash-1.3.0/splash/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-12 13:19:41.000000 django-splash-1.3.0/splash/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:48.158086 django-splash-1.3.0/splash/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1934 2023-06-12 13:19:41.000000 django-splash-1.3.0/splash/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:41.000000 django-splash-1.3.0/splash/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-06-12 13:19:41.000000 django-splash-1.3.0/splash/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 13:19:48.158086 django-splash-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8164 2023-06-12 13:19:41.000000 django-splash-1.3.0/tests/test_splash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5720 2023-06-12 13:19:41.000000 django-splash-1.3.0/tests/test_views.py
```

### Comparing `django-splash-1.2.1/CHANGELOG.rst` & `django-splash-1.3.0/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[1.3.0] - 2023-06-09
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Added 
+_____
+
+* Added Support for Django42.
+
 [1.2.0] - 2022-01-26
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Removed
 _______
 
 * Removed Support for Django22, 30, 31
```

### Comparing `django-splash-1.2.1/LICENSE.txt` & `django-splash-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-splash-1.2.1/PKG-INFO` & `django-splash-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: django-splash
-Version: 1.2.1
+Version: 1.3.0
 Summary: Splash screen middleware for Django apps
-Home-page: https://github.com/edx/django-splash
+Home-page: https://github.com/openedx/django-splash
 Author: edX
 Author-email: oscm@edx.org
 License: Apache Software License 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 License-File: AUTHORS
@@ -32,17 +32,17 @@
 --------
 
 Checks incoming requests, to redirect users to a configured splash screen URL
 if they don't have the proper cookie set. This can be used to display a small
 marketing landing page, protect an alpha website from the public eye, make an
 announcement, etc.
 
-Meant to be used with https://github.com/edx/edx-platform/ -- or you will need
+Meant to be used with https://github.com/openedx/edx-platform/ -- or you will need
 to import the config_models application to your Django application:
-https://github.com/edx/django-config-models
+https://github.com/openedx/django-config-models
 
 Installation
 ------------
 
 Add the application to the `INSTALLED_APPS`:
 
 ::
@@ -86,18 +86,16 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -109,28 +107,28 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/django-splash.svg
     :target: https://pypi.python.org/pypi/django-splash/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/django-splash/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/django-splash/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/django-splash/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/django-splash/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/django-splash/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/django-splash?branch=master
     :alt: Codecov
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/django-splash.svg
     :target: https://pypi.python.org/pypi/django-splash/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/django-splash.svg
-    :target: https://github.com/edx/django-splash/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/django-splash/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -144,14 +142,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[1.3.0] - 2023-06-09
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Added 
+_____
+
+* Added Support for Django42.
+
 [1.2.0] - 2022-01-26
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Removed
 _______
 
 * Removed Support for Django22, 30, 31
@@ -181,9 +187,7 @@
 [0.2.1] - 2018-02-07
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `django-splash-1.2.1/README.rst` & `django-splash-1.3.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------
 
 Checks incoming requests, to redirect users to a configured splash screen URL
 if they don't have the proper cookie set. This can be used to display a small
 marketing landing page, protect an alpha website from the public eye, make an
 announcement, etc.
 
-Meant to be used with https://github.com/edx/edx-platform/ -- or you will need
+Meant to be used with https://github.com/openedx/edx-platform/ -- or you will need
 to import the config_models application to your Django application:
-https://github.com/edx/django-config-models
+https://github.com/openedx/django-config-models
 
 Installation
 ------------
 
 Add the application to the `INSTALLED_APPS`:
 
 ::
@@ -64,18 +64,16 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -87,22 +85,22 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/django-splash.svg
     :target: https://pypi.python.org/pypi/django-splash/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/django-splash/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/django-splash/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/django-splash/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/django-splash/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/django-splash/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/django-splash?branch=master
     :alt: Codecov
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/django-splash.svg
     :target: https://pypi.python.org/pypi/django-splash/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/django-splash.svg
-    :target: https://github.com/edx/django-splash/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/django-splash/blob/master/LICENSE.txt
     :alt: License
```

### Comparing `django-splash-1.2.1/django_splash.egg-info/PKG-INFO` & `django-splash-1.3.0/django_splash.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: django-splash
-Version: 1.2.1
+Version: 1.3.0
 Summary: Splash screen middleware for Django apps
-Home-page: https://github.com/edx/django-splash
+Home-page: https://github.com/openedx/django-splash
 Author: edX
 Author-email: oscm@edx.org
 License: Apache Software License 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 License-File: AUTHORS
@@ -32,17 +32,17 @@
 --------
 
 Checks incoming requests, to redirect users to a configured splash screen URL
 if they don't have the proper cookie set. This can be used to display a small
 marketing landing page, protect an alpha website from the public eye, make an
 announcement, etc.
 
-Meant to be used with https://github.com/edx/edx-platform/ -- or you will need
+Meant to be used with https://github.com/openedx/edx-platform/ -- or you will need
 to import the config_models application to your Django application:
-https://github.com/edx/django-config-models
+https://github.com/openedx/django-config-models
 
 Installation
 ------------
 
 Add the application to the `INSTALLED_APPS`:
 
 ::
@@ -86,18 +86,16 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -109,28 +107,28 @@
 .. _list of resources: https://open.edx.org/getting-help
 
 
 .. |pypi-badge| image:: https://img.shields.io/pypi/v/django-splash.svg
     :target: https://pypi.python.org/pypi/django-splash/
     :alt: PyPI
 
-.. |ci-badge| image:: https://github.com/edx/django-splash/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/django-splash/actions?query=workflow%3A%22Python+CI%22
+.. |ci-badge| image:: https://github.com/openedx/django-splash/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/django-splash/actions?query=workflow%3A%22Python+CI%22
     :alt: CI
 
 .. |codecov-badge| image:: http://codecov.io/github/edx/django-splash/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/django-splash?branch=master
     :alt: Codecov
 
 .. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/django-splash.svg
     :target: https://pypi.python.org/pypi/django-splash/
     :alt: Supported Python versions
 
 .. |license-badge| image:: https://img.shields.io/github/license/edx/django-splash.svg
-    :target: https://github.com/edx/django-splash/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/django-splash/blob/master/LICENSE.txt
     :alt: License
 
 
 Change Log
 ----------
 
 ..
@@ -144,14 +142,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
 *
 
+[1.3.0] - 2023-06-09
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Added 
+_____
+
+* Added Support for Django42.
+
 [1.2.0] - 2022-01-26
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Removed
 _______
 
 * Removed Support for Django22, 30, 31
@@ -181,9 +187,7 @@
 [0.2.1] - 2018-02-07
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Added
 _____
 
 * First release on PyPI.
-
-
```

### Comparing `django-splash-1.2.1/setup.py` & `django-splash-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,30 +34,31 @@
 setup(
     name='django-splash',
     version=VERSION,
     description="""Splash screen middleware for Django apps""",
     long_description=README + '\n\n' + CHANGELOG,
     author='edX',
     author_email='oscm@edx.org',
-    url='https://github.com/edx/django-splash',
+    url='https://github.com/openedx/django-splash',
     packages=[
         'splash',
     ],
     include_package_data=True,
     install_requires=[
-        "Django<4.0"
+        "Django<5.0"
     ],
     license="Apache Software License 2.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

### Comparing `django-splash-1.2.1/splash/middleware.py` & `django-splash-1.3.0/splash/middleware.py`

 * *Files identical despite different names*

### Comparing `django-splash-1.2.1/splash/migrations/0001_initial.py` & `django-splash-1.3.0/splash/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-splash-1.2.1/splash/models.py` & `django-splash-1.3.0/splash/models.py`

 * *Files identical despite different names*

