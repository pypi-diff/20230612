# Comparing `tmp/django-ical-1.9.1.tar.gz` & `tmp/django-ical-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ical-1.9.1.tar", last modified: Mon May  1 08:19:54 2023, max compression
+gzip compressed data, was "django-ical-1.9.2.tar", last modified: Mon Jun 12 15:20:22 2023, max compression
```

## Comparing `django-ical-1.9.1.tar` & `django-ical-1.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 08:19:34.000000 django-ical-1.9.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.136628 django-ical-1.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-01 08:19:34.000000 django-ical-1.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-01 08:19:34.000000 django-ical-1.9.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 08:19:34.000000 django-ical-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 08:19:34.000000 django-ical-1.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 08:19:34.000000 django-ical-1.9.1/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-01 08:19:34.000000 django-ical-1.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-01 08:19:34.000000 django-ical-1.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-01 08:19:34.000000 django-ical-1.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 08:19:34.000000 django-ical-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 08:19:34.000000 django-ical-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-01 08:19:54.144627 django-ical-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-01 08:19:34.000000 django-ical-1.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/django_ical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/feedgenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/django_ical/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/tests/test_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/tests/test_recurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-01 08:19:34.000000 django-ical-1.9.1/django_ical/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.140627 django-ical-1.9.1/django_ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 08:19:54.000000 django-ical-1.9.1/django_ical.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/django_ical.feedgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:19:54.144627 django-ical-1.9.1/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/django_ical.feedgenerator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/django_ical.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/django_ical.views.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-05-01 08:19:34.000000 django-ical-1.9.1/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 08:19:34.000000 django-ical-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 08:19:54.144627 django-ical-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-01 08:19:34.000000 django-ical-1.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-01 08:19:34.000000 django-ical-1.9.1/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-01 08:19:34.000000 django-ical-1.9.1/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-01 08:19:34.000000 django-ical-1.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.926928 django-ical-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:20:07.000000 django-ical-1.9.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.918927 django-ical-1.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.922928 django-ical-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-12 15:20:07.000000 django-ical-1.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-12 15:20:07.000000 django-ical-1.9.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-12 15:20:07.000000 django-ical-1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 15:20:07.000000 django-ical-1.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 15:20:07.000000 django-ical-1.9.2/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-12 15:20:07.000000 django-ical-1.9.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-12 15:20:07.000000 django-ical-1.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-12 15:20:07.000000 django-ical-1.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-12 15:20:07.000000 django-ical-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 15:20:07.000000 django-ical-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-12 15:20:22.926928 django-ical-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-12 15:20:07.000000 django-ical-1.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.922928 django-ical-1.9.2/django_ical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:07.000000 django-ical-1.9.2/django_ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-12 15:20:07.000000 django-ical-1.9.2/django_ical/feedgenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.926928 django-ical-1.9.2/django_ical/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:07.000000 django-ical-1.9.2/django_ical/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19581 2023-06-12 15:20:07.000000 django-ical-1.9.2/django_ical/tests/test_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-12 15:20:07.000000 django-ical-1.9.2/django_ical/tests/test_recurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-12 15:20:07.000000 django-ical-1.9.2/django_ical/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-12 15:20:07.000000 django-ical-1.9.2/django_ical/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.922928 django-ical-1.9.2/django_ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-12 15:20:22.000000 django-ical-1.9.2/django_ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-12 15:20:22.000000 django-ical-1.9.2/django_ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:20:22.000000 django-ical-1.9.2/django_ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 15:20:22.000000 django-ical-1.9.2/django_ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 15:20:22.000000 django-ical-1.9.2/django_ical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.926928 django-ical-1.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.926928 django-ical-1.9.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/django_ical.feedgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:20:22.926928 django-ical-1.9.2/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/reference/django_ical.feedgenerator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/reference/django_ical.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/reference/django_ical.views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22932 2023-06-12 15:20:07.000000 django-ical-1.9.2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 15:20:07.000000 django-ical-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:20:22.926928 django-ical-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-12 15:20:07.000000 django-ical-1.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-12 15:20:07.000000 django-ical-1.9.2/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-12 15:20:07.000000 django-ical-1.9.2/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-12 15:20:07.000000 django-ical-1.9.2/tox.ini
```

### Comparing `django-ical-1.9.1/.github/workflows/release.yml` & `django-ical-1.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/.github/workflows/test.yml` & `django-ical-1.9.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/CHANGES.rst` & `django-ical-1.9.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 
 Changes
 =======
 
 
+1.9.2 (2023-06-12)
+------------------
+
+- Support all properties specified in RFC 5545
+  [magicbrothers]
+
+
 1.9.1 (2023-05-01)
 ------------------
 
 - Fix multiple CATEGORIES and add tests
   [mjfinney]
