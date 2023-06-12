# Comparing `tmp/irails-1.3.42.tar.gz` & `tmp/irails-1.3.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.42.tar", last modified: Sun Jun 11 06:40:15 2023, max compression
+gzip compressed data, was "irails-1.3.43.tar", last modified: Mon Jun 12 06:25:16 2023, max compression
```

## Comparing `irails-1.3.42.tar` & `irails-1.3.43.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.760856 irails-1.3.42/
--rw-rw-rw-   0        0        0      116 2023-06-11 06:38:55.000000 irails-1.3.42/MANIFEST.in
--rw-rw-rw-   0        0        0     4956 2023-06-11 06:40:15.759860 irails-1.3.42/PKG-INFO
--rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.42/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.650360 irails-1.3.42/irails/
--rw-rw-rw-   0        0        0      327 2023-06-11 06:39:57.000000 irails-1.3.42/irails/__init__.py
--rw-rw-rw-   0        0        0     7048 2023-06-07 13:53:06.000000 irails-1.3.42/irails/_i18n.py
--rw-rw-rw-   0        0        0     7858 2023-06-11 06:29:40.000000 irails-1.3.42/irails/_loader.py
--rw-rw-rw-   0        0        0     8782 2023-06-10 07:10:22.000000 irails-1.3.42/irails/_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.664322 irails-1.3.42/irails/apps/
--rw-rw-rw-   0        0        0      133 2023-06-09 17:09:11.000000 irails-1.3.42/irails/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.666317 irails-1.3.42/irails/apps/__pycache__/
--rw-rw-rw-   0        0        0      379 2023-06-09 17:10:37.000000 irails-1.3.42/irails/apps/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    15361 2023-06-07 11:59:43.000000 irails-1.3.42/irails/auth.py
--rw-rw-rw-   0        0        0    13740 2023-06-09 06:23:19.000000 irails-1.3.42/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.668319 irails-1.3.42/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.671304 irails-1.3.42/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9337 2023-05-31 14:37:50.000000 irails-1.3.42/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.42/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10665 2023-05-31 14:37:46.000000 irails-1.3.42/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.42/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.42/irails/config.py
--rw-rw-rw-   0        0        0    13255 2023-06-11 03:00:37.000000 irails-1.3.42/irails/controller_utils.py
--rw-rw-rw-   0        0        0    27768 2023-06-10 15:00:29.000000 irails-1.3.42/irails/core.py
--rw-rw-rw-   0        0        0    22094 2023-06-10 08:28:27.000000 irails-1.3.42/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.42/irails/log.py
--rw-rw-rw-   0        0        0     9351 2023-06-10 14:44:56.000000 irails-1.3.42/irails/midware.py
--rw-rw-rw-   0        0        0     9175 2023-06-01 06:44:57.000000 irails-1.3.42/irails/midware_session.py
--rw-rw-rw-   0        0        0     4336 2023-06-01 06:22:43.000000 irails-1.3.42/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.687537 irails-1.3.42/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.42/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7278 2023-06-10 07:10:17.000000 irails-1.3.42/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7095 2023-06-09 07:51:49.000000 irails-1.3.42/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.42/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1336 2023-06-09 05:34:08.000000 irails-1.3.42/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     4080 2023-06-09 08:02:27.000000 irails-1.3.42/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.42/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.42/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.42/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     5765 2023-06-09 05:34:08.000000 irails-1.3.42/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.42/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.610474 irails-1.3.42/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.703750 irails-1.3.42/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.42/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.42/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.42/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.42/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0      179 2023-06-09 07:16:16.000000 irails-1.3.42/irails/scripts/tpls/app/manifest.jinja
--rw-rw-rw-   0        0        0      999 2023-06-09 05:47:40.000000 irails-1.3.42/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.42/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.42/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.42/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.42/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.706741 irails-1.3.42/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.42/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.708745 irails-1.3.42/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.42/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.719706 irails-1.3.42/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.42/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      323 2023-05-30 07:17:46.000000 irails-1.3.42/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.42/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.735888 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.42/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.42/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.42/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.42/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.42/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.614456 irails-1.3.42/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.738883 irails-1.3.42/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.42/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.42/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.42/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.42/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.744866 irails-1.3.42/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.42/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.42/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.747886 irails-1.3.42/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.618445 irails-1.3.42/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.750882 irails-1.3.42/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.42/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.753874 irails-1.3.42/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.42/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.42/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.42/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.619442 irails-1.3.42/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.755867 irails-1.3.42/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.42/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1048 2023-05-30 07:13:21.000000 irails-1.3.42/irails/scripts/tpls/project/public/vue_home.html
--rw-rw-rw-   0        0        0     1733 2023-06-09 05:34:08.000000 irails-1.3.42/irails/unit_test.py
--rw-rw-rw-   0        0        0     3053 2023-05-30 07:10:08.000000 irails-1.3.42/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-06-11 06:40:15.661330 irails-1.3.42/irails.egg-info/
--rw-rw-rw-   0        0        0     4956 2023-06-11 06:40:15.000000 irails-1.3.42/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3321 2023-06-11 06:40:15.000000 irails-1.3.42/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 06:40:15.000000 irails-1.3.42/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-11 06:40:15.000000 irails-1.3.42/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-06-11 06:40:15.000000 irails-1.3.42/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 06:40:15.000000 irails-1.3.42/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 06:40:15.760856 irails-1.3.42/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.478099 irails-1.3.43/
+-rw-rw-rw-   0        0        0      116 2023-06-11 06:38:55.000000 irails-1.3.43/MANIFEST.in
+-rw-rw-rw-   0        0        0     4956 2023-06-12 06:25:16.477103 irails-1.3.43/PKG-INFO
+-rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.43/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.324404 irails-1.3.43/irails/
+-rw-rw-rw-   0        0        0      327 2023-06-12 06:25:07.000000 irails-1.3.43/irails/__init__.py
+-rw-rw-rw-   0        0        0     7048 2023-06-07 13:53:06.000000 irails-1.3.43/irails/_i18n.py
+-rw-rw-rw-   0        0        0     7865 2023-06-12 06:24:42.000000 irails-1.3.43/irails/_loader.py
+-rw-rw-rw-   0        0        0     8782 2023-06-10 07:10:22.000000 irails-1.3.43/irails/_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.335374 irails-1.3.43/irails/apps/
+-rw-rw-rw-   0        0        0      133 2023-06-09 17:09:11.000000 irails-1.3.43/irails/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.336372 irails-1.3.43/irails/apps/__pycache__/
+-rw-rw-rw-   0        0        0      379 2023-06-09 17:10:37.000000 irails-1.3.43/irails/apps/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15361 2023-06-07 11:59:43.000000 irails-1.3.43/irails/auth.py
+-rw-rw-rw-   0        0        0    13740 2023-06-09 06:23:19.000000 irails-1.3.43/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.338368 irails-1.3.43/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.340361 irails-1.3.43/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9337 2023-05-31 14:37:50.000000 irails-1.3.43/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.43/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10665 2023-05-31 14:37:46.000000 irails-1.3.43/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.43/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.43/irails/config.py
+-rw-rw-rw-   0        0        0    13255 2023-06-11 03:00:37.000000 irails-1.3.43/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    27768 2023-06-10 15:00:29.000000 irails-1.3.43/irails/core.py
+-rw-rw-rw-   0        0        0    22094 2023-06-10 08:28:27.000000 irails-1.3.43/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.43/irails/log.py
+-rw-rw-rw-   0        0        0     9351 2023-06-10 14:44:56.000000 irails-1.3.43/irails/midware.py
+-rw-rw-rw-   0        0        0     9175 2023-06-01 06:44:57.000000 irails-1.3.43/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4336 2023-06-01 06:22:43.000000 irails-1.3.43/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.357321 irails-1.3.43/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.43/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7278 2023-06-10 07:10:17.000000 irails-1.3.43/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7095 2023-06-09 07:51:49.000000 irails-1.3.43/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.43/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1336 2023-06-09 05:34:08.000000 irails-1.3.43/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     4080 2023-06-09 08:02:27.000000 irails-1.3.43/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.43/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.43/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.43/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     5765 2023-06-09 05:34:08.000000 irails-1.3.43/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.43/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.289138 irails-1.3.43/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.376429 irails-1.3.43/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.43/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.43/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.43/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.43/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0      179 2023-06-09 07:16:16.000000 irails-1.3.43/irails/scripts/tpls/app/manifest.jinja
+-rw-rw-rw-   0        0        0      999 2023-06-09 05:47:40.000000 irails-1.3.43/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.43/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.43/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.43/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.43/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.378404 irails-1.3.43/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.43/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.380399 irails-1.3.43/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.43/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.394151 irails-1.3.43/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.43/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      323 2023-05-30 07:17:46.000000 irails-1.3.43/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.43/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.409097 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.43/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.43/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.43/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.43/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.43/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.293674 irails-1.3.43/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.431038 irails-1.3.43/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.43/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.43/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.43/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.43/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.446998 irails-1.3.43/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.43/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.43/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.452980 irails-1.3.43/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.296666 irails-1.3.43/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.459963 irails-1.3.43/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.43/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.468951 irails-1.3.43/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.43/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.43/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.43/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.297664 irails-1.3.43/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.471930 irails-1.3.43/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.43/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1048 2023-05-30 07:13:21.000000 irails-1.3.43/irails/scripts/tpls/project/public/vue_home.html
+-rw-rw-rw-   0        0        0     1733 2023-06-09 05:34:08.000000 irails-1.3.43/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3053 2023-05-30 07:10:08.000000 irails-1.3.43/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-06-12 06:25:16.331385 irails-1.3.43/irails.egg-info/
+-rw-rw-rw-   0        0        0     4956 2023-06-12 06:25:15.000000 irails-1.3.43/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3321 2023-06-12 06:25:16.000000 irails-1.3.43/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 06:25:15.000000 irails-1.3.43/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-12 06:25:15.000000 irails-1.3.43/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-06-12 06:25:15.000000 irails-1.3.43/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 06:25:15.000000 irails-1.3.43/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 06:25:16.478099 irails-1.3.43/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.43/setup.py
```

### Comparing `irails-1.3.42/PKG-INFO` & `irails-1.3.43/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.42
+Version: 1.3.43
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.42/README.md` & `irails-1.3.43/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/_i18n.py` & `irails-1.3.43/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/_loader.py` & `irails-1.3.43/irails/_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,16 +174,17 @@
 
 def collect_apps(debug=False, do_load: bool = True, application: object = None):
     global app_dirs, app_enabled
     app_cfg = config.get('app')
     if app_cfg:
         app_dirs = app_cfg.get("appdir")
         app_enabled = app_cfg.get("enabled")
