# Comparing `tmp/mayan-importer-2.3.tar.gz` & `tmp/mayan-importer-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-2.3.tar", last modified: Thu Sep  8 10:38:44 2022, max compression
+gzip compressed data, was "mayan-importer-2.3.1.tar", last modified: Mon Jun 12 09:50:00 2023, max compression
```

## Comparing `mayan-importer-2.3.tar` & `mayan-importer-2.3.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.458978 mayan-importer-2.3/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5342 2022-09-08 10:38:27.000000 mayan-importer-2.3/HISTORY.rst
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)      555 2020-09-02 03:45:36.000000 mayan-importer-2.3/LICENSE
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)       39 2020-09-02 04:35:02.000000 mayan-importer-2.3/MANIFEST.in
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8203 2022-09-08 10:38:44.458978 mayan-importer-2.3/PKG-INFO
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-09-07 08:54:25.000000 mayan-importer-2.3/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.450978 mayan-importer-2.3/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2021-06-03 17:33:12.000000 mayan-importer-2.3/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      835 2020-12-27 06:14:34.000000 mayan-importer-2.3/importer/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4601 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8631 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    10581 2022-08-18 10:12:10.000000 mayan-importer-2.3/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      237 2020-09-09 05:26:05.000000 mayan-importer-2.3/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1563 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      214 2020-10-03 09:07:14.000000 mayan-importer-2.3/importer/exceptions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4029 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1973 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4374 2020-10-04 09:43:02.000000 mayan-importer-2.3/importer/import_setup_actions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7696 2021-06-03 17:38:13.000000 mayan-importer-2.3/importer/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6328 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      737 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.454978 mayan-importer-2.3/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-09-07 09:03:59.000000 mayan-importer-2.3/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-09-08 09:18:53.000000 mayan-importer-2.3/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-09-08 09:18:53.000000 mayan-importer-2.3/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2020-10-05 06:33:47.000000 mayan-importer-2.3/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2020-10-05 06:34:15.000000 mayan-importer-2.3/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2020-10-05 06:34:20.000000 mayan-importer-2.3/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2020-10-05 06:34:30.000000 mayan-importer-2.3/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2020-10-05 06:34:50.000000 mayan-importer-2.3/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2020-10-05 06:36:27.000000 mayan-importer-2.3/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2020-10-05 06:36:35.000000 mayan-importer-2.3/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2020-10-05 06:45:38.000000 mayan-importer-2.3/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2020-10-05 06:37:05.000000 mayan-importer-2.3/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2020-12-27 06:14:34.000000 mayan-importer-2.3/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2020-12-27 06:14:34.000000 mayan-importer-2.3/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-09-02 06:51:06.000000 mayan-importer-2.3/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.454978 mayan-importer-2.3/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      141 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2304 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/models/import_setup_action_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6288 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8572 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1957 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/models/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1114 2020-09-30 09:46:34.000000 mayan-importer-2.3/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1141 2021-06-17 07:00:01.000000 mayan-importer-2.3/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3460 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2295 2022-08-19 09:23:52.000000 mayan-importer-2.3/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.454978 mayan-importer-2.3/importer/templatetags/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-03 09:18:21.000000 mayan-importer-2.3/importer/templatetags/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2966 2020-10-03 09:18:46.000000 mayan-importer-2.3/importer/templatetags/templating_tags.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.458978 mayan-importer-2.3/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       64 2020-10-04 09:30:25.000000 mayan-importer-2.3/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      270 2020-10-03 09:07:14.000000 mayan-importer-2.3/importer/tests/import_setup_actions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1553 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      643 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11061 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/tests/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7199 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/tests/test_import_setup_action_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7870 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12228 2022-09-08 10:38:27.000000 mayan-importer-2.3/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6415 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6686 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.458978 mayan-importer-2.3/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6634 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/views/import_setup_action_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    15441 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5598 2022-09-01 09:34:36.000000 mayan-importer-2.3/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2022-09-08 10:38:44.458978 mayan-importer-2.3/mayan_importer.egg-info/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8203 2022-09-08 10:38:44.000000 mayan-importer-2.3/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2268 2022-09-08 10:38:44.000000 mayan-importer-2.3/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2022-09-08 10:38:44.000000 mayan-importer-2.3/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2022-09-08 10:38:44.000000 mayan-importer-2.3/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2022-09-08 10:38:44.000000 mayan-importer-2.3/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2022-09-08 10:38:44.000000 mayan-importer-2.3/mayan_importer.egg-info/top_level.txt
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)      129 2022-09-08 10:38:44.458978 mayan-importer-2.3/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3066 2022-09-08 10:38:27.000000 mayan-importer-2.3/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.948027 mayan-importer-2.3.1/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5463 2023-06-12 09:49:02.000000 mayan-importer-2.3.1/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/MANIFEST.in
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8326 2023-06-12 09:50:00.948027 mayan-importer-2.3.1/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.940027 mayan-importer-2.3.1/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      835 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4601 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8631 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    10581 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      237 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/importer/dependencies.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1563 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      214 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/exceptions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4029 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1973 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4374 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/import_setup_actions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7696 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6328 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      737 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.944027 mayan-importer-2.3.1/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.944027 mayan-importer-2.3.1/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      141 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2400 2023-06-12 09:35:45.000000 mayan-importer-2.3.1/importer/models/import_setup_action_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6433 2023-06-12 09:36:14.000000 mayan-importer-2.3.1/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8668 2023-06-12 09:37:55.000000 mayan-importer-2.3.1/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1957 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/models/mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1114 2020-10-02 10:42:37.000000 mayan-importer-2.3.1/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1141 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3460 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2295 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.944027 mayan-importer-2.3.1/importer/templatetags/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/templatetags/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2966 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/templatetags/templating_tags.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.944027 mayan-importer-2.3.1/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       64 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      270 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/import_setup_actions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1553 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      643 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11061 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7199 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/test_import_setup_action_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7870 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12228 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6415 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6686 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.948027 mayan-importer-2.3.1/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6634 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/views/import_setup_action_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    15441 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5598 2023-04-12 05:57:59.000000 mayan-importer-2.3.1/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2023-06-12 09:50:00.948027 mayan-importer-2.3.1/mayan_importer.egg-info/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8326 2023-06-12 09:50:00.000000 mayan-importer-2.3.1/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2268 2023-06-12 09:50:00.000000 mayan-importer-2.3.1/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2023-06-12 09:50:00.000000 mayan-importer-2.3.1/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2023-06-12 09:50:00.000000 mayan-importer-2.3.1/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       41 2023-06-12 09:50:00.000000 mayan-importer-2.3.1/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2023-06-12 09:50:00.000000 mayan-importer-2.3.1/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2023-06-12 09:50:00.948027 mayan-importer-2.3.1/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3070 2023-06-12 09:34:39.000000 mayan-importer-2.3.1/setup.py
```

### Comparing `mayan-importer-2.3/HISTORY.rst` & `mayan-importer-2.3.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.3.1 (2023-06-12)
+==================
+- Require credentials version 1.4.1.
+- Support new event manager module location.
+
 2.3 (2022-09-08)
 ================
 - Split models module.
 - Support item time buffer.
 
 2.2 (2022-09-03)
 ================
