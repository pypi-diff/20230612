# Comparing `tmp/fullask-rest-framework-0.1.2.tar.gz` & `tmp/fullask-rest-framework-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullask-rest-framework-0.1.2.tar", last modified: Mon Jun  5 17:34:27 2023, max compression
+gzip compressed data, was "fullask-rest-framework-0.1.3.tar", last modified: Mon Jun 12 13:26:43 2023, max compression
```

## Comparing `fullask-rest-framework-0.1.2.tar` & `fullask-rest-framework-0.1.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      175 2023-04-17 01:36:01.000000 fullask-rest-framework-0.1.2/AUTHORS.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1070 2023-04-17 01:40:34.000000 fullask-rest-framework-0.1.2/LICENSE
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      306 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/MANIFEST.in
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5482 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/PKG-INFO
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     4659 2023-06-05 17:27:25.000000 fullask-rest-framework-0.1.2/README.md
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.875509 fullask-rest-framework-0.1.2/docs/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      632 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/Makefile
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.875509 fullask-rest-framework-0.1.2/docs/docfiles/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/authors.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5075 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/conf.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1997 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/contributing.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      313 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/index.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1246 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/installation.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       99 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/docfiles/usage.rst
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      829 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/docs/make.bat
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      150 2023-06-05 17:33:38.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      604 2023-04-21 13:51:24.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/cli.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-18 18:19:58.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/index.html
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      851 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/login_form.html
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/static/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1146 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/views.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.871509 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/__init__.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/models.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/resources.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/app_template/schemas.txt
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-08 13:47:33.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/__init__.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      112 2023-03-12 13:06:42.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/app.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      322 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/config.py.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      628 2023-04-18 19:16:45.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/factory.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       65 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/tests.txt
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-07 17:34:01.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       49 2023-05-15 10:40:45.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/base_entity.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      346 2023-05-08 13:47:35.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/filtering.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      450 2023-06-05 16:00:39.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/pagination.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      407 2023-05-15 10:15:36.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/entities/sorting.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.883509 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-02 15:45:42.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3875 2023-06-05 16:58:36.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/app_factory.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      641 2023-06-05 06:20:45.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/factory/extensions.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:06:42.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-13 16:25:47.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      228 2023-06-05 16:15:54.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/base_model.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      985 2023-06-05 16:15:24.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/mixins.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       37 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/.gitignore
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      191 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      302 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/README.md
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.871509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.887509 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       69 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/lastfailed
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       63 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        2 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-20 07:40:30.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      427 2023-06-05 16:03:17.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/base.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     2852 2023-06-05 16:03:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/crud.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     8568 2023-06-05 16:03:08.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/sqlalchemy.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1212 2023-05-15 07:28:57.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/fields.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      267 2023-06-05 16:08:35.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/filtering.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1033 2023-06-05 16:10:52.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/pagination.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      636 2023-06-05 16:11:02.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/sorting.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/fullask_rest_framework/service/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-12 12:54:11.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/service/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/fullask_rest_framework/utils/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/utils/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      572 2023-04-14 13:52:15.000000 fullask-rest-framework-0.1.2/fullask_rest_framework/utils/jwt.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.879509 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5482 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/PKG-INFO
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3189 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       68 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/entry_points.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/not-zip-safe
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      153 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/requires.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       23 2023-06-05 17:34:27.000000 fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/top_level.txt
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      846 2023-06-05 15:57:14.000000 fullask-rest-framework-0.1.2/pyproject.toml
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      394 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/setup.cfg
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1654 2023-06-05 17:30:32.000000 fullask-rest-framework-0.1.2/setup.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/tests/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:34:17.000000 fullask-rest-framework-0.1.2/tests/__init__.py
-drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 17:34:27.891510 fullask-rest-framework-0.1.2/tests/repositories/
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:35:54.000000 fullask-rest-framework-0.1.2/tests/repositories/__init__.py
--rw-rw-r--   0 goddessana  (1000) goddessana  (1000)    20125 2023-06-05 16:00:28.000000 fullask-rest-framework-0.1.2/tests/repositories/test_sqlalchemy_repository.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      175 2023-04-17 01:36:01.000000 fullask-rest-framework-0.1.3/AUTHORS.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1070 2023-04-17 01:40:34.000000 fullask-rest-framework-0.1.3/LICENSE
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      306 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/MANIFEST.in
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5399 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     4576 2023-06-05 17:51:33.000000 fullask-rest-framework-0.1.3/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.874318 fullask-rest-framework-0.1.3/docs/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      632 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/Makefile
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.878319 fullask-rest-framework-0.1.3/docs/docfiles/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       31 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/docfiles/authors.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5075 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/docfiles/conf.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1997 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/docfiles/contributing.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      313 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/docfiles/index.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1246 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/docfiles/installation.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       99 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/docfiles/usage.rst
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      829 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/docs/make.bat
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.878319 fullask-rest-framework-0.1.3/fullask_rest_framework/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      150 2023-06-12 13:26:25.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      604 2023-04-21 13:51:24.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/cli.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.882321 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-18 18:19:58.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.882321 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.882321 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/templates/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/templates/index.html
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      851 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/templates/login_form.html
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.882321 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/templates/static/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1146 2023-03-11 15:35:53.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/views.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.870317 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.882321 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/app_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/app_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/app_template/models.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/app_template/resources.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/app_template/schemas.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.882321 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/project_template/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-08 13:47:33.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/project_template/__init__.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      112 2023-03-12 13:06:42.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/project_template/app.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      322 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/project_template/config.py.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      628 2023-04-18 19:16:45.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/project_template/factory.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       65 2023-02-24 07:55:09.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/project_template/tests.txt
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.882321 fullask-rest-framework-0.1.3/fullask_rest_framework/entities/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-07 17:34:01.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/entities/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       49 2023-05-15 10:40:45.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/entities/base_entity.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      346 2023-05-08 13:47:35.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/entities/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      450 2023-06-05 16:00:39.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/entities/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      407 2023-05-15 10:15:36.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/entities/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.886322 fullask-rest-framework-0.1.3/fullask_rest_framework/factory/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-02 15:45:42.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/factory/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3875 2023-06-11 15:43:54.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/factory/app_factory.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      641 2023-06-11 15:37:37.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/factory/extensions.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.886322 fullask-rest-framework-0.1.3/fullask_rest_framework/orm/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-06-05 16:06:42.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/orm/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.886322 fullask-rest-framework-0.1.3/fullask_rest_framework/orm/sqlalchemy/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-13 16:25:47.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/orm/sqlalchemy/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      228 2023-06-05 16:15:54.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/orm/sqlalchemy/base_model.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      985 2023-06-05 16:15:24.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/orm/sqlalchemy/mixins.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.886322 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.886322 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       37 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/.gitignore
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      191 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      302 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/README.md
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.874318 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/v/
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/v/cache/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       69 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/v/cache/lastfailed
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       63 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        2 2023-04-23 22:27:34.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-20 07:40:30.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      427 2023-06-05 16:03:17.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/base.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     2852 2023-06-05 16:03:27.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/crud.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     8658 2023-06-12 13:24:52.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/sqlalchemy.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1212 2023-05-15 07:28:57.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/fields.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      267 2023-06-05 16:08:35.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/filtering.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1033 2023-06-05 16:10:52.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/pagination.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      636 2023-06-05 16:11:02.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/sorting.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/fullask_rest_framework/service/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-03-12 12:54:11.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/service/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/fullask_rest_framework/utils/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-04-09 07:43:13.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/utils/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      572 2023-04-14 13:52:15.000000 fullask-rest-framework-0.1.3/fullask_rest_framework/utils/jwt.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.878319 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     5399 2023-06-12 13:26:43.000000 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     3189 2023-06-12 13:26:43.000000 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-12 13:26:43.000000 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       68 2023-06-12 13:26:43.000000 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/entry_points.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        1 2023-06-12 13:26:43.000000 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/not-zip-safe
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      153 2023-06-12 13:26:43.000000 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/requires.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)       23 2023-06-12 13:26:43.000000 fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/top_level.txt
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      846 2023-06-05 15:57:14.000000 fullask-rest-framework-0.1.3/pyproject.toml
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)      394 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/setup.cfg
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)     1654 2023-06-12 13:26:07.000000 fullask-rest-framework-0.1.3/setup.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/tests/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:34:17.000000 fullask-rest-framework-0.1.3/tests/__init__.py
+drwxrwxr-x   0 goddessana  (1000) goddessana  (1000)        0 2023-06-12 13:26:43.890324 fullask-rest-framework-0.1.3/tests/repositories/
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)        0 2023-05-08 08:35:54.000000 fullask-rest-framework-0.1.3/tests/repositories/__init__.py
+-rw-rw-r--   0 goddessana  (1000) goddessana  (1000)    20125 2023-06-05 16:00:28.000000 fullask-rest-framework-0.1.3/tests/repositories/test_sqlalchemy_repository.py
```

### Comparing `fullask-rest-framework-0.1.2/LICENSE` & `fullask-rest-framework-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/PKG-INFO` & `fullask-rest-framework-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fully-supported flask extension to build REST API.
 Home-page: https://github.com/tgoddessana/fullask-rest-framework
 Author: tgoddessana
 Author-email: twicegoddessana1229@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -43,18 +43,14 @@
 <h3 align="center">Fullask-REST-Framework</h3>
 
   <p align="center">
     A fully-supported flask extension to build REST API.
     <br />
     <a href="https://tgoddessana.github.io/fullask-rest-framework/"><strong>Explore the docs »</strong></a>
     <br />
