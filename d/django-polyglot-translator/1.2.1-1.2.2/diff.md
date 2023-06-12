# Comparing `tmp/django-polyglot-translator-1.2.1.tar.gz` & `tmp/django-polyglot-translator-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-polyglot-translator-1.2.1.tar", last modified: Sat Sep 24 14:12:35 2022, max compression
+gzip compressed data, was "django-polyglot-translator-1.2.2.tar", last modified: Mon Jun 12 07:46:44 2023, max compression
```

## Comparing `django-polyglot-translator-1.2.1.tar` & `django-polyglot-translator-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 14:12:35.644996 django-polyglot-translator-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-09-24 14:12:35.644996 django-polyglot-translator-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 14:12:35.640996 django-polyglot-translator-1.2.1/djangoPolyglot/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 14:12:35.640996 django-polyglot-translator-1.2.1/djangoPolyglot/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 14:12:35.640996 django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/arguments.py
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/django-polyglot.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/license.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/models.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/djangoPolyglot/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 14:12:35.640996 django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2499 2022-09-24 14:12:35.000000 django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-24 14:12:35.000000 django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-24 14:12:35.000000 django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-24 14:12:35.000000 django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-24 14:12:35.000000 django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-24 14:12:35.644996 django-polyglot-translator-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-09-24 14:12:23.000000 django-polyglot-translator-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:46:44.343263 django-polyglot-translator-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-12 07:46:44.343263 django-polyglot-translator-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:46:44.339263 django-polyglot-translator-1.2.2/djangoPolyglot/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:46:44.339263 django-polyglot-translator-1.2.2/djangoPolyglot/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:46:44.339263 django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/django-polyglot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/djangoPolyglot/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 07:46:44.343263 django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-12 07:46:44.000000 django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-12 07:46:44.000000 django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 07:46:44.000000 django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 07:46:44.000000 django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 07:46:44.000000 django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 07:46:44.343263 django-polyglot-translator-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-12 07:46:31.000000 django-polyglot-translator-1.2.2/setup.py
```

### Comparing `django-polyglot-translator-1.2.1/LICENSE` & `django-polyglot-translator-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-polyglot-translator-1.2.1/PKG-INFO` & `django-polyglot-translator-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-polyglot-translator
-Version: 1.2.1
+Version: 1.2.2
 Summary: Polyglot integration for Django Web Framework
 Home-page: https://github.com/riccardoFasan/django-polyglot
 Author: Riccardo Fasan
 Author-email: fasanriccardo21@gmail.com
 License: MIT
 Project-URL: BugTracker, https://github.com/riccardoFasan/django-polyglot/issues
 Project-URL: Homepage, https://github.com/riccardoFasan/django-polyglot
```

### Comparing `django-polyglot-translator-1.2.1/README.md` & `django-polyglot-translator-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/arguments.py` & `django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/arguments.py`

 * *Files identical despite different names*

### Comparing `django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/django-polyglot.py` & `django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/django-polyglot.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,13 +85,13 @@
                         source_lang=source_lang.upper(),
                     )
                 )
                 options: arguments.Arguments = collector.arguments
                 polyglot.Polyglot(options).execute_command()
 
                 # Polyglot names output files like this: "{lang_code}.po" so we have to rename in "django.po"
-                os.rename(f"{output_dir}/{lang}.po", f"{output_dir}/django.po")
-                os.rename(f"{output_dir}/{lang}.mo", f"{output_dir}/django.mo")
+                os.replace(f"{output_dir}/{lang}.po", f"{output_dir}/django.po")
+                os.replace(f"{output_dir}/{lang}.mo", f"{output_dir}/django.mo")
 
     def __compile_messages(self) -> None:
         print("\n========== compilemessages ==========")
         management.call_command("compilemessages", locale=self.__languages)
```

### Comparing `django-polyglot-translator-1.2.1/djangoPolyglot/management/commands/license.py` & `django-polyglot-translator-1.2.2/djangoPolyglot/management/commands/license.py`

 * *Files identical despite different names*

### Comparing `django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/PKG-INFO` & `django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-polyglot-translator
-Version: 1.2.1
+Version: 1.2.2
 Summary: Polyglot integration for Django Web Framework
 Home-page: https://github.com/riccardoFasan/django-polyglot
 Author: Riccardo Fasan
 Author-email: fasanriccardo21@gmail.com
 License: MIT
 Project-URL: BugTracker, https://github.com/riccardoFasan/django-polyglot/issues
 Project-URL: Homepage, https://github.com/riccardoFasan/django-polyglot
```

### Comparing `django-polyglot-translator-1.2.1/django_polyglot_translator.egg-info/SOURCES.txt` & `django-polyglot-translator-1.2.2/django_polyglot_translator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-polyglot-translator-1.2.1/setup.py` & `django-polyglot-translator-1.2.2/setup.py`

 * *Files identical despite different names*

