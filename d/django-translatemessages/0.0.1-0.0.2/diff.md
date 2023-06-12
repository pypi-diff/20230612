# Comparing `tmp/django-translatemessages-0.0.1.tar.gz` & `tmp/django-translatemessages-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-translatemessages-0.0.1.tar", last modified: Sun Jun 11 14:28:09 2023, max compression
+gzip compressed data, was "django-translatemessages-0.0.2.tar", last modified: Mon Jun 12 08:57:36 2023, max compression
```

## Comparing `django-translatemessages-0.0.1.tar` & `django-translatemessages-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 14:28:09.107246 django-translatemessages-0.0.1/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       56 2023-06-11 10:46:30.000000 django-translatemessages-0.0.1/CHANGELOG.rst
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.1/LICENSE
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.1/MANIFEST.in
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1166 2023-06-11 14:28:09.107246 django-translatemessages-0.0.1/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      121 2023-06-11 10:44:12.000000 django-translatemessages-0.0.1/README.rst
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 14:28:09.107246 django-translatemessages-0.0.1/django_translatemessages/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       21 2023-06-11 10:51:33.000000 django-translatemessages-0.0.1/django_translatemessages/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 14:28:09.107246 django-translatemessages-0.0.1/django_translatemessages/management/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.1/django_translatemessages/management/__init__.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 14:28:09.107246 django-translatemessages-0.0.1/django_translatemessages/management/commands/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.1/django_translatemessages/management/commands/__init__.py
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     4612 2023-06-11 14:25:02.000000 django-translatemessages-0.0.1/django_translatemessages/management/commands/translatemessages.py
-drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 14:28:09.107246 django-translatemessages-0.0.1/django_translatemessages.egg-info/
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1166 2023-06-11 14:28:09.000000 django-translatemessages-0.0.1/django_translatemessages.egg-info/PKG-INFO
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-11 14:28:09.000000 django-translatemessages-0.0.1/django_translatemessages.egg-info/SOURCES.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-11 14:28:09.000000 django-translatemessages-0.0.1/django_translatemessages.egg-info/dependency_links.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-11 14:28:09.000000 django-translatemessages-0.0.1/django_translatemessages.egg-info/not-zip-safe
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-11 14:28:09.000000 django-translatemessages-0.0.1/django_translatemessages.egg-info/requires.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-11 14:28:09.000000 django-translatemessages-0.0.1/django_translatemessages.egg-info/top_level.txt
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-11 14:28:09.107246 django-translatemessages-0.0.1/setup.cfg
--rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.1/setup.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       53 2023-06-12 08:55:29.000000 django-translatemessages-0.0.2/CHANGELOG.rst
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     1071 2023-06-11 10:32:38.000000 django-translatemessages-0.0.2/LICENSE
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       89 2023-06-11 10:46:30.000000 django-translatemessages-0.0.2/MANIFEST.in
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3452 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2410 2023-06-12 08:55:29.000000 django-translatemessages-0.0.2/README.rst
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       22 2023-06-12 08:55:34.000000 django-translatemessages-0.0.2/django_translatemessages/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages/management/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:02.000000 django-translatemessages-0.0.2/django_translatemessages/management/__init__.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages/management/commands/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        0 2023-06-11 10:47:14.000000 django-translatemessages-0.0.2/django_translatemessages/management/commands/__init__.py
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)    11238 2023-06-12 08:57:11.000000 django-translatemessages-0.0.2/django_translatemessages/management/commands/translatemessages.py
+drwxrwxr-x   0 elapouya  (1000) elapouya  (1000)        0 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/django_translatemessages.egg-info/
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     3452 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/PKG-INFO
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)      557 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/SOURCES.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/dependency_links.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)        1 2023-06-11 14:28:09.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/not-zip-safe
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/requires.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       25 2023-06-12 08:57:36.000000 django-translatemessages-0.0.2/django_translatemessages.egg-info/top_level.txt
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)       67 2023-06-12 08:57:36.703662 django-translatemessages-0.0.2/setup.cfg
+-rw-rw-r--   0 elapouya  (1000) elapouya  (1000)     2008 2023-06-11 14:28:07.000000 django-translatemessages-0.0.2/setup.py
```

### Comparing `django-translatemessages-0.0.1/LICENSE` & `django-translatemessages-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.1/django_translatemessages.egg-info/SOURCES.txt` & `django-translatemessages-0.0.2/django_translatemessages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-translatemessages-0.0.1/setup.py` & `django-translatemessages-0.0.2/setup.py`

 * *Files identical despite different names*