-    <br />
-    <a href="">Report Bug</a>
-    ·
-    <a href="">Request Feature</a>
   </p>
 </div>
 
 
 <!---------------------------------------------------------------------------------------------->
 
 <br/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.3 Summary: A
 fully-supported flask extension to build REST API. Home-page: https://
 github.com/tgoddessana/fullask-rest-framework Author: tgoddessana Author-email:
 twicegoddessana1229@gmail.com License: MIT license Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -14,16 +14,14 @@
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                        >
                        **** Fullask-REST-Framework ****
              A fully-supported flask extension to build REST API.
                              Explore_the_docs_Â»
 
-                         Report Bug Â· Request Feature
-
 ## About Fullask-REST-Framework --- Fullask REST Framework is a framework that
 makes it easier and faster to build REST APIs.
                                                                   (back_to_top)
 ### Built With ![Flask][Flask] ![Python][Python]
                                                                   (back_to_top)
 
 ## Requirements --- - python 3.8+ - flask 2.0 +
```

### Comparing `fullask-rest-framework-0.1.2/README.md` & `fullask-rest-framework-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,14 @@
 <h3 align="center">Fullask-REST-Framework</h3>
 
   <p align="center">
     A fully-supported flask extension to build REST API.
     <br />
     <a href="https://tgoddessana.github.io/fullask-rest-framework/"><strong>Explore the docs »</strong></a>
     <br />
