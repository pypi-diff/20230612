# Comparing `tmp/anycluster-2.3.0.tar.gz` & `tmp/anycluster-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.3.0.tar", last modified: Wed Jun  7 08:30:01 2023, max compression
+gzip compressed data, was "anycluster-2.3.1.tar", last modified: Mon Jun 12 05:58:22 2023, max compression
```

## Comparing `anycluster-2.3.0.tar` & `anycluster-2.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-07 08:30:01.943661 anycluster-2.3.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.935661 anycluster-2.3.0/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.0/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-26 12:34:24.000000 anycluster-2.3.0/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    37213 2023-06-06 12:31:46.000000 anycluster-2.3.0/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.0/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.0/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3918 2023-06-06 10:47:45.000000 anycluster-2.3.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.0/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     7868 2023-06-07 08:23:18.000000 anycluster-2.3.0/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.0/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3670 2023-06-06 10:10:33.000000 anycluster-2.3.0/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.3.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.3.0/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.0/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.0/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9915 2023-06-07 08:21:53.000000 anycluster-2.3.0/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.0/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.0/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.935661 anycluster-2.3.0/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.935661 anycluster-2.3.0/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.0/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.943661 anycluster-2.3.0/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.0/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    14813 2023-05-26 08:50:17.000000 anycluster-2.3.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.0/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.0/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.0/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.0/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    25353 2023-05-26 08:50:15.000000 anycluster-2.3.0/anycluster/tests/test_MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.0/anycluster/utils.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-07 08:30:01.939661 anycluster-2.3.0/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-07 08:30:01.000000 anycluster-2.3.0/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-07 08:30:01.943661 anycluster-2.3.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-07 08:12:27.000000 anycluster-2.3.0/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.3.1/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.3.1/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-12 05:58:22.963686 anycluster-2.3.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.3.1/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.3.1/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-26 12:34:24.000000 anycluster-2.3.1/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    37218 2023-06-07 12:40:46.000000 anycluster-2.3.1/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.3.1/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.3.1/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.3.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.3.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3918 2023-06-06 10:47:45.000000 anycluster-2.3.1/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1192 2023-05-26 08:42:05.000000 anycluster-2.3.1/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     7902 2023-06-07 12:40:00.000000 anycluster-2.3.1/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.3.1/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3670 2023-06-06 10:10:33.000000 anycluster-2.3.1/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.3.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.3.1/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10045 2023-06-07 08:21:32.000000 anycluster-2.3.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.3.1/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14763 2023-06-07 08:21:29.000000 anycluster-2.3.1/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1165 2023-05-26 08:37:19.000000 anycluster-2.3.1/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9915 2023-06-12 05:58:07.000000 anycluster-2.3.1/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.3.1/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.3.1/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.3.1/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.963686 anycluster-2.3.1/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.3.1/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2865 2023-05-26 05:42:40.000000 anycluster-2.3.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    14813 2023-05-26 08:50:17.000000 anycluster-2.3.1/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.3.1/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2230 2023-05-26 05:42:38.000000 anycluster-2.3.1/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.3.1/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.3.1/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    25353 2023-05-26 08:50:15.000000 anycluster-2.3.1/anycluster/tests/test_MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2023-06-06 12:24:50.000000 anycluster-2.3.1/anycluster/utils.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-06-12 05:58:22.959685 anycluster-2.3.1/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2211 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-06-12 05:58:22.000000 anycluster-2.3.1/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-06-12 05:58:22.963686 anycluster-2.3.1/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-06-12 05:56:19.000000 anycluster-2.3.1/setup.py
```

### Comparing `anycluster-2.3.0/LICENSE` & `anycluster-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/PKG-INFO` & `anycluster-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.0
+Version: 2.3.1
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.0/README.md` & `anycluster-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/ClusterCache.py` & `anycluster-2.3.1/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/FilterComposer.py` & `anycluster-2.3.1/anycluster/FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/MapClusterer.py` & `anycluster-2.3.1/anycluster/MapClusterer.py`

 * *Files 0% similar despite different names*

```diff
@@ -865,15 +865,15 @@
 
         cursor = connections['default'].cursor()
         cursor.execute(grouped_count_sql)
         results = cursor.fetchall()
         
         for result in results:
             count = result[0]
-            group_name = result[1]
+            group_name = str(result[1])
 
             if group_name not in groups:
                 groups[group_name] = {
                     'count' : count,
                 }
 
             else:
```

### Comparing `anycluster-2.3.0/anycluster/MapTools.py` & `anycluster-2.3.1/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/__pycache__/serializers.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/__pycache__/serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/__pycache__/views.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/__pycache__/views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jun  7 08:21:53 2023 UTC, .py size: 9915 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 213e 8064 bb26 0000  U.......!>.d.&..
+00000000: 550d 0d0a 0000 0000 9a7a 8064 d626 0000  U........z.d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 6001 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -42,451 +42,453 @@
 00000290: 4d61 7043 6f6e 7465 6e74 436f 756e 7453  MapContentCountS
 000002a0: 6572 6961 6c69 7a65 72da 1b47 726f 7570  erializer..Group
 000002b0: 6564 4d61 7043 6f6e 7465 6e74 5365 7269  edMapContentSeri
 000002c0: 616c 697a 6572 da1c 4172 6561 436f 6e74  alizer..AreaCont
 000002d0: 656e 7452 6571 7565 7374 5365 7269 616c  entRequestSerial
 000002e0: 697a 6572 2901 da0c 436c 7573 7465 7243  izer)...ClusterC
 000002f0: 6163 6865 2901 da0d 696d 706f 7274 5f6d  ache)...import_m
-00000300: 6f64 756c 655a 1f41 4e59 434c 5553 5445  oduleZ.ANYCLUSTE
+00000300: 6f64 756c 65da 1f41 4e59 434c 5553 5445  odule..ANYCLUSTE
 00000310: 525f 4749 535f 4d4f 4445 4c5f 5345 5249  R_GIS_MODEL_SERI
 00000320: 414c 495a 4552 7a2d 616e 7963 6c75 7374  ALIZERz-anyclust
 00000330: 6572 2e61 7069 2e73 6572 6961 6c69 7a65  er.api.serialize
 00000340: 7273 2e47 6973 4d6f 6465 6c53 6572 6961  rs.GisModelSeria
 00000350: 6c69 7a65 724e 6300 0000 0000 0000 0000  lizerNc.........
 00000360: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
 00000370: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
 00000380: 8400 5a03 6403 5300 2904 da07 4150 4948  ..Z.d.S.)...APIH
 00000390: 6f6d 6563 0200 0000 0000 0000 0000 0000  omec............
 000003a0: 0400 0000 0300 0000 4f00 0000 730c 0000  ........O...s...
 000003b0: 0074 0064 0164 0269 0183 0153 0029 034e  .t.d.d.i...S.).N
 000003c0: da07 7375 6363 6573 7354 7205 0000 0029  ..successTr....)
 000003d0: 04da 0473 656c 66da 0772 6571 7565 7374  ...self..request
 000003e0: da04 6172 6773 da06 6b77 6172 6773 a900  ..args..kwargs..
