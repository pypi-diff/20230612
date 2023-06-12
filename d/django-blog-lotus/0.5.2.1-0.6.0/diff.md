# Comparing `tmp/django-blog-lotus-0.5.2.1.tar.gz` & `tmp/django-blog-lotus-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-blog-lotus-0.5.2.1.tar", last modified: Sat Jun  3 01:20:31 2023, max compression
+gzip compressed data, was "django-blog-lotus-0.6.0.tar", last modified: Mon Jun 12 00:49:51 2023, max compression
```

## Comparing `django-blog-lotus-0.5.2.1.tar` & `django-blog-lotus-0.6.0.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      304 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2575 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1330 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2575 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2721 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      322 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       14 2023-06-03 01:20:31.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-05-03 20:30:50.000000 django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/zip-safe
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      152 2022-12-19 01:25:34.000000 django-blog-lotus-0.5.2.1/lotus/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      258 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4001 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/admin/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/admin/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1418 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/admin/translated.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      231 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/apps.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      785 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/choices.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/contrib/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/contrib/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1667 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/contrib/django_configuration.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      330 2023-01-21 14:51:37.000000 django-blog-lotus-0.5.2.1/lotus/exceptions.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/factories/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      376 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7596 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1573 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/author.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2520 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1592 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/factories/tag.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/forms/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      367 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/forms/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5662 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/forms/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3464 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/forms/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1285 2021-10-25 23:19:15.000000 django-blog-lotus-0.5.2.1/lotus/forms/translated.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/locale/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/locale/de/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.512260 django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8674 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8627 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/django.pot
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/locale/en/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8674 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/locale/fr/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7232 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    11353 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4091 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/lookups.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/management/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/management/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/management/commands/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/management/commands/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    22425 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/management/commands/lotus_demo.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5480 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/managers.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/migrations/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    12384 2023-06-03 01:20:11.000000 django-blog-lotus-0.5.2.1/lotus/migrations/0001_initial.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-01-01 21:16:12.000000 django-blog-lotus-0.5.2.1/lotus/migrations/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/models/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      148 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/lotus/models/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    12914 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/models/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1599 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/models/author.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3232 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/models/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      551 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/models/translated.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      194 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2.1/lotus/responses.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2733 2023-06-03 01:07:36.000000 django-blog-lotus-0.5.2.1/lotus/settings.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/templates/admin/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.508260 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4914 2023-05-03 20:48:05.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/change_form.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1515 2023-01-16 21:53:43.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/translate_original.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1633 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/change_form.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1519 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/translate_original.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     9789 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      752 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2798 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      383 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/siblings.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      738 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      717 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/partials/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      340 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/partials/item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      164 2022-01-02 21:03:15.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/base.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.516260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1514 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      751 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      587 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/item.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/siblings.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      613 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/pagination.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      544 2022-12-18 14:29:13.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/preview_switch.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      726 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/detail.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      951 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/list.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/templatetags/
--rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2021-07-04 20:57:38.000000 django-blog-lotus-0.5.2.1/lotus/templatetags/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    11813 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/templatetags/lotus.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1659 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/urls.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/lotus/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1719 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/utils/factory.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    13239 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/utils/imaging.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     8329 2023-04-03 23:40:23.000000 django-blog-lotus-0.5.2.1/lotus/utils/tests.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/views/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      768 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/views/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/lotus/views/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      300 2023-01-16 00:55:04.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      295 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      299 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3770 2022-01-03 00:27:11.000000 django-blog-lotus-0.5.2.1/lotus/views/admin/mixins.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4610 2023-03-19 17:30:54.000000 django-blog-lotus-0.5.2.1/lotus/views/article.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3156 2022-12-18 15:40:32.000000 django-blog-lotus-0.5.2.1/lotus/views/author.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3148 2022-12-18 15:40:43.000000 django-blog-lotus-0.5.2.1/lotus/views/category.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5633 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/views/mixins.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2614 2022-07-04 12:22:57.000000 django-blog-lotus-0.5.2.1/lotus/views/preview.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5347 2023-04-04 00:51:02.000000 django-blog-lotus-0.5.2.1/lotus/views/tag.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2099 2023-06-03 01:20:31.520260 django-blog-lotus-0.5.2.1/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-05-29 23:54:08.000000 django-blog-lotus-0.5.2.1/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.815154 django-blog-lotus-0.6.0/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      304 2021-05-29 23:54:08.000000 django-blog-lotus-0.6.0/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2681 2023-06-12 00:49:51.815154 django-blog-lotus-0.6.0/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1363 2023-06-12 00:49:35.000000 django-blog-lotus-0.6.0/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.803154 django-blog-lotus-0.6.0/django_blog_lotus.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2681 2023-06-12 00:49:51.000000 django-blog-lotus-0.6.0/django_blog_lotus.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2742 2023-06-12 00:49:51.000000 django-blog-lotus-0.6.0/django_blog_lotus.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-06-12 00:49:51.000000 django-blog-lotus-0.6.0/django_blog_lotus.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      322 2023-06-12 00:49:51.000000 django-blog-lotus-0.6.0/django_blog_lotus.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       14 2023-06-12 00:49:51.000000 django-blog-lotus-0.6.0/django_blog_lotus.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-06-11 00:10:41.000000 django-blog-lotus-0.6.0/django_blog_lotus.egg-info/zip-safe
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      152 2022-12-19 01:25:34.000000 django-blog-lotus-0.6.0/lotus/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      127 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4247 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/admin/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2754 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/admin/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2211 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/admin_filters.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      231 2022-01-03 00:27:11.000000 django-blog-lotus-0.6.0/lotus/apps.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      785 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/choices.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/contrib/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/contrib/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1739 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/contrib/django_configuration.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      330 2023-01-21 14:51:37.000000 django-blog-lotus-0.6.0/lotus/exceptions.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/factories/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      376 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/factories/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7596 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/factories/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1573 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/factories/author.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2520 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/factories/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1592 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/factories/tag.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/forms/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      367 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/forms/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5662 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/forms/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3464 2022-01-03 00:27:11.000000 django-blog-lotus-0.6.0/lotus/forms/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1285 2021-10-25 23:19:15.000000 django-blog-lotus-0.6.0/lotus/forms/translated.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/locale/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.803154 django-blog-lotus-0.6.0/lotus/locale/de/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2023-06-12 00:42:27.000000 django-blog-lotus-0.6.0/lotus/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10634 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10587 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/locale/django.pot
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.803154 django-blog-lotus-0.6.0/lotus/locale/en/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2023-06-12 00:42:27.000000 django-blog-lotus-0.6.0/lotus/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10634 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.803154 django-blog-lotus-0.6.0/lotus/locale/fr/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7687 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    13457 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4091 2023-06-09 12:31:44.000000 django-blog-lotus-0.6.0/lotus/lookups.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/management/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/management/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.807154 django-blog-lotus-0.6.0/lotus/management/commands/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/management/commands/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    22425 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/management/commands/lotus_demo.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5480 2023-04-04 00:51:02.000000 django-blog-lotus-0.6.0/lotus/managers.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/migrations/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    12384 2023-06-03 01:22:28.000000 django-blog-lotus-0.6.0/lotus/migrations/0001_initial.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-01-01 21:16:12.000000 django-blog-lotus-0.6.0/lotus/migrations/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/models/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      148 2021-05-29 23:54:08.000000 django-blog-lotus-0.6.0/lotus/models/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    12914 2023-04-04 00:51:02.000000 django-blog-lotus-0.6.0/lotus/models/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1599 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/models/author.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3458 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/models/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      551 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/models/translated.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      194 2022-07-04 12:22:57.000000 django-blog-lotus-0.6.0/lotus/responses.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3291 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/settings.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.803154 django-blog-lotus-0.6.0/lotus/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.803154 django-blog-lotus-0.6.0/lotus/templates/admin/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.803154 django-blog-lotus-0.6.0/lotus/templates/admin/lotus/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/admin/lotus/article/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2645 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/admin/lotus/article/change_form.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1515 2023-06-11 12:54:08.000000 django-blog-lotus-0.6.0/lotus/templates/admin/lotus/article/translate_original.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/admin/lotus/category/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2364 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/admin/lotus/category/change_form.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1519 2022-01-03 00:27:11.000000 django-blog-lotus-0.6.0/lotus/templates/admin/lotus/category/translate_original.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/article/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     9782 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/article/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      756 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/article/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/article/partials/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2798 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/article/partials/item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1070 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/article/partials/siblings.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/author/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      742 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/author/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      721 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/author/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/author/partials/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      340 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/author/partials/item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      164 2022-01-02 21:03:15.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/base.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/category/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3281 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/category/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      755 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/category/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/category/partials/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      587 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/category/partials/item.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      741 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/category/partials/siblings.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      613 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/pagination.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      544 2022-12-18 14:29:13.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/preview_switch.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templates/lotus/tag/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      730 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/tag/detail.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      955 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templates/lotus/tag/list.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.811154 django-blog-lotus-0.6.0/lotus/templatetags/
+-rw-r--r--   0 emencia   (1001) emencia   (1001)        0 2021-07-04 20:57:38.000000 django-blog-lotus-0.6.0/lotus/templatetags/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    13113 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/templatetags/lotus.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1651 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/urls.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.815154 django-blog-lotus-0.6.0/lotus/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2021-05-29 23:54:08.000000 django-blog-lotus-0.6.0/lotus/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1719 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/utils/factory.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    13239 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/utils/imaging.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1071 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/utils/language.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     8329 2023-04-03 23:40:23.000000 django-blog-lotus-0.6.0/lotus/utils/tests.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.815154 django-blog-lotus-0.6.0/lotus/views/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      768 2023-04-04 00:51:02.000000 django-blog-lotus-0.6.0/lotus/views/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-06-12 00:49:51.815154 django-blog-lotus-0.6.0/lotus/views/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      300 2023-01-16 00:55:04.000000 django-blog-lotus-0.6.0/lotus/views/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      295 2022-01-03 00:27:11.000000 django-blog-lotus-0.6.0/lotus/views/admin/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      299 2022-01-03 00:27:11.000000 django-blog-lotus-0.6.0/lotus/views/admin/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3770 2022-01-03 00:27:11.000000 django-blog-lotus-0.6.0/lotus/views/admin/mixins.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4704 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/views/article.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3195 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/views/author.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3186 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/views/category.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6187 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/views/mixins.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2614 2022-07-04 12:22:57.000000 django-blog-lotus-0.6.0/lotus/views/preview.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5386 2023-06-12 00:49:36.000000 django-blog-lotus-0.6.0/lotus/views/tag.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2158 2023-06-12 00:49:51.815154 django-blog-lotus-0.6.0/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-05-29 23:54:08.000000 django-blog-lotus-0.6.0/setup.py
```

### Comparing `django-blog-lotus-0.5.2.1/LICENCE.txt` & `django-blog-lotus-0.6.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/PKG-INFO` & `django-blog-lotus-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: django-blog-lotus
-Version: 0.5.2.1
+Version: 0.6.0
 Summary: A weblog application with Django.
 Home-page: https://github.com/emencia/django-blog-lotus
 Author: Emencia
 Author-email: support@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/django-blog-lotus
 Project-URL: Issue Tracker, https://github.com/emencia/django-blog-lotus/issues
 Project-URL: Changelog, https://django-blog-lotus.readthedocs.io/en/latest/history.html
 Project-URL: Documentation, https://django-blog-lotus.readthedocs.io/
 Keywords: Python Django Blog
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: breadcrumbs
 Provides-Extra: dev
 Provides-Extra: quality
 Provides-Extra: doc
 License-File: LICENCE.txt
 
@@ -38,21 +40,21 @@
 .. _django-taggit: https://github.com/jazzband/django-taggit
 
 
 =================
 Django Blog Lotus
 =================
 
-A Django weblog application with builtin multilingual content and inspired from
-deceased Zinnia weblog.
+A Django weblog application with builtin multilingual content and some other features.
+
 
 Features
 ********
 
-* Multilingual articles and categories;
+* Multilingual articles and categories (but still compatible with single language site);
 * Tags for Articles;
 * Featuring, pinning, private and draft modes;
 * Configured CKEditor to write rich text in admin;
 * Preview mode for admins;
 * Publishing date and publishing end date;
 * Included image thumbnailing;
 * SVG soft support in image fields;
```

### Comparing `django-blog-lotus-0.5.2.1/README.rst` & `django-blog-lotus-0.6.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 .. _django-taggit: https://github.com/jazzband/django-taggit
 
 
 =================
 Django Blog Lotus
 =================
 
-A Django weblog application with builtin multilingual content and inspired from
-deceased Zinnia weblog.
+A Django weblog application with builtin multilingual content and some other features.
+
 
 Features
 ********
 
-* Multilingual articles and categories;
+* Multilingual articles and categories (but still compatible with single language site);
 * Tags for Articles;
 * Featuring, pinning, private and draft modes;
 * Configured CKEditor to write rich text in admin;
 * Preview mode for admins;
 * Publishing date and publishing end date;
 * Included image thumbnailing;
 * SVG soft support in image fields;
```

### Comparing `django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/PKG-INFO` & `django-blog-lotus-0.6.0/django_blog_lotus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: django-blog-lotus
-Version: 0.5.2.1
+Version: 0.6.0
 Summary: A weblog application with Django.
 Home-page: https://github.com/emencia/django-blog-lotus
 Author: Emencia
 Author-email: support@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/django-blog-lotus
 Project-URL: Issue Tracker, https://github.com/emencia/django-blog-lotus/issues
 Project-URL: Changelog, https://django-blog-lotus.readthedocs.io/en/latest/history.html
 Project-URL: Documentation, https://django-blog-lotus.readthedocs.io/
 Keywords: Python Django Blog
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: breadcrumbs
 Provides-Extra: dev
 Provides-Extra: quality
 Provides-Extra: doc
 License-File: LICENCE.txt
 
@@ -38,21 +40,21 @@
 .. _django-taggit: https://github.com/jazzband/django-taggit
 
 
 =================
 Django Blog Lotus
 =================
 
-A Django weblog application with builtin multilingual content and inspired from
-deceased Zinnia weblog.
+A Django weblog application with builtin multilingual content and some other features.
+
 
 Features
 ********
 
-* Multilingual articles and categories;
+* Multilingual articles and categories (but still compatible with single language site);
 * Tags for Articles;
 * Featuring, pinning, private and draft modes;
 * Configured CKEditor to write rich text in admin;
 * Preview mode for admins;
 * Publishing date and publishing end date;
 * Included image thumbnailing;
 * SVG soft support in image fields;
```

### Comparing `django-blog-lotus-0.5.2.1/django_blog_lotus.egg-info/SOURCES.txt` & `django-blog-lotus-0.6.0/django_blog_lotus.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 django_blog_lotus.egg-info/PKG-INFO
 django_blog_lotus.egg-info/SOURCES.txt
 django_blog_lotus.egg-info/dependency_links.txt
 django_blog_lotus.egg-info/requires.txt
 django_blog_lotus.egg-info/top_level.txt
 django_blog_lotus.egg-info/zip-safe
 lotus/__init__.py
+lotus/admin_filters.py
 lotus/apps.py
 lotus/choices.py
 lotus/exceptions.py
 lotus/lookups.py
 lotus/managers.py
 lotus/responses.py
 lotus/settings.py
 lotus/urls.py
 lotus/admin/__init__.py
 lotus/admin/article.py
 lotus/admin/category.py
