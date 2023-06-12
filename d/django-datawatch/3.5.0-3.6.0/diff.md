# Comparing `tmp/django-datawatch-3.5.0.tar.gz` & `tmp/django-datawatch-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-datawatch-3.5.0.tar", last modified: Thu Apr 20 14:56:55 2023, max compression
+gzip compressed data, was "django-datawatch-3.6.0.tar", last modified: Mon Jun 12 13:34:30 2023, max compression
```

## Comparing `django-datawatch-3.5.0.tar` & `django-datawatch-3.6.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.698883 django-datawatch-3.5.0/django_datawatch/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/backends/synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/common/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/datawatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.686883 django-datawatch-3.5.0/django_datawatch/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.686883 django-datawatch-3.5.0/django_datawatch/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_list_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_refresh_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_run_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.702883 django-datawatch-3.5.0/django_datawatch/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/0002_auto_20180807_1508.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/0003_resultstatushistory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/querysets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.686883 django-datawatch-3.5.0/django_datawatch/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/django_datawatch/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/templatetags/class_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/django_datawatch/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_base_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_post_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/tests/test_trigger_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/django_datawatch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:56:55.698883 django-datawatch-3.5.0/django_datawatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 14:56:55.000000 django-datawatch-3.5.0/django_datawatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-20 14:56:55.706883 django-datawatch-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-20 14:56:49.000000 django-datawatch-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.080683 django-datawatch-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-06-12 13:34:30.080683 django-datawatch-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.068683 django-datawatch-3.6.0/django_datawatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.072683 django-datawatch-3.6.0/django_datawatch/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/backends/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/backends/synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.072683 django-datawatch-3.6.0/django_datawatch/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/datawatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.056683 django-datawatch-3.6.0/django_datawatch/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.056683 django-datawatch-3.6.0/django_datawatch/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.072683 django-datawatch-3.6.0/django_datawatch/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.072683 django-datawatch-3.6.0/django_datawatch/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.076683 django-datawatch-3.6.0/django_datawatch/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/management/commands/datawatch_clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/management/commands/datawatch_list_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/management/commands/datawatch_refresh_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/management/commands/datawatch_run_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.076683 django-datawatch-3.6.0/django_datawatch/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/migrations/0002_auto_20180807_1508.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/migrations/0003_resultstatushistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/querysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.060683 django-datawatch-3.6.0/django_datawatch/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.076683 django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.080683 django-datawatch-3.6.0/django_datawatch/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/templatetags/class_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.080683 django-datawatch-3.6.0/django_datawatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/tests/test_base_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/tests/test_post_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/tests/test_trigger_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/django_datawatch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:34:30.068683 django-datawatch-3.6.0/django_datawatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-06-12 13:34:30.000000 django-datawatch-3.6.0/django_datawatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-12 13:34:30.000000 django-datawatch-3.6.0/django_datawatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:34:30.000000 django-datawatch-3.6.0/django_datawatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 13:34:30.000000 django-datawatch-3.6.0/django_datawatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-12 13:34:30.000000 django-datawatch-3.6.0/django_datawatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-12 13:34:30.080683 django-datawatch-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-12 13:34:22.000000 django-datawatch-3.6.0/setup.py
```

### Comparing `django-datawatch-3.5.0/LICENSE` & `django-datawatch-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/PKG-INFO` & `django-datawatch-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-datawatch
-Version: 3.5.0
+Version: 3.6.0
 Summary: Django Datawatch runs automated data checks in your Django installation
 Home-page: https://github.com/RegioHelden/django-datawatch
 Download-URL: 
 Author: Jens Nistler <opensource@jensnistler.de>, Bogdan Radko <bogdan.radko@regiohelden.de>
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,monitoring,datawatch,check,checks
@@ -252,14 +252,16 @@
 docker compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