-    if not app_cfg or not app_dir:
+    if not app_cfg or not app_dirs:
         raise RuntimeError(_("Config error,app configs is empty."))
+    
     load_failed = 0
     loaded = 0
     apps = []
     for app_dir in app_dirs:
         abs_app_dir = os.path.abspath(os.path.join(ROOT_PATH, app_dir))
 
         app_list = __list_directories(abs_app_dir)
```

### Comparing `irails-1.3.42/irails/_utils.py` & `irails-1.3.43/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/auth.py` & `irails-1.3.43/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/base_controller.py` & `irails-1.3.43/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.43/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.43/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.43/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/cbv.py` & `irails-1.3.43/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/config.py` & `irails-1.3.43/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/controller_utils.py` & `irails-1.3.43/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/core.py` & `irails-1.3.43/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/database.py` & `irails-1.3.43/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/log.py` & `irails-1.3.43/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/midware.py` & `irails-1.3.43/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/midware_session.py` & `irails-1.3.43/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/mvc_router.py` & `irails-1.3.43/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_app.py` & `irails-1.3.43/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_controller.py` & `irails-1.3.43/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_i18n.py` & `irails-1.3.43/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_migrate.py` & `irails-1.3.43/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_model.py` & `irails-1.3.43/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_project.py` & `irails-1.3.43/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_run.py` & `irails-1.3.43/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_shell.py` & `irails-1.3.43/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/_test.py` & `irails-1.3.43/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/main.py` & `irails-1.3.43/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.43/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/app/home.tpl` & `irails-1.3.43/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/app/model.jinja` & `irails-1.3.43/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.43/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.43/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.43/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.43/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.43/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.43/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.43/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.43/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.43/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.43/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.43/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.43/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/scripts/tpls/project/public/vue_home.html` & `irails-1.3.43/irails/scripts/tpls/project/public/vue_home.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/unit_test.py` & `irails-1.3.43/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails/view.py` & `irails-1.3.43/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/irails.egg-info/PKG-INFO` & `irails-1.3.43/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.42
+Version: 1.3.43
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.42/irails.egg-info/SOURCES.txt` & `irails-1.3.43/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.42/setup.py` & `irails-1.3.43/setup.py`

 * *Files identical despite different names*