-lotus/admin/translated.py
 lotus/contrib/__init__.py
 lotus/contrib/django_configuration.py
 lotus/factories/__init__.py
 lotus/factories/article.py
 lotus/factories/author.py
 lotus/factories/category.py
 lotus/factories/tag.py
@@ -71,14 +71,15 @@
 lotus/templates/lotus/tag/detail.html
 lotus/templates/lotus/tag/list.html
 lotus/templatetags/__init__.py
 lotus/templatetags/lotus.py
 lotus/utils/__init__.py
 lotus/utils/factory.py
 lotus/utils/imaging.py
+lotus/utils/language.py
 lotus/utils/tests.py
 lotus/views/__init__.py
 lotus/views/article.py
 lotus/views/author.py
 lotus/views/category.py
 lotus/views/mixins.py
 lotus/views/preview.py
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/admin/article.py` & `django-blog-lotus-0.6.0/lotus/admin/article.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 
 from smart_media.admin import SmartModelAdmin
 
 from ..forms import ArticleAdminForm
 from ..models import Article
 from ..views.admin import ArticleAdminTranslateView
 
-from .translated import LanguageListFilter, TranslationStateListFilter
+from ..admin_filters import (
+    LanguageListFilter,
+    PublicationFilter,
+    TranslationStateListFilter,
+)
 
 
 LANGUAGE_NAMES = dict(settings.LANGUAGES)
 """
 Shortcut to get setting as a dict
 """
 
@@ -31,24 +35,29 @@
         "featured",
         "last_update",
         "private",
     )
     list_filter = (
         LanguageListFilter,
         TranslationStateListFilter,
+        PublicationFilter,
         "pinned",
         "featured",
         "private",
     )
     prepopulated_fields = {
         "slug": ("title",),
     }
     ordering = Article.COMMON_ORDER_BY
     search_fields = [
         "title",
+        "seo_title",
+        "lead",
+        "introduction",
+        "content",
     ]
     filter_horizontal = (
         "categories",
         "authors",
         "related",
     )
     fieldsets = (
@@ -113,15 +122,17 @@
         ),
     )
 
     def language_name(self, obj):
         """
         Return humanized name for object language code.
         """
-        return LANGUAGE_NAMES[obj.language]
+        if obj.language in LANGUAGE_NAMES:
+            return LANGUAGE_NAMES[obj.language]
+        return "{} (disabled)".format(obj.language)
     language_name.short_description = _("language")
     language_name.admin_order_field = "language"
 
     def publish_datetime(self, obj):
         """
         Return the merged publish date and time.
         """
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/admin/category.py` & `django-blog-lotus-0.6.0/lotus/admin/category.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from smart_media.admin import SmartModelAdmin
 
 from ..forms import CategoryAdminForm
 from ..models import Category
 from ..views.admin import CategoryAdminTranslateView
 
-from .translated import LanguageListFilter, TranslationStateListFilter
+from ..admin_filters import LanguageListFilter, TranslationStateListFilter
 
 
 LANGUAGE_NAMES = dict(settings.LANGUAGES)
 """
 Shortcut to get setting as a dict
 """
 
@@ -34,14 +34,16 @@
     list_per_page = 50
     prepopulated_fields = {
         "slug": ("title",),
     }
     ordering = Category.COMMON_ORDER_BY
     search_fields = [
         "title",
+        "lead",
+        "description",
     ]
     fieldsets = (
         (
             None, {
                 "fields": (
                     "title",
                     "slug",
@@ -69,15 +71,17 @@
                     "lead",
                 )
             }
         ),
     )
 
     def language_name(self, obj):
-        return LANGUAGE_NAMES[obj.language]
+        if obj.language in LANGUAGE_NAMES:
+            return LANGUAGE_NAMES[obj.language]
+        return "{} (disabled)".format(obj.language)
     language_name.short_description = _("language")
     language_name.admin_order_field = "language"
 
     def is_original(self, obj):
         """
         Check article is an original or a translation.
         """
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/admin/translated.py` & `django-blog-lotus-0.6.0/lotus/admin_filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.contrib import admin
 from django.utils.translation import gettext_lazy as _
 
-from ..choices import get_language_choices
+from .choices import get_language_choices
 
 
 class LanguageListFilter(admin.SimpleListFilter):
     """
     Add Human-readable language title as defined in LANGUAGES setting.
     """
     title = _("language")
@@ -44,7 +44,36 @@
 
     def queryset(self, request, queryset):
         if self.value() == "original":
             return queryset.filter(original__isnull=True)
 
         if self.value() == "translation":
             return queryset.exclude(original__isnull=True)
+
+
+class PublicationFilter(admin.SimpleListFilter):
+    """
+    Filter on article publication state.
+    """
+    title = _("publication state")
+
+    # Parameter for the filter that will be used in the URL query.
+    parameter_name = "is_published"
+
+    def lookups(self, request, model_admin):
+        """
+        Build choices from available languages.
+        """
+        return (
+            ("true", _("Is published")),
+            ("false", _("Is not published")),
+        )
+
+    def queryset(self, request, queryset):
+        """
+        Filter on published or unpublished article depending value is true or false.
+        """
+        if self.value() == "true":
+            return queryset.get_published()
+
+        if self.value() == "false":
+            return queryset.get_unpublished()
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/choices.py` & `django-blog-lotus-0.6.0/lotus/choices.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/contrib/django_configuration.py` & `django-blog-lotus-0.6.0/lotus/contrib/django_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     LOTUS_ENABLE_TAG_INDEX_VIEW,
     LOTUS_ARTICLE_PUBLICATION_STATE_NAMES,
     LOTUS_ARTICLE_SIBLING_TEMPLATE,
     LOTUS_CATEGORY_SIBLING_TEMPLATE,
     LOTUS_PREVIEW_KEYWORD,
     LOTUS_PREVIEW_VARNAME,
     LOTUS_PREVIEW_SWITCH_TEMPLATE,