```

### Comparing `mayan-importer-2.3/LICENSE` & `mayan-importer-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/PKG-INFO` & `mayan-importer-2.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 2.3
+Version: 2.3.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -92,14 +92,19 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+2.3.1 (2023-06-12)
+==================
+- Require credentials version 1.4.1.
+- Support new event manager module location.
+
 2.3 (2022-09-08)
 ================
 - Split models module.
 - Support item time buffer.
 
 2.2 (2022-09-03)
 ================
```

### Comparing `mayan-importer-2.3/README.rst` & `mayan-importer-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/admin.py` & `mayan-importer-2.3.1/importer/admin.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/api_views.py` & `mayan-importer-2.3.1/importer/api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/apps.py` & `mayan-importer-2.3.1/importer/apps.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/classes.py` & `mayan-importer-2.3.1/importer/classes.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/events.py` & `mayan-importer-2.3.1/importer/events.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/forms.py` & `mayan-importer-2.3.1/importer/forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/icons.py` & `mayan-importer-2.3.1/importer/icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/import_setup_actions.py` & `mayan-importer-2.3.1/importer/import_setup_actions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/importers.py` & `mayan-importer-2.3.1/importer/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/links.py` & `mayan-importer-2.3.1/importer/links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/literals.py` & `mayan-importer-2.3.1/importer/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0001_initial.py` & `mayan-importer-2.3.1/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-2.3.1/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-2.3.1/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-2.3.1/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0005_importsetup_state.py` & `mayan-importer-2.3.1/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-2.3.1/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0009_importsetupaction.py` & `mayan-importer-2.3.1/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-2.3.1/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-2.3.1/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-2.3.1/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-2.3.1/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-2.3.1/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/models/import_setup_action_models.py` & `mayan-importer-2.3.1/importer/models/import_setup_action_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from django.db import models
 from django.db.models import Max
 from django.utils.translation import ugettext_lazy as _
 