```

### Comparing `django-ical-1.9.1/CODE_OF_CONDUCT.md` & `django-ical-1.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/LICENSE` & `django-ical-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/PKG-INFO` & `django-ical-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ical
-Version: 1.9.1
+Version: 1.9.2
 Summary: iCal feeds for Django based on Django's syndication feed framework.
 Home-page: https://github.com/jazzband/django-ical
 Author: Ian Lewis
 Author-email: security@jazzband.com
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.com
 License: MIT License
@@ -82,14 +82,21 @@
    :alt: Jazzband
 
 
 Changes
 =======
 
 
+1.9.2 (2023-06-12)
+------------------
+
+- Support all properties specified in RFC 5545
+  [magicbrothers]
+
+
 1.9.1 (2023-05-01)
 ------------------
 
 - Fix multiple CATEGORIES and add tests
   [mjfinney]
```

### Comparing `django-ical-1.9.1/README.rst` & `django-ical-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/django_ical/feedgenerator.py` & `django-ical-1.9.2/django_ical/feedgenerator.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,37 @@
     ("valarm", None),
     # additional properties supported by the Todo class (VTODO calendar component).
     # see https://icalendar.readthedocs.io/en/latest/_modules/icalendar/cal.html#Todo
     ("completed", "completed"),
     ("percent_complete", "percent-complete"),
     ("priority", "priority"),
     ("due", "due"),
+    ("calscale", "calscale"),
+    ("method", "method"),
+    ("prodid", "prodid"),
+    ("version", "version"),
+    ("attach", "attach"),
+    ("class", "class"),
+    ("comment", "comment"),
+    ("resources", "resources"),
+    ("duration", "duration"),
+    ("freebusy", "freebusy"),
+    ("tzid", "tzid"),
+    ("tzname", "tzname"),
+    ("tzoffsetfrom", "tzoffsetfrom"),
+    ("tzoffsetto", "tzoffsetto"),
+    ("tzurl", "tzurl"),
+    ("contact", "contact"),
+    ("recurrence_id", "recurrence-id"),
+    ("related_to", "related-to"),
+    ("action", "action"),
+    ("repeat", "repeat"),
+    ("trigger", "trigger"),
+    ("sequence", "sequence"),
+    ("request_status", "request-status"),
 )
 
 class ICal20Feed(SyndicationFeed):
     """
     iCalendar 2.0 Feed implementation.
     """
```

### Comparing `django-ical-1.9.1/django_ical/tests/test_feed.py` & `django-ical-1.9.2/django_ical/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/django_ical/tests/test_recurrence.py` & `django-ical-1.9.2/django_ical/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/django_ical/utils.py` & `django-ical-1.9.2/django_ical/utils.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/django_ical/views.py` & `django-ical-1.9.2/django_ical/views.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/django_ical.egg-info/PKG-INFO` & `django-ical-1.9.2/django_ical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ical
-Version: 1.9.1
+Version: 1.9.2
 Summary: iCal feeds for Django based on Django's syndication feed framework.
 Home-page: https://github.com/jazzband/django-ical
 Author: Ian Lewis
 Author-email: security@jazzband.com
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.com
 License: MIT License
@@ -82,14 +82,21 @@
    :alt: Jazzband
 
 
 Changes
 =======
 
 
+1.9.2 (2023-06-12)
+------------------
+
+- Support all properties specified in RFC 5545
+  [magicbrothers]
+
+
 1.9.1 (2023-05-01)
 ------------------
 
 - Fix multiple CATEGORIES and add tests
   [mjfinney]
```

### Comparing `django-ical-1.9.1/django_ical.egg-info/SOURCES.txt` & `django-ical-1.9.2/django_ical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/docs/Makefile` & `django-ical-1.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/docs/make.bat` & `django-ical-1.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/docs/source/conf.py` & `django-ical-1.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/docs/source/index.rst` & `django-ical-1.9.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/docs/source/usage.rst` & `django-ical-1.9.2/docs/source/usage.rst`

 * *Files 18% similar despite different names*

```diff
@@ -311,20 +311,66 @@
 |                       |                       | indication the completion   |
 |                       |                       | of the task.                |
 +-----------------------+-----------------------+-----------------------------+
 | item_priority         | `PRIORITY`_           | An integer from 0 to 9.     |
 |                       |                       | 0 means undefined.          |
 |                       |                       | 1 means highest priority.   |
 +-----------------------+-----------------------+-----------------------------+
-| item_due              | `DUE`      _          | The date a task is due.     |
+| item_due              | `DUE`_                | The date a task is due.     |
 +-----------------------+-----------------------+-----------------------------+
 | item_categories       | `CATEGORIES`_         | A list of strings, each     |
 |                       |                       | being a category of the     |
 |                       |                       | task.                       |
 +-----------------------+-----------------------+-----------------------------+