+    LOTUS_CRUMBS_TITLES,
 )
 
 
 class LotusDefaultSettings:
     """
     Default Lotus settings class to use with a "django-configuration" class.
 
@@ -50,7 +51,9 @@
     LOTUS_CATEGORY_SIBLING_TEMPLATE = LOTUS_CATEGORY_SIBLING_TEMPLATE
 
     LOTUS_PREVIEW_KEYWORD = LOTUS_PREVIEW_KEYWORD
 
     LOTUS_PREVIEW_VARNAME = LOTUS_PREVIEW_VARNAME
 
     LOTUS_PREVIEW_SWITCH_TEMPLATE = LOTUS_PREVIEW_SWITCH_TEMPLATE
+
+    LOTUS_CRUMBS_TITLES = LOTUS_CRUMBS_TITLES
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/factories/article.py` & `django-blog-lotus-0.6.0/lotus/factories/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/factories/author.py` & `django-blog-lotus-0.6.0/lotus/factories/author.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/factories/category.py` & `django-blog-lotus-0.6.0/lotus/factories/category.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/factories/tag.py` & `django-blog-lotus-0.6.0/lotus/factories/tag.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/forms/article.py` & `django-blog-lotus-0.6.0/lotus/forms/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/forms/category.py` & `django-blog-lotus-0.6.0/lotus/forms/category.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/forms/translated.py` & `django-blog-lotus-0.6.0/lotus/forms/translated.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/locale/de/LC_MESSAGES/django.po` & `django-blog-lotus-0.6.0/lotus/locale/de/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,295 +4,325 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-01-03 01:24+0100\n"
+"POT-Creation-Date: 2023-06-12 02:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin/article.py:64 admin/category.py:51
+#: admin/article.py:73 admin/category.py:54
 msgid "Language"
 msgstr ""
 
-#: admin/article.py:71
+#: admin/article.py:80
 msgid "Parameters"
 msgstr ""
 
-#: admin/article.py:79
+#: admin/article.py:88
 msgid "Dates"
 msgstr ""
 
-#: admin/article.py:87 admin/category.py:58
+#: admin/article.py:96 admin/category.py:61
 msgid "Content"
 msgstr ""
 
-#: admin/article.py:97 admin/category.py:66
+#: admin/article.py:106 admin/category.py:69
 msgid "SEO"
 msgstr ""
 
-#: admin/article.py:105
+#: admin/article.py:114
 msgid "Relations"
 msgstr ""
 
-#: admin/article.py:120 admin/category.py:76 admin/translated.py:16
-#: admin/translated.py:58 models/translated.py:18
+#: admin/article.py:132 admin/category.py:81 admin_filters.py:11
+#: models/translated.py:12
 msgid "language"
 msgstr ""
 
-#: admin/article.py:128
+#: admin/article.py:140
 msgid "publish date"
 msgstr ""
 
-#: admin/article.py:142
+#: admin/article.py:148
 msgid "published"
 msgstr ""
 
-#: admin/article.py:150 admin/category.py:84
+#: admin/article.py:156 admin/category.py:89
 msgid "original"
 msgstr ""
 
-#: admin/category.py:89
+#: admin/category.py:94
 msgid "articles"
 msgstr ""
 
-#: admin/translated.py:27
-msgid "Default language"
+#: admin_filters.py:34
+msgid "translation state"
 msgstr ""
 
-#: admin/translated.py:38
-msgid "All"
+#: admin_filters.py:41
+msgid "Is an original"
 msgstr ""
 
-#: admin/translated.py:81
-msgid "translation state"
+#: admin_filters.py:42
+msgid "Is a translation"
 msgstr ""
 
-#: admin/translated.py:88
-msgid "Is an original"
+#: admin_filters.py:57
+msgid "publication state"
 msgstr ""
 
-#: admin/translated.py:89
-msgid "Is a translation"
+#: admin_filters.py:67
+msgid "Is published"
+msgstr ""
+
+#: admin_filters.py:68
+msgid "Is not published"
 msgstr ""
 
 #: apps.py:7
 msgid "Lotus weblog"
 msgstr ""
 
-#: choices.py:15
+#: choices.py:16
 msgid "draft"
 msgstr ""
 
-#: choices.py:16
+#: choices.py:17
 msgid "available"
 msgstr ""
 
-#: forms/article.py:95 forms/category.py:66
+#: forms/article.py:106 forms/category.py:66
 msgid "You can't have a language identical to the original relation."
 msgstr ""
 
-#: forms/article.py:105 forms/category.py:76
+#: forms/article.py:116 forms/category.py:76
 msgid "You can't have an original relation in the same language."
 msgstr ""
 
-#: forms/article.py:121
+#: forms/article.py:132
 msgid "You can't have related articles in different language."
 msgstr ""
 
-#: forms/article.py:137
+#: forms/article.py:148
 msgid "You can't have categories in different language."
 msgstr ""
 
 #: forms/category.py:90
 msgid ""
 "Some article in different language relate to this category, you can't change "
 "language until those article are not related anymore."
 msgstr ""
 
 #: forms/translated.py:34
 msgid "Available languages"
 msgstr ""
 
-#: models/article.py:33
+#: models/article.py:28
 msgid "original article"
 msgstr ""
 
-#: models/article.py:39
+#: models/article.py:34
 msgid "Mark this article as a translation of an original article."
 msgstr ""
 
-#: models/article.py:47
+#: models/article.py:42
 msgid "status"
 msgstr ""
 
-#: models/article.py:52
+#: models/article.py:47
 msgid "Publication status."
 msgstr ""
 
-#: models/article.py:60
+#: models/article.py:55
 msgid "featured"
 msgstr ""
 
-#: models/article.py:64
+#: models/article.py:59
 msgid "Mark this article as featured."
 msgstr ""
 
-#: models/article.py:72
+#: models/article.py:67
 msgid "pinned"
 msgstr ""
 
-#: models/article.py:76
+#: models/article.py:71
 msgid "A pinned article is enforced at top of order results."
 msgstr ""
 
-#: models/article.py:84
+#: models/article.py:79
 msgid "private"
 msgstr ""
 
-#: models/article.py:88
+#: models/article.py:83
 msgid "Private article is only available for authenticated users."
 msgstr ""
 
-#: models/article.py:96
+#: models/article.py:91
 msgid "publication date"
 msgstr ""
 
-#: models/article.py:100
+#: models/article.py:95
 msgid "Start date of publication."
 msgstr ""
 
-#: models/article.py:108
+#: models/article.py:103
 msgid "publication time"
 msgstr ""
 
-#: models/article.py:111
+#: models/article.py:106
 msgid "Start time of publication."
 msgstr ""
 
-#: models/article.py:119
+#: models/article.py:114
 msgid "publication end"
 msgstr ""
 
-#: models/article.py:125
+#: models/article.py:120
 msgid "End date of publication."
 msgstr ""
 
-#: models/article.py:133
+#: models/article.py:128
 msgid "last update"
 msgstr ""
 
-#: models/article.py:141 models/category.py:41
+#: models/article.py:136 models/category.py:34
 msgid "title"
 msgstr ""
 
-#: models/article.py:151 models/category.py:51
+#: models/article.py:146 models/category.py:44
 msgid "slug"
 msgstr ""
 
-#: models/article.py:154
+#: models/article.py:149
 msgid "Used to build the article URL."
 msgstr ""
 
-#: models/article.py:162
+#: models/article.py:157
 msgid "SEO title"
 msgstr ""
 
-#: models/article.py:167
+#: models/article.py:162
 msgid ""
 "This value will be used as page meta title if not blank, else the article "
 "title is used."
 msgstr ""
 
-#: models/article.py:177 models/category.py:59
+#: models/article.py:172 models/category.py:52
 msgid "lead"
 msgstr ""
 
-#: models/article.py:180 models/category.py:62
+#: models/article.py:175 models/category.py:55
 msgid "Lead paragraph, commonly used for SEO purposes in page meta tags."
 msgstr ""
 
-#: models/article.py:188
+#: models/article.py:183
 msgid "introduction"
 msgstr ""
 
-#: models/article.py:196
+#: models/article.py:191
 msgid "content"
 msgstr ""
 
-#: models/article.py:205 models/category.py:78
+#: models/article.py:200 models/category.py:71
 msgid "cover image"
 msgstr ""
 
-#: models/article.py:211
+#: models/article.py:206
 msgid "Article cover image."
 msgstr ""
 
-#: models/article.py:219
+#: models/article.py:214
 msgid "main image"
 msgstr ""
 
-#: models/article.py:225
+#: models/article.py:220
 msgid "Article large image."
 msgstr ""
 
-#: models/article.py:234
+#: models/article.py:229
 msgid "categories"
 msgstr ""
 
-#: models/article.py:244
+#: models/article.py:239
 msgid "authors"
 msgstr ""
 
-#: models/article.py:254
+#: models/article.py:249
 msgid "related articles"
 msgstr ""
 
 #: models/article.py:276
 msgid "Article"
 msgstr ""
 
-#: models/article.py:277 templates/lotus/article/list.html:4
+#: models/article.py:277 settings.py:101 templates/lotus/article/list.html:4
 #: templates/lotus/article/list.html:8 templates/lotus/author/detail.html:11
-#: templates/lotus/category/detail.html:22 views/article.py:25
+#: templates/lotus/category/detail.html:31 templates/lotus/tag/detail.html:11
 msgid "Articles"
 msgstr ""
 
-#: models/category.py:33
+#: models/category.py:26
 msgid "Mark this category as a translation of an original category."
 msgstr ""
 
-#: models/category.py:70
+#: models/category.py:63
 msgid "description"
 msgstr ""
 
-#: models/category.py:97
+#: models/category.py:91
 msgid "Category"
 msgstr ""
 
-#: models/category.py:98 templates/lotus/article/detail.html:104
-#: templates/lotus/category/list.html:4 templates/lotus/category/list.html:8
-#: views/category.py:25
+#: models/category.py:92 settings.py:103
+#: templates/lotus/article/detail.html:123 templates/lotus/category/list.html:4
+#: templates/lotus/category/list.html:8
 msgid "Categories"
 msgstr ""
 
-#: templates/admin/lotus/article/change_form.html:19
-#: templates/admin/lotus/category/change_form.html:19
+#: settings.py:102 templates/lotus/article/detail.html:158
+#: templates/lotus/author/list.html:4 templates/lotus/author/list.html:8
+msgid "Authors"
+msgstr ""
+
+#: settings.py:104 templates/lotus/article/detail.html:140
+#: templates/lotus/tag/list.html:4 templates/lotus/tag/list.html:8
+msgid "Tags"
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:20
+#: templates/admin/lotus/category/change_form.html:20
+#: templates/lotus/article/detail.html:45
+#: templates/lotus/category/detail.html:54
 msgid "Translate"
 msgstr ""
 
-#: templates/admin/lotus/article/change_form.html:28
+#: templates/admin/lotus/article/change_form.html:26
+msgid "Preview"
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:34
+#, python-format
+msgid ""
+"<strong>Article language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this article won't "
+"reachable from your site.<br><br>You may be able to edit this article but it "
+"will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:40
 msgid "Existing language(s) for this article:"
 msgstr ""
 
 #: templates/admin/lotus/article/translate_original.html:7
 #: templates/admin/lotus/category/translate_original.html:7
 msgid "Home"
 msgstr ""
@@ -315,15 +345,25 @@
 msgstr ""
 
 #: templates/admin/lotus/article/translate_original.html:31
 #: templates/admin/lotus/category/translate_original.html:31
 msgid "Confirm"
 msgstr ""
 
-#: templates/admin/lotus/category/change_form.html:28
+#: templates/admin/lotus/category/change_form.html:29
+#, python-format
+msgid ""
+"<strong>Category language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this category won't "
+"reachable from your site.<br><br>You may be able to edit this category but "
+"it will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/category/change_form.html:35
 msgid "Existing language(s) for this category:"
 msgstr ""
 
 #: templates/admin/lotus/category/translate_original.html:17
 msgid "No available languages for this category."
 msgstr ""
 
@@ -336,69 +376,98 @@
 #: templates/admin/lotus/category/translate_original.html:22
 #, python-format
 msgid ""
 "You requested to translate a translation category, this will send you to a "
 "create form to translate the original category '%(title)s' instead."
 msgstr ""
 
-#: templates/lotus/article/detail.html:31
+#: templates/lotus/article/detail.html:39
+#: templates/lotus/category/detail.html:48
 msgid "Edit"
 msgstr ""
 
-#: templates/lotus/article/detail.html:38
+#: templates/lotus/article/detail.html:53
 msgid "Cover"
 msgstr ""
 
-#: templates/lotus/article/detail.html:52
+#: templates/lotus/article/detail.html:72
 msgid "States"
 msgstr ""
 
-#: templates/lotus/article/detail.html:57 templates/lotus/article/item.html:23
+#: templates/lotus/article/detail.html:77
+#: templates/lotus/article/partials/item.html:28
 msgid "Featured"
 msgstr ""
 
-#: templates/lotus/article/detail.html:62 templates/lotus/article/item.html:26
+#: templates/lotus/article/detail.html:82
+#: templates/lotus/article/partials/item.html:31
 msgid "Pinned"
 msgstr ""
 
-#: templates/lotus/article/detail.html:67 templates/lotus/article/item.html:29
+#: templates/lotus/article/detail.html:87
+#: templates/lotus/article/partials/item.html:34
 msgid "Draft"
 msgstr ""
 
-#: templates/lotus/article/detail.html:72 templates/lotus/article/item.html:32
+#: templates/lotus/article/detail.html:92
+#: templates/lotus/article/partials/item.html:37
 msgid "Private"
 msgstr ""
 
-#: templates/lotus/article/detail.html:77 templates/lotus/article/item.html:35
+#: templates/lotus/article/detail.html:97
+#: templates/lotus/article/partials/item.html:40
 msgid "Scheduled publication"
 msgstr ""
 
-#: templates/lotus/article/detail.html:82 templates/lotus/article/item.html:38
+#: templates/lotus/article/detail.html:102
+#: templates/lotus/article/partials/item.html:43
 msgid "Ended publication"
 msgstr ""
 
-#: templates/lotus/article/detail.html:94
+#: templates/lotus/article/detail.html:113
+#: templates/lotus/category/detail.html:63
 msgid "Available in languages"
 msgstr ""
 
-#: templates/lotus/article/detail.html:121 templates/lotus/author/list.html:4
-#: templates/lotus/author/list.html:8 views/author.py:24
-msgid "Authors"
+#: templates/lotus/article/detail.html:173
+msgid "Related articles"
 msgstr ""
 
-#: templates/lotus/article/detail.html:136
-msgid "Related articles"
+#: templates/lotus/article/partials/siblings.html:9
+msgid "Published"
 msgstr ""
 
-#: templates/lotus/pagination.html:4
+#: templates/lotus/article/partials/siblings.html:11
+msgid "Not published"
+msgstr ""
+
+#: templates/lotus/article/partials/siblings.html:16
+#: templates/lotus/category/partials/siblings.html:9
+msgid "Is original"
+msgstr ""
+
+#: templates/lotus/article/partials/siblings.html:18
+#: templates/lotus/category/partials/siblings.html:11
+msgid "Is not original"
+msgstr ""
+
+#: templates/lotus/pagination.html:3
 msgid "Pagination"
 msgstr ""
 
+#: templates/lotus/preview_switch.html:6
+msgid "Disable preview"
+msgstr ""
+
+#: templates/lotus/preview_switch.html:8
+msgid "Enable preview"
+msgstr ""
+
 #: views/admin/mixins.py:98
 #, python-format
 msgid "Translate '%(title)s'"
 msgstr ""
 
-#: views/article.py:104
+#: views/article.py:110
 #, python-format
 msgid "No %(verbose_name)s found matching the query"
 msgstr ""
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/locale/django.pot` & `django-blog-lotus-0.6.0/lotus/locale/en/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,294 +4,325 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-01-03 01:24+0100\n"
+"POT-Creation-Date: 2023-06-12 02:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin/article.py:64 admin/category.py:51
+#: admin/article.py:73 admin/category.py:54
 msgid "Language"
 msgstr ""
 
-#: admin/article.py:71
+#: admin/article.py:80
 msgid "Parameters"
 msgstr ""
 
-#: admin/article.py:79
+#: admin/article.py:88
 msgid "Dates"
 msgstr ""
 
-#: admin/article.py:87 admin/category.py:58
+#: admin/article.py:96 admin/category.py:61
 msgid "Content"
 msgstr ""
 
-#: admin/article.py:97 admin/category.py:66
+#: admin/article.py:106 admin/category.py:69
 msgid "SEO"
 msgstr ""
 
-#: admin/article.py:105
+#: admin/article.py:114
 msgid "Relations"
 msgstr ""
 
-#: admin/article.py:120 admin/category.py:76 admin/translated.py:16
-#: admin/translated.py:58 models/translated.py:18
+#: admin/article.py:132 admin/category.py:81 admin_filters.py:11
+#: models/translated.py:12
 msgid "language"
 msgstr ""
 
-#: admin/article.py:128
+#: admin/article.py:140
 msgid "publish date"
 msgstr ""
 
-#: admin/article.py:142
+#: admin/article.py:148
 msgid "published"
 msgstr ""
 
-#: admin/article.py:150 admin/category.py:84
+#: admin/article.py:156 admin/category.py:89
 msgid "original"
 msgstr ""
 
-#: admin/category.py:89
+#: admin/category.py:94
 msgid "articles"
 msgstr ""
 
-#: admin/translated.py:27
-msgid "Default language"
+#: admin_filters.py:34
+msgid "translation state"
 msgstr ""
 
-#: admin/translated.py:38
-msgid "All"
+#: admin_filters.py:41
+msgid "Is an original"
 msgstr ""
 
-#: admin/translated.py:81
-msgid "translation state"
+#: admin_filters.py:42
+msgid "Is a translation"
 msgstr ""
 
-#: admin/translated.py:88
-msgid "Is an original"
+#: admin_filters.py:57
+msgid "publication state"
 msgstr ""
 
-#: admin/translated.py:89
-msgid "Is a translation"
+#: admin_filters.py:67
+msgid "Is published"
+msgstr ""
+
+#: admin_filters.py:68
+msgid "Is not published"
 msgstr ""
 
 #: apps.py:7
 msgid "Lotus weblog"
 msgstr ""
 
-#: choices.py:15
+#: choices.py:16
 msgid "draft"
 msgstr ""
 
-#: choices.py:16
+#: choices.py:17
 msgid "available"
 msgstr ""
 
-#: forms/article.py:95 forms/category.py:66
+#: forms/article.py:106 forms/category.py:66
 msgid "You can't have a language identical to the original relation."
 msgstr ""
 
-#: forms/article.py:105 forms/category.py:76
+#: forms/article.py:116 forms/category.py:76
 msgid "You can't have an original relation in the same language."
 msgstr ""
 
-#: forms/article.py:121
+#: forms/article.py:132
 msgid "You can't have related articles in different language."
 msgstr ""
 
-#: forms/article.py:137
+#: forms/article.py:148
 msgid "You can't have categories in different language."
 msgstr ""
 
 #: forms/category.py:90
 msgid ""
 "Some article in different language relate to this category, you can't change "
 "language until those article are not related anymore."
 msgstr ""
 
 #: forms/translated.py:34
 msgid "Available languages"
 msgstr ""
 
-#: models/article.py:33
+#: models/article.py:28
 msgid "original article"
 msgstr ""
 
-#: models/article.py:39
+#: models/article.py:34
 msgid "Mark this article as a translation of an original article."
 msgstr ""
 
-#: models/article.py:47
+#: models/article.py:42
 msgid "status"
 msgstr ""
 
-#: models/article.py:52
+#: models/article.py:47
 msgid "Publication status."
 msgstr ""
 
-#: models/article.py:60
+#: models/article.py:55
 msgid "featured"
 msgstr ""
 
-#: models/article.py:64
+#: models/article.py:59
 msgid "Mark this article as featured."
 msgstr ""
 
-#: models/article.py:72
+#: models/article.py:67
 msgid "pinned"
 msgstr ""
 
-#: models/article.py:76
+#: models/article.py:71
 msgid "A pinned article is enforced at top of order results."
 msgstr ""
 
-#: models/article.py:84
+#: models/article.py:79
 msgid "private"
 msgstr ""
 
-#: models/article.py:88
+#: models/article.py:83
 msgid "Private article is only available for authenticated users."
 msgstr ""
 
-#: models/article.py:96
+#: models/article.py:91
 msgid "publication date"
 msgstr ""
 
-#: models/article.py:100
+#: models/article.py:95
 msgid "Start date of publication."
 msgstr ""
 
-#: models/article.py:108
+#: models/article.py:103
 msgid "publication time"
 msgstr ""
 
-#: models/article.py:111
+#: models/article.py:106
 msgid "Start time of publication."
 msgstr ""
 
-#: models/article.py:119
+#: models/article.py:114
 msgid "publication end"
 msgstr ""
 
-#: models/article.py:125
+#: models/article.py:120
 msgid "End date of publication."
 msgstr ""
 
-#: models/article.py:133
+#: models/article.py:128
 msgid "last update"
 msgstr ""
 
-#: models/article.py:141 models/category.py:41
+#: models/article.py:136 models/category.py:34
 msgid "title"
 msgstr ""
 
-#: models/article.py:151 models/category.py:51
+#: models/article.py:146 models/category.py:44
 msgid "slug"
 msgstr ""
 
-#: models/article.py:154
+#: models/article.py:149
 msgid "Used to build the article URL."
 msgstr ""
 
-#: models/article.py:162
+#: models/article.py:157
 msgid "SEO title"
 msgstr ""
 
-#: models/article.py:167
+#: models/article.py:162
 msgid ""
 "This value will be used as page meta title if not blank, else the article "
 "title is used."
 msgstr ""
 
-#: models/article.py:177 models/category.py:59
+#: models/article.py:172 models/category.py:52
 msgid "lead"
 msgstr ""
 
-#: models/article.py:180 models/category.py:62
+#: models/article.py:175 models/category.py:55
 msgid "Lead paragraph, commonly used for SEO purposes in page meta tags."
 msgstr ""
 
-#: models/article.py:188
+#: models/article.py:183
 msgid "introduction"
 msgstr ""
 
-#: models/article.py:196
+#: models/article.py:191
 msgid "content"
 msgstr ""
 
-#: models/article.py:205 models/category.py:78
+#: models/article.py:200 models/category.py:71
 msgid "cover image"
 msgstr ""
 
-#: models/article.py:211
+#: models/article.py:206
 msgid "Article cover image."
 msgstr ""
 
-#: models/article.py:219
+#: models/article.py:214
 msgid "main image"
 msgstr ""
 
-#: models/article.py:225
+#: models/article.py:220
 msgid "Article large image."
 msgstr ""
 
-#: models/article.py:234
+#: models/article.py:229
 msgid "categories"
 msgstr ""
 
-#: models/article.py:244
+#: models/article.py:239
 msgid "authors"
 msgstr ""
 
-#: models/article.py:254
+#: models/article.py:249
 msgid "related articles"
 msgstr ""
 
 #: models/article.py:276
 msgid "Article"
 msgstr ""
 
-#: models/article.py:277 templates/lotus/article/list.html:4
+#: models/article.py:277 settings.py:101 templates/lotus/article/list.html:4
 #: templates/lotus/article/list.html:8 templates/lotus/author/detail.html:11
-#: templates/lotus/category/detail.html:22 views/article.py:25
+#: templates/lotus/category/detail.html:31 templates/lotus/tag/detail.html:11
 msgid "Articles"
 msgstr ""
 
-#: models/category.py:33
+#: models/category.py:26
 msgid "Mark this category as a translation of an original category."
 msgstr ""
 
-#: models/category.py:70
+#: models/category.py:63
 msgid "description"
 msgstr ""
 
-#: models/category.py:97
+#: models/category.py:91
 msgid "Category"
 msgstr ""
 
-#: models/category.py:98 templates/lotus/article/detail.html:104
-#: templates/lotus/category/list.html:4 templates/lotus/category/list.html:8
-#: views/category.py:25
+#: models/category.py:92 settings.py:103
+#: templates/lotus/article/detail.html:123 templates/lotus/category/list.html:4
+#: templates/lotus/category/list.html:8
 msgid "Categories"
 msgstr ""
 
-#: templates/admin/lotus/article/change_form.html:19
-#: templates/admin/lotus/category/change_form.html:19
+#: settings.py:102 templates/lotus/article/detail.html:158
+#: templates/lotus/author/list.html:4 templates/lotus/author/list.html:8
+msgid "Authors"
+msgstr ""
+
+#: settings.py:104 templates/lotus/article/detail.html:140
+#: templates/lotus/tag/list.html:4 templates/lotus/tag/list.html:8
+msgid "Tags"
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:20
+#: templates/admin/lotus/category/change_form.html:20
+#: templates/lotus/article/detail.html:45
+#: templates/lotus/category/detail.html:54
 msgid "Translate"
 msgstr ""
 
-#: templates/admin/lotus/article/change_form.html:28
+#: templates/admin/lotus/article/change_form.html:26
+msgid "Preview"
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:34
+#, python-format
+msgid ""
+"<strong>Article language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this article won't "
+"reachable from your site.<br><br>You may be able to edit this article but it "
+"will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:40
 msgid "Existing language(s) for this article:"
 msgstr ""
 
 #: templates/admin/lotus/article/translate_original.html:7
 #: templates/admin/lotus/category/translate_original.html:7
 msgid "Home"
 msgstr ""
@@ -314,15 +345,25 @@
 msgstr ""
 
 #: templates/admin/lotus/article/translate_original.html:31
 #: templates/admin/lotus/category/translate_original.html:31
 msgid "Confirm"
 msgstr ""
 
-#: templates/admin/lotus/category/change_form.html:28
+#: templates/admin/lotus/category/change_form.html:29
+#, python-format
+msgid ""
+"<strong>Category language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this category won't "
+"reachable from your site.<br><br>You may be able to edit this category but "
+"it will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/category/change_form.html:35
 msgid "Existing language(s) for this category:"
 msgstr ""
 
 #: templates/admin/lotus/category/translate_original.html:17
 msgid "No available languages for this category."
 msgstr ""
 
@@ -335,69 +376,98 @@
 #: templates/admin/lotus/category/translate_original.html:22
 #, python-format
 msgid ""
 "You requested to translate a translation category, this will send you to a "
 "create form to translate the original category '%(title)s' instead."
 msgstr ""
 
-#: templates/lotus/article/detail.html:31
+#: templates/lotus/article/detail.html:39
+#: templates/lotus/category/detail.html:48
 msgid "Edit"
 msgstr ""
 
-#: templates/lotus/article/detail.html:38
+#: templates/lotus/article/detail.html:53
 msgid "Cover"
 msgstr ""
 
-#: templates/lotus/article/detail.html:52
+#: templates/lotus/article/detail.html:72
 msgid "States"
 msgstr ""
 
-#: templates/lotus/article/detail.html:57 templates/lotus/article/item.html:23
+#: templates/lotus/article/detail.html:77
+#: templates/lotus/article/partials/item.html:28
 msgid "Featured"
 msgstr ""
 
-#: templates/lotus/article/detail.html:62 templates/lotus/article/item.html:26
+#: templates/lotus/article/detail.html:82
+#: templates/lotus/article/partials/item.html:31
 msgid "Pinned"
 msgstr ""
 
-#: templates/lotus/article/detail.html:67 templates/lotus/article/item.html:29
+#: templates/lotus/article/detail.html:87
+#: templates/lotus/article/partials/item.html:34
 msgid "Draft"
 msgstr ""
 
-#: templates/lotus/article/detail.html:72 templates/lotus/article/item.html:32
+#: templates/lotus/article/detail.html:92
+#: templates/lotus/article/partials/item.html:37
 msgid "Private"
 msgstr ""
 
-#: templates/lotus/article/detail.html:77 templates/lotus/article/item.html:35
+#: templates/lotus/article/detail.html:97
+#: templates/lotus/article/partials/item.html:40
 msgid "Scheduled publication"
 msgstr ""
 
-#: templates/lotus/article/detail.html:82 templates/lotus/article/item.html:38
+#: templates/lotus/article/detail.html:102
+#: templates/lotus/article/partials/item.html:43
 msgid "Ended publication"
 msgstr ""
 
-#: templates/lotus/article/detail.html:94
+#: templates/lotus/article/detail.html:113
+#: templates/lotus/category/detail.html:63
 msgid "Available in languages"
 msgstr ""
 
-#: templates/lotus/article/detail.html:121 templates/lotus/author/list.html:4
-#: templates/lotus/author/list.html:8 views/author.py:24
-msgid "Authors"
+#: templates/lotus/article/detail.html:173
+msgid "Related articles"
 msgstr ""
 
-#: templates/lotus/article/detail.html:136
-msgid "Related articles"
+#: templates/lotus/article/partials/siblings.html:9
+msgid "Published"
 msgstr ""
 
-#: templates/lotus/pagination.html:4
+#: templates/lotus/article/partials/siblings.html:11
+msgid "Not published"
+msgstr ""
+
+#: templates/lotus/article/partials/siblings.html:16
+#: templates/lotus/category/partials/siblings.html:9
+msgid "Is original"
+msgstr ""
+
+#: templates/lotus/article/partials/siblings.html:18
+#: templates/lotus/category/partials/siblings.html:11
+msgid "Is not original"
+msgstr ""
+
+#: templates/lotus/pagination.html:3
 msgid "Pagination"
 msgstr ""
 
+#: templates/lotus/preview_switch.html:6
+msgid "Disable preview"
+msgstr ""
+
+#: templates/lotus/preview_switch.html:8
+msgid "Enable preview"
+msgstr ""
+
 #: views/admin/mixins.py:98
 #, python-format
 msgid "Translate '%(title)s'"
 msgstr ""
 
-#: views/article.py:104
+#: views/article.py:110
 #, python-format
 msgid "No %(verbose_name)s found matching the query"
 msgstr ""
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/locale/en/LC_MESSAGES/django.po` & `django-blog-lotus-0.6.0/lotus/locale/django.pot`

 * *Files 13% similar despite different names*

```diff
@@ -4,295 +4,324 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-01-03 01:24+0100\n"
+"POT-Creation-Date: 2023-06-12 02:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin/article.py:64 admin/category.py:51
+#: admin/article.py:73 admin/category.py:54
 msgid "Language"
 msgstr ""
 
-#: admin/article.py:71
+#: admin/article.py:80
 msgid "Parameters"
 msgstr ""
 
-#: admin/article.py:79
+#: admin/article.py:88
 msgid "Dates"
 msgstr ""
 
-#: admin/article.py:87 admin/category.py:58
+#: admin/article.py:96 admin/category.py:61
 msgid "Content"
 msgstr ""
 
-#: admin/article.py:97 admin/category.py:66
+#: admin/article.py:106 admin/category.py:69
 msgid "SEO"
 msgstr ""
 
-#: admin/article.py:105
+#: admin/article.py:114
 msgid "Relations"
 msgstr ""
 
-#: admin/article.py:120 admin/category.py:76 admin/translated.py:16
-#: admin/translated.py:58 models/translated.py:18
+#: admin/article.py:132 admin/category.py:81 admin_filters.py:11
+#: models/translated.py:12
 msgid "language"
 msgstr ""
 
-#: admin/article.py:128
+#: admin/article.py:140
 msgid "publish date"
 msgstr ""
 
-#: admin/article.py:142
+#: admin/article.py:148
 msgid "published"
 msgstr ""
 
-#: admin/article.py:150 admin/category.py:84
+#: admin/article.py:156 admin/category.py:89
 msgid "original"
 msgstr ""
 
-#: admin/category.py:89
+#: admin/category.py:94
 msgid "articles"
 msgstr ""
 
-#: admin/translated.py:27
-msgid "Default language"
+#: admin_filters.py:34
+msgid "translation state"
 msgstr ""
 
-#: admin/translated.py:38
-msgid "All"
+#: admin_filters.py:41
+msgid "Is an original"
 msgstr ""
 
-#: admin/translated.py:81
-msgid "translation state"
+#: admin_filters.py:42
+msgid "Is a translation"
 msgstr ""
 
-#: admin/translated.py:88
-msgid "Is an original"
+#: admin_filters.py:57
+msgid "publication state"
 msgstr ""
 
-#: admin/translated.py:89
-msgid "Is a translation"
+#: admin_filters.py:67
+msgid "Is published"
+msgstr ""
+
+#: admin_filters.py:68
+msgid "Is not published"
 msgstr ""
 
 #: apps.py:7
 msgid "Lotus weblog"
 msgstr ""
 
-#: choices.py:15
+#: choices.py:16
 msgid "draft"
 msgstr ""
 
-#: choices.py:16
+#: choices.py:17
 msgid "available"
 msgstr ""
 
-#: forms/article.py:95 forms/category.py:66
+#: forms/article.py:106 forms/category.py:66
 msgid "You can't have a language identical to the original relation."
 msgstr ""
 
-#: forms/article.py:105 forms/category.py:76
+#: forms/article.py:116 forms/category.py:76
 msgid "You can't have an original relation in the same language."
 msgstr ""
 
-#: forms/article.py:121
+#: forms/article.py:132
 msgid "You can't have related articles in different language."
 msgstr ""
 
-#: forms/article.py:137
+#: forms/article.py:148
 msgid "You can't have categories in different language."
 msgstr ""
 
 #: forms/category.py:90
 msgid ""
 "Some article in different language relate to this category, you can't change "
 "language until those article are not related anymore."
 msgstr ""
 
 #: forms/translated.py:34
 msgid "Available languages"
 msgstr ""
 
-#: models/article.py:33
+#: models/article.py:28
 msgid "original article"
 msgstr ""
 
-#: models/article.py:39
+#: models/article.py:34
 msgid "Mark this article as a translation of an original article."
 msgstr ""
 
-#: models/article.py:47
+#: models/article.py:42
 msgid "status"
 msgstr ""
 
-#: models/article.py:52
+#: models/article.py:47
 msgid "Publication status."
 msgstr ""
 
-#: models/article.py:60
+#: models/article.py:55
 msgid "featured"
 msgstr ""
 
-#: models/article.py:64
+#: models/article.py:59
 msgid "Mark this article as featured."
 msgstr ""
 
-#: models/article.py:72
+#: models/article.py:67
 msgid "pinned"
 msgstr ""
 
-#: models/article.py:76
+#: models/article.py:71
 msgid "A pinned article is enforced at top of order results."
 msgstr ""
 
-#: models/article.py:84
+#: models/article.py:79
 msgid "private"
 msgstr ""
 
-#: models/article.py:88
+#: models/article.py:83
 msgid "Private article is only available for authenticated users."
 msgstr ""
 
-#: models/article.py:96
+#: models/article.py:91
 msgid "publication date"
 msgstr ""
 
-#: models/article.py:100
+#: models/article.py:95
 msgid "Start date of publication."
 msgstr ""
 
-#: models/article.py:108
+#: models/article.py:103
 msgid "publication time"
 msgstr ""
 
-#: models/article.py:111
+#: models/article.py:106
 msgid "Start time of publication."
 msgstr ""
 
-#: models/article.py:119
+#: models/article.py:114
 msgid "publication end"
 msgstr ""
 
-#: models/article.py:125
+#: models/article.py:120
 msgid "End date of publication."
 msgstr ""
 
-#: models/article.py:133
+#: models/article.py:128
 msgid "last update"
 msgstr ""
 
-#: models/article.py:141 models/category.py:41
+#: models/article.py:136 models/category.py:34
 msgid "title"
 msgstr ""
 
-#: models/article.py:151 models/category.py:51
+#: models/article.py:146 models/category.py:44
 msgid "slug"
 msgstr ""
 
-#: models/article.py:154
+#: models/article.py:149
 msgid "Used to build the article URL."
 msgstr ""
 
-#: models/article.py:162
+#: models/article.py:157
 msgid "SEO title"
 msgstr ""
 
-#: models/article.py:167
+#: models/article.py:162
 msgid ""
 "This value will be used as page meta title if not blank, else the article "
 "title is used."
 msgstr ""
 
-#: models/article.py:177 models/category.py:59
+#: models/article.py:172 models/category.py:52
 msgid "lead"
 msgstr ""
 
-#: models/article.py:180 models/category.py:62
+#: models/article.py:175 models/category.py:55
 msgid "Lead paragraph, commonly used for SEO purposes in page meta tags."
 msgstr ""
 
-#: models/article.py:188
+#: models/article.py:183
 msgid "introduction"
 msgstr ""
 
-#: models/article.py:196
+#: models/article.py:191
 msgid "content"
 msgstr ""
 
-#: models/article.py:205 models/category.py:78
+#: models/article.py:200 models/category.py:71
 msgid "cover image"
 msgstr ""
 
-#: models/article.py:211
+#: models/article.py:206
 msgid "Article cover image."
 msgstr ""
 
-#: models/article.py:219
+#: models/article.py:214
 msgid "main image"
 msgstr ""
 
-#: models/article.py:225
+#: models/article.py:220
 msgid "Article large image."
 msgstr ""
 
-#: models/article.py:234
+#: models/article.py:229
 msgid "categories"
 msgstr ""
 
-#: models/article.py:244
+#: models/article.py:239
 msgid "authors"
 msgstr ""
 
-#: models/article.py:254
+#: models/article.py:249
 msgid "related articles"
 msgstr ""
 
 #: models/article.py:276
 msgid "Article"
 msgstr ""
 
-#: models/article.py:277 templates/lotus/article/list.html:4
+#: models/article.py:277 settings.py:101 templates/lotus/article/list.html:4
 #: templates/lotus/article/list.html:8 templates/lotus/author/detail.html:11
-#: templates/lotus/category/detail.html:22 views/article.py:25
+#: templates/lotus/category/detail.html:31 templates/lotus/tag/detail.html:11
 msgid "Articles"
 msgstr ""
 
-#: models/category.py:33
+#: models/category.py:26
 msgid "Mark this category as a translation of an original category."
 msgstr ""
 
-#: models/category.py:70
+#: models/category.py:63
 msgid "description"
 msgstr ""
 
-#: models/category.py:97
+#: models/category.py:91
 msgid "Category"
 msgstr ""
 
-#: models/category.py:98 templates/lotus/article/detail.html:104
-#: templates/lotus/category/list.html:4 templates/lotus/category/list.html:8
-#: views/category.py:25
+#: models/category.py:92 settings.py:103
+#: templates/lotus/article/detail.html:123 templates/lotus/category/list.html:4
+#: templates/lotus/category/list.html:8
 msgid "Categories"
 msgstr ""
 
-#: templates/admin/lotus/article/change_form.html:19
-#: templates/admin/lotus/category/change_form.html:19
+#: settings.py:102 templates/lotus/article/detail.html:158
+#: templates/lotus/author/list.html:4 templates/lotus/author/list.html:8
+msgid "Authors"
+msgstr ""
+
+#: settings.py:104 templates/lotus/article/detail.html:140
+#: templates/lotus/tag/list.html:4 templates/lotus/tag/list.html:8
+msgid "Tags"
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:20
+#: templates/admin/lotus/category/change_form.html:20
+#: templates/lotus/article/detail.html:45
+#: templates/lotus/category/detail.html:54
 msgid "Translate"
 msgstr ""
 
-#: templates/admin/lotus/article/change_form.html:28
+#: templates/admin/lotus/article/change_form.html:26
+msgid "Preview"
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:34
+#, python-format
+msgid ""
+"<strong>Article language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this article won't "
+"reachable from your site.<br><br>You may be able to edit this article but it "
+"will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:40
 msgid "Existing language(s) for this article:"
 msgstr ""
 
 #: templates/admin/lotus/article/translate_original.html:7
 #: templates/admin/lotus/category/translate_original.html:7
 msgid "Home"
 msgstr ""
@@ -315,15 +344,25 @@
 msgstr ""
 
 #: templates/admin/lotus/article/translate_original.html:31
 #: templates/admin/lotus/category/translate_original.html:31
 msgid "Confirm"
 msgstr ""
 
-#: templates/admin/lotus/category/change_form.html:28
+#: templates/admin/lotus/category/change_form.html:29
+#, python-format
+msgid ""
+"<strong>Category language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this category won't "
+"reachable from your site.<br><br>You may be able to edit this category but "
+"it will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/category/change_form.html:35
 msgid "Existing language(s) for this category:"
 msgstr ""
 
 #: templates/admin/lotus/category/translate_original.html:17
 msgid "No available languages for this category."
 msgstr ""
 
@@ -336,69 +375,98 @@
 #: templates/admin/lotus/category/translate_original.html:22
 #, python-format
 msgid ""
 "You requested to translate a translation category, this will send you to a "
 "create form to translate the original category '%(title)s' instead."
 msgstr ""
 
-#: templates/lotus/article/detail.html:31
+#: templates/lotus/article/detail.html:39
+#: templates/lotus/category/detail.html:48
 msgid "Edit"
 msgstr ""
 
-#: templates/lotus/article/detail.html:38
+#: templates/lotus/article/detail.html:53
 msgid "Cover"
 msgstr ""
 
-#: templates/lotus/article/detail.html:52
+#: templates/lotus/article/detail.html:72
 msgid "States"
 msgstr ""
 
-#: templates/lotus/article/detail.html:57 templates/lotus/article/item.html:23
+#: templates/lotus/article/detail.html:77
+#: templates/lotus/article/partials/item.html:28
 msgid "Featured"
 msgstr ""
 
-#: templates/lotus/article/detail.html:62 templates/lotus/article/item.html:26
+#: templates/lotus/article/detail.html:82
+#: templates/lotus/article/partials/item.html:31
 msgid "Pinned"
 msgstr ""
 
-#: templates/lotus/article/detail.html:67 templates/lotus/article/item.html:29
+#: templates/lotus/article/detail.html:87
+#: templates/lotus/article/partials/item.html:34
 msgid "Draft"
 msgstr ""
 
-#: templates/lotus/article/detail.html:72 templates/lotus/article/item.html:32
+#: templates/lotus/article/detail.html:92
+#: templates/lotus/article/partials/item.html:37
 msgid "Private"
 msgstr ""
 
-#: templates/lotus/article/detail.html:77 templates/lotus/article/item.html:35
+#: templates/lotus/article/detail.html:97
+#: templates/lotus/article/partials/item.html:40
 msgid "Scheduled publication"
 msgstr ""
 
-#: templates/lotus/article/detail.html:82 templates/lotus/article/item.html:38
+#: templates/lotus/article/detail.html:102
+#: templates/lotus/article/partials/item.html:43
 msgid "Ended publication"
 msgstr ""
 
-#: templates/lotus/article/detail.html:94
+#: templates/lotus/article/detail.html:113
+#: templates/lotus/category/detail.html:63
 msgid "Available in languages"
 msgstr ""
 
-#: templates/lotus/article/detail.html:121 templates/lotus/author/list.html:4
-#: templates/lotus/author/list.html:8 views/author.py:24
-msgid "Authors"
+#: templates/lotus/article/detail.html:173
+msgid "Related articles"
 msgstr ""
 
-#: templates/lotus/article/detail.html:136
-msgid "Related articles"
+#: templates/lotus/article/partials/siblings.html:9
+msgid "Published"
 msgstr ""
 
-#: templates/lotus/pagination.html:4
+#: templates/lotus/article/partials/siblings.html:11
+msgid "Not published"
+msgstr ""
+
+#: templates/lotus/article/partials/siblings.html:16
+#: templates/lotus/category/partials/siblings.html:9
+msgid "Is original"
+msgstr ""
+
+#: templates/lotus/article/partials/siblings.html:18
+#: templates/lotus/category/partials/siblings.html:11
+msgid "Is not original"
+msgstr ""
+
+#: templates/lotus/pagination.html:3
 msgid "Pagination"
 msgstr ""
 
+#: templates/lotus/preview_switch.html:6
+msgid "Disable preview"
+msgstr ""
+
+#: templates/lotus/preview_switch.html:8
+msgid "Enable preview"
+msgstr ""
+
 #: views/admin/mixins.py:98
 #, python-format
 msgid "Translate '%(title)s'"
 msgstr ""
 
-#: views/article.py:104
+#: views/article.py:110
 #, python-format
 msgid "No %(verbose_name)s found matching the query"
 msgstr ""
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.mo` & `django-blog-lotus-0.6.0/lotus/locale/fr/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,17 +10,14 @@
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "A pinned article is enforced at top of order results."
 msgstr "Un article épinglé est forcé vers le haut des résultats."
 
-msgid "All"
-msgstr "Tout"
-
 msgid "Article"
 msgstr "Article"
 
 msgid "Article cover image."
 msgstr "L'image de couverture de l'article."
 
 msgid "Article large image."
@@ -52,17 +49,14 @@
 
 msgid "Cover"
 msgstr "Couverture"
 
 msgid "Dates"
 msgstr "Dates"
 
-msgid "Default language"
-msgstr "Langue par défaut"
-
 msgid "Draft"
 msgstr "Brouillon"
 
 msgid "Edit"
 msgstr "Éditer"
 
 msgid "End date of publication."
@@ -76,20 +70,35 @@
 
 msgid "Existing language(s) for this category:"
 msgstr "Langue(s) existante(s) pour cette catégorie:"
 
 msgid "Featured"
 msgstr "En une"
 
+msgid "Home"
+msgstr "Accueil"
+
 msgid "Is a translation"
 msgstr "Est une traduction"
 
 msgid "Is an original"
 msgstr "Est un original"
 
+msgid "Is not original"
+msgstr "N'est pas un original"
+
+msgid "Is not published"
+msgstr "Non publié"
+
+msgid "Is original"
+msgstr "Est un original"
+
+msgid "Is published"
+msgstr "Publié"
+
 msgid "Language"
 msgstr "Langue"
 
 msgid "Lead paragraph, commonly used for SEO purposes in page meta tags."
 msgstr ""
 "Un paragraphe d'accroche, couramment utilisé à des fins de SEO dans les "
 "métas informations de la page."
@@ -100,39 +109,51 @@
 msgid "Mark this article as featured."
 msgstr "Marquez cet article comme en une."
 
 msgid "Mark this category as a translation of an original category."
 msgstr ""
 "Marquez cette catégorie comme une traduction d'une catégorie originale."
 
+msgid "No %(verbose_name)s found matching the query"
+msgstr "Pas de %(verbose_name)s trouvés pour la requête"
+
 msgid "No available languages for this article."
 msgstr "Aucune langue disponible pour cet article."
 
 msgid "No available languages for this category."
 msgstr "Aucune langue disponible pour cette catégorie."
 
+msgid "Not published"
+msgstr "Non publié"
+
 msgid "Pagination"
 msgstr "Pagination"
 
 msgid "Parameters"
 msgstr "Paramètres"
 
 msgid "Pinned"
 msgstr "Épinglé"
 
+msgid "Preview"
+msgstr "Aperçu"
+
 msgid "Private"
 msgstr "Privé"
 
 msgid "Private article is only available for authenticated users."
 msgstr ""
 "Un articlé privé est seulement disponible aux utilisateurs authentifiés."
 
 msgid "Publication status."
 msgstr "État de publication."
 
+msgid "Published"
+msgstr "Publié"
+
 msgid "Related articles"
 msgstr "Articles reliés"
 
 msgid "Relations"
 msgstr "Relations"
 
 msgid "SEO"
@@ -156,14 +177,17 @@
 
 msgid "Start time of publication."
 msgstr "Heure de début de publication."
 
 msgid "States"
 msgstr "États"
 
+msgid "Tags"
+msgstr "Étiquettes"
+
 msgid ""
 "This value will be used as page meta title if not blank, else the article "
 "title is used."
 msgstr ""
 "Cette valeur sera utilisé comme le titre de méta information de la page s'il "
 "n'est pas vide, sinon le titre de l'article est utilisé."
 
@@ -274,14 +298,17 @@
 
 msgid "publication date"
 msgstr "date de publication"
 
 msgid "publication end"
 msgstr "fin de la publication"
 
+msgid "publication state"
+msgstr "état de publication"
+
 msgid "publication time"
 msgstr "heure de publication"
 
 msgid "publish date"
 msgstr "date de publication"
 
 msgid "published"
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/locale/fr/LC_MESSAGES/django.po` & `django-blog-lotus-0.6.0/lotus/locale/fr/LC_MESSAGES/django.po`

 * *Files 11% similar despite different names*

```diff
@@ -4,114 +4,118 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-01-03 01:24+0100\n"
+"POT-Creation-Date: 2023-06-12 02:35+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: admin/article.py:64 admin/category.py:51
+#: admin/article.py:73 admin/category.py:54
 msgid "Language"
 msgstr "Langue"
 
-#: admin/article.py:71
+#: admin/article.py:80
 msgid "Parameters"
 msgstr "Paramètres"
 
-#: admin/article.py:79
+#: admin/article.py:88
 msgid "Dates"
 msgstr "Dates"
 
-#: admin/article.py:87 admin/category.py:58
+#: admin/article.py:96 admin/category.py:61
 msgid "Content"
 msgstr "Contenu"
 
-#: admin/article.py:97 admin/category.py:66
+#: admin/article.py:106 admin/category.py:69
 msgid "SEO"
 msgstr "SEO"
 
-#: admin/article.py:105
+#: admin/article.py:114
 msgid "Relations"
 msgstr "Relations"
 
-#: admin/article.py:120 admin/category.py:76 admin/translated.py:16
-#: admin/translated.py:58 models/translated.py:18
+#: admin/article.py:132 admin/category.py:81 admin_filters.py:11
+#: models/translated.py:12
 msgid "language"
 msgstr "langue"
 
-#: admin/article.py:128
+#: admin/article.py:140
 msgid "publish date"
 msgstr "date de publication"
 
-#: admin/article.py:142
+#: admin/article.py:148
 msgid "published"
 msgstr "publié"
 
-#: admin/article.py:150 admin/category.py:84
+#: admin/article.py:156 admin/category.py:89
 msgid "original"
 msgstr "original"
 
-#: admin/category.py:89
+#: admin/category.py:94
 msgid "articles"
 msgstr "articles"
 
-#: admin/translated.py:27
-msgid "Default language"
-msgstr "Langue par défaut"
-
-#: admin/translated.py:38
-msgid "All"
-msgstr "Tout"
-
-#: admin/translated.py:81
+#: admin_filters.py:34
 msgid "translation state"
 msgstr "état de traduction"
 
-#: admin/translated.py:88
+#: admin_filters.py:41
 msgid "Is an original"
 msgstr "Est un original"
 
-#: admin/translated.py:89
+#: admin_filters.py:42
 msgid "Is a translation"
 msgstr "Est une traduction"
 
+#: admin_filters.py:57
+msgid "publication state"
+msgstr "état de publication"
+
+#: admin_filters.py:67
+msgid "Is published"
+msgstr "Publié"
+
+#: admin_filters.py:68
+msgid "Is not published"
+msgstr "Non publié"
+
 #: apps.py:7
 msgid "Lotus weblog"
 msgstr ""
 
-#: choices.py:15
+#: choices.py:16
 msgid "draft"
 msgstr "brouillon"
 
-#: choices.py:16
+#: choices.py:17
 msgid "available"
 msgstr "disponible"
 
-#: forms/article.py:95 forms/category.py:66
+#: forms/article.py:106 forms/category.py:66
 msgid "You can't have a language identical to the original relation."
 msgstr "Vous ne pouvez avoir une langue identique à celle de l'original."
 
-#: forms/article.py:105 forms/category.py:76
+#: forms/article.py:116 forms/category.py:76
 msgid "You can't have an original relation in the same language."
 msgstr "Vous ne pouvez avoir une relation vers un original de la même langue."
 
-#: forms/article.py:121
+#: forms/article.py:132
 msgid "You can't have related articles in different language."
 msgstr "Vous ne pouvez avoir des articles reliés avec une langue différente."
 
-#: forms/article.py:137
+#: forms/article.py:148
 msgid "You can't have categories in different language."
 msgstr "Vous ne pouvez avoir de catégories avec une langue différente."
 
 #: forms/category.py:90
 msgid ""
 "Some article in different language relate to this category, you can't change "
 "language until those article are not related anymore."
@@ -119,195 +123,221 @@
 "Certains articles dans une autre langue sont reliés à cette catégorie, vous "
 "ne pouvez changer la langue tant que ces articles n'y sont plus reliés."
 
 #: forms/translated.py:34
 msgid "Available languages"
 msgstr "Langues disponibles"
 
-#: models/article.py:33
+#: models/article.py:28
 msgid "original article"
 msgstr "article original"
 
-#: models/article.py:39
+#: models/article.py:34
 msgid "Mark this article as a translation of an original article."
 msgstr "Marquez cette article comme une traduction d'un article original"
 
-#: models/article.py:47
+#: models/article.py:42
 msgid "status"
 msgstr "état"
 
-#: models/article.py:52
+#: models/article.py:47
 msgid "Publication status."
 msgstr "État de publication."
 
-#: models/article.py:60
+#: models/article.py:55
 msgid "featured"
 msgstr "en une"
 
-#: models/article.py:64
+#: models/article.py:59
 msgid "Mark this article as featured."
 msgstr "Marquez cet article comme en une."
 
-#: models/article.py:72
+#: models/article.py:67
 msgid "pinned"
 msgstr "épinglé"
 
-#: models/article.py:76
+#: models/article.py:71
 msgid "A pinned article is enforced at top of order results."
 msgstr "Un article épinglé est forcé vers le haut des résultats."
 
-#: models/article.py:84
+#: models/article.py:79
 msgid "private"
 msgstr "privé"
 
-#: models/article.py:88
+#: models/article.py:83
 msgid "Private article is only available for authenticated users."
 msgstr ""
 "Un articlé privé est seulement disponible aux utilisateurs authentifiés."
 
-#: models/article.py:96
+#: models/article.py:91
 msgid "publication date"
 msgstr "date de publication"
 
-#: models/article.py:100
+#: models/article.py:95
 msgid "Start date of publication."
 msgstr "Date de début de publication."
 
-#: models/article.py:108
+#: models/article.py:103
 msgid "publication time"
 msgstr "heure de publication"
 
-#: models/article.py:111
+#: models/article.py:106
 msgid "Start time of publication."
 msgstr "Heure de début de publication."
 
-#: models/article.py:119
+#: models/article.py:114
 msgid "publication end"
 msgstr "fin de la publication"
 
-#: models/article.py:125
+#: models/article.py:120
 msgid "End date of publication."
 msgstr "Date de fin de la publication."
 
-#: models/article.py:133
+#: models/article.py:128
 msgid "last update"
 msgstr "dernière mise à jour"
 
-#: models/article.py:141 models/category.py:41
+#: models/article.py:136 models/category.py:34
 msgid "title"
 msgstr "titre"
 
-#: models/article.py:151 models/category.py:51
+#: models/article.py:146 models/category.py:44
 msgid "slug"
 msgstr "slug"
 
-#: models/article.py:154
+#: models/article.py:149
 msgid "Used to build the article URL."
 msgstr "Utilisé pour construire l'URL de l'article."
 
-#: models/article.py:162
+#: models/article.py:157
 msgid "SEO title"
 msgstr "Titre SEO"
 
-#: models/article.py:167
+#: models/article.py:162
 msgid ""
 "This value will be used as page meta title if not blank, else the article "
 "title is used."
 msgstr ""
 "Cette valeur sera utilisé comme le titre de méta information de la page s'il "
 "n'est pas vide, sinon le titre de l'article est utilisé."
 
-#: models/article.py:177 models/category.py:59
+#: models/article.py:172 models/category.py:52
 msgid "lead"
 msgstr "accroche"
 
-#: models/article.py:180 models/category.py:62
+#: models/article.py:175 models/category.py:55
 msgid "Lead paragraph, commonly used for SEO purposes in page meta tags."
 msgstr ""
 "Un paragraphe d'accroche, couramment utilisé à des fins de SEO dans les "
 "métas informations de la page."
 
-#: models/article.py:188
+#: models/article.py:183
 msgid "introduction"
 msgstr "introduction"
 
-#: models/article.py:196
+#: models/article.py:191
 msgid "content"
 msgstr "contenu"
 
-#: models/article.py:205 models/category.py:78
+#: models/article.py:200 models/category.py:71
 msgid "cover image"
 msgstr "image de couverture"
 
-#: models/article.py:211
+#: models/article.py:206
 msgid "Article cover image."
 msgstr "L'image de couverture de l'article."
 
-#: models/article.py:219
+#: models/article.py:214
 msgid "main image"
 msgstr "image principale"
 
-#: models/article.py:225
+#: models/article.py:220
 msgid "Article large image."
 msgstr "Une image large pour l'article."
 
-#: models/article.py:234
+#: models/article.py:229
 msgid "categories"
 msgstr "catégories"
 
-#: models/article.py:244
+#: models/article.py:239
 msgid "authors"
 msgstr "auteurs"
 
-#: models/article.py:254
+#: models/article.py:249
 msgid "related articles"
 msgstr "articles reliés"
 
 #: models/article.py:276
 msgid "Article"
 msgstr "Article"
 
-#: models/article.py:277 templates/lotus/article/list.html:4
+#: models/article.py:277 settings.py:101 templates/lotus/article/list.html:4
 #: templates/lotus/article/list.html:8 templates/lotus/author/detail.html:11
-#: templates/lotus/category/detail.html:22 views/article.py:25
+#: templates/lotus/category/detail.html:31 templates/lotus/tag/detail.html:11
 msgid "Articles"
 msgstr "Articles"
 
-#: models/category.py:33
+#: models/category.py:26
 msgid "Mark this category as a translation of an original category."
 msgstr ""
 "Marquez cette catégorie comme une traduction d'une catégorie originale."
 
-#: models/category.py:70
+#: models/category.py:63
 msgid "description"
 msgstr "description"
 
-#: models/category.py:97
+#: models/category.py:91
 msgid "Category"
 msgstr "Catégorie"
 
-#: models/category.py:98 templates/lotus/article/detail.html:104
-#: templates/lotus/category/list.html:4 templates/lotus/category/list.html:8
-#: views/category.py:25
+#: models/category.py:92 settings.py:103
+#: templates/lotus/article/detail.html:123 templates/lotus/category/list.html:4
+#: templates/lotus/category/list.html:8
 msgid "Categories"
 msgstr "Catégories"
 
-#: templates/admin/lotus/article/change_form.html:19
-#: templates/admin/lotus/category/change_form.html:19
+#: settings.py:102 templates/lotus/article/detail.html:158
+#: templates/lotus/author/list.html:4 templates/lotus/author/list.html:8
+msgid "Authors"
+msgstr "Auteurs"
+
+#: settings.py:104 templates/lotus/article/detail.html:140
+#: templates/lotus/tag/list.html:4 templates/lotus/tag/list.html:8
+msgid "Tags"
+msgstr "Étiquettes"
+
+#: templates/admin/lotus/article/change_form.html:20
+#: templates/admin/lotus/category/change_form.html:20
+#: templates/lotus/article/detail.html:45
+#: templates/lotus/category/detail.html:54
 msgid "Translate"
 msgstr "Traduire"
 
-#: templates/admin/lotus/article/change_form.html:28
+#: templates/admin/lotus/article/change_form.html:26
+msgid "Preview"
+msgstr "Aperçu"
+
+#: templates/admin/lotus/article/change_form.html:34
+#, python-format
+msgid ""
+"<strong>Article language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this article won't "
+"reachable from your site.<br><br>You may be able to edit this article but it "
+"will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/article/change_form.html:40
 msgid "Existing language(s) for this article:"
 msgstr "Langue(s) existante(s) pour cet article:"
 
 #: templates/admin/lotus/article/translate_original.html:7
 #: templates/admin/lotus/category/translate_original.html:7
 msgid "Home"
-msgstr ""
+msgstr "Accueil"
 
 #: templates/admin/lotus/article/translate_original.html:17
 msgid "No available languages for this article."
 msgstr "Aucune langue disponible pour cet article."
 
 #: templates/admin/lotus/article/translate_original.html:20
 msgid ""
@@ -328,15 +358,25 @@
 "à la place."
 
 #: templates/admin/lotus/article/translate_original.html:31
 #: templates/admin/lotus/category/translate_original.html:31
 msgid "Confirm"
 msgstr "Confirmez"
 
-#: templates/admin/lotus/category/change_form.html:28
+#: templates/admin/lotus/category/change_form.html:29
+#, python-format
+msgid ""
+"<strong>Category language '%(object_lang)s' is not in available project "
+"languages: %(available_langs)s</strong>. In this state, this category won't "
+"reachable from your site.<br><br>You may be able to edit this category but "
+"it will change language to an available one and you may have to change some "
+"related fields."
+msgstr ""
+
+#: templates/admin/lotus/category/change_form.html:35
 msgid "Existing language(s) for this category:"
 msgstr "Langue(s) existante(s) pour cette catégorie:"
 
 #: templates/admin/lotus/category/translate_original.html:17
 msgid "No available languages for this category."
 msgstr "Aucune langue disponible pour cette catégorie."
 
@@ -354,69 +394,98 @@
 "You requested to translate a translation category, this will send you to a "
 "create form to translate the original category '%(title)s' instead."
 msgstr ""
 "Vous avez requis une traduction pour cette catégorie de traduction, vous "
 "allez être conduit vers un formulaire pour traduire la catégorie originale "
 "'%(title)s' à la place."
 
-#: templates/lotus/article/detail.html:31
+#: templates/lotus/article/detail.html:39
+#: templates/lotus/category/detail.html:48
 msgid "Edit"
 msgstr "Éditer"
 
-#: templates/lotus/article/detail.html:38
+#: templates/lotus/article/detail.html:53
 msgid "Cover"
 msgstr "Couverture"
 
-#: templates/lotus/article/detail.html:52
+#: templates/lotus/article/detail.html:72
 msgid "States"
 msgstr "États"
 
-#: templates/lotus/article/detail.html:57 templates/lotus/article/item.html:23
+#: templates/lotus/article/detail.html:77
+#: templates/lotus/article/partials/item.html:28
 msgid "Featured"
 msgstr "En une"
 
-#: templates/lotus/article/detail.html:62 templates/lotus/article/item.html:26
+#: templates/lotus/article/detail.html:82
+#: templates/lotus/article/partials/item.html:31
 msgid "Pinned"
 msgstr "Épinglé"
 
-#: templates/lotus/article/detail.html:67 templates/lotus/article/item.html:29
+#: templates/lotus/article/detail.html:87
+#: templates/lotus/article/partials/item.html:34
 msgid "Draft"
 msgstr "Brouillon"
 
-#: templates/lotus/article/detail.html:72 templates/lotus/article/item.html:32
+#: templates/lotus/article/detail.html:92
+#: templates/lotus/article/partials/item.html:37
 msgid "Private"
 msgstr "Privé"
 
-#: templates/lotus/article/detail.html:77 templates/lotus/article/item.html:35
+#: templates/lotus/article/detail.html:97
+#: templates/lotus/article/partials/item.html:40
 msgid "Scheduled publication"
 msgstr "Publication programmée"
 
-#: templates/lotus/article/detail.html:82 templates/lotus/article/item.html:38
+#: templates/lotus/article/detail.html:102
+#: templates/lotus/article/partials/item.html:43
 msgid "Ended publication"
 msgstr "Publication finie"
 
-#: templates/lotus/article/detail.html:94
+#: templates/lotus/article/detail.html:113
+#: templates/lotus/category/detail.html:63
 msgid "Available in languages"
 msgstr "Disponible dans les langues"
 
-#: templates/lotus/article/detail.html:121 templates/lotus/author/list.html:4
-#: templates/lotus/author/list.html:8 views/author.py:24
-msgid "Authors"
-msgstr "Auteurs"
-
-#: templates/lotus/article/detail.html:136
+#: templates/lotus/article/detail.html:173
 msgid "Related articles"
 msgstr "Articles reliés"
 
-#: templates/lotus/pagination.html:4
+#: templates/lotus/article/partials/siblings.html:9
+msgid "Published"
+msgstr "Publié"
+
+#: templates/lotus/article/partials/siblings.html:11
+msgid "Not published"
+msgstr "Non publié"
+
+#: templates/lotus/article/partials/siblings.html:16
+#: templates/lotus/category/partials/siblings.html:9
+msgid "Is original"
+msgstr "Est un original"
+
+#: templates/lotus/article/partials/siblings.html:18
+#: templates/lotus/category/partials/siblings.html:11
+msgid "Is not original"
+msgstr "N'est pas un original"
+
+#: templates/lotus/pagination.html:3
 msgid "Pagination"
 msgstr "Pagination"
 
+#: templates/lotus/preview_switch.html:6
+msgid "Disable preview"
+msgstr ""
+
+#: templates/lotus/preview_switch.html:8
+msgid "Enable preview"
+msgstr ""
+
 #: views/admin/mixins.py:98
 #, python-format
 msgid "Translate '%(title)s'"
 msgstr "Traduire '%(title)s'"
 
-#: views/article.py:104
+#: views/article.py:110
 #, python-format
 msgid "No %(verbose_name)s found matching the query"
-msgstr ""
+msgstr "Pas de %(verbose_name)s trouvés pour la requête"
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/lookups.py` & `django-blog-lotus-0.6.0/lotus/lookups.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/management/commands/lotus_demo.py` & `django-blog-lotus-0.6.0/lotus/management/commands/lotus_demo.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/managers.py` & `django-blog-lotus-0.6.0/lotus/managers.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/migrations/0001_initial.py` & `django-blog-lotus-0.6.0/lotus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/models/article.py` & `django-blog-lotus-0.6.0/lotus/models/article.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/models/author.py` & `django-blog-lotus-0.6.0/lotus/models/author.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/models/category.py` & `django-blog-lotus-0.6.0/lotus/models/category.py`

 * *Files 7% similar despite different names*

```diff
@@ -118,14 +118,23 @@
         return translate_url(
             reverse("lotus:category-detail", kwargs={
                 "slug": self.slug,
             }),
             self.language
         )
 
+    def get_edit_url(self):
+        """
+        Return absolute URL to edit article from admin.
+
+        Returns:
+            string: An URL.
+        """
+        return reverse("admin:lotus_category_change", args=(self.id,))
+
     def get_cover_format(self):
         return self.media_format(self.cover)
 
 
 # Connect some signals
 post_delete.connect(
     auto_purge_files_on_delete(["cover"]),
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/models/translated.py` & `django-blog-lotus-0.6.0/lotus/models/translated.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/settings.py` & `django-blog-lotus-0.6.0/lotus/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from django.utils.translation import gettext_lazy as _
+
 """
 These are the default settings you can override in your own project settings
 right after the line which load the default app settings.
 """
 LOTUS_CATEGORY_PAGINATION = 5
 """
 Category per page limit for pagination, set it to ``None`` to disable
