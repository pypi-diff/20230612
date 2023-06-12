# Comparing `tmp/django-userextensions-0.3.0.tar.gz` & `tmp/django-userextensions-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-userextensions-0.3.0.tar", last modified: Sun Jun  4 01:04:06 2023, max compression
+gzip compressed data, was "django-userextensions-0.3.1.tar", last modified: Mon Jun 12 21:19:38 2023, max compression
```

## Comparing `django-userextensions-0.3.0.tar` & `django-userextensions-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.418177 django-userextensions-0.3.0/django_userextensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 01:04:06.000000 django-userextensions-0.3.0/django_userextensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.418177 django-userextensions-0.3.0/userextensions/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/management/commands/add_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0002_userpreference_start_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0003_auto_20200117_2153.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0005_auto_20201114_0548.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0006_auto_20210507_1831.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/0007_auto_20220807_2104.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.414177 django-userextensions-0.3.0/userextensions/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/templates/userextensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/get_users_per_group.htm
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/show_srv_acct_token.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.422177 django-userextensions-0.3.0/userextensions/templates/userextensions/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/custom/create_custom_service_account.htm
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/custom/manage_service_accounts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/detail/detail_user.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/form/
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/form/edit_favorite.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/user_theme.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templates/userextensions/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_favorites.htm
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_recents.htm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templates/userextensions/userextensions_base.htm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/templatetags/userextension_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:04:06.426178 django-userextensions-0.3.0/userextensions/views/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/ajax.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-06-04 01:03:54.000000 django-userextensions-0.3.0/userextensions/views/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.813411 django-userextensions-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-12 21:19:38.813411 django-userextensions-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.801411 django-userextensions-0.3.1/django_userextensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-12 21:19:38.000000 django-userextensions-0.3.1/django_userextensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-12 21:19:38.000000 django-userextensions-0.3.1/django_userextensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:19:38.000000 django-userextensions-0.3.1/django_userextensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 21:19:38.000000 django-userextensions-0.3.1/django_userextensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 21:19:38.000000 django-userextensions-0.3.1/django_userextensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:19:38.813411 django-userextensions-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.801411 django-userextensions-0.3.1/userextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.805411 django-userextensions-0.3.1/userextensions/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.805411 django-userextensions-0.3.1/userextensions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/management/commands/add_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/0002_userpreference_start_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/0003_auto_20200117_2153.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/0005_auto_20201114_0548.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/0006_auto_20210507_1831.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/0007_auto_20220807_2104.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.797411 django-userextensions-0.3.1/userextensions/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templates/userextensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templates/userextensions/ajax/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/ajax/get_users_per_group.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/ajax/show_srv_acct_token.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templates/userextensions/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/custom/create_custom_service_account.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/custom/manage_service_accounts.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templates/userextensions/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/detail/detail_user.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templates/userextensions/form/
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/form/edit_favorite.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templates/userextensions/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/snippets/user_theme.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templates/userextensions/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/table/table_favorites.htm
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/table/table_recents.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templates/userextensions/userextensions_base.htm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.809411 django-userextensions-0.3.1/userextensions/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/templatetags/userextension_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:38.813411 django-userextensions-0.3.1/userextensions/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17502 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/views/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/views/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-06-12 21:19:27.000000 django-userextensions-0.3.1/userextensions/views/gui.py
```

### Comparing `django-userextensions-0.3.0/LICENSE` & `django-userextensions-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/PKG-INFO` & `django-userextensions-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: django-userextensions
-Version: 0.3.0
+Version: 0.3.1
 Summary: A user extension module for django
 Home-page: https://github.com/davidslusser/django-userextensions
-Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.0.tar.gz
+Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.1.tar.gz
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GPL-3.0
 Keywords: django,helpers,extension,user,profile
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-userextensions
```

### Comparing `django-userextensions-0.3.0/README.md` & `django-userextensions-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/django_userextensions.egg-info/PKG-INFO` & `django-userextensions-0.3.1/django_userextensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: django-userextensions
-Version: 0.3.0
+Version: 0.3.1
 Summary: A user extension module for django
 Home-page: https://github.com/davidslusser/django-userextensions
-Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.0.tar.gz
+Download-URL: https://github.com/davidslusser/django-userextensions/archive/0.3.1.tar.gz
 Author: David Slusser
 Author-email: dbslusser@gmail.com
 License: GPL-3.0
 Keywords: django,helpers,extension,user,profile
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-userextensions
```

### Comparing `django-userextensions-0.3.0/django_userextensions.egg-info/SOURCES.txt` & `django-userextensions-0.3.1/django_userextensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/setup.py` & `django-userextensions-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,13 +27,13 @@
     keywords=['django', 'helpers', 'extension', 'user', 'profile'],
     install_requires=required,
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Framework :: Django :: 2.2',
+        'Framework :: Django :: 4.2',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
```

### Comparing `django-userextensions-0.3.0/userextensions/admin.py` & `django-userextensions-0.3.1/userextensions/admin.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/forms.py` & `django-userextensions-0.3.1/userextensions/forms.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/management/commands/add_service_account.py` & `django-userextensions-0.3.1/userextensions/management/commands/add_service_account.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/middleware.py` & `django-userextensions-0.3.1/userextensions/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-"""
-
-"""
 from django.utils import timezone
 from django.conf import settings
 from django.urls import resolve
 from urllib.parse import urlparse
 
 # Use MiddlewareMixin when present (Django >= 1.10)
 try:
@@ -31,14 +28,23 @@
                 SKIP_URL_PREFIX_LIST = ['/admin/', '/__debug__/']
 
         static URLs: will not track the specified URLs
                 SKIP_FIXED_URL_LIST = ['/', '/login/', '/logout/', ]
     """
     def process_request(self, request):
         """ read user and url (path) from request, if valid and not in a skip list, add to recents """
+
+        # do not track ajax requests
+        if request.headers.get('x-requested-with') == 'XMLHttpRequest':
+            return
+
+        # do not track htmx requests
+        if request.headers.get("Hx-Request", None):
+            return
+
         # only track specified methods
         track_method_list = getattr(settings, 'TRACK_METHOD_LIST', ['GET'])
         if request.method not in track_method_list:
             return
 
         # do not track url if user is not authenticated
         if not request.user.is_authenticated:
```

### Comparing `django-userextensions-0.3.0/userextensions/migrations/0001_initial.py` & `django-userextensions-0.3.1/userextensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/migrations/0003_auto_20200117_2153.py` & `django-userextensions-0.3.1/userextensions/migrations/0003_auto_20200117_2153.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py` & `django-userextensions-0.3.1/userextensions/migrations/0004_serviceaccount_serviceaccounttokenhistory.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/migrations/0005_auto_20201114_0548.py` & `django-userextensions-0.3.1/userextensions/migrations/0005_auto_20201114_0548.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/migrations/0006_auto_20210507_1831.py` & `django-userextensions-0.3.1/userextensions/migrations/0006_auto_20210507_1831.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/migrations/0007_auto_20220807_2104.py` & `django-userextensions-0.3.1/userextensions/migrations/0007_auto_20220807_2104.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/mixins.py` & `django-userextensions-0.3.1/userextensions/mixins.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/models.py` & `django-userextensions-0.3.1/userextensions/models.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/signals.py` & `django-userextensions-0.3.1/userextensions/signals.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm` & `django-userextensions-0.3.1/userextensions/templates/userextensions/ajax/get_token_history_for_srv_acct.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/custom/create_custom_service_account.htm` & `django-userextensions-0.3.1/userextensions/templates/userextensions/custom/create_custom_service_account.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/custom/manage_service_accounts.html` & `django-userextensions-0.3.1/userextensions/templates/userextensions/custom/manage_service_accounts.html`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 {% endblock local_head %}
 
 {% block content %}
 <div class="container-fluid my-5 animated fadeIn">
     <h1 class="text-primary"><b>Manage Service Accounts: </b></h1>
 </div>
 <div>&nbsp;</div>
-<div class="container-fluid pl-5 pr-5">
+<div class="container-fluid ps-5 pe-5">
     <div class="row mb-5 animated fadeIn" style="animation-delay: .25s;">
-        <div class="col-sm-12 col-md-3 col-lg-2 mb-3 pl-0">
+        <div class="col-sm-12 col-md-3 col-lg-2 mb-3 ps-0">
             <i class="fas fa-users-cog fa-6x text-primary"></i><br/>
         </div>
         <div class="col-sm-12 col-md-9 col-lg-10">
             <div class="row">
-                <div class="h3 text-primary font-weight-bold mb-3 pl-0">Service Accounts</div>
+                <div class="h3 text-primary font-weight-bold mb-3 ps-0">Service Accounts</div>
             </div>
             <div class="row">
                 <table style="width: 100%">
                     <thead>
                         <tr>
                             <th class="bg-transparent text-secondary">User Account</th>
                             <th class="bg-transparent text-secondary">Group</th>
@@ -33,123 +33,123 @@
                     <tbody>
                     {% for row in service_accounts %}
                     <tr class="border-top border-secondary">
                         <td><span class="mx-1">{{ row.user }}</span></td>
                         <td><span class="mx-1">{{ row.group }}</span></td>
                         <td>
                             {% if row.enabled %}
-                            <span class="text-primary mx-2"><i class="fas fa-check"></i></span>
+                            <span class="text-primary mx-1"><i class="fas fa-check"></i></span>
                             {% else %}
-                            <span class="text-danger mx-2"><i class="fas fa-times"></i></span>
+                            <span class="text-danger mx-1"><i class="fas fa-times"></i></span>
                             {% endif %}
                         </td>
                         <td>
                             {% if row.admin_enabled %}
-                            <span class="text-primary mx-2"><i class="fas fa-check"></i></span>
+                            <span class="text-primary mx-1"><i class="fas fa-check"></i></span>
                             {% else %}
-                            <span class="text-danger mx-2"><i class="fas fa-times"></i></span>
+                            <span class="text-danger mx-1"><i class="fas fa-times"></i></span>
                             {% endif %}
                         </td>
                         <td>
                             <!-- view api token -->
-                            <a href="#" title="view api token" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="view api token" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="showInfo('{% url "userextensions:show_srv_acct_token" %}', '{{ row.user.auth_token }}', 'API Token: <small><i>{{ row.user.username }}</i></small>', 'lg');">
-                                <i class="fas fa-key mx-2"></i>
+                                <i class="fas fa-key mx-1"></i>
                             </a>
 
                             <!-- refresh api token -->
-                            <a href="#" title="refresh api token" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="refresh api token" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="confirmAction('{% url "userextensions:refresh_srv_acct_token" %}?srv_acct_id={{ row.id }}', 'Update Token', 'This will delete the API token and create a new one. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-sync-alt mx-2"></i>
+                                <i class="fas fa-sync-alt mx-1"></i>
                             </a>
 
                             <!-- api token history -->
-                            <a href="#" title="view api token history" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="view api token history" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="showInfo('{% url "userextensions:get_srv_acct_token_history" %}', '{{ row.id }}', 'Token Refresh History: <small><i>{{ row.user.username }}</i></small>', 'lg');">
-                                <i class="fas fa-history mx-2"></i>
+                                <i class="fas fa-history mx-1"></i>
                             </a>
 
                             <!-- enable/disable -->
                             {% if row.enabled %}
-                            <a href="#" title="disable service account" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="disable service account" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="confirmAction('{% url "userextensions:disable_srv_account" %}?srv_acct_id={{ row.id }}', 'Disable Service Account', 'This will set the <i>{{ row.user }}</i> service account to disabled. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-toggle-off mx-2"></i>
+                                <i class="fas fa-toggle-off mx-1"></i>
                             </a>
                             {% else %}
-                            <a href="#" title="enable service account" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="enable service account" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                 onClick="confirmAction('{% url "userextensions:enable_srv_account" %}?srv_acct_id={{ row.id }}', 'Enable Service Account', 'This will set the <i>{{ row.user }}</i> service account to enabled. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-toggle-on mx-2"></i>
+                                <i class="fas fa-toggle-on mx-1"></i>
                             </a>
                             {% endif %}
 
                             <!-- view users in group -->
-                            <a href="#" title="view users in {{ row.group }}" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="view users in {{ row.group }}" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="showInfo('{% url "userextensions:get_users_per_group" %}', '{{ row.group.id }}', 'Users: <small><i>{{ row.group.name }}</i></small>', 'lg');">
-                            <i class="fas fa-user-friends mx-2"></i>
+                            <i class="fas fa-user-friends mx-1"></i>
                             </a>
 
-                            <a href="#" title="create custom service account in {{ row.group }}" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="create custom service account in {{ row.group }}" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="createCustomServiceAccount('{% url 'userextensions:create_custom_srv_account' %}?id={{ row.group.id }}', 'Create Custom Service Account', 'Create');">
-                                <i class="fas fa-user-plus mx-2"></i>
+                                <i class="fas fa-user-plus mx-1"></i>
                             </a>
 
                             <!-- delete -->
-                            <a href="#" title="delete service account" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="delete service account" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="confirmAction('{% url "userextensions:delete_srv_account" %}?srv_acct_id={{ row.id }}', 'Delete Service Account', 'This will permanently delete the <i>{{ row.user }}</i> service account. Do you wish to continue?', 'Continue', 'POST');">
-                               <i class="fas fa-trash mx-2"></i>
+                               <i class="fas fa-trash mx-1"></i>
                             </a>
                         </td>
                     </tr>
                     {% endfor %}
                     </tbody>
                 </table>
             </div>
         </div>
     </div>
 
     &nbsp;<br/>
 
     {% if groups %}
     <div class="row mb-5 animated fadeIn" style="animation-delay: .5s;">
-        <div class="col-sm-12 col-md-3 col-lg-2 mb-3 pl-0">
+        <div class="col-sm-12 col-md-3 col-lg-2 mb-3 ps-0">
             <i class="fas fa-users fa-6x text-primary"></i>
         </div>
         <div class="col-sm-12 col-md-9 col-lg-10">
             <div class="row">
-                <h3 class="text-primary font-weight-bold mb-3 pl-0">Groups Without Service Accounts</h3>
+                <h3 class="text-primary font-weight-bold mb-3 ps-0">Groups Without Service Accounts</h3>
             </div>
             <div class="row">
                 <table style="width: 100%">
                     <thead>
                     <tr>
                         <th class="bg-transparent text-secondary">Group</th>
                         <th class="bg-transparent text-secondary">User Count</th>
                         <th class="bg-transparent text-secondary">Actions</th>
                     </tr>
                     </thead>
                     <tbody>
                     {% for row in groups %}
                     <tr class="border-top border-secondary">
-                        <td><span class="ml-1">{{ row.name }}</span></td>
-                        <td><span class="ml-1">
-                            <a href="#" title="view users in {{ row }}" role="button" data-toggle="tooltip" data-placement="left"
+                        <td><span class="ms-1">{{ row.name }}</span></td>
+                        <td><span class="ms-1">
+                            <a href="#" title="view users in {{ row }}" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="showInfo('{% url "userextensions:get_users_per_group" %}', '{{ row.id }}', 'Users: <small><i>{{ row.name }}</i></small>', 'lg');">{{ row.user_set.count }}</a>
                         </span></td>
                         <td>
-                            <a href="#" title="view users in {{ row }}" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="view users in {{ row }}" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="showInfo('{% url "userextensions:get_users_per_group" %}', '{{ row.id }}', 'Users: <small><i>{{ row.name }}</i></small>', 'lg');">
-                                <i class="fas fa-user-friends mx-2"></i>
+                                <i class="fas fa-user-friends mx-1"></i>
                             </a>
-                            <a href="#" title="create service account" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="create service account" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="confirmAction('{% url 'userextensions:create_srv_account' %}?group_id={{ row.id }}', 'Create Service Account', 'This will create a new service account linked to <b><i>{{ row.name }}</i></b>. Do you wish to continue?', 'Continue', 'POST');">
-                                <i class="fas fa-plus mx-2"></i>
+                                <i class="fas fa-plus mx-1"></i>
                             </a>
-                            <a href="#" title="create custom service account" role="button" data-toggle="tooltip" data-placement="left"
+                            <a href="#" title="create custom service account" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                                onClick="createCustomServiceAccount('{% url 'userextensions:create_custom_srv_account' %}?id={{ row.id }}', 'Create Custom Service Account', 'Create');">
-                                <i class="fas fa-user-plus mx-2"></i>
+                                <i class="fas fa-user-plus mx-1"></i>
                             </a>
                         </td>
                     </tr>
                     {% endfor %}
                     </tbody>
                 </table>
             </div>
```

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/detail/detail_user.html` & `django-userextensions-0.3.1/userextensions/templates/userextensions/detail/detail_user.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,158 +3,158 @@
 
 {% block local_head %}
 {% include 'handyhelpers/component/clipboard.htm' %}
 {% endblock local_head %}
 
 
 {% block content %}
-<div class="container-fluid mb-5 animated fadeIn">
+<div class="container-fluid my-5 animated fadeIn">
     <h1 class="text-primary"><b>User Profile: </b><span class="text-secondary"><small>{{ user.username }}</small></span></h1>
 </div>
 
-<div class="container-fluid pl-5 pr-5">
+<div class="container-fluid ps-5 pe-5">
 
     <!-- user details -->
     <div class="row mb-5 animated fadeIn" style="animation-delay: .15s;">
         <div class="col-sm-12 col-md-3 col-lg-2 mb-3 text-sm-left text-md-center">
             <div class="text-primary mb-2"><i class="fa-regular fa-id-card fa-6x"></i></div>
-            <div class="text-secondary font-weight-bold">Identity</div>
+            <div class="text-secondary fw-bold">Identity</div>
         </div>
 
         <div class="col-sm-12 col-md-9 col-lg-10">
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Is Active: </div>
+                <div class="col-sm-3 fw-bold text-primary">Is Active: </div>
                 <div class="col-sm-9">
                     {% if user.is_active %}
                     <span class="text-primary"><i class="fa fa-check fa-fw"></i></span>
                     {% else %}
                     <span class="text-danger"><i class="fa fa-times fa-fw"></i></span>
                     {% endif %}
                 </div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Is Staff: </div>
+                <div class="col-sm-3 fw-bold text-primary">Is Staff: </div>
                 <div class="col-sm-9">
                     {% if user.is_staff %}
                     <span class="text-primary"><i class="fa fa-check fa-fw"></i></span>
                     {% else %}
                     <span class="text-danger"><i class="fa fa-times fa-fw"></i></span>
                     {% endif %}
                 </div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Is Superuser: </div>
+                <div class="col-sm-3 fw-bold text-primary">Is Superuser: </div>
                 <div class="col-sm-9">
                     {% if user.is_superuser %}
                     <span class="text-primary"><i class="fa fa-check fa-fw"></i></span>
                     {% else %}
                     <span class="text-danger"><i class="fa fa-times fa-fw"></i></span>
                     {% endif %}
                 </div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Date Joined: </div>
+                <div class="col-sm-3 fw-bold text-primary">Date Joined: </div>
                 <div class="col-sm-9">{{ user.date_joined }}</div>
             </div>
 
             <div class="row p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">API Token: </div>
+                <div class="col-sm-3 fw-bold text-primary">API Token: </div>
                 <div class="col-sm-9 text-primary">
                     <span id="clipboardExample1">{{ token }}</span> &nbsp;
-                    <a href="#" title="copy token" class="cpy ml-1 mr-1" data-clipboard-target="#clipboardExample1"><i class="fas fa-copy"></i></a>
-                    <a href="#" title="refresh token" class="ml-1 mr-1"
+                    <a href="#" title="copy token" class="hvr-grow align-baseline cpy ms-1 me-1" data-clipboard-target="#clipboardExample1"><i class="fas fa-copy"></i></a>
+                    <a href="#" title="refresh token" class="hvr-grow align-baseline ms-1 me-1"
                        onClick="confirmAction('{% url "userextensions:refresh_api_token" %}', 'Update Token', 'This will delete your API token and create a new one. Do you wish to continue?', 'Continue', 'POST');" role="button" data-bs-toggle="tooltip" data-placement="left">
                         <i class="fas fa-sync-alt"></i>
                     </a>
                 </div>
             </div>
 
         </div>
     </div>
     <br/>
 
     <!-- user profile -->
     <div class="row mb-5 animated fadeIn" style="animation-delay: .3s;">
         <div class="col-sm-12 col-md-3 col-lg-2 mb-3 text-sm-left text-md-center">
             <div class="text-primary mb-2"><i class="fas fa-cogs fa-6x"></i></div>
-            <div class="text-secondary font-weight-bold">Settings</div>
+            <div class="text-secondary fw-bold">Settings</div>
         </div>
 
         <div class="col-sm-12 col-md-9 col-lg-10">
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Theme: </div>
+                <div class="col-sm-3 fw-bold text-primary">Theme: </div>
                 <div class="col-sm-9">{{ user.preference.theme }}</div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Timezone: </div>
+                <div class="col-sm-3 fw-bold text-primary">Timezone: </div>
                 <div class="col-sm-9">{{ user.preference.timezone }}</div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Help Text Enabled: </div>
+                <div class="col-sm-3 fw-bold text-primary">Help Text Enabled: </div>
                 <div class="col-sm-9">
                     {% if user.preference.help_text_enable %}
                     <span class="text-primary"><i class="fa fa-check fa-fw"></i></span>
                     {% else %}
                     <span class="text-danger"><i class="fa fa-times fa-fw"></i></span>
                     {% endif %}
                 </div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Recents Count: </div>
+                <div class="col-sm-3 fw-bold text-primary">Recents Count: </div>
                 <div class="col-sm-9">{{ user.preference.recents_count }}</div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Page Refresh: </div>
+                <div class="col-sm-3 fw-bold text-primary">Page Refresh: </div>
                 <div class="col-sm-9">{{ user.preference.page_refresh_time }}</div>
             </div>
 
             <div class="row border-bottom border-secondary p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Start Page: </div>
+                <div class="col-sm-3 fw-bold text-primary">Start Page: </div>
                 <div class="col-sm-9">
                     {% if user.preference.start_page %}
                     <a href="{{ user.preference.start_page }}">{{ user.preference.start_page }}</a>
                     {% else %}
                     None
                     {% endif %}
                 </div>
             </div>
 
             <div class="row p-2">
-                <div class="col-sm-3 font-weight-bold text-primary">Edit: </div>
+                <div class="col-sm-3 fw-bold text-primary">Edit: </div>
                 <div class="col-sm-9">
-                    <a href="#" class="no-underline" data-bs-toggle="modal" data-bs-target="#modal_{{ form_data_user_preferences.modal_name }}">
+                    <a href="#" class="hvr-grow align-baseline" data-bs-toggle="modal" data-bs-target="#modal_{{ form_data_user_preferences.modal_name }}">
                         <i class="fas fa-edit"></i>
                     </a>
                 </div>
             </div>
 
         </div>
     </div>
     <br/>
 
     <!-- groups -->
     <div class="row mb-5 animated fadeIn" style="animation-delay: .45s;">
         <div class="col-sm-12 col-md-3 col-lg-2 mb-3 text-sm-left text-md-center">
             <div class="text-primary mb-2"><i class="fas fa-users fa-6x"></i></div>
-            <div class="text-secondary font-weight-bold">Groups</div>
+            <div class="text-secondary fw-bold">Groups</div>
         </div>
 
         <div class="col-sm-12 col-md-9 col-lg-10">
             <div class="row">
                 {% if groups %}
                 {% for group in groups %}
                 <div class="col-sm-12 col-md-8 col-lg-4">
-                    <a href="#" title="view users in {{ group }}" role="button" data-toggle="tooltip" data-placement="left"
+                    <a href="#" title="view users in {{ group }}" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                        onClick="showInfo('{% url "userextensions:get_users_per_group" %}', '{{ group.id }}', 'Users: <small><i>{{ group }}</i></small>', 'lg');">
                         {{ group }}
                     </a>
                 </div>
                 {% endfor %}
                 {% else %}
                 <div>no group memberships found</div>
```

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/form/edit_favorite.htm` & `django-userextensions-0.3.1/userextensions/templates/userextensions/form/edit_favorite.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm` & `django-userextensions-0.3.1/userextensions/templates/userextensions/snippets/user_extensions_nav_menu.htm`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 
 To use this, add the following in your navbar where appropriate:
     {% include 'snippits/user_theme.htm' %}
 
 {% endcomment %}
 {% load userextension_tags %}
 
-<a class="dropdown-item" href="{% url 'userextensions:detail_user' %}"><i class="fa fa-address-card fw" style="margin-right: .9em"></i>Profile</a>
-<a class="dropdown-item" href="{% url 'userextensions:manage_service_accounts' %}"><i class="fas fa-users-cog fw" style="margin-right: .75em"></i>Service Accounts</a>
-<a class="dropdown-item" href="{% url 'userextensions:list_recents' %}"><b class="far fa-clock fw mr-3"></b>Recents</a>
-<a class="dropdown-item" href="{% url 'userextensions:list_favorites' %}"><i class="far fa-heart mr-3"></i>Favorites</a>
+<a class="dropdown-item" href="{% url 'userextensions:detail_user' %}"><i class="fa fa-address-card fw" style="margin-right: .85em"></i>Profile</a>
+<a class="dropdown-item" href="{% url 'userextensions:manage_service_accounts' %}"><i class="fas fa-users-cog fw" style="margin-right: .8em"></i>Service Accounts</a>
+<a class="dropdown-item" href="{% url 'userextensions:list_recents' %}"><b class="far fa-clock fw me-3"></b>Recents</a>
+<a class="dropdown-item" href="{% url 'userextensions:list_favorites' %}"><i class="far fa-heart me-3"></i>Favorites</a>
 <div class="dropdown-divider"></div>
 <div class="dropdown-item">
     {% is_favorite request as favorite_id %}
     {% if favorite_id %}
         <form name="addFavoriteForm" method="POST" action="{% url 'userextensions:delete_favorite' favorite_id %}">
             {% csrf_token %}
             <input type="hidden" name="name" value="">
-            <a href="javascript:document.addFavoriteForm.submit()"><i class="fas fa-heart-broken mr-3"></i></b>Remove Favorite</a>
+            <a href="javascript:document.addFavoriteForm.submit()"><i class="fas fa-heart-broken me-3"></i></b>Remove Favorite</a>
         </form>
     {% else %}
         <form name="deleteFavoriteForm" method="POST" action="{% url 'userextensions:add_favorite' %}">
             {% csrf_token %}
             <input type="hidden" name="name" value="">
-            <a href="javascript:document.deleteFavoriteForm.submit()"><b class="fas fa-heart mr-3"></b>Add Favorite</a>
+            <a href="javascript:document.deleteFavoriteForm.submit()"><b class="fas fa-heart me-3"></b>Add Favorite</a>
         </form>
     {% endif %}
 </div>
 <div class="dropdown-item">
     <form name="startPageForm" method="POST" action="{% url 'userextensions:set_start_page' %}">
         {% csrf_token %}
         <input type="hidden" name="name" value="">
-        <a href="javascript:document.startPageForm.submit()"><b class="fas fa-sign-in-alt mr-3"></b>Set start page</a>
+        <a href="javascript:document.startPageForm.submit()"><b class="fas fa-sign-in-alt me-3"></b>Set start page</a>
     </form>
 </div>
```

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_favorites.htm` & `django-userextensions-0.3.1/userextensions/templates/userextensions/table/table_favorites.htm`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,22 @@
             <td>{{ row.name }}</td>
             <td><a href="{{ row.url }}">{{ row.url }}</a></td>
             <td>{{ row.updated_at }}</td>
 
             <!-- actions -->
             <td>
                 <!-- edit favorite -->
-                <a href="#" title="edit favorite" role="button" data-toggle="tooltip" data-placement="left"
+                <a href="#" title="edit favorite" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                    onClick="EditFavorite('{% url 'userextensions:edit_favorite' %}?id={{ row.id }}', 'Edit Favorite: {{ row.name }} ', '{{ row.name }}', 'Update');">
-                    <i class="fas fa-edit text-primary ml-1 mr-1"></i>
+                    <i class="fas fa-edit text-primary ms-1 me-1"></i>
                 </a>
 
                 <!-- delete favorite -->
-                <a href="#" title="delete favorite" role="button" data-toggle="tooltip" data-placement="left"
+                <a href="#" title="delete favorite" role="button" data-toggle="tooltip" data-placement="left" class="hvr-grow align-baseline"
                    onClick="confirmAction('{% url "userextensions:delete_favorite" row.pk %}', 'Delete Favorite', 'This favorite will be permanently removed from your list of favorites; do you wish to continue?', 'Continue', 'POST');">
-                   <i class="fas fa-trash ml-1 mr-1"></i>
+                   <i class="fas fa-trash ms-1 me-1"></i>
                 </a>
             </td>
         </tr>
     {% endfor %}
     </tbody>
 </table>
```

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/table/table_recents.htm` & `django-userextensions-0.3.1/userextensions/templates/userextensions/table/table_recents.htm`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     {% for row in queryset %}
         <tr>
             <td><a href="{{ row.url }}">{{ row.url }}</a></td>
             <td>{{ row.updated_at }}</td>
 
             <!-- actions -->
             <td>
-                <a href="#" onClick="confirmAction('{% url "userextensions:delete_recent" row.pk %}', 'Delete Recent', 'This recent will be permanently removed from your list of recents; do you wish to continue?', 'Continue', 'POST');">
-                    <i class="fas fa-trash ml-1 mr-1"></i>
+                <a href="#" class="hvr-grow align-baseline"
+                    onClick="confirmAction('{% url "userextensions:delete_recent" row.pk %}', 'Delete Recent', 'This recent will be permanently removed from your list of recents; do you wish to continue?', 'Continue', 'POST');">
+                    <i class="fas fa-trash ms-1 me-1"></i>
                 </a>
             </td>
         </tr>
     {% endfor %}
     </tbody>
 </table>
```

### Comparing `django-userextensions-0.3.0/userextensions/templates/userextensions/userextensions_base.htm` & `django-userextensions-0.3.1/userextensions/templates/userextensions/userextensions_base.htm`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/templatetags/userextension_tags.py` & `django-userextensions-0.3.1/userextensions/templatetags/userextension_tags.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/urls.py` & `django-userextensions-0.3.1/userextensions/urls.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/views/action.py` & `django-userextensions-0.3.1/userextensions/views/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,27 +79,23 @@
         except Exception as err:
             messages.add_message(request, messages.ERROR, f'Error adding favorite: {err}',
                                  extra_tags='alert-danger')
         return redirect(referrer)
 
 
 class DeleteFavorite(LoginRequiredMixin, DeleteView):
-    """ delete a favorite (by pk) and return to the referring page """
-    def delete(self, request, *args, **kwargs):
-        UserFavorite.objects.filter(**kwargs).delete()
-        messages.add_message(self.request, messages.INFO, 'Favorite successfully deleted', extra_tags='alert-info')
-        return redirect(self.request.META.get('HTTP_REFERER'))
+    """ delete a favorite (by pk) and return list favorites page """
+    model = UserFavorite
+    success_url = "/userextensions/list_favorites"
 
 
 class DeleteRecent(LoginRequiredMixin, DeleteView):
-    """ delete a recent (by pk) and return to the referring page """
-    def delete(self, request, *args, **kwargs):
-        UserRecent.objects.filter(**kwargs).delete()
-        messages.add_message(self.request, messages.INFO, 'Recent successfully deleted', extra_tags='alert-info')
-        return redirect(self.request.META.get('HTTP_REFERER'))
+    """ delete a recent (by pk) and return list recents page """
+    model = UserRecent
+    success_url = "/userextensions/list_recents"
 
 
 class UserLoginRedirect(LoginRequiredMixin, View):
     """ Check if a user has a preferred 'start page' to load after login. If so, redirect to that page after login, else
         redirect to the project root page.
         To enable this redirect, set the LOGIN_REDIRECT_URL parameter in the settings.py to
         /userextensions/user_login_redirect and include userextensions.urls in the project level urls.py
```

### Comparing `django-userextensions-0.3.0/userextensions/views/ajax.py` & `django-userextensions-0.3.1/userextensions/views/ajax.py`

 * *Files identical despite different names*

### Comparing `django-userextensions-0.3.0/userextensions/views/gui.py` & `django-userextensions-0.3.1/userextensions/views/gui.py`

 * *Files identical despite different names*