-from mayan.apps.events.classes import EventManagerSave
+try:
+    from mayan.apps.events.classes import EventManagerSave
+except ImportError:
+    from mayan.apps.events.event_managers import EventManagerSave
+
 from mayan.apps.events.decorators import method_event
 
 from ..events import event_import_setup_edited
 
 from .import_setup_models import ImportSetup
 from .mixins import BackendModelMixin
```

### Comparing `mayan-importer-2.3/importer/models/import_setup_item_models.py` & `mayan-importer-2.3.1/importer/models/import_setup_item_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,23 @@
 from django.db import models
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.documents.models.document_models import Document
 from mayan.apps.documents.tasks import task_document_file_upload
-from mayan.apps.events.classes import (
-    EventManagerMethodAfter, EventManagerSave
-)
+try:
+    from mayan.apps.events.classes import (
+        EventManagerMethodAfter, EventManagerSave
+    )
+except ImportError:
+    from mayan.apps.events.event_managers import (
+        EventManagerMethodAfter, EventManagerSave
+    )
+
 from mayan.apps.events.decorators import method_event
 
 from ..events import (
     event_import_setup_item_completed, event_import_setup_item_created,
     event_import_setup_item_deleted, event_import_setup_item_edited
 )
 from ..literals import (
```

### Comparing `mayan-importer-2.3/importer/models/import_setup_models.py` & `mayan-importer-2.3.1/importer/models/import_setup_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from django.conf import settings
 from django.contrib.humanize.templatetags.humanize import intcomma
 from django.db import models
 from django.urls import reverse
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.documents.models.document_type_models import DocumentType
-from mayan.apps.events.classes import EventManagerSave
+try:
+    from mayan.apps.events.classes import EventManagerSave
+except ImportError:
+    from mayan.apps.events.event_managers import EventManagerSave
+
 from mayan.apps.events.decorators import method_event
 
 from credentials.models import StoredCredential
 
 from ..events import (
     event_import_setup_created, event_import_setup_edited,
     event_import_setup_populate_ended, event_import_setup_populate_started,
```

### Comparing `mayan-importer-2.3/importer/models/mixins.py` & `mayan-importer-2.3.1/importer/models/mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/permissions.py` & `mayan-importer-2.3.1/importer/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/queues.py` & `mayan-importer-2.3.1/importer/queues.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/serializers.py` & `mayan-importer-2.3.1/importer/serializers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tasks.py` & `mayan-importer-2.3.1/importer/tasks.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/templatetags/templating_tags.py` & `mayan-importer-2.3.1/importer/templatetags/templating_tags.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/importers.py` & `mayan-importer-2.3.1/importer/tests/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/literals.py` & `mayan-importer-2.3.1/importer/tests/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/mixins.py` & `mayan-importer-2.3.1/importer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/test_import_setup_action_views.py` & `mayan-importer-2.3.1/importer/tests/test_import_setup_action_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/test_import_setup_api.py` & `mayan-importer-2.3.1/importer/tests/test_import_setup_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/test_import_setup_item_api.py` & `mayan-importer-2.3.1/importer/tests/test_import_setup_item_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/test_import_setup_item_views.py` & `mayan-importer-2.3.1/importer/tests/test_import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/tests/test_import_setup_views.py` & `mayan-importer-2.3.1/importer/tests/test_import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/urls.py` & `mayan-importer-2.3.1/importer/urls.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/views/import_setup_action_views.py` & `mayan-importer-2.3.1/importer/views/import_setup_action_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/views/import_setup_item_views.py` & `mayan-importer-2.3.1/importer/views/import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/importer/views/import_setup_views.py` & `mayan-importer-2.3.1/importer/views/import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-2.3.1/mayan_importer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 2.3
+Version: 2.3.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -92,14 +92,19 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+2.3.1 (2023-06-12)
+==================
+- Require credentials version 1.4.1.
+- Support new event manager module location.
+
 2.3 (2022-09-08)
 ================
 - Split models module.
 - Support item time buffer.
 
 2.2 (2022-09-03)
 ================
```

### Comparing `mayan-importer-2.3/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-2.3.1/mayan_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.3/setup.py` & `mayan-importer-2.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 )
 
     return packages
 
 
 install_requires = (
     'dropbox==10.4.1',
-    'mayan-credentials==1.4',
+    'mayan-credentials==1.4.1',
 )
 
 with open('README.rst') as f:
     readme = f.read()
 with open('HISTORY.rst') as f:
     history = f.read()
 
@@ -95,10 +95,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/importer',
-    version='2.3',
+    version='2.3.1',
     zip_safe=False,
 )
```