@@ -91,8 +93,23 @@
 """
 
 LOTUS_PREVIEW_SWITCH_TEMPLATE = "lotus/preview_switch.html"
 """
 Template path to use to render template tag ``preview_switch``.
 """
 
-_foobar = dir()
+LOTUS_CRUMBS_TITLES = {
+    "article-index": _("Articles"),
+    "author-index": _("Authors"),
+    "category-index": _("Categories"),
+    "tag-index": _("Tags"),
+}
+"""
+Crumb title to use for views breadcrumbs, for each item key uses the url name and value
+is the title to display. You must not remove any of these, just change the value.
+
+.. Note::
+
+    Not all views have a static crumb title, like all detail views use directly the
+    object title as a crumb title, so they won't be editable from this setting.
+
+"""
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/article/translate_original.html` & `django-blog-lotus-0.6.0/lotus/templates/admin/lotus/article/translate_original.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/change_form.html` & `django-blog-lotus-0.6.0/lotus/templates/admin/lotus/category/change_form.html`

 * *Files 11% similar despite different names*

```diff
@@ -7,26 +7,33 @@
     "object-tools-items", also this enable us to share results from tag
     "translation_siblings" instead of executing it twice.
 {% endcomment %}
 {% block object-tools %}
     {% if change %}
         {% if not is_popup %}
             {% translation_siblings original preview=True as sibling_stats %}
+            {% check_object_lang_availability original as object_lang_availability %}
 
             <ul class="object-tools">
                 {% block object-tools-items %}
                     {% if sibling_stats.available_languages %}
                     <li>
                         <a class="lotus-translate-link" href="{% url "admin:lotus_category_translate_original" id=original.id %}">{% trans "Translate" %}</a>
                     </li>
                     {% endif %}
                     {% change_form_object_tools %}
                 {% endblock %}
             </ul>
 
+            {% if not object_lang_availability.is_available %}
+            <p class="lotus-language-availability errornote">
+                {% blocktranslate with object_lang=original.language available_langs=object_lang_availability.language_keys|join:", " %}<strong>Category language '{{ object_lang }}' is not in available project languages: {{ available_langs }}</strong>. In this state, this category won't reachable from your site.<br><br>You may be able to edit this category but it will change language to an available one and you may have to change some related fields.{% endblocktranslate %}
+            </p>
+            {% endif %}
+
             {% if sibling_stats.siblings %}
             <p class="lotus-siblings-resume"><em>
                 {% blocktrans %}Existing language(s) for this category:{% endblocktrans %}
                 {% for sibling in sibling_stats.siblings %}
                     {% get_language_info for sibling.language as lang %}
                     <a href="{% url opts|admin_urlname:'change' sibling.pk %}" data-lotus-langcode="{{ sibling.language }}">{{ lang.name_translated }}</a>
                     {% if not forloop.last %} |{% endif %}
```

#### html2text {}

```diff
@@ -1,15 +1,26 @@
 {% extends "admin/change_form.html" %} {% load i18n admin_urls admin_modify
 lotus %} {% comment %} NOTE: We override the whole object-tools block since we
 add stuff in and around "object-tools-items", also this enable us to share
 results from tag "translation_siblings" instead of executing it twice. {%
 endcomment %} {% block object-tools %} {% if change %} {% if not is_popup %} {%
-translation_siblings original preview=True as sibling_stats %}
+translation_siblings original preview=True as sibling_stats %} {%
+check_object_lang_availability original as object_lang_availability %}
     * {% block object-tools-items %} {% if sibling_stats.available_languages %}
     *  id=original.id %}">{% trans "Translate" %}
 {% endif %} {% change_form_object_tools %} {% endblock %}
-{% if sibling_stats.siblings %}
+{% if not object_lang_availability.is_available %}
+{% blocktranslate with object_lang=original.language
+available_langs=object_lang_availability.language_keys|join:", " %}Category
+language '{{ object_lang }}' is not in available project languages: {
+{ available_langs }}. In this state, this category won't reachable from your
+site.
+
+You may be able to edit this category but it will change language to an
+available one and you may have to change some related fields.{%
+endblocktranslate %}
+{% endif %} {% if sibling_stats.siblings %}
 {% blocktrans %}Existing language(s) for this category:{% endblocktrans %} {%
 for sibling in sibling_stats.siblings %} {% get_language_info for
 sibling.language as lang %} {{_lang.name_translated_}} {% if not forloop.last
 %} |{% endif %} {% endfor %}
 {% endif %} {% endif %} {% endif %} {% endblock %}
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/admin/lotus/category/translate_original.html` & `django-blog-lotus-0.6.0/lotus/templates/admin/lotus/category/translate_original.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/detail.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/article/detail.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% extends "lotus/base.html" %}
 {% load i18n lotus smart_image %}
 
-{% block head_title %}{% if article_object.seo_title %}{{ article_object.seo_title }}{% else %}{{ article_object.title }}{% endif %}{% endblock head_title %}
-{% block head_metas %}
+{% block header-title %}{% if article_object.seo_title %}{{ article_object.seo_title }}{% else %}{{ article_object.title }}{% endif %}{% endblock header-title %}
+{% block metas %}
     {% if article_object.lead %}
         <meta name="description" content="{{ article_object.lead|striptags }}">
     {% endif %}
-{% endblock head_metas %}
+{% endblock metas %}
 
 {% block lotus_content %}{% spaceless %}
 {% translation_siblings article_object as sibling_stats %}
 <div class="article-detail {% article_states article_object prefix="article--" %}">
     <div class="container">
         <div class="row">
             <div class="col-12 col-lg-9">
@@ -103,15 +103,14 @@
                                     </li>
                                 {% endif %}
                             </ul>
                         </div>
                     {% endif %}
                 {% endif %}
 
-
                 {% if sibling_stats.siblings %}
                     <div class="siblings card mb-4">
                         <div class="card-header">
                             <strong>{% trans "Available in languages" %}</strong>
                         </div>
                         {% include "lotus/article/partials/siblings.html" with siblings=sibling_stats.siblings %}
                     </div>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends "lotus/base.html" %} {% load i18n lotus smart_image %} {% block
-head_title %}{% if article_object.seo_title %}{{ article_object.seo_title }}{%
-else %}{{ article_object.title }}{% endif %}{% endblock head_title %} {% block
-head_metas %} {% if article_object.lead %}
- {% endif %} {% endblock head_metas %} {% block lotus_content %}{% spaceless %}
-{% translation_siblings article_object as sibling_stats %}
+header-title %}{% if article_object.seo_title %}{{ article_object.seo_title }}
+{% else %}{{ article_object.title }}{% endif %}{% endblock header-title %} {%
+block metas %} {% if article_object.lead %}
+ {% endif %} {% endblock metas %} {% block lotus_content %}{% spaceless %} {%
+translation_siblings article_object as sibling_stats %}
  %}">
 {% if article_object.image %}
 {%_media_thumb_article_object.image_"948x416"_as_image_thumb_%}
 {% endif %}
 ****** {{ article_object.title }} ******
 {{ article_object.publish_datetime }}
 {{ article_object.introduction|safe }}
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/list.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/tag/detail.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 {% extends "lotus/base.html" %}
 {% load i18n %}
 
-{% block head_title %}{% trans "Articles" %}{% endblock head_title %}
+{% block header-title %}{{ tag_object }}{% endblock header-title %}
 
 {% block lotus_content %}{% spaceless %}
-<div class="article-list-container">
-    <h1 class="title border-bottom border-5 py-1 mb-3">{% trans "Articles" %}</h1>
+<div class="tag-detail">
+    <h1 class="title">{{ tag_object }}</h1>
 
-    <div class="list container">
-        <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4">
-            {% for article in article_list %}
+    <div class="articles container">
+        <h2>{% trans "Articles" %}</h2>
+
+        <div class="row row-cols-1 row-cols-md-3 g-4">
+            {% for article in object_list %}
                 <div class="col">
-                    {% include "lotus/article/partials/item.html" with article_object=article from="article-list" %}
+                    {% include "lotus/article/partials/item.html" with article_object=article from="tag-detail" %}
                 </div>
             {% endfor %}
         </div>
+        {% include "lotus/pagination.html" %}
     </div>
-
-    {% include "lotus/pagination.html" %}
 </div>
 {% endspaceless %}{% endblock lotus_content %}
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/article/partials/item.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/article/partials/item.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/detail.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/author/detail.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends "lotus/base.html" %}
 {% load i18n %}
 
-{% block head_title %}{{ author_object }}{% endblock head_title %}
+{% block header-title %}{{ author_object }}{% endblock header-title %}
 
 {% block lotus_content %}{% spaceless %}
 <div class="author-detail">
     <h1 class="title">{{ author_object }}</h1>
 
     <div class="articles container">
         <h2>{% trans "Articles" %}</h2>
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/author/list.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/article/list.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% extends "lotus/base.html" %}
 {% load i18n %}
 
-{% block head_title %}{% trans "Authors" %}{% endblock head_title %}
+{% block header-title %}{% trans "Articles" %}{% endblock header-title %}
 
 {% block lotus_content %}{% spaceless %}
-<div class="author-list-container">
-    <h1 class="title border-bottom border-5 py-1 mb-3">{% trans "Authors" %}</h1>
+<div class="article-list-container">
+    <h1 class="title border-bottom border-5 py-1 mb-3">{% trans "Articles" %}</h1>
 
     <div class="list container">
-        <div class="row row-cols-1 row-cols-md-4 g-4">
-            {% for author in author_list %}
-            <div class="col">
-                {% include "lotus/author/partials/item.html" with author_object=author from="author-list" %}
-            </div>
+        <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4">
+            {% for article in article_list %}
+                <div class="col">
+                    {% include "lotus/article/partials/item.html" with article_object=article from="article-list" %}
+                </div>
             {% endfor %}
         </div>
     </div>
 
     {% include "lotus/pagination.html" %}
 </div>
 {% endspaceless %}{% endblock lotus_content %}
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/detail.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/category/detail.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,72 @@
 {% extends "lotus/base.html" %}
-{% load i18n smart_image %}
+{% load i18n lotus smart_image %}
 
-{% block head_title %}{{ category_object.title }}{% endblock head_title %}
-{% block head_metas %}
+{% block header-title %}{{ category_object.title }}{% endblock header-title %}
+{% block metas %}
     {% if category_object.lead %}<meta name="description" content="{{ category_object.lead|striptags }}">{% endif %}
-{% endblock head_metas %}
+{% endblock metas %}
 
 {% block lotus_content %}{% spaceless %}
+{% translation_siblings category_object as sibling_stats %}
 <div class="category-detail">
-    <div class="detail mb-4">
-        <h1 class="title">{{ category_object.title }}</h1>
+    <div class="container">
+        <div class="row">
+            <div class="col-12 col-lg-9">
+                <div class="detail mb-4">
+                    <h1 class="title">{{ category_object.title }}</h1>
+
+                    <div class="cover bg-light rounded text-center mb-2 p-2">
+                        {% if category_object.cover %}
+                            <a href="{{ category_object.cover.url }}" target="_blank">
+                                {% media_thumb category_object.cover "800x640" crop="center" as cover_thumb %}
+                                <img src="{{ cover_thumb.url }}" class="rounded img-fluid" alt="">
+                            </a>
+                        {% endif %}
+                    </div>
 
-        <div class="cover bg-light rounded text-center mb-2 p-2">
-            {% if category_object.cover %}
-                <a href="{{ category_object.cover.url }}" target="_blank">
-                    {% media_thumb category_object.cover "800x640" crop="center" as cover_thumb %}
-                    <img src="{{ cover_thumb.url }}" class="rounded img-fluid" alt="">
-                </a>
-            {% endif %}
-        </div>
-
-        <div class="description p-2 fs-5">{{ category_object.description|safe }}</div>
-    </div>
+                    <div class="description p-2 fs-5">{{ category_object.description|safe }}</div>
+                </div>
 
-    <div class="articles container">
-        <h2>{% trans "Articles" %}</h2>
+                <div class="articles container">
+                    <h2>{% trans "Articles" %}</h2>
 
-        <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
-            {% for article in object_list %}
-                <div class="col">
-                    {% include "lotus/article/partials/item.html" with article_object=article from="category-detail" %}
+                    <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
+                        {% for article in object_list %}
+                            <div class="col">
+                                {% include "lotus/article/partials/item.html" with article_object=article from="category-detail" %}
+                            </div>
+                        {% endfor %}
+                    </div>
+                    {% include "lotus/pagination.html" %}
                 </div>
-            {% endfor %}
+            </div>
+
+            <div class="col-12 col-lg-3">
+                {% if user.is_authenticated and user.is_staff %}
+                    <div class="d-grid mb-4">
+                        <a class="detail-edit btn btn-primary" href="{{ category_object.get_edit_url }}" target="_blank">
+                            {% trans "Edit" %}
+                        </a>
+                        {% if sibling_stats.available_languages %}
+                            <a class="detail-translate btn btn-primary mt-1"
+                               href="{% url "admin:lotus_category_translate_original" id=category_object.id %}"
+                               target="_blank">
+                                {% trans "Translate" %}
+                            </a>
+                        {% endif %}
+                    </div>
+                {% endif %}
+
+                {% if sibling_stats.siblings %}
+                    <div class="siblings card mb-4">
+                        <div class="card-header">
+                            <strong>{% trans "Available in languages" %}</strong>
+                        </div>
+                        {% include "lotus/category/partials/siblings.html" with siblings=sibling_stats.siblings %}
+                    </div>
+                {% endif %}
+            </div>
         </div>
-        {% include "lotus/pagination.html" %}
     </div>
 </div>
 {% endspaceless %}{% endblock lotus_content %}
```

#### html2text {}

```diff
@@ -1,16 +1,26 @@
-{% extends "lotus/base.html" %} {% load i18n smart_image %} {% block head_title
-%}{{ category_object.title }}{% endblock head_title %} {% block head_metas %}
-{% if category_object.lead %}
-{% endif %} {% endblock head_metas %} {% block lotus_content %}{% spaceless %}
+{% extends "lotus/base.html" %} {% load i18n lotus smart_image %} {% block
+header-title %}{{ category_object.title }}{% endblock header-title %} {% block
+metas %} {% if category_object.lead %}
+{% endif %} {% endblock metas %} {% block lotus_content %}{% spaceless %} {%
+translation_siblings category_object as sibling_stats %}
 ****** {{ category_object.title }} ******
 {% if category_object.cover %}
 {%_media_thumb_category_object.cover_"800x640"_crop="center"_as_cover_thumb_%}
  {% endif %}
 {{ category_object.description|safe }}
 ***** {% trans "Articles" %} *****
 {% for article in object_list %}
 {% include "lotus/article/partials/item.html" with article_object=article
 from="category-detail" %}
 {% endfor %}
 {% include "lotus/pagination.html" %}
+{% if user.is_authenticated and user.is_staff %}
+{%_trans_"Edit"_%} {% if sibling_stats.available_languages %}
+ id=category_object.id %}" target="_blank"> {% trans "Translate" %}
+ {% endif %}
+{% endif %} {% if sibling_stats.siblings %}
+{% trans "Available in languages" %}
+{% include "lotus/category/partials/siblings.html" with
+siblings=sibling_stats.siblings %}
+{% endif %}
 {% endspaceless %}{% endblock lotus_content %}
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/list.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/category/list.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends "lotus/base.html" %}
 {% load i18n %}
 
-{% block head_title %}{% trans "Categories" %}{% endblock head_title %}
+{% block header-title %}{% trans "Categories" %}{% endblock header-title %}
 
 {% block lotus_content %}{% spaceless %}
 <div class="category-list-container">
     <h1 class="title border-bottom border-5 py-1 mb-3">{% trans "Categories" %}</h1>
 
     <div class="list container">
         <div class="row row-cols-1 row-cols-md-3 row-cols-lg-5 g-4">
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/category/partials/item.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/category/partials/item.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/pagination.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/pagination.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/preview_switch.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/preview_switch.html`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/detail.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/author/list.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 {% extends "lotus/base.html" %}
 {% load i18n %}
 
-{% block head_title %}{{ tag_object }}{% endblock head_title %}
+{% block header-title %}{% trans "Authors" %}{% endblock header-title %}
 
 {% block lotus_content %}{% spaceless %}
-<div class="tag-detail">
-    <h1 class="title">{{ tag_object }}</h1>
+<div class="author-list-container">
+    <h1 class="title border-bottom border-5 py-1 mb-3">{% trans "Authors" %}</h1>
 
-    <div class="articles container">
-        <h2>{% trans "Articles" %}</h2>
-
-        <div class="row row-cols-1 row-cols-md-3 g-4">
-            {% for article in object_list %}
-                <div class="col">
-                    {% include "lotus/article/partials/item.html" with article_object=article from="tag-detail" %}
-                </div>
+    <div class="list container">
+        <div class="row row-cols-1 row-cols-md-4 g-4">
+            {% for author in author_list %}
+            <div class="col">
+                {% include "lotus/author/partials/item.html" with author_object=author from="author-list" %}
+            </div>
             {% endfor %}
         </div>
-        {% include "lotus/pagination.html" %}
     </div>
+
+    {% include "lotus/pagination.html" %}
 </div>
 {% endspaceless %}{% endblock lotus_content %}
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templates/lotus/tag/list.html` & `django-blog-lotus-0.6.0/lotus/templates/lotus/tag/list.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends "lotus/base.html" %}
 {% load i18n %}
 
-{% block head_title %}{% trans "Tags" %}{% endblock head_title %}
+{% block header-title %}{% trans "Tags" %}{% endblock header-title %}
 
 {% block lotus_content %}{% spaceless %}
 <div class="tag-list-container">
     <h1 class="title border-bottom border-5 py-1 mb-3">{% trans "Tags" %}</h1>
 
     <div class="list container">
         <div class="row justify-content-center">
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/templatetags/lotus.py` & `django-blog-lotus-0.6.0/lotus/templatetags/lotus.py`

 * *Files 5% similar despite different names*

```diff
@@ -299,7 +299,43 @@
 
     return {
         "user": user,
         "allowed": allowed,
         "current_mode": current_mode,
         "redirection": redirection,
     }
+
+
+@register.simple_tag(takes_context=True)
+def check_object_lang_availability(context, source, **kwargs):
+    """
+    Determine if an object has a language that are not available from ``LANGUAGES``
+    setting.
+
+    Example:
+        This tag does not expect any argument: ::
+
+            {% load lotus %}
+            {% check_object_lang_availability article_object as object_lang_availability %}
+
+    Arguments:
+        context (object): Either a ``django.template.Context`` or a dictionnary for
+            context variables. It is not used from this tag.
+        source (object): Any object with an attribute ``language`` that will be checked
+            against ``settings.LANGUAGES`` however the tag will fails silently for
+            given source that does not have this attribute.
+
+    Returns:
+        dict: A dictionnary with summary informations of object language and its
+            availability.
+    """  # noqa: E501
+    is_available = False
+
+    if getattr(source, "language", None):
+        is_available = source.language in [k for k, v in settings.LANGUAGES]
+
+    return {
+        "is_available": is_available,
+        "languages": settings.LANGUAGES,
+        "language_keys": [k for k, v in settings.LANGUAGES],
+        "language_labels": [v for k, v in settings.LANGUAGES],
+    }
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/urls.py` & `django-blog-lotus-0.6.0/lotus/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,14 @@
 
 
 app_name = "lotus"
 
 
 urlpatterns = [
     path("", ArticleIndexView.as_view(), name="article-index"),
-    path(
-        "articles/<int:year>/<int:month>/<int:day>/<slug:slug>/",
-        ArticleDetailView.as_view(),
-        name="article-detail"
-    ),
 
     path("authors/", AuthorIndexView.as_view(), name="author-index"),
     path(
         "authors/<slug:username>/",
         AuthorDetailView.as_view(),
         name="author-detail"
     ),
@@ -60,8 +55,14 @@
         name="tag-autocomplete",
     ),
     path(
         "tags/<str:tag>/",
         TagDetailView.as_view(),
         name="tag-detail"
     ),
+
+    path(
+        "<int:year>/<int:month>/<int:day>/<slug:slug>/",
+        ArticleDetailView.as_view(),
+        name="article-detail"
+    ),
 ]
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/utils/factory.py` & `django-blog-lotus-0.6.0/lotus/utils/factory.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/utils/imaging.py` & `django-blog-lotus-0.6.0/lotus/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/utils/tests.py` & `django-blog-lotus-0.6.0/lotus/utils/tests.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/__init__.py` & `django-blog-lotus-0.6.0/lotus/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/admin/mixins.py` & `django-blog-lotus-0.6.0/lotus/views/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/article.py` & `django-blog-lotus-0.6.0/lotus/views/article.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from django.conf import settings
 from django.http import Http404, HttpResponseForbidden
 from django.views.generic import DetailView, ListView
 from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 
 from ..models import Article
-from .mixins import PreviewModeMixin, ArticleFilterMixin, LotusContextStage
+from .mixins import (
+    ArticleFilterMixin,
+    LanguageMixin,
+    LotusContextStage,
+    PreviewModeMixin,
+)
 
 try:
     from view_breadcrumbs import BaseBreadcrumbMixin
 except ImportError:
     from .mixins import NoOperationBreadcrumMixin as BaseBreadcrumbMixin
 
 
 class ArticleIndexView(BaseBreadcrumbMixin, LotusContextStage, ArticleFilterMixin,
-                       PreviewModeMixin, ListView):
+                       PreviewModeMixin, LanguageMixin, ListView):
     """
     Paginated list of articles.
     """
     model = Article
     template_name = "lotus/article/list.html"
     paginate_by = settings.LOTUS_ARTICLE_PAGINATION
     context_object_name = "article_list"
-    crumb_title = _("Articles")
+    crumb_title = settings.LOTUS_CRUMBS_TITLES["article-index"]
     crumb_urlname = "lotus:article-index"
     lotus_stage = "articles"
 
     @property
     def crumbs(self):
         return [
             (self.crumb_title, reverse(self.crumb_urlname)),
         ]
 
     def get_queryset(self):
-        q = self.apply_article_lookups(self.model.objects, self.request.LANGUAGE_CODE)
+        q = self.apply_article_lookups(self.model.objects, self.get_language_code())
 
         return q.order_by(*self.model.COMMON_ORDER_BY)
 
 
 class ArticleDetailView(BaseBreadcrumbMixin, LotusContextStage, ArticleFilterMixin,
-                        PreviewModeMixin, DetailView):
+                        PreviewModeMixin, LanguageMixin, DetailView):
     """
     Article detail.
     """
     model = Article
     pk_url_kwarg = "article_pk"
     template_name = "lotus/article/detail.html"
     context_object_name = "article_object"
@@ -73,15 +78,15 @@
         depending preview mode.
 
         Preview mode is enabled from a flag in session and only for staff user. If it is
         disabled publication criterias are applied on lookups.
 
         Also apply lookup for "private" mode for non authenticated users.
         """