-    <br />
-    <a href="">Report Bug</a>
-    ·
-    <a href="">Request Feature</a>
   </p>
 </div>
 
 
 <!---------------------------------------------------------------------------------------------->
 
 <br/>
```

#### html2text {}

```diff
@@ -3,16 +3,14 @@
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                        >
                        **** Fullask-REST-Framework ****
              A fully-supported flask extension to build REST API.
                              Explore_the_docs_Â»
 
-                         Report Bug Â· Request Feature
-
 ## About Fullask-REST-Framework --- Fullask REST Framework is a framework that
 makes it easier and faster to build REST APIs.
                                                                   (back_to_top)
 ### Built With ![Flask][Flask] ![Python][Python]
                                                                   (back_to_top)
 
 ## Requirements --- - python 3.8+ - flask 2.0 +
```

### Comparing `fullask-rest-framework-0.1.2/docs/Makefile` & `fullask-rest-framework-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/docs/docfiles/conf.py` & `fullask-rest-framework-0.1.3/docs/docfiles/conf.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/docs/docfiles/contributing.rst` & `fullask-rest-framework-0.1.3/docs/docfiles/contributing.rst`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/docs/docfiles/installation.rst` & `fullask-rest-framework-0.1.3/docs/docfiles/installation.rst`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/docs/make.bat` & `fullask-rest-framework-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/cli.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/cli.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/login_form.html` & `fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css` & `fullask-rest-framework-0.1.3/fullask_rest_framework/contrib/admin/templates/static/loigin_form.css`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/createproject_template/project_template/factory.txt` & `fullask-rest-framework-0.1.3/fullask_rest_framework/createproject_template/project_template/factory.txt`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/factory/app_factory.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/factory/app_factory.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/factory/extensions.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/factory/extensions.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/orm/sqlalchemy/mixins.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/orm/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/crud.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/crud.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/repositories/sqlalchemy.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/repositories/sqlalchemy.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,19 +200,22 @@
             if field_name != "id":
                 setattr(model_instance, field_name, field_value)
 
 
 def read_by_fields(func):
     @wraps(func)
     def wrapper(self, *args, **kwargs):