-000003f0: 721e 0000 00fa 382f 686f 6d65 2f74 6f6d  r.....8/home/tom
-00000400: 2f61 6e79 636c 7573 7465 722f 6465 6d6f  /anycluster/demo
-00000410: 2f64 6a61 6e67 6f2f 616e 7963 6c75 7374  /django/anyclust
-00000420: 6572 2f61 7069 2f76 6965 7773 2e70 79da  er/api/views.py.
-00000430: 0367 6574 1900 0000 7302 0000 0000 017a  .get....s......z
-00000440: 0b41 5049 486f 6d65 2e67 6574 4ea9 04da  .APIHome.getN...
-00000450: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000460: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000470: 655f 5f72 2000 0000 721e 0000 0072 1e00  e__r ...r....r..
-00000480: 0000 721e 0000 0072 1f00 0000 7218 0000  ..r....r....r...
-00000490: 0017 0000 0073 0200 0000 0802 7218 0000  .....s......r...
-000004a0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000004b0: 0000 0200 0000 4000 0000 7340 0000 0065  ......@...s@...e
-000004c0: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
-000004d0: 005a 0464 0464 0584 005a 0564 0664 0784  .Z.d.d...Z.d.d..
-000004e0: 005a 0664 0864 0984 005a 0764 0a64 0b84  .Z.d.d...Z.d.d..
-000004f0: 005a 0864 0c64 0d84 005a 0964 0e53 0029  .Z.d.d...Z.d.S.)
-00000500: 0fda 124d 6170 436c 7573 7465 7256 6965  ...MapClusterVie
-00000510: 7742 6173 655a 1061 6e79 636c 7573 7465  wBaseZ.anycluste
-00000520: 725f 6361 6368 6563 0200 0000 0000 0000  r_cachec........
-00000530: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000540: 7316 0000 0074 007c 01a0 0164 01a1 0164  s....t.|...d...d
-00000550: 0219 0083 017d 027c 0253 0029 034e fa01  .....}.|.S.).N..
-00000560: 3ae9 ffff ffff 2902 da03 696e 74da 0573  :.....)...int..s
-00000570: 706c 6974 2903 721a 0000 005a 0873 7269  plit).r....Z.sri
-00000580: 645f 7374 72da 0b6f 7574 7075 745f 7372  d_str..output_sr
-00000590: 6964 721e 0000 0072 1e00 0000 721f 0000  idr....r....r...
-000005a0: 00da 0a70 6172 7365 5f73 7269 6421 0000  ...parse_srid!..
-000005b0: 0073 0400 0000 0001 1201 7a1d 4d61 7043  .s........z.MapC
-000005c0: 6c75 7374 6572 5669 6577 4261 7365 2e70  lusterViewBase.p
-000005d0: 6172 7365 5f73 7269 6463 0200 0000 0000  arse_sridc......
-000005e0: 0000 0000 0000 0200 0000 0100 0000 4300  ..............C.
-000005f0: 0000 7304 0000 0064 0153 0029 024e da06  ..s....d.S.).N..
-00000600: 7075 626c 6963 721e 0000 0029 0272 1a00  publicr....).r..
-00000610: 0000 721b 0000 0072 1e00 0000 721e 0000  ..r....r....r...
-00000620: 0072 1f00 0000 da0f 6765 745f 7363 6865  .r......get_sche
-00000630: 6d61 5f6e 616d 6526 0000 0073 0200 0000  ma_name&...s....
-00000640: 0001 7a22 4d61 7043 6c75 7374 6572 5669  ..z"MapClusterVi
-00000650: 6577 4261 7365 2e67 6574 5f73 6368 656d  ewBase.get_schem
-00000660: 615f 6e61 6d65 6307 0000 0000 0000 0000  a_namec.........
-00000670: 0000 000d 0000 0007 0000 004b 0000 0073  ...........K...s
-00000680: 5800 0000 7c07 6401 1900 7d08 7c07 6402  X...|.d...}.|.d.
-00000690: 1900 7d09 7c04 6403 6b02 7228 7400 7c01  ..}.|.d.k.r(t.|.
-000006a0: 7c09 7c02 7c03 8304 7d0a 6e12 7c00 a001  |.|.|...}.n.|...
-000006b0: 7c01 7c09 7c02 7c06 7c03 a105 7d0a 7c00  |.|.|.|.|...}.|.
-000006c0: a002 7c06 a101 7d0b 7403 7c0a 7c08 7c05  ..|...}.t.|.|.|.
-000006d0: 7c0b 6404 8d04 7d0c 7c0c 5300 2905 4eda  |.d...}.|.S.).N.
-000006e0: 0967 7269 645f 7369 7a65 da04 7a6f 6f6d  .grid_size..zoom
-000006f0: 5429 0372 2e00 0000 722a 0000 00da 0b73  T).r....r*.....s
-00000700: 6368 656d 615f 6e61 6d65 2904 7216 0000  chema_name).r...
-00000710: 00da 0967 6574 5f63 6163 6865 722d 0000  ...get_cacher-..
-00000720: 0072 0a00 0000 290d 721a 0000 00da 0d67  .r....).r......g
-00000730: 656f 6d65 7472 795f 7479 7065 da0b 636c  eometry_type..cl
-00000740: 7573 7465 7274 7970 65da 0766 696c 7465  ustertype..filte
-00000750: 7273 da0b 636c 6561 725f 6361 6368 6572  rs..clear_cacher
-00000760: 2a00 0000 721b 0000 0072 1d00 0000 722e  *...r....r....r.
-00000770: 0000 0072 2f00 0000 da0d 636c 7573 7465  ...r/.....cluste
-00000780: 725f 6361 6368 6572 3000 0000 5a09 636c  r_cacher0...Z.cl
-00000790: 7573 7465 7265 7272 1e00 0000 721e 0000  ustererr....r...
-000007a0: 0072 1f00 0000 da11 6765 745f 6d61 705f  .r......get_map_
-000007b0: 636c 7573 7465 7265 722a 0000 0073 1000  clusterer*...s..
-000007c0: 0000 0002 0801 0802 0801 1002 1202 0a01  ................
-000007d0: 1001 7a24 4d61 7043 6c75 7374 6572 5669  ..z$MapClusterVi
-000007e0: 6577 4261 7365 2e67 6574 5f6d 6170 5f63  ewBase.get_map_c
-000007f0: 6c75 7374 6572 6572 6306 0000 0000 0000  lustererc.......
-00000800: 0000 0000 0008 0000 0005 0000 0043 0000  .............C..
-00000810: 0073 2c00 0000 7c04 6a00 a001 7c00 6a02  .s,...|.j...|.j.
-00000820: 6900 a102 7d06 7403 7c01 7c02 7c03 7c05  i...}.t.|.|.|.|.
-00000830: 8304 7d07 7c07 a004 7c06 a101 0100 7c07  ..}.|...|.....|.
-00000840: 5300 a901 4e29 05da 0773 6573 7369 6f6e  S...N)...session
-00000850: 7220 0000 00da 0a63 6163 6865 5f6e 616d  r .....cache_nam
-00000860: 6572 1600 0000 da0f 6c6f 6164 5f67 656f  er......load_geo
-00000870: 6d65 7472 6965 7329 0872 1a00 0000 7232  metries).r....r2
-00000880: 0000 0072 2f00 0000 7233 0000 0072 1b00  ...r/...r3...r..
-00000890: 0000 7234 0000 00da 0663 6163 6865 6472  ..r4.....cachedr
-000008a0: 3600 0000 721e 0000 0072 1e00 0000 721f  6...r....r....r.
-000008b0: 0000 0072 3100 0000 3900 0000 7308 0000  ...r1...9...s...
-000008c0: 0000 0110 010e 020a 017a 1c4d 6170 436c  .........z.MapCl
-000008d0: 7573 7465 7256 6965 7742 6173 652e 6765  usterViewBase.ge
-000008e0: 745f 6361 6368 6563 0300 0000 0000 0000  t_cachec........
-000008f0: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
-00000900: 7318 0000 007c 02a0 00a1 007d 037c 037c  s....|.....}.|.|
-00000910: 016a 017c 006a 023c 0064 0053 0072 3800  .j.|.j.<.d.S.r8.
-00000920: 0000 2903 da09 7365 7269 616c 697a 6572  ..)...serializer
-00000930: 3900 0000 723a 0000 0029 0472 1a00 0000  9...r:...).r....
-00000940: 721b 0000 0072 3600 0000 5a12 636c 7573  r....r6...Z.clus
-00000950: 7465 725f 6361 6368 655f 6a73 6f6e 721e  ter_cache_jsonr.
-00000960: 0000 0072 1e00 0000 721f 0000 00da 0973  ...r....r......s
-00000970: 6574 5f63 6163 6865 4100 0000 7304 0000  et_cacheA...s...
-00000980: 0000 0108 017a 1c4d 6170 436c 7573 7465  .....z.MapCluste
-00000990: 7256 6965 7742 6173 652e 7365 745f 6361  rViewBase.set_ca
-000009a0: 6368 6563 0300 0000 0000 0000 0000 0000  chec............
-000009b0: 0700 0000 0400 0000 4300 0000 7332 0000  ........C...s2..
-000009c0: 0064 0164 0284 007c 0244 0083 017d 0374  .d.d...|.D...}.t
-000009d0: 006a 016a 027c 0364 038d 017d 0474 037c  .j.j.|.d...}.t.|
-000009e0: 0464 0464 058d 027d 057c 056a 047d 067c  .d.d...}.|.j.}.|
-000009f0: 0653 0029 064e 6301 0000 0000 0000 0000  .S.).Nc.........
-00000a00: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
-00000a10: 1200 0000 6700 7c00 5d0a 7d01 7c01 6a00  ....g.|.].}.|.j.
-00000a20: 9102 7104 5300 721e 0000 0029 01da 0270  ..q.S.r....)...p
-00000a30: 6b29 02da 022e 30da 0169 721e 0000 0072  k)....0..ir....r
-00000a40: 1e00 0000 721f 0000 00da 0a3c 6c69 7374  ....r......<list
-00000a50: 636f 6d70 3e48 0000 0073 0400 0000 0600  comp>H...s......
-00000a60: 0200 7a3f 4d61 7043 6c75 7374 6572 5669  ..z?MapClusterVi
-00000a70: 6577 4261 7365 2e73 6572 6961 6c69 7a65  ewBase.serialize
-00000a80: 5f67 6973 5f6d 6f64 656c 5f6c 6973 742e  _gis_model_list.
-00000a90: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000aa0: 6d70 3e29 01da 0670 6b5f 5f69 6e54 2901  mp>)...pk__inT).
-00000ab0: da04 6d61 6e79 2905 720b 0000 00da 076f  ..many).r......o
-00000ac0: 626a 6563 7473 da06 6669 6c74 6572 da12  bjects..filter..
-00000ad0: 4769 734d 6f64 656c 5365 7269 616c 697a  GisModelSerializ
-00000ae0: 6572 da04 6461 7461 2907 721a 0000 00da  er..data).r.....
-00000af0: 0d6d 6170 5f63 6c75 7374 6572 6572 5a0e  .map_clustererZ.
-00000b00: 696e 7374 616e 6365 735f 6c69 7374 5a0d  instances_listZ.
-00000b10: 696e 7374 616e 6365 735f 706b 735a 0c67  instances_pksZ.g
-00000b20: 6973 5f71 7565 7279 7365 74da 0a73 6572  is_queryset..ser
-00000b30: 6961 6c69 7a65 7272 4800 0000 721e 0000  ializerrH...r...
-00000b40: 0072 1e00 0000 721f 0000 00da 1873 6572  .r....r......ser
-00000b50: 6961 6c69 7a65 5f67 6973 5f6d 6f64 656c  ialize_gis_model
-00000b60: 5f6c 6973 7446 0000 0073 0a00 0000 0002  _listF...s......
-00000b70: 0e02 0e02 0c01 0602 7a2b 4d61 7043 6c75  ........z+MapClu
-00000b80: 7374 6572 5669 6577 4261 7365 2e73 6572  sterViewBase.ser
-00000b90: 6961 6c69 7a65 5f67 6973 5f6d 6f64 656c  ialize_gis_model
-00000ba0: 5f6c 6973 744e 290a 7222 0000 0072 2300  _listN).r"...r#.
-00000bb0: 0000 7224 0000 0072 3a00 0000 722b 0000  ..r$...r:...r+..
-00000bc0: 0072 2d00 0000 7237 0000 0072 3100 0000  .r-...r7...r1...
-00000bd0: 723e 0000 0072 4b00 0000 721e 0000 0072  r>...rK...r....r
-00000be0: 1e00 0000 721e 0000 0072 1f00 0000 7225  ....r....r....r%
-00000bf0: 0000 001d 0000 0073 0e00 0000 0802 0402  .......s........
-00000c00: 0805 0804 080f 0808 0805 7225 0000 0063  ..........r%...c
-00000c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c20: 0200 0000 4000 0000 7322 0000 0065 005a  ....@...s"...e.Z
-00000c30: 0164 005a 0267 005a 0367 005a 0465 0567  .d.Z.g.Z.g.Z.e.g
-00000c40: 015a 0664 0164 0284 005a 0764 0353 0029  .Z.d.d...Z.d.S.)
-00000c50: 04da 0b47 7269 6443 6c75 7374 6572 6302  ...GridClusterc.
-00000c60: 0000 0000 0000 0000 0000 000c 0000 0007  ................
-00000c70: 0000 004f 0000 0073 9c00 0000 7400 7c01  ...O...s....t.|.
-00000c80: 6a01 6401 8d01 7d04 7c04 a002 a100 728c  j.d...}.|.....r.
-00000c90: 7c04 6a03 6402 1900 7d05 7c00 a004 7c04  |.j.d...}.|...|.
-00000ca0: 6a03 6403 1900 a101 7d06 7c04 6a03 6404  j.d.....}.|.j.d.
-00000cb0: 1900 7d07 7c00 6a05 7406 7407 7c07 7c05  ..}.|.j.t.t.|.|.
-00000cc0: 7c06 7c01 6606 7c03 8e01 7d08 7c04 6a03  |.|.f.|...}.|.j.
-00000cd0: 6405 1900 7d09 7c03 6406 1900 7d0a 7c08  d...}.|.d...}.|.
-00000ce0: a008 7c09 7c0a 7c07 a103 7d0b 7c00 a009  ..|.|.|...}.|...
-00000cf0: 7c01 7c08 6a0a a102 0100 740b 7c0b 740c  |.|.j.....t.|.t.
-00000d00: 6a0d 6407 8d02 5300 740b 7c04 6a0e 740c  j.d...S.t.|.j.t.
-00000d10: 6a0f 6407 8d02 5300 2908 4ea9 0172 4800  j.d...S.).N..rH.
-00000d20: 0000 7235 0000 0072 2a00 0000 7234 0000  ..r5...r*...r4..
-00000d30: 00da 0767 656f 6a73 6f6e 722f 0000 0072  ...geojsonr/...r
-00000d40: 0800 0000 2910 7211 0000 0072 4800 0000  ....).r....rH...
-00000d50: da08 6973 5f76 616c 6964 da0e 7661 6c69  ..is_valid..vali
-00000d60: 6461 7465 645f 6461 7461 722b 0000 0072  dated_datar+...r
-00000d70: 3700 0000 720c 0000 0072 0e00 0000 da0c  7...r....r......
-00000d80: 6772 6964 5f63 6c75 7374 6572 723e 0000  grid_clusterr>..
-00000d90: 0072 3600 0000 7206 0000 0072 0900 0000  .r6...r....r....
-00000da0: da0b 4854 5450 5f32 3030 5f4f 4bda 0665  ..HTTP_200_OK..e
-00000db0: 7272 6f72 73da 1448 5454 505f 3430 305f  rrors..HTTP_400_
-00000dc0: 4241 445f 5245 5155 4553 5429 0c72 1a00  BAD_REQUEST).r..
-00000dd0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00000de0: 0072 4a00 0000 7235 0000 0072 2a00 0000  .rJ...r5...r*...
-00000df0: 7234 0000 0072 4900 0000 724e 0000 0072  r4...rI...rN...r
-00000e00: 2f00 0000 da04 6772 6964 721e 0000 0072  /.....gridr....r
-00000e10: 1e00 0000 721f 0000 00da 0470 6f73 745b  ....r......post[
-00000e20: 0000 0073 2200 0000 0002 0c02 0802 0a01  ...s"...........
-00000e30: 1002 0a02 0c01 0200 02ff 0201 02ff 0403  ................
-00000e40: 0a01 0802 0e02 0e01 0e02 7a10 4772 6964  ..........z.Grid
-00000e50: 436c 7573 7465 722e 706f 7374 4e29 0872  Cluster.postN).r
-00000e60: 2200 0000 7223 0000 0072 2400 0000 5a16  "...r#...r$...Z.
-00000e70: 6175 7468 656e 7469 6361 7469 6f6e 5f63  authentication_c
-00000e80: 6c61 7373 6573 5a12 7065 726d 6973 7369  lassesZ.permissi
-00000e90: 6f6e 5f63 6c61 7373 6573 7207 0000 005a  on_classesr....Z
-00000ea0: 1072 656e 6465 7265 725f 636c 6173 7365  .renderer_classe
-00000eb0: 7372 5600 0000 721e 0000 0072 1e00 0000  srV...r....r....
-00000ec0: 721e 0000 0072 1f00 0000 724c 0000 0055  r....r....rL...U
-00000ed0: 0000 0073 0800 0000 0802 0401 0401 0602  ...s............
-00000ee0: 724c 0000 0063 0000 0000 0000 0000 0000  rL...c..........
-00000ef0: 0000 0000 0000 0200 0000 4000 0000 7314  ..........@...s.
-00000f00: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
-00000f10: 005a 0364 0353 0029 04da 0d4b 6d65 616e  .Z.d.S.)...Kmean
-00000f20: 7343 6c75 7374 6572 6302 0000 0000 0000  sClusterc.......
-00000f30: 0000 0000 000d 0000 0007 0000 004f 0000  .............O..
-00000f40: 0073 a200 0000 7400 7c01 6a01 6401 8d01  .s....t.|.j.d...
-00000f50: 7d04 7c04 a002 a100 7292 7c04 6a03 6402  }.|.....r.|.j.d.
-00000f60: 1900 7d05 7c04 6a03 6403 1900 7d06 7c00  ..}.|.j.d...}.|.
-00000f70: a004 7c04 6a03 6404 1900 a101 7d07 7c04  ..|.j.d.....}.|.
-00000f80: 6a03 6405 1900 7d08 7c00 6a05 7c05 7406  j.d...}.|.j.|.t.
-00000f90: 7c08 7c06 7c07 7c01 6606 7c03 8e01 7d09  |.|.|.|.f.|...}.
-00000fa0: 7c04 6a03 6406 1900 7d0a 7c03 6407 1900  |.j.d...}.|.d...
-00000fb0: 7d0b 7c09 a007 7c0a 7c05 7c0b 7c08 a104  }.|...|.|.|.|...
-00000fc0: 7d0c 7c00 a008 7c01 7c09 6a09 a102 0100  }.|...|.|.j.....
-00000fd0: 740a 7c0c 8301 5300 740a 7c04 6a0b 740c  t.|...S.t.|.j.t.
-00000fe0: 6a0d 6408 8d02 5300 2909 4e72 4d00 0000  j.d...S.).NrM...
-00000ff0: 7232 0000 0072 3500 0000 722a 0000 0072  r2...r5...r*...r
-00001000: 3400 0000 724e 0000 0072 2f00 0000 7208  4...rN...r/...r.
-00001010: 0000 0029 0e72 1100 0000 7248 0000 0072  ...).r....rH...r
-00001020: 4f00 0000 7250 0000 0072 2b00 0000 7237  O...rP...r+...r7
-00001030: 0000 0072 0f00 0000 da0e 6b6d 6561 6e73  ...r......kmeans
-00001040: 5f63 6c75 7374 6572 723e 0000 0072 3600  _clusterr>...r6.
-00001050: 0000 7206 0000 0072 5300 0000 7209 0000  ..r....rS...r...
-00001060: 0072 5400 0000 290d 721a 0000 0072 1b00  .rT...).r....r..
-00001070: 0000 721c 0000 0072 1d00 0000 724a 0000  ..r....r....rJ..
-00001080: 0072 3200 0000 7235 0000 0072 2a00 0000  .r2...r5...r*...
-00001090: 7234 0000 0072 4900 0000 724e 0000 0072  r4...rI...rN...r
-000010a0: 2f00 0000 da07 6d61 726b 6572 7372 1e00  /.....markersr..
-000010b0: 0000 721e 0000 0072 1f00 0000 7256 0000  ..r....r....rV..
-000010c0: 0077 0000 0073 2200 0000 0002 0c02 0802  .w...s".........
-000010d0: 0a01 0a01 1002 0a02 0e01 02ff 0201 02ff  ................
-000010e0: 0403 0a01 0802 1001 0e01 0802 7a12 4b6d  ............z.Km
-000010f0: 6561 6e73 436c 7573 7465 722e 706f 7374  eansCluster.post
-00001100: 4ea9 0472 2200 0000 7223 0000 0072 2400  N..r"...r#...r$.
-00001110: 0000 7256 0000 0072 1e00 0000 721e 0000  ..rV...r....r...
-00001120: 0072 1e00 0000 721f 0000 0072 5700 0000  .r....r....rW...
-00001130: 7500 0000 7302 0000 0008 0272 5700 0000  u...s......rW...
-00001140: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001150: 0002 0000 0040 0000 0073 1400 0000 6500  .....@...s....e.
-00001160: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00001170: 5300 2904 da11 4765 7443 6c75 7374 6572  S.)...GetCluster
-00001180: 436f 6e74 656e 7463 0200 0000 0000 0000  Contentc........
-00001190: 0000 0000 1000 0000 0900 0000 4f00 0000  ............O...
-000011a0: 73c2 0000 0074 007c 016a 0164 018d 017d  s....t.|.j.d...}
-000011b0: 047c 04a0 02a1 0072 b27c 046a 0364 0219  .|.....r.|.j.d..
-000011c0: 007d 057c 00a0 047c 046a 0364 0319 00a1  .}.|...|.j.d....
-000011d0: 017d 067c 00a0 047c 046a 0364 0419 00a1  .}.|...|.j.d....
-000011e0: 017d 077c 046a 0364 0519 007d 087c 006a  .}.|.j.d...}.|.j
-000011f0: 057c 0574 067c 0864 067c 067c 0166 067c  .|.t.|.d.|.|.f.|
-00001200: 038e 017d 097c 046a 0364 0719 007d 0a7c  ...}.|.j.d...}.|
-00001210: 046a 0364 0819 007d 0b7c 046a 0364 0919  .j.d...}.|.j.d..
-00001220: 007d 0c7c 0364 0a19 007d 0d7c 096a 077c  .}.|.d...}.|.j.|
-00001230: 057c 0a7c 0b7c 0c7c 087c 0d7c 0764 0b8d  .|.|.|.|.|.|.d..
-00001240: 077d 0e7c 00a0 087c 097c 0ea1 027d 0f74  .}.|...|.|...}.t
-00001250: 097c 0f83 0153 0074 097c 046a 0a74 0b6a  .|...S.t.|.j.t.j
-00001260: 0c64 0c8d 0253 0029 0d4e 724d 0000 0072  .d...S.).NrM...r
-00001270: 3200 0000 722a 0000 00da 0a69 6e70 7574  2...r*.....input
-00001280: 5f73 7269 6472 3400 0000 46da 0369 6473  _sridr4...F..ids
-00001290: da01 78da 0179 722f 0000 0029 0172 5c00  ..x..yr/...).r\.
-000012a0: 0000 7208 0000 0029 0d72 1200 0000 7248  ..r....).r....rH
-000012b0: 0000 0072 4f00 0000 7250 0000 0072 2b00  ...rO...rP...r+.
-000012c0: 0000 7237 0000 0072 0f00 0000 da1a 6765  ..r7...r......ge
-000012d0: 745f 6b6d 6561 6e73 5f63 6c75 7374 6572  t_kmeans_cluster
-000012e0: 5f63 6f6e 7465 6e74 724b 0000 0072 0600  _contentrK...r..
-000012f0: 0000 7253 0000 0072 0900 0000 7254 0000  ..rS...r....rT..
-00001300: 0029 1072 1a00 0000 721b 0000 0072 1c00  .).r....r....r..
-00001310: 0000 721d 0000 0072 4a00 0000 7232 0000  ..r....rJ...r2..
-00001320: 0072 2a00 0000 725c 0000 0072 3400 0000  .r*...r\...r4...
-00001330: 7249 0000 0072 5d00 0000 725e 0000 0072  rI...r]...r^...r
-00001340: 5f00 0000 722f 0000 005a 0f63 6c75 7374  _...r/...Z.clust
-00001350: 6572 5f63 6f6e 7465 6e74 7248 0000 0072  er_contentrH...r
-00001360: 1e00 0000 721e 0000 0072 1f00 0000 7256  ....r....r....rV
-00001370: 0000 0095 0000 0073 2a00 0000 0002 0c02  .......s*.......
-00001380: 0802 0a01 1001 1002 0a02 0e01 02ff 0201  ................
-00001390: 02ff 0403 0a01 0a01 0a02 0802 1001 02ff  ................
-000013a0: 0603 0c02 0802 7a16 4765 7443 6c75 7374  ......z.GetClust
-000013b0: 6572 436f 6e74 656e 742e 706f 7374 4e72  erContent.postNr
-000013c0: 5a00 0000 721e 0000 0072 1e00 0000 721e  Z...r....r....r.
-000013d0: 0000 0072 1f00 0000 725b 0000 0093 0000  ...r....r[......
-000013e0: 0073 0200 0000 0802 725b 0000 0063 0000  .s......r[...c..
-000013f0: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00001400: 0000 4000 0000 7314 0000 0065 005a 0164  ..@...s....e.Z.d
-00001410: 005a 0264 0164 0284 005a 0364 0353 0029  .Z.d.d...Z.d.S.)
-00001420: 04da 0e47 6574 4172 6561 436f 6e74 656e  ...GetAreaConten
-00001430: 7463 0200 0000 0000 0000 0000 0000 0e00  tc..............
-00001440: 0000 0700 0000 4f00 0000 73aa 0000 0074  ......O...s....t
-00001450: 007c 016a 0164 018d 017d 047c 04a0 02a1  .|.j.d...}.|....
-00001460: 0072 9a7c 046a 0364 0219 007d 057c 00a0  .r.|.j.d...}.|..
-00001470: 047c 046a 0364 0319 00a1 017d 067c 046a  .|.j.d.....}.|.j
-00001480: 03a0 0564 0464 00a1 027d 077c 046a 03a0  ...d.d...}.|.j..
-00001490: 0564 0564 00a1 027d 087c 046a 0364 0619  .d.d...}.|.j.d..
-000014a0: 007d 097c 006a 067c 0574 077c 0964 077c  .}.|.j.|.t.|.d.|
-000014b0: 067c 0166 067c 038e 017d 0a7c 046a 0364  .|.f.|...}.|.j.d
-000014c0: 0819 007d 0b7c 0aa0 087c 0b7c 097c 077c  ...}.|...|.|.|.|
-000014d0: 08a1 047d 0c7c 00a0 097c 0a7c 0ca1 027d  ...}.|...|.|...}
-000014e0: 0d74 0a7c 0d83 0153 0074 0a7c 046a 0b74  .t.|...S.t.|.j.t
-000014f0: 0c6a 0d64 098d 0253 0029 0a4e 724d 0000  .j.d...S.).NrM..
-00001500: 0072 3200 0000 722a 0000 00da 056c 696d  .r2...r*.....lim
-00001510: 6974 da06 6f66 6673 6574 7234 0000 0046  it..offsetr4...F
-00001520: 724e 0000 0072 0800 0000 290e 7215 0000  rN...r....).r...
-00001530: 0072 4800 0000 724f 0000 0072 5000 0000  .rH...rO...rP...
-00001540: 722b 0000 0072 2000 0000 7237 0000 0072  r+...r ...r7...r
-00001550: 0f00 0000 da10 6765 745f 6172 6561 5f63  ......get_area_c
-00001560: 6f6e 7465 6e74 724b 0000 0072 0600 0000  ontentrK...r....
-00001570: 7253 0000 0072 0900 0000 7254 0000 0029  rS...r....rT...)
-00001580: 0e72 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00001590: 721d 0000 0072 4a00 0000 7232 0000 0072  r....rJ...r2...r
-000015a0: 2a00 0000 7262 0000 0072 6300 0000 7234  *...rb...rc...r4
-000015b0: 0000 0072 4900 0000 724e 0000 005a 0c61  ...rI...rN...Z.a
-000015c0: 7265 615f 636f 6e74 656e 7472 4800 0000  rea_contentrH...
-000015d0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000015e0: 5600 0000 ba00 0000 7322 0000 0000 020c  V.......s"......
-000015f0: 0208 020a 0110 020e 010e 020a 020e 0102  ................
-00001600: ff02 0102 ff04 030a 0210 020c 0208 027a  ...............z
-00001610: 1347 6574 4172 6561 436f 6e74 656e 742e  .GetAreaContent.
-00001620: 706f 7374 4e72 5a00 0000 721e 0000 0072  postNrZ...r....r
-00001630: 1e00 0000 721e 0000 0072 1f00 0000 7261  ....r....r....ra
-00001640: 0000 00b8 0000 0073 0200 0000 0802 7261  .......s......ra
-00001650: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001660: 0000 0000 0200 0000 4000 0000 7314 0000  ........@...s...
-00001670: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-00001680: 0364 0353 0029 04da 1147 6574 4461 7461  .d.S.)...GetData
-00001690: 7365 7443 6f6e 7465 6e74 6302 0000 0000  setContentc.....
-000016a0: 0000 0000 0000 000b 0000 0007 0000 004f  ...............O
-000016b0: 0000 0073 5200 0000 7c01 6a00 a001 6401  ...sR...|.j...d.
-000016c0: 6402 a102 7d04 6700 7d05 7c00 6a02 7403  d...}.g.}.|.j.t.
-000016d0: 7404 7c05 6403 7c04 7c01 6606 7c03 8e01  t.|.d.|.|.f.|...
-000016e0: 7d06 7c03 6404 1900 7d07 7c06 a005 7c07  }.|.d...}.|...|.
-000016f0: a101 7d08 7406 7c08 8301 7d09 7c09 6a07  ..}.t.|...}.|.j.
-00001700: 7d0a 7408 7c0a 8301 5300 2905 4e72 2a00  }.t.|...S.).Nr*.
-00001710: 0000 69e6 1000 0046 da0a 6461 7461 7365  ..i....F..datase
-00001720: 745f 6964 2909 da03 4745 5472 2000 0000  t_id)...GETr ...
-00001730: 7237 0000 0072 0c00 0000 720e 0000 00da  r7...r....r.....
-00001740: 1367 6574 5f64 6174 6173 6574 5f63 6f6e  .get_dataset_con
-00001750: 7465 6e74 7247 0000 0072 4800 0000 7206  tentrG...rH...r.
-00001760: 0000 0029 0b72 1a00 0000 721b 0000 0072  ...).r....r....r
-00001770: 1c00 0000 721d 0000 0072 2a00 0000 7234  ....r....r*...r4
-00001780: 0000 0072 4900 0000 7266 0000 005a 0764  ...rI...rf...Z.d
-00001790: 6174 6173 6574 724a 0000 0072 4800 0000  atasetrJ...rH...
-000017a0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000017b0: 2000 0000 d900 0000 7318 0000 0000 020e   .......s.......
-000017c0: 0204 020e 0102 ff02 0102 ff04 0308 020a  ................
-000017d0: 0208 0106 027a 1547 6574 4461 7461 7365  .....z.GetDatase
-000017e0: 7443 6f6e 7465 6e74 2e67 6574 4e72 2100  tContent.getNr!.
-000017f0: 0000 721e 0000 0072 1e00 0000 721e 0000  ..r....r....r...
-00001800: 0072 1f00 0000 7265 0000 00d7 0000 0073  .r....re.......s
-00001810: 0200 0000 0802 7265 0000 0063 0000 0000  ......re...c....
-00001820: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00001830: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00001840: 0264 0164 0284 005a 0364 0353 0029 04da  .d.d...Z.d.S.)..
-00001850: 1247 6574 4d61 7043 6f6e 7465 6e74 436f  .GetMapContentCo
-00001860: 756e 7463 0200 0000 0000 0000 0000 0000  untc............
-00001870: 0e00 0000 0700 0000 4f00 0000 73a0 0000  ........O...s...
-00001880: 0074 007c 016a 0164 018d 017d 047c 04a0  .t.|.j.d...}.|..
-00001890: 02a1 0072 9064 027d 057c 046a 0364 0319  ...r.d.}.|.j.d..
-000018a0: 007d 067c 046a 0364 0419 007d 077c 00a0  .}.|.j.d...}.|..
-000018b0: 047c 046a 0364 0519 00a1 017d 087c 046a  .|.j.d.....}.|.j
-000018c0: 0364 0619 007d 097c 0364 0719 007d 0a7c  .d...}.|.d...}.|
-000018d0: 046a 0364 0819 007d 0b7c 006a 057c 0774  .j.d...}.|.j.|.t
-000018e0: 067c 067c 057c 087c 0166 067c 038e 017d  .|.|.|.|.f.|...}
-000018f0: 0c7c 0ca0 077c 097c 077c 067c 0a7c 0ba1  .|...|.|.|.|.|..
-00001900: 057d 0d74 087c 0d74 096a 0a64 098d 0253  .}.t.|.t.j.d...S
-00001910: 0074 087c 046a 0b74 096a 0c64 098d 0253  .t.|.j.t.j.d...S
-00001920: 0029 0a4e 724d 0000 0054 7234 0000 0072  .).NrM...Tr4...r
-00001930: 3200 0000 722a 0000 0072 4e00 0000 722f  2...r*...rN...r/
-00001940: 0000 00da 0b6d 6f64 756c 6174 696f 6e73  .....modulations
-00001950: 7208 0000 0029 0d72 1300 0000 7248 0000  r....).r....rH..
-00001960: 0072 4f00 0000 7250 0000 0072 2b00 0000  .rO...rP...r+...
-00001970: 7237 0000 0072 0f00 0000 5a16 6765 745f  r7...r....Z.get_
-00001980: 6d61 705f 636f 6e74 656e 745f 636f 756e  map_content_coun
-00001990: 7473 7206 0000 0072 0900 0000 7252 0000  tsr....r....rR..
-000019a0: 0072 5300 0000 7254 0000 0029 0e72 1a00  .rS...rT...).r..
-000019b0: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-000019c0: 0072 4a00 0000 7235 0000 0072 3400 0000  .rJ...r5...r4...
-000019d0: 7232 0000 0072 2a00 0000 724e 0000 0072  r2...r*...rN...r
-000019e0: 2f00 0000 726a 0000 0072 4900 0000 5a12  /...rj...rI...Z.
-000019f0: 6d61 705f 636f 6e74 656e 745f 636f 756e  map_content_coun
-00001a00: 7473 721e 0000 0072 1e00 0000 721f 0000  tsr....r....r...
-00001a10: 0072 5600 0000 ee00 0000 7322 0000 0000  .rV.......s"....
-00001a20: 020c 0208 0204 010a 010a 0110 020a 0108  ................
-00001a30: 010a 020e 0102 ff02 0102 ff04 0312 020e  ................
-00001a40: 027a 1747 6574 4d61 7043 6f6e 7465 6e74  .z.GetMapContent
-00001a50: 436f 756e 742e 706f 7374 4e72 5a00 0000  Count.postNrZ...
-00001a60: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-00001a70: 1f00 0000 7269 0000 00ec 0000 0073 0200  ....ri.......s..
-00001a80: 0000 0802 7269 0000 0063 0000 0000 0000  ....ri...c......
-00001a90: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00001aa0: 0000 7314 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00001ab0: 0164 0284 005a 0364 0353 0029 04da 1547  .d...Z.d.S.)...G
-00001ac0: 6574 4772 6f75 7065 644d 6170 436f 6e74  etGroupedMapCont
-00001ad0: 656e 7473 6302 0000 0000 0000 0000 0000  entsc...........
-00001ae0: 000e 0000 0007 0000 004f 0000 0073 a000  .........O...s..
-00001af0: 0000 7400 7c01 6a01 6401 8d01 7d04 7c04  ..t.|.j.d...}.|.
-00001b00: a002 a100 7290 6402 7d05 7c04 6a03 6403  ....r.d.}.|.j.d.
-00001b10: 1900 7d06 7c04 6a03 6404 1900 7d07 7c00  ..}.|.j.d...}.|.
-00001b20: a004 7c04 6a03 6405 1900 a101 7d08 7c04  ..|.j.d.....}.|.
-00001b30: 6a03 6406 1900 7d09 7c03 6407 1900 7d0a  j.d...}.|.d...}.
-00001b40: 7c04 6a03 6408 1900 7d0b 7c00 6a05 7c07  |.j.d...}.|.j.|.
-00001b50: 7406 7c06 7c05 7c08 7c01 6606 7c03 8e01  t.|.|.|.|.f.|...
-00001b60: 7d0c 7c0c a007 7c09 7c07 7c0a 7c06 7c0b  }.|...|.|.|.|.|.
-00001b70: a105 7d0d 7408 7c0d 7409 6a0a 6409 8d02  ..}.t.|.t.j.d...
-00001b80: 5300 7408 7c04 6a0b 7409 6a0c 6409 8d02  S.t.|.j.t.j.d...
-00001b90: 5300 290a 4e72 4d00 0000 5472 3400 0000  S.).NrM...Tr4...
-00001ba0: 7232 0000 0072 2a00 0000 724e 0000 0072  r2...r*...rN...r
-00001bb0: 2f00 0000 da08 6772 6f75 705f 6279 7208  /.....group_byr.
-00001bc0: 0000 0029 0d72 1400 0000 7248 0000 0072  ...).r....rH...r
-00001bd0: 4f00 0000 7250 0000 0072 2b00 0000 7237  O...rP...r+...r7
-00001be0: 0000 0072 0f00 0000 da18 6765 745f 6772  ...r......get_gr
-00001bf0: 6f75 7065 645f 6d61 705f 636f 6e74 656e  ouped_map_conten
-00001c00: 7473 7206 0000 0072 0900 0000 7252 0000  tsr....r....rR..
-00001c10: 0072 5300 0000 7254 0000 0029 0e72 1a00  .rS...rT...).r..
-00001c20: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00001c30: 0072 4a00 0000 7235 0000 0072 3400 0000  .rJ...r5...r4...
-00001c40: 7232 0000 0072 2a00 0000 724e 0000 0072  r2...r*...rN...r
-00001c50: 2f00 0000 726c 0000 0072 4900 0000 da06  /...rl...rI.....
-00001c60: 6772 6f75 7073 721e 0000 0072 1e00 0000  groupsr....r....
-00001c70: 721f 0000 0072 5600 0000 0901 0000 7322  r....rV.......s"
-00001c80: 0000 0000 020c 0208 0204 010a 010a 0110  ................
-00001c90: 020a 0108 020a 020e 0102 ff02 0102 ff04  ................
-00001ca0: 0312 020e 027a 1a47 6574 4772 6f75 7065  .....z.GetGroupe
-00001cb0: 644d 6170 436f 6e74 656e 7473 2e70 6f73  dMapContents.pos
-00001cc0: 744e 725a 0000 0072 1e00 0000 721e 0000  tNrZ...r....r...
-00001cd0: 0072 1e00 0000 721f 0000 0072 6b00 0000  .r....r....rk...
-00001ce0: 0701 0000 7302 0000 0008 0272 6b00 0000  ....s......rk...
-00001cf0: 292a da0b 646a 616e 676f 2e63 6f6e 6672  )*..django.confr
-00001d00: 0200 0000 da0b 646a 616e 676f 2e63 6f72  ......django.cor
-00001d10: 6572 0300 0000 5a14 7265 7374 5f66 7261  er....Z.rest_fra
-00001d20: 6d65 776f 726b 2e76 6965 7773 7204 0000  mework.viewsr...
-00001d30: 005a 1772 6573 745f 6672 616d 6577 6f72  .Z.rest_framewor
-00001d40: 6b2e 7265 7370 6f6e 7365 7206 0000 005a  k.responser....Z
-00001d50: 1872 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
-00001d60: 7265 6e64 6572 6572 7372 0700 0000 da0e  renderersr......
-00001d70: 7265 7374 5f66 7261 6d65 776f 726b 7209  rest_frameworkr.
-00001d80: 0000 005a 1761 6e79 636c 7573 7465 722e  ...Z.anycluster.
-00001d90: 4d61 7043 6c75 7374 6572 6572 720a 0000  MapClustererr...
-00001da0: 0072 0b00 0000 da16 616e 7963 6c75 7374  .r......anyclust
-00001db0: 6572 2e64 6566 696e 6974 696f 6e73 720c  er.definitionsr.
-00001dc0: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
-00001dd0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001de0: 0072 1400 0000 7215 0000 00da 0a61 6e79  .r....r......any
-00001df0: 636c 7573 7465 7272 1600 0000 5a10 616e  clusterr....Z.an
-00001e00: 7963 6c75 7374 6572 2e75 7469 6c73 7217  ycluster.utilsr.
-00001e10: 0000 00da 0767 6574 6174 7472 5a13 6769  .....getattrZ.gi
-00001e20: 735f 7365 7269 616c 697a 6572 5f70 6174  s_serializer_pat
-00001e30: 6872 4700 0000 da04 6a73 6f6e 7218 0000  hrG.....jsonr...
-00001e40: 0072 2500 0000 724c 0000 0072 5700 0000  .r%...rL...rW...
-00001e50: 725b 0000 0072 6100 0000 7265 0000 0072  r[...ra...re...r
-00001e60: 6900 0000 726b 0000 0072 1e00 0000 721e  i...rk...r....r.
-00001e70: 0000 0072 1e00 0000 721f 0000 00da 083c  ...r....r......<
-00001e80: 6d6f 6475 6c65 3e01 0000 0073 2c00 0000  module>....s,...
-00001e90: 0c01 0c02 0c01 0c01 0c01 0c02 1001 1802  ................
-00001ea0: 1c03 0c01 0c02 0c01 0802 0802 1006 0e38  ...............8
-00001eb0: 1220 121e 1225 121f 1215 121b            . ...%......
+000003f0: 721f 0000 00fa 492f 686f 6d65 2f74 6f6d  r.....I/home/tom
+00000400: 2f6c 6f63 616c 636f 736d 6f73 2d70 7269  /localcosmos-pri
+00000410: 7661 7465 2f6c 6f63 616c 636f 736d 6f73  vate/localcosmos
+00000420: 5f70 7269 7661 7465 2f61 6e79 636c 7573  _private/anyclus
+00000430: 7465 722f 6170 692f 7669 6577 732e 7079  ter/api/views.py
+00000440: da03 6765 7419 0000 0073 0200 0000 0001  ..get....s......
+00000450: 7a0b 4150 4948 6f6d 652e 6765 744e a904  z.APIHome.getN..
+00000460: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000470: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000480: 6d65 5f5f 7221 0000 0072 1f00 0000 721f  me__r!...r....r.
+00000490: 0000 0072 1f00 0000 7220 0000 0072 1900  ...r....r ...r..
+000004a0: 0000 1700 0000 7302 0000 0008 0272 1900  ......s......r..
+000004b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000004c0: 0000 0002 0000 0040 0000 0073 4000 0000  .......@...s@...
+000004d0: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
+000004e0: 8400 5a04 6404 6405 8400 5a05 6406 6407  ..Z.d.d...Z.d.d.
+000004f0: 8400 5a06 6408 6409 8400 5a07 640a 640b  ..Z.d.d...Z.d.d.
+00000500: 8400 5a08 640c 640d 8400 5a09 640e 5300  ..Z.d.d...Z.d.S.
+00000510: 290f da12 4d61 7043 6c75 7374 6572 5669  )...MapClusterVi
+00000520: 6577 4261 7365 5a10 616e 7963 6c75 7374  ewBaseZ.anyclust
+00000530: 6572 5f63 6163 6865 6302 0000 0000 0000  er_cachec.......
+00000540: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000550: 0073 1600 0000 7400 7c01 a001 6401 a101  .s....t.|...d...
+00000560: 6402 1900 8301 7d02 7c02 5300 2903 4efa  d.....}.|.S.).N.
+00000570: 013a e9ff ffff ff29 02da 0369 6e74 da05  .:.....)...int..
+00000580: 7370 6c69 7429 0372 1b00 0000 da08 7372  split).r......sr
+00000590: 6964 5f73 7472 da0b 6f75 7470 7574 5f73  id_str..output_s
+000005a0: 7269 6472 1f00 0000 721f 0000 0072 2000  ridr....r....r .
+000005b0: 0000 da0a 7061 7273 655f 7372 6964 2100  ....parse_srid!.
+000005c0: 0000 7304 0000 0000 0112 017a 1d4d 6170  ..s........z.Map
+000005d0: 436c 7573 7465 7256 6965 7742 6173 652e  ClusterViewBase.
+000005e0: 7061 7273 655f 7372 6964 6302 0000 0000  parse_sridc.....
+000005f0: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
+00000600: 0000 0073 0400 0000 6401 5300 2902 4eda  ...s....d.S.).N.
+00000610: 0670 7562 6c69 6372 1f00 0000 2902 721b  .publicr....).r.
+00000620: 0000 0072 1c00 0000 721f 0000 0072 1f00  ...r....r....r..
+00000630: 0000 7220 0000 00da 0f67 6574 5f73 6368  ..r .....get_sch
+00000640: 656d 615f 6e61 6d65 2600 0000 7302 0000  ema_name&...s...
+00000650: 0000 017a 224d 6170 436c 7573 7465 7256  ...z"MapClusterV
+00000660: 6965 7742 6173 652e 6765 745f 7363 6865  iewBase.get_sche
+00000670: 6d61 5f6e 616d 6563 0700 0000 0000 0000  ma_namec........
+00000680: 0000 0000 0d00 0000 0700 0000 4b00 0000  ............K...
+00000690: 7358 0000 007c 0764 0119 007d 087c 0764  sX...|.d...}.|.d
+000006a0: 0219 007d 097c 0464 036b 0272 2874 007c  ...}.|.d.k.r(t.|
+000006b0: 017c 097c 027c 0383 047d 0a6e 127c 00a0  .|.|.|...}.n.|..
+000006c0: 017c 017c 097c 027c 067c 03a1 057d 0a7c  .|.|.|.|.|...}.|
+000006d0: 00a0 027c 06a1 017d 0b74 037c 0a7c 087c  ...|...}.t.|.|.|
+000006e0: 057c 0b64 048d 047d 0c7c 0c53 0029 054e  .|.d...}.|.S.).N
+000006f0: da09 6772 6964 5f73 697a 65da 047a 6f6f  ..grid_size..zoo
+00000700: 6d54 2903 7230 0000 0072 2c00 0000 da0b  mT).r0...r,.....
+00000710: 7363 6865 6d61 5f6e 616d 6529 0472 1600  schema_name).r..
+00000720: 0000 da09 6765 745f 6361 6368 6572 2f00  ....get_cacher/.
+00000730: 0000 720a 0000 0029 0d72 1b00 0000 da0d  ..r....).r......
+00000740: 6765 6f6d 6574 7279 5f74 7970 65da 0b63  geometry_type..c
+00000750: 6c75 7374 6572 7479 7065 da07 6669 6c74  lustertype..filt
+00000760: 6572 73da 0b63 6c65 6172 5f63 6163 6865  ers..clear_cache
+00000770: 722c 0000 0072 1c00 0000 721e 0000 0072  r,...r....r....r
+00000780: 3000 0000 7231 0000 00da 0d63 6c75 7374  0...r1.....clust
+00000790: 6572 5f63 6163 6865 7232 0000 005a 0963  er_cacher2...Z.c
+000007a0: 6c75 7374 6572 6572 721f 0000 0072 1f00  lustererr....r..
+000007b0: 0000 7220 0000 00da 1167 6574 5f6d 6170  ..r .....get_map
+000007c0: 5f63 6c75 7374 6572 6572 2a00 0000 7310  _clusterer*...s.
+000007d0: 0000 0000 0208 0108 0208 0110 0212 020a  ................
+000007e0: 0110 017a 244d 6170 436c 7573 7465 7256  ...z$MapClusterV
+000007f0: 6965 7742 6173 652e 6765 745f 6d61 705f  iewBase.get_map_
+00000800: 636c 7573 7465 7265 7263 0600 0000 0000  clustererc......
+00000810: 0000 0000 0000 0800 0000 0500 0000 4300  ..............C.
+00000820: 0000 732c 0000 007c 046a 00a0 017c 006a  ..s,...|.j...|.j
+00000830: 0269 00a1 027d 0674 037c 017c 027c 037c  .i...}.t.|.|.|.|
+00000840: 0583 047d 077c 07a0 047c 06a1 0101 007c  ...}.|...|.....|
+00000850: 0753 00a9 014e 2905 da07 7365 7373 696f  .S...N)...sessio
+00000860: 6e72 2100 0000 da0a 6361 6368 655f 6e61  nr!.....cache_na
+00000870: 6d65 7216 0000 00da 0f6c 6f61 645f 6765  mer......load_ge
+00000880: 6f6d 6574 7269 6573 2908 721b 0000 0072  ometries).r....r
+00000890: 3400 0000 7231 0000 0072 3500 0000 721c  4...r1...r5...r.
+000008a0: 0000 0072 3600 0000 da06 6361 6368 6564  ...r6.....cached
+000008b0: 7238 0000 0072 1f00 0000 721f 0000 0072  r8...r....r....r
+000008c0: 2000 0000 7233 0000 0039 0000 0073 0800   ...r3...9...s..
+000008d0: 0000 0001 1001 0e02 0a01 7a1c 4d61 7043  ..........z.MapC
+000008e0: 6c75 7374 6572 5669 6577 4261 7365 2e67  lusterViewBase.g
+000008f0: 6574 5f63 6163 6865 6303 0000 0000 0000  et_cachec.......
+00000900: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
+00000910: 0073 1800 0000 7c02 a000 a100 7d03 7c03  .s....|.....}.|.
+00000920: 7c01 6a01 7c00 6a02 3c00 6400 5300 723a  |.j.|.j.<.d.S.r:
+00000930: 0000 0029 03da 0973 6572 6961 6c69 7a65  ...)...serialize
+00000940: 723b 0000 0072 3c00 0000 2904 721b 0000  r;...r<...).r...
+00000950: 0072 1c00 0000 7238 0000 005a 1263 6c75  .r....r8...Z.clu
+00000960: 7374 6572 5f63 6163 6865 5f6a 736f 6e72  ster_cache_jsonr
+00000970: 1f00 0000 721f 0000 0072 2000 0000 da09  ....r....r .....
+00000980: 7365 745f 6361 6368 6541 0000 0073 0400  set_cacheA...s..
+00000990: 0000 0001 0801 7a1c 4d61 7043 6c75 7374  ......z.MapClust
+000009a0: 6572 5669 6577 4261 7365 2e73 6574 5f63  erViewBase.set_c
+000009b0: 6163 6865 6303 0000 0000 0000 0000 0000  achec...........
+000009c0: 0007 0000 0004 0000 0043 0000 0073 3200  .........C...s2.
+000009d0: 0000 6401 6402 8400 7c02 4400 8301 7d03  ..d.d...|.D...}.
+000009e0: 7400 6a01 6a02 7c03 6403 8d01 7d04 7403  t.j.j.|.d...}.t.
+000009f0: 7c04 6404 6405 8d02 7d05 7c05 6a04 7d06  |.d.d...}.|.j.}.
+00000a00: 7c06 5300 2906 4e63 0100 0000 0000 0000  |.S.).Nc........
+00000a10: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00000a20: 7312 0000 0067 007c 005d 0a7d 017c 016a  s....g.|.].}.|.j
+00000a30: 0091 0271 0453 0072 1f00 0000 2901 da02  ...q.S.r....)...
+00000a40: 706b 2902 da02 2e30 da01 6972 1f00 0000  pk)....0..ir....
+00000a50: 721f 0000 0072 2000 0000 da0a 3c6c 6973  r....r .....<lis
+00000a60: 7463 6f6d 703e 4800 0000 7304 0000 0006  tcomp>H...s.....
+00000a70: 0002 007a 3f4d 6170 436c 7573 7465 7256  ...z?MapClusterV
+00000a80: 6965 7742 6173 652e 7365 7269 616c 697a  iewBase.serializ
+00000a90: 655f 6769 735f 6d6f 6465 6c5f 6c69 7374  e_gis_model_list
+00000aa0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00000ab0: 6f6d 703e 2901 da06 706b 5f5f 696e 5429  omp>)...pk__inT)
+00000ac0: 01da 046d 616e 7929 0572 0b00 0000 da07  ...many).r......
+00000ad0: 6f62 6a65 6374 73da 0666 696c 7465 72da  objects..filter.
+00000ae0: 1247 6973 4d6f 6465 6c53 6572 6961 6c69  .GisModelSeriali
+00000af0: 7a65 72da 0464 6174 6129 0772 1b00 0000  zer..data).r....
+00000b00: da0d 6d61 705f 636c 7573 7465 7265 725a  ..map_clustererZ
+00000b10: 0e69 6e73 7461 6e63 6573 5f6c 6973 745a  .instances_listZ
+00000b20: 0d69 6e73 7461 6e63 6573 5f70 6b73 5a0c  .instances_pksZ.
+00000b30: 6769 735f 7175 6572 7973 6574 da0a 7365  gis_queryset..se
+00000b40: 7269 616c 697a 6572 724a 0000 0072 1f00  rializerrJ...r..
+00000b50: 0000 721f 0000 0072 2000 0000 da18 7365  ..r....r .....se
+00000b60: 7269 616c 697a 655f 6769 735f 6d6f 6465  rialize_gis_mode
+00000b70: 6c5f 6c69 7374 4600 0000 730a 0000 0000  l_listF...s.....
+00000b80: 020e 020e 020c 0106 027a 2b4d 6170 436c  .........z+MapCl
+00000b90: 7573 7465 7256 6965 7742 6173 652e 7365  usterViewBase.se
+00000ba0: 7269 616c 697a 655f 6769 735f 6d6f 6465  rialize_gis_mode
+00000bb0: 6c5f 6c69 7374 4e29 0a72 2300 0000 7224  l_listN).r#...r$
+00000bc0: 0000 0072 2500 0000 723c 0000 0072 2d00  ...r%...r<...r-.
+00000bd0: 0000 722f 0000 0072 3900 0000 7233 0000  ..r/...r9...r3..
+00000be0: 0072 4000 0000 724d 0000 0072 1f00 0000  .r@...rM...r....
+00000bf0: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00000c00: 2600 0000 1d00 0000 730e 0000 0008 0204  &.......s.......
+00000c10: 0208 0508 0408 0f08 0808 0572 2600 0000  ...........r&...
+00000c20: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000c30: 0002 0000 0040 0000 0073 2200 0000 6500  .....@...s"...e.
+00000c40: 5a01 6400 5a02 6700 5a03 6700 5a04 6505  Z.d.Z.g.Z.g.Z.e.
+00000c50: 6701 5a06 6401 6402 8400 5a07 6403 5300  g.Z.d.d...Z.d.S.
+00000c60: 2904 da0b 4772 6964 436c 7573 7465 7263  )...GridClusterc
+00000c70: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
+00000c80: 0700 0000 4f00 0000 739c 0000 0074 007c  ....O...s....t.|
+00000c90: 016a 0164 018d 017d 047c 04a0 02a1 0072  .j.d...}.|.....r
+00000ca0: 8c7c 046a 0364 0219 007d 057c 00a0 047c  .|.j.d...}.|...|
+00000cb0: 046a 0364 0319 00a1 017d 067c 046a 0364  .j.d.....}.|.j.d
+00000cc0: 0419 007d 077c 006a 0574 0674 077c 077c  ...}.|.j.t.t.|.|
+00000cd0: 057c 067c 0166 067c 038e 017d 087c 046a  .|.|.f.|...}.|.j
+00000ce0: 0364 0519 007d 097c 0364 0619 007d 0a7c  .d...}.|.d...}.|
+00000cf0: 08a0 087c 097c 0a7c 07a1 037d 0b7c 00a0  ...|.|.|...}.|..
+00000d00: 097c 017c 086a 0aa1 0201 0074 0b7c 0b74  .|.|.j.....t.|.t
+00000d10: 0c6a 0d64 078d 0253 0074 0b7c 046a 0e74  .j.d...S.t.|.j.t
+00000d20: 0c6a 0f64 078d 0253 0029 084e a901 724a  .j.d...S.).N..rJ
+00000d30: 0000 0072 3700 0000 722c 0000 0072 3600  ...r7...r,...r6.
+00000d40: 0000 da07 6765 6f6a 736f 6e72 3100 0000  ....geojsonr1...
+00000d50: 7208 0000 0029 1072 1100 0000 724a 0000  r....).r....rJ..
+00000d60: 00da 0869 735f 7661 6c69 64da 0e76 616c  ...is_valid..val
+00000d70: 6964 6174 6564 5f64 6174 6172 2d00 0000  idated_datar-...
+00000d80: 7239 0000 0072 0c00 0000 720e 0000 005a  r9...r....r....Z
+00000d90: 0c67 7269 645f 636c 7573 7465 7272 4000  .grid_clusterr@.
+00000da0: 0000 7238 0000 0072 0600 0000 7209 0000  ..r8...r....r...
+00000db0: 00da 0b48 5454 505f 3230 305f 4f4b da06  ...HTTP_200_OK..
+00000dc0: 6572 726f 7273 da14 4854 5450 5f34 3030  errors..HTTP_400
+00000dd0: 5f42 4144 5f52 4551 5545 5354 290c 721b  _BAD_REQUEST).r.
+00000de0: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000df0: 0000 724c 0000 0072 3700 0000 722c 0000  ..rL...r7...r,..
+00000e00: 0072 3600 0000 724b 0000 0072 5000 0000  .r6...rK...rP...
+00000e10: 7231 0000 00da 0467 7269 6472 1f00 0000  r1.....gridr....
+00000e20: 721f 0000 0072 2000 0000 da04 706f 7374  r....r .....post
+00000e30: 5b00 0000 7322 0000 0000 020c 0208 020a  [...s"..........
+00000e40: 0110 020a 020c 0102 0002 ff02 0102 ff04  ................
+00000e50: 030a 0108 020e 020e 010e 027a 1047 7269  ...........z.Gri
+00000e60: 6443 6c75 7374 6572 2e70 6f73 744e 2908  dCluster.postN).
+00000e70: 7223 0000 0072 2400 0000 7225 0000 00da  r#...r$...r%....
+00000e80: 1661 7574 6865 6e74 6963 6174 696f 6e5f  .authentication_
+00000e90: 636c 6173 7365 73da 1270 6572 6d69 7373  classes..permiss
+00000ea0: 696f 6e5f 636c 6173 7365 7372 0700 0000  ion_classesr....
+00000eb0: da10 7265 6e64 6572 6572 5f63 6c61 7373  ..renderer_class
+00000ec0: 6573 7257 0000 0072 1f00 0000 721f 0000  esrW...r....r...
+00000ed0: 0072 1f00 0000 7220 0000 0072 4e00 0000  .r....r ...rN...
+00000ee0: 5500 0000 7308 0000 0008 0204 0104 0106  U...s...........
+00000ef0: 0272 4e00 0000 6300 0000 0000 0000 0000  .rN...c.........
+00000f00: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00000f10: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+00000f20: 8400 5a03 6403 5300 2904 da0d 4b6d 6561  ..Z.d.S.)...Kmea
+00000f30: 6e73 436c 7573 7465 7263 0200 0000 0000  nsClusterc......
+00000f40: 0000 0000 0000 0d00 0000 0700 0000 4f00  ..............O.
+00000f50: 0000 73a2 0000 0074 007c 016a 0164 018d  ..s....t.|.j.d..
+00000f60: 017d 047c 04a0 02a1 0072 927c 046a 0364  .}.|.....r.|.j.d
+00000f70: 0219 007d 057c 046a 0364 0319 007d 067c  ...}.|.j.d...}.|
+00000f80: 00a0 047c 046a 0364 0419 00a1 017d 077c  ...|.j.d.....}.|
+00000f90: 046a 0364 0519 007d 087c 006a 057c 0574  .j.d...}.|.j.|.t
+00000fa0: 067c 087c 067c 077c 0166 067c 038e 017d  .|.|.|.|.f.|...}
+00000fb0: 097c 046a 0364 0619 007d 0a7c 0364 0719  .|.j.d...}.|.d..
+00000fc0: 007d 0b7c 09a0 077c 0a7c 057c 0b7c 08a1  .}.|...|.|.|.|..
+00000fd0: 047d 0c7c 00a0 087c 017c 096a 09a1 0201  .}.|...|.|.j....
+00000fe0: 0074 0a7c 0c83 0153 0074 0a7c 046a 0b74  .t.|...S.t.|.j.t
+00000ff0: 0c6a 0d64 088d 0253 0029 094e 724f 0000  .j.d...S.).NrO..
+00001000: 0072 3400 0000 7237 0000 0072 2c00 0000  .r4...r7...r,...
+00001010: 7236 0000 0072 5000 0000 7231 0000 0072  r6...rP...r1...r
+00001020: 0800 0000 290e 7211 0000 0072 4a00 0000  ....).r....rJ...
+00001030: 7251 0000 0072 5200 0000 722d 0000 0072  rQ...rR...r-...r
+00001040: 3900 0000 720f 0000 005a 0e6b 6d65 616e  9...r....Z.kmean
+00001050: 735f 636c 7573 7465 7272 4000 0000 7238  s_clusterr@...r8
+00001060: 0000 0072 0600 0000 7254 0000 0072 0900  ...r....rT...r..
+00001070: 0000 7255 0000 0029 0d72 1b00 0000 721c  ..rU...).r....r.
+00001080: 0000 0072 1d00 0000 721e 0000 0072 4c00  ...r....r....rL.
+00001090: 0000 7234 0000 0072 3700 0000 722c 0000  ..r4...r7...r,..
+000010a0: 0072 3600 0000 724b 0000 0072 5000 0000  .r6...rK...rP...
+000010b0: 7231 0000 00da 076d 6172 6b65 7273 721f  r1.....markersr.
+000010c0: 0000 0072 1f00 0000 7220 0000 0072 5700  ...r....r ...rW.
+000010d0: 0000 7700 0000 7322 0000 0000 020c 0208  ..w...s"........
+000010e0: 020a 010a 0110 020a 020e 0102 ff02 0102  ................
+000010f0: ff04 030a 0108 0210 010e 0108 027a 124b  .............z.K
+00001100: 6d65 616e 7343 6c75 7374 6572 2e70 6f73  meansCluster.pos
+00001110: 744e a904 7223 0000 0072 2400 0000 7225  tN..r#...r$...r%
+00001120: 0000 0072 5700 0000 721f 0000 0072 1f00  ...rW...r....r..
+00001130: 0000 721f 0000 0072 2000 0000 725b 0000  ..r....r ...r[..
+00001140: 0075 0000 0073 0200 0000 0802 725b 0000  .u...s......r[..
+00001150: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001160: 0000 0200 0000 4000 0000 7314 0000 0065  ......@...s....e
+00001170: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
+00001180: 0353 0029 04da 1147 6574 436c 7573 7465  .S.)...GetCluste
+00001190: 7243 6f6e 7465 6e74 6302 0000 0000 0000  rContentc.......
+000011a0: 0000 0000 0010 0000 0009 0000 004f 0000  .............O..
+000011b0: 0073 c200 0000 7400 7c01 6a01 6401 8d01  .s....t.|.j.d...
+000011c0: 7d04 7c04 a002 a100 72b2 7c04 6a03 6402  }.|.....r.|.j.d.
+000011d0: 1900 7d05 7c00 a004 7c04 6a03 6403 1900  ..}.|...|.j.d...
+000011e0: a101 7d06 7c00 a004 7c04 6a03 6404 1900  ..}.|...|.j.d...
+000011f0: a101 7d07 7c04 6a03 6405 1900 7d08 7c00  ..}.|.j.d...}.|.
+00001200: 6a05 7c05 7406 7c08 6406 7c06 7c01 6606  j.|.t.|.d.|.|.f.
+00001210: 7c03 8e01 7d09 7c04 6a03 6407 1900 7d0a  |...}.|.j.d...}.
+00001220: 7c04 6a03 6408 1900 7d0b 7c04 6a03 6409  |.j.d...}.|.j.d.
+00001230: 1900 7d0c 7c03 640a 1900 7d0d 7c09 6a07  ..}.|.d...}.|.j.
+00001240: 7c05 7c0a 7c0b 7c0c 7c08 7c0d 7c07 640b  |.|.|.|.|.|.|.d.
+00001250: 8d07 7d0e 7c00 a008 7c09 7c0e a102 7d0f  ..}.|...|.|...}.
+00001260: 7409 7c0f 8301 5300 7409 7c04 6a0a 740b  t.|...S.t.|.j.t.
+00001270: 6a0c 640c 8d02 5300 290d 4e72 4f00 0000  j.d...S.).NrO...
+00001280: 7234 0000 0072 2c00 0000 da0a 696e 7075  r4...r,.....inpu
+00001290: 745f 7372 6964 7236 0000 0046 da03 6964  t_sridr6...F..id
+000012a0: 73da 0178 da01 7972 3100 0000 2901 725f  s..x..yr1...).r_
+000012b0: 0000 0072 0800 0000 290d 7212 0000 0072  ...r....).r....r
+000012c0: 4a00 0000 7251 0000 0072 5200 0000 722d  J...rQ...rR...r-
+000012d0: 0000 0072 3900 0000 720f 0000 005a 1a67  ...r9...r....Z.g
+000012e0: 6574 5f6b 6d65 616e 735f 636c 7573 7465  et_kmeans_cluste
+000012f0: 725f 636f 6e74 656e 7472 4d00 0000 7206  r_contentrM...r.
+00001300: 0000 0072 5400 0000 7209 0000 0072 5500  ...rT...r....rU.
+00001310: 0000 2910 721b 0000 0072 1c00 0000 721d  ..).r....r....r.
+00001320: 0000 0072 1e00 0000 724c 0000 0072 3400  ...r....rL...r4.
+00001330: 0000 722c 0000 0072 5f00 0000 7236 0000  ..r,...r_...r6..
+00001340: 0072 4b00 0000 7260 0000 0072 6100 0000  .rK...r`...ra...
+00001350: 7262 0000 0072 3100 0000 5a0f 636c 7573  rb...r1...Z.clus
+00001360: 7465 725f 636f 6e74 656e 7472 4a00 0000  ter_contentrJ...
+00001370: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00001380: 5700 0000 9500 0000 732a 0000 0000 020c  W.......s*......
+00001390: 0208 020a 0110 0110 020a 020e 0102 ff02  ................
+000013a0: 0102 ff04 030a 010a 010a 0208 0210 0102  ................
+000013b0: ff06 030c 0208 027a 1647 6574 436c 7573  .......z.GetClus
+000013c0: 7465 7243 6f6e 7465 6e74 2e70 6f73 744e  terContent.postN
+000013d0: 725d 0000 0072 1f00 0000 721f 0000 0072  r]...r....r....r
+000013e0: 1f00 0000 7220 0000 0072 5e00 0000 9300  ....r ...r^.....
+000013f0: 0000 7302 0000 0008 0272 5e00 0000 6300  ..s......r^...c.
+00001400: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00001410: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
+00001420: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
+00001430: 2904 da0e 4765 7441 7265 6143 6f6e 7465  )...GetAreaConte
+00001440: 6e74 6302 0000 0000 0000 0000 0000 000e  ntc.............
+00001450: 0000 0007 0000 004f 0000 0073 aa00 0000  .......O...s....
+00001460: 7400 7c01 6a01 6401 8d01 7d04 7c04 a002  t.|.j.d...}.|...
+00001470: a100 729a 7c04 6a03 6402 1900 7d05 7c00  ..r.|.j.d...}.|.
+00001480: a004 7c04 6a03 6403 1900 a101 7d06 7c04  ..|.j.d.....}.|.
+00001490: 6a03 a005 6404 6400 a102 7d07 7c04 6a03  j...d.d...}.|.j.
+000014a0: a005 6405 6400 a102 7d08 7c04 6a03 6406  ..d.d...}.|.j.d.
+000014b0: 1900 7d09 7c00 6a06 7c05 7407 7c09 6407  ..}.|.j.|.t.|.d.
+000014c0: 7c06 7c01 6606 7c03 8e01 7d0a 7c04 6a03  |.|.f.|...}.|.j.
+000014d0: 6408 1900 7d0b 7c0a a008 7c0b 7c09 7c07  d...}.|...|.|.|.
+000014e0: 7c08 a104 7d0c 7c00 a009 7c0a 7c0c a102  |...}.|...|.|...
+000014f0: 7d0d 740a 7c0d 8301 5300 740a 7c04 6a0b  }.t.|...S.t.|.j.
+00001500: 740c 6a0d 6409 8d02 5300 290a 4e72 4f00  t.j.d...S.).NrO.
+00001510: 0000 7234 0000 0072 2c00 0000 da05 6c69  ..r4...r,.....li
+00001520: 6d69 74da 066f 6666 7365 7472 3600 0000  mit..offsetr6...
+00001530: 4672 5000 0000 7208 0000 0029 0e72 1500  FrP...r....).r..
+00001540: 0000 724a 0000 0072 5100 0000 7252 0000  ..rJ...rQ...rR..
+00001550: 0072 2d00 0000 7221 0000 0072 3900 0000  .r-...r!...r9...
+00001560: 720f 0000 005a 1067 6574 5f61 7265 615f  r....Z.get_area_
+00001570: 636f 6e74 656e 7472 4d00 0000 7206 0000  contentrM...r...
+00001580: 0072 5400 0000 7209 0000 0072 5500 0000  .rT...r....rU...
+00001590: 290e 721b 0000 0072 1c00 0000 721d 0000  ).r....r....r...
+000015a0: 0072 1e00 0000 724c 0000 0072 3400 0000  .r....rL...r4...
+000015b0: 722c 0000 0072 6400 0000 7265 0000 0072  r,...rd...re...r
+000015c0: 3600 0000 724b 0000 0072 5000 0000 5a0c  6...rK...rP...Z.
+000015d0: 6172 6561 5f63 6f6e 7465 6e74 724a 0000  area_contentrJ..
+000015e0: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+000015f0: 7257 0000 00ba 0000 0073 2200 0000 0002  rW.......s".....
+00001600: 0c02 0802 0a01 1002 0e01 0e02 0a02 0e01  ................
+00001610: 02ff 0201 02ff 0403 0a02 1002 0c02 0802  ................
+00001620: 7a13 4765 7441 7265 6143 6f6e 7465 6e74  z.GetAreaContent
+00001630: 2e70 6f73 744e 725d 0000 0072 1f00 0000  .postNr]...r....
+00001640: 721f 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+00001650: 6300 0000 b800 0000 7302 0000 0008 0272  c.......s......r
+00001660: 6300 0000 6300 0000 0000 0000 0000 0000  c...c...........
+00001670: 0000 0000 0002 0000 0040 0000 0073 1400  .........@...s..
+00001680: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+00001690: 5a03 6403 5300 2904 da11 4765 7444 6174  Z.d.S.)...GetDat
+000016a0: 6173 6574 436f 6e74 656e 7463 0200 0000  asetContentc....
+000016b0: 0000 0000 0000 0000 0b00 0000 0700 0000  ................
+000016c0: 4f00 0000 7352 0000 007c 016a 00a0 0164  O...sR...|.j...d
+000016d0: 0164 02a1 027d 0467 007d 057c 006a 0274  .d...}.g.}.|.j.t
+000016e0: 0374 047c 0564 037c 047c 0166 067c 038e  .t.|.d.|.|.f.|..
+000016f0: 017d 067c 0364 0419 007d 077c 06a0 057c  .}.|.d...}.|...|
+00001700: 07a1 017d 0874 067c 0883 017d 097c 096a  ...}.t.|...}.|.j
+00001710: 077d 0a74 087c 0a83 0153 0029 054e 722c  .}.t.|...S.).Nr,
+00001720: 0000 0069 e610 0000 46da 0a64 6174 6173  ...i....F..datas
+00001730: 6574 5f69 6429 09da 0347 4554 7221 0000  et_id)...GETr!..
+00001740: 0072 3900 0000 720c 0000 0072 0e00 0000  .r9...r....r....
+00001750: 5a13 6765 745f 6461 7461 7365 745f 636f  Z.get_dataset_co
+00001760: 6e74 656e 7472 4900 0000 724a 0000 0072  ntentrI...rJ...r
+00001770: 0600 0000 290b 721b 0000 0072 1c00 0000  ....).r....r....
+00001780: 721d 0000 0072 1e00 0000 722c 0000 0072  r....r....r,...r
+00001790: 3600 0000 724b 0000 0072 6700 0000 da07  6...rK...rg.....
+000017a0: 6461 7461 7365 7472 4c00 0000 724a 0000  datasetrL...rJ..
+000017b0: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+000017c0: 7221 0000 00d9 0000 0073 1800 0000 0002  r!.......s......
+000017d0: 0e02 0402 0e01 02ff 0201 02ff 0403 0802  ................
+000017e0: 0a02 0801 0602 7a15 4765 7444 6174 6173  ......z.GetDatas
+000017f0: 6574 436f 6e74 656e 742e 6765 744e 7222  etContent.getNr"
+00001800: 0000 0072 1f00 0000 721f 0000 0072 1f00  ...r....r....r..
+00001810: 0000 7220 0000 0072 6600 0000 d700 0000  ..r ...rf.......
+00001820: 7302 0000 0008 0272 6600 0000 6300 0000  s......rf...c...
+00001830: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00001840: 0040 0000 0073 1400 0000 6500 5a01 6400  .@...s....e.Z.d.
+00001850: 5a02 6401 6402 8400 5a03 6403 5300 2904  Z.d.d...Z.d.S.).
+00001860: da12 4765 744d 6170 436f 6e74 656e 7443  ..GetMapContentC
+00001870: 6f75 6e74 6302 0000 0000 0000 0000 0000  ountc...........
+00001880: 000e 0000 0007 0000 004f 0000 0073 a000  .........O...s..
+00001890: 0000 7400 7c01 6a01 6401 8d01 7d04 7c04  ..t.|.j.d...}.|.
+000018a0: a002 a100 7290 6402 7d05 7c04 6a03 6403  ....r.d.}.|.j.d.
+000018b0: 1900 7d06 7c04 6a03 6404 1900 7d07 7c00  ..}.|.j.d...}.|.
+000018c0: a004 7c04 6a03 6405 1900 a101 7d08 7c04  ..|.j.d.....}.|.
+000018d0: 6a03 6406 1900 7d09 7c03 6407 1900 7d0a  j.d...}.|.d...}.
+000018e0: 7c04 6a03 6408 1900 7d0b 7c00 6a05 7c07  |.j.d...}.|.j.|.
+000018f0: 7406 7c06 7c05 7c08 7c01 6606 7c03 8e01  t.|.|.|.|.f.|...
+00001900: 7d0c 7c0c a007 7c09 7c07 7c06 7c0a 7c0b  }.|...|.|.|.|.|.
+00001910: a105 7d0d 7408 7c0d 7409 6a0a 6409 8d02  ..}.t.|.t.j.d...
+00001920: 5300 7408 7c04 6a0b 7409 6a0c 6409 8d02  S.t.|.j.t.j.d...
+00001930: 5300 290a 4e72 4f00 0000 5472 3600 0000  S.).NrO...Tr6...
+00001940: 7234 0000 0072 2c00 0000 7250 0000 0072  r4...r,...rP...r
+00001950: 3100 0000 da0b 6d6f 6475 6c61 7469 6f6e  1.....modulation
+00001960: 7372 0800 0000 290d 7213 0000 0072 4a00  sr....).r....rJ.
+00001970: 0000 7251 0000 0072 5200 0000 722d 0000  ..rQ...rR...r-..
+00001980: 0072 3900 0000 720f 0000 005a 1667 6574  .r9...r....Z.get
+00001990: 5f6d 6170 5f63 6f6e 7465 6e74 5f63 6f75  _map_content_cou
+000019a0: 6e74 7372 0600 0000 7209 0000 0072 5300  ntsr....r....rS.
+000019b0: 0000 7254 0000 0072 5500 0000 290e 721b  ..rT...rU...).r.
+000019c0: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+000019d0: 0000 724c 0000 0072 3700 0000 7236 0000  ..rL...r7...r6..
+000019e0: 0072 3400 0000 722c 0000 0072 5000 0000  .r4...r,...rP...
+000019f0: 7231 0000 0072 6b00 0000 724b 0000 005a  r1...rk...rK...Z
+00001a00: 126d 6170 5f63 6f6e 7465 6e74 5f63 6f75  .map_content_cou
+00001a10: 6e74 7372 1f00 0000 721f 0000 0072 2000  ntsr....r....r .
+00001a20: 0000 7257 0000 00ee 0000 0073 2200 0000  ..rW.......s"...
+00001a30: 0002 0c02 0802 0401 0a01 0a01 1002 0a01  ................
+00001a40: 0801 0a02 0e01 02ff 0201 02ff 0403 1202  ................
+00001a50: 0e02 7a17 4765 744d 6170 436f 6e74 656e  ..z.GetMapConten
+00001a60: 7443 6f75 6e74 2e70 6f73 744e 725d 0000  tCount.postNr]..
+00001a70: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00001a80: 7220 0000 0072 6a00 0000 ec00 0000 7302  r ...rj.......s.
+00001a90: 0000 0008 0272 6a00 0000 6300 0000 0000  .....rj...c.....
+00001aa0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00001ab0: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00001ac0: 6401 6402 8400 5a03 6403 5300 2904 da15  d.d...Z.d.S.)...
+00001ad0: 4765 7447 726f 7570 6564 4d61 7043 6f6e  GetGroupedMapCon
+00001ae0: 7465 6e74 7363 0200 0000 0000 0000 0000  tentsc..........
+00001af0: 0000 0e00 0000 0700 0000 4f00 0000 73a8  ..........O...s.
+00001b00: 0000 0074 007c 016a 0164 018d 017d 047c  ...t.|.j.d...}.|
+00001b10: 04a0 02a1 0072 9864 027d 057c 046a 0364  .....r.d.}.|.j.d
+00001b20: 0319 007d 067c 046a 0364 0419 007d 077c  ...}.|.j.d...}.|
+00001b30: 00a0 047c 046a 0364 0519 00a1 017d 087c  ...|.j.d.....}.|
+00001b40: 046a 0364 0619 007d 097c 0364 0719 007d  .j.d...}.|.d...}
+00001b50: 0a7c 046a 0364 0819 007d 0b7c 006a 057c  .|.j.d...}.|.j.|
+00001b60: 0774 067c 067c 057c 087c 0166 067c 038e  .t.|.|.|.|.f.|..
+00001b70: 017d 0c7c 0ca0 077c 097c 077c 0a7c 067c  .}.|...|.|.|.|.|
+00001b80: 0ba1 057d 0d74 087c 0d83 0101 0074 097c  ...}.t.|.....t.|
+00001b90: 0d74 0a6a 0b64 098d 0253 0074 097c 046a  .t.j.d...S.t.|.j
+00001ba0: 0c74 0a6a 0d64 098d 0253 0029 0a4e 724f  .t.j.d...S.).NrO
+00001bb0: 0000 0054 7236 0000 0072 3400 0000 722c  ...Tr6...r4...r,
+00001bc0: 0000 0072 5000 0000 7231 0000 00da 0867  ...rP...r1.....g
+00001bd0: 726f 7570 5f62 7972 0800 0000 290e 7214  roup_byr....).r.
+00001be0: 0000 0072 4a00 0000 7251 0000 0072 5200  ...rJ...rQ...rR.
+00001bf0: 0000 722d 0000 0072 3900 0000 720f 0000  ..r-...r9...r...
+00001c00: 005a 1867 6574 5f67 726f 7570 6564 5f6d  .Z.get_grouped_m
+00001c10: 6170 5f63 6f6e 7465 6e74 73da 0570 7269  ap_contents..pri
+00001c20: 6e74 7206 0000 0072 0900 0000 7253 0000  ntr....r....rS..
+00001c30: 0072 5400 0000 7255 0000 0029 0e72 1b00  .rT...rU...).r..
+00001c40: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00001c50: 0072 4c00 0000 7237 0000 0072 3600 0000  .rL...r7...r6...
+00001c60: 7234 0000 0072 2c00 0000 7250 0000 0072  r4...r,...rP...r
+00001c70: 3100 0000 726d 0000 0072 4b00 0000 da06  1...rm...rK.....
+00001c80: 6772 6f75 7073 721f 0000 0072 1f00 0000  groupsr....r....
+00001c90: 7220 0000 0072 5700 0000 0901 0000 7324  r ...rW.......s$
+00001ca0: 0000 0000 020c 0208 0204 010a 010a 0110  ................
+00001cb0: 020a 0108 020a 020e 0102 ff02 0102 ff04  ................
+00001cc0: 0312 0208 020e 027a 1a47 6574 4772 6f75  .......z.GetGrou
+00001cd0: 7065 644d 6170 436f 6e74 656e 7473 2e70  pedMapContents.p
+00001ce0: 6f73 744e 725d 0000 0072 1f00 0000 721f  ostNr]...r....r.
+00001cf0: 0000 0072 1f00 0000 7220 0000 0072 6c00  ...r....r ...rl.
+00001d00: 0000 0701 0000 7302 0000 0008 0272 6c00  ......s......rl.
+00001d10: 0000 292a da0b 646a 616e 676f 2e63 6f6e  ..)*..django.con
+00001d20: 6672 0200 0000 da0b 646a 616e 676f 2e63  fr......django.c
+00001d30: 6f72 6572 0300 0000 da14 7265 7374 5f66  orer......rest_f
+00001d40: 7261 6d65 776f 726b 2e76 6965 7773 7204  ramework.viewsr.
+00001d50: 0000 00da 1772 6573 745f 6672 616d 6577  .....rest_framew
+00001d60: 6f72 6b2e 7265 7370 6f6e 7365 7206 0000  ork.responser...
+00001d70: 00da 1872 6573 745f 6672 616d 6577 6f72  ...rest_framewor
+00001d80: 6b2e 7265 6e64 6572 6572 7372 0700 0000  k.renderersr....
+00001d90: da0e 7265 7374 5f66 7261 6d65 776f 726b  ..rest_framework
+00001da0: 7209 0000 005a 1761 6e79 636c 7573 7465  r....Z.anycluste
+00001db0: 722e 4d61 7043 6c75 7374 6572 6572 720a  r.MapClustererr.
+00001dc0: 0000 0072 0b00 0000 da16 616e 7963 6c75  ...r......anyclu
+00001dd0: 7374 6572 2e64 6566 696e 6974 696f 6e73  ster.definitions
+00001de0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00001df0: 0f00 0000 7211 0000 0072 1200 0000 7213  ....r....r....r.
+00001e00: 0000 0072 1400 0000 7215 0000 00da 0a61  ...r....r......a
+00001e10: 6e79 636c 7573 7465 7272 1600 0000 5a10  nyclusterr....Z.
+00001e20: 616e 7963 6c75 7374 6572 2e75 7469 6c73  anycluster.utils
+00001e30: 7217 0000 00da 0767 6574 6174 7472 5a13  r......getattrZ.
+00001e40: 6769 735f 7365 7269 616c 697a 6572 5f70  gis_serializer_p
+00001e50: 6174 6872 4900 0000 da04 6a73 6f6e 7219  athrI.....jsonr.
+00001e60: 0000 0072 2600 0000 724e 0000 0072 5b00  ...r&...rN...r[.
+00001e70: 0000 725e 0000 0072 6300 0000 7266 0000  ..r^...rc...rf..
+00001e80: 0072 6a00 0000 726c 0000 0072 1f00 0000  .rj...rl...r....
+00001e90: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00001ea0: 083c 6d6f 6475 6c65 3e01 0000 0073 2c00  .<module>....s,.
+00001eb0: 0000 0c01 0c02 0c01 0c01 0c01 0c02 1001  ................
+00001ec0: 1802 1c03 0c01 0c02 0c01 0802 0802 1006  ................
+00001ed0: 0e38 1220 121e 1225 121f 1215 121b       .8. ...%......
```