-        q = self.apply_article_lookups(self.model.objects, self.request.LANGUAGE_CODE)
+        q = self.apply_article_lookups(self.model.objects, self.get_language_code())
 
         return q
 
     def get_object(self, queryset=None):
         """
         Apply the right filters to get the article object.
         """
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/author.py` & `django-blog-lotus-0.6.0/lotus/views/author.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 from django.conf import settings
 from django.views.generic import ListView
 from django.views.generic.detail import SingleObjectMixin
-from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 
 from ..models import Article, Author
-from .mixins import PreviewModeMixin, ArticleFilterMixin, LotusContextStage
+from .mixins import (
+    ArticleFilterMixin,
+    LanguageMixin,
+    LotusContextStage,
+    PreviewModeMixin,
+)
 
 try:
     from view_breadcrumbs import BaseBreadcrumbMixin
 except ImportError:
     from .mixins import NoOperationBreadcrumMixin as BaseBreadcrumbMixin
 
 
 class AuthorIndexView(BaseBreadcrumbMixin, LotusContextStage, PreviewModeMixin,
-                      ListView):
+                      LanguageMixin, ListView):
     """
     List of authors which have contributed at least to one article.
     """
     model = Author
     template_name = "lotus/author/list.html"
     paginate_by = settings.LOTUS_AUTHOR_PAGINATION
     context_object_name = "author_list"