-        columns = inspect(self.sqlalchemy_model).columns
-        for column in columns:
-            print(column, column.unique)
         field_name = func.__name__[len("read_by_") :]
+        if field_name in kwargs:
+            field_value = kwargs[field_name]
+        else:
+            if len(args) < 1:
+                raise ValueError(f"{field_name} argument is missing")
+            field_value = args[0]
         query_result = self.sqlalchemy_model.query.filter_by(
-            **{field_name: kwargs[field_name]}
+            **{field_name: field_value}
         ).first()
         if query_result:
             return self._sqlalchemy_model_to_entity(query_result)
         return None
 
     return wrapper
```

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/fields.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/pagination.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/schemas/sorting.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/schemas/sorting.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework/utils/jwt.py` & `fullask-rest-framework-0.1.3/fullask_rest_framework/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/PKG-INFO` & `fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullask-rest-framework
-Version: 0.1.2
+Version: 0.1.3
 Summary: A fully-supported flask extension to build REST API.
 Home-page: https://github.com/tgoddessana/fullask-rest-framework
 Author: tgoddessana
 Author-email: twicegoddessana1229@gmail.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -43,18 +43,14 @@
 <h3 align="center">Fullask-REST-Framework</h3>
 
   <p align="center">
     A fully-supported flask extension to build REST API.
     <br />
     <a href="https://tgoddessana.github.io/fullask-rest-framework/"><strong>Explore the docs »</strong></a>
     <br />
-    <br />
-    <a href="">Report Bug</a>
-    ·
-    <a href="">Request Feature</a>
   </p>
 </div>
 
 
 <!---------------------------------------------------------------------------------------------->
 
 <br/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: fullask-rest-framework Version: 0.1.3 Summary: A
 fully-supported flask extension to build REST API. Home-page: https://
 github.com/tgoddessana/fullask-rest-framework Author: tgoddessana Author-email:
 twicegoddessana1229@gmail.com License: MIT license Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -14,16 +14,14 @@
       shield]][issues-url] [![MIT License][license-shield]][license-url]
 
                                        >
                        **** Fullask-REST-Framework ****
              A fully-supported flask extension to build REST API.
                              Explore_the_docs_Â»
 
-                         Report Bug Â· Request Feature
-
 ## About Fullask-REST-Framework --- Fullask REST Framework is a framework that
 makes it easier and faster to build REST APIs.
                                                                   (back_to_top)
 ### Built With ![Flask][Flask] ![Python][Python]
                                                                   (back_to_top)
 
 ## Requirements --- - python 3.8+ - flask 2.0 +
```

### Comparing `fullask-rest-framework-0.1.2/fullask_rest_framework.egg-info/SOURCES.txt` & `fullask-rest-framework-0.1.3/fullask_rest_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/pyproject.toml` & `fullask-rest-framework-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fullask-rest-framework-0.1.2/setup.py` & `fullask-rest-framework-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     name="fullask-rest-framework",
     packages=find_packages(
         include=["fullask_rest_framework", "fullask_rest_framework.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/tgoddessana/fullask-rest-framework",
-    version="0.1.2",
+    version="0.1.3",
     zip_safe=False,
 )
```

### Comparing `fullask-rest-framework-0.1.2/tests/repositories/test_sqlalchemy_repository.py` & `fullask-rest-framework-0.1.3/tests/repositories/test_sqlalchemy_repository.py`

 * *Files identical despite different names*