### Comparing `anycluster-2.3.0/anycluster/api/json_schemas.py` & `anycluster-2.3.1/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/serializers.py` & `anycluster-2.3.1/anycluster/api/serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.3.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/tests/test_serializers.py` & `anycluster-2.3.1/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/tests/test_views.py` & `anycluster-2.3.1/anycluster/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/urls.py` & `anycluster-2.3.1/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/api/views.py` & `anycluster-2.3.1/anycluster/api/views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/clusters.py` & `anycluster-2.3.1/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/definitions.py` & `anycluster-2.3.1/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/globalmaptiles.py` & `anycluster-2.3.1/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/10.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/100.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/1000.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/10000.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/5.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/50.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.3.1/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.3.1/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.3.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.3.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.3.1/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc` & `anycluster-2.3.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc` & `anycluster-2.3.1/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/common.py` & `anycluster-2.3.1/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/mixins.py` & `anycluster-2.3.1/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/test_ClusterCache.py` & `anycluster-2.3.1/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/test_FilterComposer.py` & `anycluster-2.3.1/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster/tests/test_MapClusterer.py` & `anycluster-2.3.1/anycluster/tests/test_MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/anycluster.egg-info/PKG-INFO` & `anycluster-2.3.1/anycluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.3.0
+Version: 2.3.1
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.3.0/anycluster.egg-info/SOURCES.txt` & `anycluster-2.3.1/anycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anycluster-2.3.0/setup.py` & `anycluster-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.3.0',
+    version='2.3.1',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