-    crumb_title = _("Authors")
+    crumb_title = settings.LOTUS_CRUMBS_TITLES["author-index"]
     crumb_urlname = "lotus:author-index"
     lotus_stage = "authors"
 
     @property
     def crumbs(self):
         return [
             (self.crumb_title, reverse(self.crumb_urlname)),
         ]
 
     def get_queryset(self):
-        q = self.model.lotus_objects.get_active(language=self.request.LANGUAGE_CODE)
+        q = self.model.lotus_objects.get_active(language=self.get_language_code())
 
         return q.order_by(*self.model.COMMON_ORDER_BY)
 
 
 class AuthorDetailView(BaseBreadcrumbMixin, LotusContextStage, ArticleFilterMixin,
-                       PreviewModeMixin, SingleObjectMixin, ListView):
+                       PreviewModeMixin, LanguageMixin, SingleObjectMixin, ListView):
     """
     Author detail and its related article list.
 
     Opposed to article or category listing, this one list objects for language from
     request, not from the author language since it dont have one.
     """
     model = Author
@@ -81,15 +85,15 @@
         """
         Build queryset base to list Author articles.
 
         Depend on "self.object" to list the Author related objects.
         """
         q = self.apply_article_lookups(
             self.object.articles,
-            self.request.LANGUAGE_CODE,
+            self.get_language_code(),
         )
 
         return q.order_by(*self.listed_model.COMMON_ORDER_BY)
 
     def get(self, request, *args, **kwargs):
         # Try to get Author object
         self.object = self.get_object(queryset=self.get_queryset_for_object())
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/category.py` & `django-blog-lotus-0.6.0/lotus/views/category.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 from django.conf import settings
 from django.views.generic import ListView
 from django.views.generic.detail import SingleObjectMixin