+| calscale              | `CALSCALE`_           | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| method                | `METHOD`_             | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| prodid                | `PRODID`_             | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| version               | `VERSION`_            | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| attach                | `ATTACH`_             | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| class                 | `CLASS`_              | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| comment               | `COMMENT`_            | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| resources             | `RESOURCES`_          | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| duration              | `DURATION`_           | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| freebusy              | `FREEBUSY`_           | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| tzid                  | `TZID`_               | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| tzname                | `TZNAME`_             | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| tzoffsetfrom          | `TZOFFSETFROM`_       | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| tzoffsetto            | `TZOFFSETTO`_         | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| tzurl                 | `TZURL`_              | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| contact               | `CONTACT`_            | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| recurrence_id         | `RECURRENCE_ID`_      | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| related_to            | `RELATED_TO`_         | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| action                | `ACTION`_             | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| repeat                | `REPEAT`_             | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| trigger               | `TRIGGER`_            | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| sequence              | `SEQUENCE`_           | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
+| request_status        | `REQUEST_STATUS`_     | Not yet documented.         |
++-----------------------+-----------------------+-----------------------------+
 
 
 .. note::
    django-ical does not use the ``link`` property required by the Django
    syndication framework.
 
 The low-level framework
@@ -358,13 +404,40 @@
 .. _ATTENDEE: https://www.kanzaki.com/docs/ical/attendee.html
 .. _RRULE: https://www.kanzaki.com/docs/ical/rrule.html
 .. _EXRULE: https://www.kanzaki.com/docs/ical/exrule.html
 .. _RDATE: https://www.kanzaki.com/docs/ical/rdate.html
 .. _EXDATE: https://www.kanzaki.com/docs/ical/exdate.html
 .. _STATUS: https://www.kanzaki.com/docs/ical/status.html
 .. _VALARM: https://www.kanzaki.com/docs/ical/valarm.html
+.. _COMPLETED: https://www.kanzaki.com/docs/ical/completed.html
+.. _PERCENT-COMPLETE: https://www.kanzaki.com/docs/ical/percentComplete.html
+.. _PRIORITY: https://www.kanzaki.com/docs/ical/priority.html
+.. _DUE: https://www.kanzaki.com/docs/ical/due.html
+.. _CALSCALE: https://www.kanzaki.com/docs/ical/calscale.html
+.. _METHOD: https://www.kanzaki.com/docs/ical/method.html
+.. _PRODID: https://www.kanzaki.com/docs/ical/prodid.html
+.. _VERSION: https://www.kanzaki.com/docs/ical/version.html
+.. _ATTACH: https://www.kanzaki.com/docs/ical/attach.html
+.. _CLASS: https://www.kanzaki.com/docs/ical/class.html
+.. _COMMENT: https://www.kanzaki.com/docs/ical/comment.html
+.. _RESOURCES: https://www.kanzaki.com/docs/ical/resources.html
+.. _DURATION: https://www.kanzaki.com/docs/ical/duration.html
+.. _FREEBUSY: https://www.kanzaki.com/docs/ical/freebusy.html
+.. _TZID: https://www.kanzaki.com/docs/ical/tzid.html
+.. _TZNAME: https://www.kanzaki.com/docs/ical/tzname.html
+.. _TZOFFSETFROM: https://www.kanzaki.com/docs/ical/tzoffsetfrom.html
+.. _TZOFFSETTO: https://www.kanzaki.com/docs/ical/tzoffsetto.html
+.. _TZURL: https://www.kanzaki.com/docs/ical/tzurl.html
+.. _CONTACT: https://www.kanzaki.com/docs/ical/contact.html
+.. _RECURRENCE-ID: https://www.kanzaki.com/docs/ical/recurrenceId.html
+.. _RELATED-TO: https://www.kanzaki.com/docs/ical/relatedTo.html
+.. _ACTION: https://www.kanzaki.com/docs/ical/action.html
+.. _REPEAT: https://www.kanzaki.com/docs/ical/repeat.html
+.. _TRIGGER: https://www.kanzaki.com/docs/ical/trigger.html
+.. _SEQUENCE: https://www.kanzaki.com/docs/ical/sequence.html
+.. _REQUEST-STATUS: https://icalendar.org/iCalendar-RFC-5545/3-8-8-3-request-status.html
 .. _X-WR-CALNAME: http://en.wikipedia.org/wiki/ICalendar#Calendar_extensions
 .. _X-WR-CALDESC: http://en.wikipedia.org/wiki/ICalendar#Calendar_extensions
 .. _X-WR-TIMEZONE: http://en.wikipedia.org/wiki/ICalendar#Calendar_extensions
 .. _iCalendar: http://icalendar.readthedocs.org/en/latest/index.html
 .. _CATEGORIES: https://www.kanzaki.com/docs/ical/categories.html
 .. _django-recurrence: https://github.com/django-recurrence/django-recurrence
```

### Comparing `django-ical-1.9.1/setup.py` & `django-ical-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/tests.py` & `django-ical-1.9.2/tests.py`

 * *Files identical despite different names*

### Comparing `django-ical-1.9.1/tox.ini` & `django-ical-1.9.2/tox.ini`

 * *Files identical despite different names*