+![Django Datawatch detail view](http://static.jensnistler.de/django_datawatch_details.png "Django Datawatch detail view")
+
 ## Run the tests
 ```bash
 docker compose run --rm app test
 ```
 
 ## Requirements upgrades
```

### Comparing `django-datawatch-3.5.0/README.md` & `django-datawatch-3.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,16 @@
 docker compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
+![Django Datawatch detail view](http://static.jensnistler.de/django_datawatch_details.png "Django Datawatch detail view")
+
 ## Run the tests
 ```bash
 docker compose run --rm app test
 ```
 
 ## Requirements upgrades
```

### Comparing `django-datawatch-3.5.0/django_datawatch/admin.py` & `django-datawatch-3.6.0/django_datawatch/admin.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/backends/celery.py` & `django-datawatch-3.6.0/django_datawatch/backends/celery.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/backends/synchronous.py` & `django-datawatch-3.6.0/django_datawatch/backends/synchronous.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/base.py` & `django-datawatch-3.6.0/django_datawatch/base.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/common/views.py` & `django-datawatch-3.6.0/django_datawatch/common/views.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/datawatch.py` & `django-datawatch-3.6.0/django_datawatch/datawatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     def delete_results(self, sender, instance, db_alias=None):
         from django_datawatch.models import Result
         for check_class in datawatch.get_checks_for_model(model=sender):
             check = check_class()
             identifier = check.get_identifier(instance)
             Result.objects.using(db_alias).filter(slug=check.slug, identifier=identifier).delete()
 
-    def update_related(self, sender, instance):
+    def update_related(self, sender, instance, db_alias=None):
         checks = datawatch.get_checks_for_related_model(sender) or []
         for check_class in checks:
             check = check_class()
             backend = datawatch.get_backend()
             model_uid = make_model_uid(instance.__class__)
             mapping = check.get_trigger_update_uid_map()
 
@@ -123,15 +123,15 @@
                 if not payload:
                     continue
 
                 # work around lambdas binding to the loop scope, see https://rules.sonarsource.com/python/RSPEC-1515
                 def execute_backend_run(slug=check.slug, identifier=check.get_identifier(payload)):
                     backend.run(slug=slug, identifier=identifier, run_async=True)
 
-                transaction.on_commit(execute_backend_run)
+                transaction.on_commit(execute_backend_run, using=db_alias)
 
 
 datawatch = DatawatchHandler()
 
 
 class Scheduler(object):
     def run_checks(self, force=False, slug=None):
@@ -200,10 +200,10 @@
     :param sender: model
     :param kwargs:
     """
     if not getattr(settings, 'DJANGO_DATAWATCH_RUN_SIGNALS',
                    defaults['RUN_SIGNALS']):
         return
     try:
-        datawatch.update_related(sender, instance)
+        datawatch.update_related(sender, instance, using)
     except Exception as e:
         logger.exception(e)
```

### Comparing `django-datawatch-3.5.0/django_datawatch/forms.py` & `django-datawatch-3.6.0/django_datawatch/forms.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.mo` & `django-datawatch-3.6.0/django_datawatch/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/locale/de/LC_MESSAGES/django.po` & `django-datawatch-3.6.0/django_datawatch/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_refresh_results.py` & `django-datawatch-3.6.0/django_datawatch/management/commands/datawatch_refresh_results.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/management/commands/datawatch_run_checks.py` & `django-datawatch-3.6.0/django_datawatch/management/commands/datawatch_run_checks.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/migrations/0001_initial.py` & `django-datawatch-3.6.0/django_datawatch/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/migrations/0002_auto_20180807_1508.py` & `django-datawatch-3.6.0/django_datawatch/migrations/0002_auto_20180807_1508.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/migrations/0003_resultstatushistory.py` & `django-datawatch-3.6.0/django_datawatch/migrations/0003_resultstatushistory.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/models.py` & `django-datawatch-3.6.0/django_datawatch/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from dateutil import relativedelta
 from django.utils import timezone
 from django.conf import settings
 from django.db import models
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from django_extensions.db.fields.json import JSONField
@@ -96,14 +98,17 @@
     def latest_warning(self):
         return self.latest_status(self.STATUS.warning)
 
     @cached_property
     def latest_critical(self):
         return self.latest_status(self.STATUS.critical)
 
+    def config_formatted(self):
+        return json.dumps(self.get_check_instance().get_config(payload=self.get_payload()), indent=4)
+
 
 class ResultStatusHistory(TimeStampedModel):
     result = models.ForeignKey(Result, models.CASCADE, 'status_history', 'status_history', verbose_name=_('Result'))
     from_status = models.IntegerField(choices=Result.STATUS, verbose_name=_('From status'), null=True)
     to_status = models.IntegerField(choices=Result.STATUS, verbose_name=_('To status'))
 
     class Meta:
```

### Comparing `django-datawatch-3.5.0/django_datawatch/querysets.py` & `django-datawatch-3.6.0/django_datawatch/querysets.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/tasks.py` & `django-datawatch-3.6.0/django_datawatch/tasks.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/base.html` & `django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/base.html`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/dashboard.html` & `django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/detail.html` & `django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/detail.html`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,20 @@
                                                         {% else %}
                                                             {% trans "Not assigned" %}
                                                         {% endif %}
                                                     </td>
                                                 </tr>
                                             {% endwith %}
                                             <tr>
+                                                <td>{% trans "Config" %}</td>
+                                                <td>
+                                                    <pre>{{ result.config_formatted }}</pre>
+                                                </td>
+                                            </tr>
+                                            <tr>
                                                 <td>{% trans "Run every" %}</td>
                                                 <td>
                                                     {% if check_instance.run_every %}
                                                         {{ check_instance.run_every }}
                                                     {% else %}
                                                         {% trans "Not set" %}
                                                     {% endif %}
```

#### html2text {}

```diff
@@ -18,14 +18,15 @@
                                     {% if check_instance.model_class %} {
 {% trans "Related model" %}         { check_instance.model_class|class_name }}
                                     {% else %} {% trans "Not assigned" %} {%
                                     endif %}
                                     {% if form_class %} {
 {% trans "Config form class" %}     { form_class|class_name }} {% else %} {%
                                     trans "Not assigned" %} {% endif %}
+{% trans "Config" %}                {{ result.config_formatted }}
                                     {% if check_instance.run_every %} {
 {% trans "Run every" %}             { check_instance.run_every }} {% else %} {%
                                     trans "Not set" %} {% endif %}
                                     {% for value in
                                     check_instance.trigger_update.values %} {
 {% trans "Update trigger models" %} { value|class_name }} {% if not
                                     forloop.last %}
```

### Comparing `django-datawatch-3.5.0/django_datawatch/templates/django_datawatch/form.html` & `django-datawatch-3.6.0/django_datawatch/templates/django_datawatch/form.html`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/tests/test_base_check.py` & `django-datawatch-3.6.0/django_datawatch/tests/test_base_check.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/tests/test_integration.py` & `django-datawatch-3.6.0/django_datawatch/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/tests/test_post_delete.py` & `django-datawatch-3.6.0/django_datawatch/tests/test_post_delete.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/tests/test_scheduler.py` & `django-datawatch-3.6.0/django_datawatch/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/tests/test_trigger_update.py` & `django-datawatch-3.6.0/django_datawatch/tests/test_trigger_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class TriggerUpdateTestCase(TestCase):
     @override_settings(DJANGO_DATAWATCH_RUN_SIGNALS=True)
     @mock.patch('django_datawatch.datawatch.DatawatchHandler.update_related')
     def test_setting_run_signals_true(self, mock_update):
         run_checks(sender='sender', instance='instance', created=None, raw=None,
                    using=None)
-        mock_update.assert_called_once_with('sender', 'instance')
+        mock_update.assert_called_once_with('sender', 'instance', None)
 
     @override_settings(DJANGO_DATAWATCH_RUN_SIGNALS=False)
     @mock.patch('django_datawatch.datawatch.DatawatchHandler.update_related')
     def test_setting_run_signals_false(self, mock_update):
         run_checks(sender=None, instance=None, created=None, raw=None,
                    using=None)
         mock_update.assert_not_called()
```

### Comparing `django-datawatch-3.5.0/django_datawatch/urls.py` & `django-datawatch-3.6.0/django_datawatch/urls.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch/views.py` & `django-datawatch-3.6.0/django_datawatch/views.py`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/django_datawatch.egg-info/PKG-INFO` & `django-datawatch-3.6.0/django_datawatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-datawatch
-Version: 3.5.0
+Version: 3.6.0
 Summary: Django Datawatch runs automated data checks in your Django installation
 Home-page: https://github.com/RegioHelden/django-datawatch
 Download-URL: 
 Author: Jens Nistler <opensource@jensnistler.de>, Bogdan Radko <bogdan.radko@regiohelden.de>
 Author-email: opensource@regiohelden.de
 License: MIT
 Keywords: django,monitoring,datawatch,check,checks
@@ -252,14 +252,16 @@
 docker compose run --rm --entrypoint celery app -A example  beat --scheduler django_celery_beat.schedulers:DatabaseScheduler
 ```
 
 You will see some failed check now after you refreshed the dashboard view.
 
 ![Django Datawatch dashboard](http://static.jensnistler.de/django_datawatch.png "Django Datawatch dashboard")
 
+![Django Datawatch detail view](http://static.jensnistler.de/django_datawatch_details.png "Django Datawatch detail view")
+
 ## Run the tests
 ```bash
 docker compose run --rm app test
 ```
 
 ## Requirements upgrades
```

### Comparing `django-datawatch-3.5.0/django_datawatch.egg-info/SOURCES.txt` & `django-datawatch-3.6.0/django_datawatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-datawatch-3.5.0/setup.py` & `django-datawatch-3.6.0/setup.py`

 * *Files identical despite different names*