-from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 
 from ..models import Article, Category
 
-from .mixins import PreviewModeMixin, ArticleFilterMixin, LotusContextStage
+from .mixins import (
+    ArticleFilterMixin,
+    LanguageMixin,
+    LotusContextStage,
+    PreviewModeMixin,
+)
 
 try:
     from view_breadcrumbs import BaseBreadcrumbMixin
 except ImportError:
     from .mixins import NoOperationBreadcrumMixin as BaseBreadcrumbMixin
 
 
 class CategoryIndexView(BaseBreadcrumbMixin, LotusContextStage, PreviewModeMixin,
-                        ListView):
+                        LanguageMixin, ListView):
     """
     List of categories
     """
     model = Category
     template_name = "lotus/category/list.html"
     paginate_by = settings.LOTUS_CATEGORY_PAGINATION
     context_object_name = "category_list"
-    crumb_title = _("Categories")
+    crumb_title = settings.LOTUS_CRUMBS_TITLES["category-index"]
     crumb_urlname = "lotus:category-index"
     lotus_stage = "categories"
 
     @property
     def crumbs(self):
         return [
             (self.crumb_title, reverse(self.crumb_urlname)),
         ]
 
     def get_queryset(self):
         """
         Build queryset base with language filtering to list categories.
         """
-        q = self.model.objects.get_for_lang(self.request.LANGUAGE_CODE)
+        q = self.model.objects.get_for_lang(self.get_language_code())
 
         return q.order_by(*self.model.COMMON_ORDER_BY)
 
 
 class CategoryDetailView(BaseBreadcrumbMixin, LotusContextStage, ArticleFilterMixin,
-                         PreviewModeMixin, SingleObjectMixin, ListView):
+                         PreviewModeMixin, LanguageMixin, SingleObjectMixin, ListView):
     """
     Category detail and its related article list.
     """
     model = Category
     listed_model = Article
     template_name = "lotus/category/detail.html"
     paginate_by = settings.LOTUS_ARTICLE_PAGINATION
@@ -71,15 +75,15 @@
             (self.object.title, reverse(self.crumb_urlname, kwargs=details_kwargs)),
         ]
 
     def get_queryset_for_object(self):
         """
         Build queryset base with language filtering to get Category.
         """
-        return self.model.objects.get_for_lang(self.request.LANGUAGE_CODE)
+        return self.model.objects.get_for_lang(self.get_language_code())
 
     def get_queryset(self):
         """
         Build queryset base to list Category articles.
 
         Depend on "self.object" to list the Category related objects filtered on its
         language.
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/mixins.py` & `django-blog-lotus-0.6.0/lotus/views/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.conf import settings
 from django.db import models
 from django.utils import timezone
 
 from ..lookups import LookupBuilder
+from ..utils.language import get_language_code
 
 
 class NoOperationBreadcrumMixin:
     """
     A dummy and empty mixin to use when 'view_breadcrumbs' is not available.
     """
     pass
@@ -168,7 +169,24 @@
     def get_context_data(self, **kwargs):
         """
         Expose the date "now" used for publication filter.
         """
         context = super().get_context_data(**kwargs)
         context["lotus_stage"] = self.get_lotus_stage()
         return context
+
+
+class LanguageMixin:
+    """
+    A mixin to provide very common logic related to language.
+    """
+    def get_language_code(self):
+        """
+        Shortand to ``get_language_code`` function that already give the request object.
+
+        .. Warning::
+            This should not be used in view code before request attribute have been set.
+
+        Returns:
+            string: Language code retrieved either from request object or settings.
+        """
+        return get_language_code(self.request)
```

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/preview.py` & `django-blog-lotus-0.6.0/lotus/views/preview.py`

 * *Files identical despite different names*

### Comparing `django-blog-lotus-0.5.2.1/lotus/views/tag.py` & `django-blog-lotus-0.6.0/lotus/views/tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from django.conf import settings
 from django.contrib.auth.mixins import UserPassesTestMixin
 from django.db.models import Count, Q
 from django.http import Http404, HttpResponseBadRequest
 from django.views.generic import ListView
 from django.views.generic.detail import SingleObjectMixin
-from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 from django.views import View
 
 from dal import autocomplete
 from taggit.models import Tag
 
 from ..models import Article
-from .mixins import PreviewModeMixin, ArticleFilterMixin, LotusContextStage
+from .mixins import (
+    ArticleFilterMixin,
+    LanguageMixin,
+    LotusContextStage,
+    PreviewModeMixin,
+)
 
 try:
     from view_breadcrumbs import BaseBreadcrumbMixin
 except ImportError:
     from .mixins import NoOperationBreadcrumMixin as BaseBreadcrumbMixin
 
 
@@ -25,23 +29,23 @@
     A very basic view which always return the common Http404 page.
     """
     def get(self, request, *args, **kwargs):
         raise Http404()
 
 
 class EnabledTagIndexView(BaseBreadcrumbMixin, LotusContextStage, ArticleFilterMixin,
-                          PreviewModeMixin, ListView):
+                          PreviewModeMixin, LanguageMixin, ListView):
     """
     List of tags that are related from at least one article.
     """
     model = Tag
     template_name = "lotus/tag/list.html"
     paginate_by = settings.LOTUS_TAG_PAGINATION
     context_object_name = "tag_list"
-    crumb_title = _("Tags")
+    crumb_title = settings.LOTUS_CRUMBS_TITLES["tag-index"]
     crumb_urlname = "lotus:tag-index"
     lotus_stage = "tags"
 
     @property
     def crumbs(self):
         return [
             (self.crumb_title, reverse(self.crumb_urlname)),
@@ -50,28 +54,28 @@
     def get_queryset(self):
         """
         Build complex queryset to get all tags which have published articles.
 
         Published articles are determined with the common publication criterias.
         """
         publication_criterias = self.build_article_lookups(
-            language=self.request.LANGUAGE_CODE,
+            language=self.get_language_code(),
             prefix="article__",
         )
 
         return Tag.objects.annotate(
             article_count=Count(
                 "article",
                 filter=Q(*publication_criterias),
             )
         ).filter(article_count__gt=0).order_by("name")
 
 
 class TagDetailView(BaseBreadcrumbMixin, LotusContextStage, ArticleFilterMixin,
-                    PreviewModeMixin, SingleObjectMixin, ListView):
+                    PreviewModeMixin, LanguageMixin, SingleObjectMixin, ListView):
     """
     Tag detail and its related article list.
 
     Opposed to article or category listing, this one list objects for language from
     request, not from the tag language since it dont have one.
     """
     model = Tag
@@ -115,15 +119,15 @@
 
         Depend on "self.object" to list the Tag related objects.
         """
         q = self.apply_article_lookups(
             self.listed_model.objects.filter(
                 tags__id__in=[self.object.id]
             ),
-            self.request.LANGUAGE_CODE,
+            self.get_language_code(),
         )
 
         return q.order_by(*self.listed_model.COMMON_ORDER_BY)
 
     def get(self, request, *args, **kwargs):
         # Try to get Tag object
         self.object = self.get_object(queryset=self.get_queryset_for_object())
```

### Comparing `django-blog-lotus-0.5.2.1/setup.cfg` & `django-blog-lotus-0.6.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 [metadata]
 name = django-blog-lotus
-version = 0.5.2.1
+version = 0.6.0
 description = A weblog application with Django.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = Emencia
 author_email = support@emencia.com
 url = https://github.com/emencia/django-blog-lotus
 project_urls = 
 	Source Code = https://github.com/emencia/django-blog-lotus
 	Issue Tracker = https://github.com/emencia/django-blog-lotus/issues
 	Changelog = https://django-blog-lotus.readthedocs.io/en/latest/history.html
 	Documentation = https://django-blog-lotus.readthedocs.io/
 license = MIT
 keywords = Python Django Blog
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 
 [options]
+python_requires = >=3.8
 include_package_data = True
 install_requires = 
-	Django>=3.1,<4.2
+	Django>=3.2,<5.0
 	django-ckeditor>=6.0.0
 	django-taggit>=3.1.0
-	django-autocomplete-light>=3.9.4
+	django-autocomplete-light>=3.9.7
 	django-smart-media>=0.2.2
 packages = find:
 zip_safe = True
 
 [options.extras_require]
 breadcrumbs = 
 	django-view-breadcrumbs>=2.2.4
@@ -84,21 +86,21 @@
 python_files = 
 	*.py
 testpaths = 
 	tests
 
 [tox:tox]
 minversion = 3.4.0
-envlist = py{38,310}-django{32,40,41}-cms
+envlist = py{38,310}-django{32,40,42}
 
 [testenv]
 deps = 
 	django32: Django>=3.2,<3.3
 	django40: Django>=4.0,<4.1
-	django41: Django>=4.1,<4.2
+	django42: Django>=4.2,<5.0
 	py38-django32: backports.zoneinfo
 commands = 
 	pip install -e .[breadcrumbs,dev]
 	pytest -vv tests
 
 [egg_info]
 tag_build =
```

