# Comparing `tmp/vatis_asr_commons-2.0.1.tar.gz` & `tmp/vatis_asr_commons-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vatis_asr_commons-2.0.1.tar", last modified: Mon Jun 12 05:57:53 2023, max compression
+gzip compressed data, was "dist/vatis_asr_commons-2.0.2.tar", last modified: Mon Jun 12 09:59:20 2023, max compression
```

## Comparing `vatis_asr_commons-2.0.1.tar` & `vatis_asr_commons-2.0.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/
--rw-r--r--   0 mac        (501) staff       (20)      601 2021-09-17 07:50:18.000000 vatis_asr_commons-2.0.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)       72 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      931 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      845 2023-01-21 11:08:04.000000 vatis_asr_commons-2.0.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/requirements/
--rw-r--r--   0 mac        (501) staff       (20)       53 2023-06-08 08:43:17.000000 vatis_asr_commons-2.0.1/requirements/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       79 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1906 2023-05-01 06:49:20.000000 vatis_asr_commons-2.0.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/
--rw-r--r--   0 mac        (501) staff       (20)        0 2021-11-19 07:42:07.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/config/
--rw-r--r--   0 mac        (501) staff       (20)      540 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/config/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6360 2023-04-09 20:40:42.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/config/audio.py
--rw-r--r--   0 mac        (501) staff       (20)      740 2022-08-01 15:26:57.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/config/headers.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/config/logging.py
--rw-r--r--   0 mac        (501) staff       (20)     7643 2023-03-10 11:08:30.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/config/parse.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/constants/
--rw-r--r--   0 mac        (501) staff       (20)       89 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/constants/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)       21 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/constants/custom_models.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/custom_models/
--rw-r--r--   0 mac        (501) staff       (20)     1014 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/custom_models/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/custom_models/en_GB.py
--rw-r--r--   0 mac        (501) staff       (20)     1112 2023-01-21 11:08:04.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/custom_models/model.py
--rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/custom_models/ro_RO.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/
--rw-r--r--   0 mac        (501) staff       (20)     1702 2023-03-07 11:38:19.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      717 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/exception.py
--rw-r--r--   0 mac        (501) staff       (20)     2146 2023-03-07 10:36:16.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/expression.py
--rw-r--r--   0 mac        (501) staff       (20)     7410 2023-03-10 10:46:39.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/find_replace.py
--rw-r--r--   0 mac        (501) staff       (20)      158 2023-04-28 08:59:22.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/speaker.py
--rw-r--r--   0 mac        (501) staff       (20)     1703 2023-02-04 10:23:36.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/spoken_commands.py
--rw-r--r--   0 mac        (501) staff       (20)     8330 2023-03-06 21:08:28.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/transcriber.py
--rw-r--r--   0 mac        (501) staff       (20)     2599 2023-04-26 19:11:33.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/domain/word.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/
--rw-r--r--   0 mac        (501) staff       (20)       87 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      212 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/i18n_keys.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/en/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/
--rw-r--r--   0 mac        (501) staff       (20)      178 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.mo
--rw-r--r--   0 mac        (501) staff       (20)      132 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.po
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/ro/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/
--rw-r--r--   0 mac        (501) staff       (20)      179 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.mo
--rw-r--r--   0 mac        (501) staff       (20)      133 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.po
--rw-r--r--   0 mac        (501) staff       (20)      114 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/locale/speakers_service.pot
--rw-r--r--   0 mac        (501) staff       (20)     2822 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/translate.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/json/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-01-22 13:07:30.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/json/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      139 2023-01-22 13:21:45.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/json/deserialization.py
--rw-r--r--   0 mac        (501) staff       (20)      106 2023-01-22 13:11:37.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/json/serialization.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/live/
--rw-r--r--   0 mac        (501) staff       (20)      333 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/live/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1325 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/live/event.py
--rw-r--r--   0 mac        (501) staff       (20)     1629 2023-03-03 19:52:10.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/live/headers.py
--rw-r--r--   0 mac        (501) staff       (20)      127 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/live/response.py
--rw-r--r--   0 mac        (501) staff       (20)       98 2021-09-17 07:02:12.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/live/sio_topics.py
--rw-r--r--   0 mac        (501) staff       (20)     1268 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/live/utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/scaler/
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/scaler/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      155 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/scaler/response.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/security/
--rw-r--r--   0 mac        (501) staff       (20)       75 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/security/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      138 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/security/jwt.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/static/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-01-23 09:41:24.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/static/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      457 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/static/exceptions.py
--rw-r--r--   0 mac        (501) staff       (20)       62 2022-04-14 11:35:28.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/static/headers.py
--rw-r--r--   0 mac        (501) staff       (20)     4532 2023-02-04 10:23:36.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/static/request.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-08 08:14:19.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7995 2023-06-11 15:38:29.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/cache.py
--rw-r--r--   0 mac        (501) staff       (20)       46 2023-06-08 10:11:19.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/exception.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/
--rw-r--r--   0 mac        (501) staff       (20)      476 2023-06-10 08:18:12.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      706 2023-06-11 15:38:29.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/local_object.py
--rw-r--r--   0 mac        (501) staff       (20)     6354 2023-06-11 16:29:29.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/s3_object.py
--rw-r--r--   0 mac        (501) staff       (20)     2374 2023-06-11 15:38:29.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/stored_object.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/utils/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-08 08:43:17.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      295 2023-06-08 09:59:27.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/utils/file.py
--rw-r--r--   0 mac        (501) staff       (20)      562 2023-06-08 08:43:17.000000 vatis_asr_commons-2.0.1/vatis/asr_commons/utils/parse.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      931 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2577 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2021-09-17 07:17:20.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)       53 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-12 05:57:53.000000 vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/
+-rw-r--r--   0 mac        (501) staff       (20)      601 2021-09-17 07:50:18.000000 vatis_asr_commons-2.0.2/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)       72 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      931 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      845 2023-01-21 11:08:04.000000 vatis_asr_commons-2.0.2/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/requirements/
+-rw-r--r--   0 mac        (501) staff       (20)       53 2023-06-08 08:43:17.000000 vatis_asr_commons-2.0.2/requirements/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       79 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1906 2023-06-12 05:58:19.000000 vatis_asr_commons-2.0.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2021-11-19 07:42:07.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/config/
+-rw-r--r--   0 mac        (501) staff       (20)      540 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/config/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6360 2023-04-09 20:40:42.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/config/audio.py
+-rw-r--r--   0 mac        (501) staff       (20)      740 2022-08-01 15:26:57.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/config/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)     1950 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/config/logging.py
+-rw-r--r--   0 mac        (501) staff       (20)     7643 2023-03-10 11:08:30.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/config/parse.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/constants/
+-rw-r--r--   0 mac        (501) staff       (20)       89 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/constants/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)       21 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/constants/custom_models.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/custom_models/
+-rw-r--r--   0 mac        (501) staff       (20)     1014 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/custom_models/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/custom_models/en_GB.py
+-rw-r--r--   0 mac        (501) staff       (20)     1112 2023-01-21 11:08:04.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/custom_models/model.py
+-rw-r--r--   0 mac        (501) staff       (20)      367 2021-12-22 09:34:48.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/custom_models/ro_RO.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/
+-rw-r--r--   0 mac        (501) staff       (20)     1702 2023-03-07 11:38:19.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      717 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/exception.py
+-rw-r--r--   0 mac        (501) staff       (20)     2146 2023-03-07 10:36:16.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/expression.py
+-rw-r--r--   0 mac        (501) staff       (20)     7410 2023-03-10 10:46:39.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/find_replace.py
+-rw-r--r--   0 mac        (501) staff       (20)      158 2023-04-28 08:59:22.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/speaker.py
+-rw-r--r--   0 mac        (501) staff       (20)     1703 2023-02-04 10:23:36.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/spoken_commands.py
+-rw-r--r--   0 mac        (501) staff       (20)     8330 2023-03-06 21:08:28.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/transcriber.py
+-rw-r--r--   0 mac        (501) staff       (20)     2599 2023-04-26 19:11:33.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/domain/word.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/
+-rw-r--r--   0 mac        (501) staff       (20)       87 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      212 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/i18n_keys.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/en/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/
+-rw-r--r--   0 mac        (501) staff       (20)      178 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.mo
+-rw-r--r--   0 mac        (501) staff       (20)      132 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/en/LC_MESSAGES/speakers_service.po
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/ro/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 mac        (501) staff       (20)      179 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.mo
+-rw-r--r--   0 mac        (501) staff       (20)      133 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/ro/LC_MESSAGES/speakers_service.po
+-rw-r--r--   0 mac        (501) staff       (20)      114 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/locale/speakers_service.pot
+-rw-r--r--   0 mac        (501) staff       (20)     2822 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/translate.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/json/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-01-22 13:07:30.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/json/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      139 2023-01-22 13:21:45.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/json/deserialization.py
+-rw-r--r--   0 mac        (501) staff       (20)      106 2023-01-22 13:11:37.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/json/serialization.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/live/
+-rw-r--r--   0 mac        (501) staff       (20)      333 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/live/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1325 2022-06-13 15:12:59.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/live/event.py
+-rw-r--r--   0 mac        (501) staff       (20)     1629 2023-03-03 19:52:10.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/live/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)      127 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/live/response.py
+-rw-r--r--   0 mac        (501) staff       (20)       98 2021-09-17 07:02:12.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/live/sio_topics.py
+-rw-r--r--   0 mac        (501) staff       (20)     1268 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/live/utils.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/scaler/
+-rw-r--r--   0 mac        (501) staff       (20)       71 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/scaler/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      155 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/scaler/response.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/security/
+-rw-r--r--   0 mac        (501) staff       (20)       75 2021-11-23 05:52:54.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/security/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      138 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/security/jwt.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/static/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2022-01-23 09:41:24.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/static/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      457 2022-04-12 09:25:40.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/static/exceptions.py
+-rw-r--r--   0 mac        (501) staff       (20)       62 2022-04-14 11:35:28.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/static/headers.py
+-rw-r--r--   0 mac        (501) staff       (20)     4532 2023-02-04 10:23:36.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/static/request.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-08 08:14:19.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     7995 2023-06-11 15:38:29.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/cache.py
+-rw-r--r--   0 mac        (501) staff       (20)       46 2023-06-08 10:11:19.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/exception.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/
+-rw-r--r--   0 mac        (501) staff       (20)      494 2023-06-12 09:46:31.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      706 2023-06-11 15:38:29.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/local_object.py
+-rw-r--r--   0 mac        (501) staff       (20)     6901 2023-06-12 09:56:31.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/s3_object.py
+-rw-r--r--   0 mac        (501) staff       (20)     2374 2023-06-11 15:38:29.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/stored_object.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/utils/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-06-08 08:43:17.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      295 2023-06-08 09:59:27.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/utils/file.py
+-rw-r--r--   0 mac        (501) staff       (20)      562 2023-06-08 08:43:17.000000 vatis_asr_commons-2.0.2/vatis/asr_commons/utils/parse.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      931 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2577 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2021-09-17 07:17:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (501) staff       (20)       53 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        6 2023-06-12 09:59:20.000000 vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/top_level.txt
```

### Comparing `vatis_asr_commons-2.0.1/LICENSE.txt` & `vatis_asr_commons-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/PKG-INFO` & `vatis_asr_commons-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vatis_asr_commons
-Version: 2.0.1
+Version: 2.0.2
 Summary: Common objects for Vatis ASR clients
 Home-page: https://gitlab.com/vatistech/asr-commons
 Maintainer: VATIS TECH
 Maintainer-email: support@vatis.tech
 License: UNKNOWN
-Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/2.0.1/asr_commons-2.0.1.zip
+Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/2.0.2/asr_commons-2.0.2.zip
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vatis_asr_commons-2.0.1/README.md` & `vatis_asr_commons-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/setup.py` & `vatis_asr_commons-2.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import find_namespace_packages, setup
 
 __name__ = 'vatis_asr_commons'
-__tag__ = '2.0.1'
+__tag__ = '2.0.2'
 __short_description__ = 'Common objects for Vatis ASR clients'
 __download_url__ = 'https://gitlab.com/vatistech/asr-commons/-/archive/{__tag__}/asr_commons-{__tag__}.zip'\
     .format(__tag__=__tag__)
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
```

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/config/__init__.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/config/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/config/audio.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/config/audio.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/config/headers.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/config/headers.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/config/logging.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/config/logging.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/config/parse.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/config/parse.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/custom_models/__init__.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/custom_models/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/custom_models/model.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/custom_models/model.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/domain/__init__.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/domain/exception.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/domain/exception.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/domain/expression.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/domain/expression.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/domain/find_replace.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/domain/find_replace.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/domain/spoken_commands.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/domain/spoken_commands.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/domain/transcriber.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/domain/transcriber.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/domain/word.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/domain/word.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/i18n/translate.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/i18n/translate.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/live/event.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/live/event.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/live/headers.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/live/headers.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/live/utils.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/live/utils.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/static/request.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/static/request.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/storage/cache.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/storage/cache.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/local_object.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/local_object.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/s3_object.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/s3_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,28 @@
 
     def size(self, follow_symlinks: bool = True) -> int:
         if not self.exists():
             return 0
 
         original_object: 'S3Object' = self._fetch_original_object() if follow_symlinks else self
 
-        return original_object._object.content_length
+        size: int = original_object._object.content_length
+
+        if original_object.is_dir(follow_symlinks=follow_symlinks):
+            bucket = original_object._s3.Bucket(original_object.bucket())
+            prefix: str = original_object.url().path + '/'
+
+            for obj in bucket.objects.filter(Prefix=prefix):
+                if obj.key != prefix:
+                    obj_url: ObjectUrl = S3Object.build_url(obj.bucket_name, obj.key)
+                    s3_obj: 'S3Object' = S3Object(obj_url)
+
+                    size += s3_obj.size(follow_symlinks=follow_symlinks)
+
+        return size
 
     def is_dir(self, follow_symlinks: bool = True) -> bool:
         if not self.exists():
             return False
 
         original_object: 'S3Object' = self._fetch_original_object() if follow_symlinks else self
```

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/storage/store/stored_object.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/storage/store/stored_object.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis/asr_commons/utils/parse.py` & `vatis_asr_commons-2.0.2/vatis/asr_commons/utils/parse.py`

 * *Files identical despite different names*

### Comparing `vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/PKG-INFO` & `vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: vatis-asr-commons
-Version: 2.0.1
+Version: 2.0.2
 Summary: Common objects for Vatis ASR clients
 Home-page: https://gitlab.com/vatistech/asr-commons
 Maintainer: VATIS TECH
 Maintainer-email: support@vatis.tech
 License: UNKNOWN
-Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/2.0.1/asr_commons-2.0.1.zip
+Download-URL: https://gitlab.com/vatistech/asr-commons/-/archive/2.0.2/asr_commons-2.0.2.zip
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `vatis_asr_commons-2.0.1/vatis_asr_commons.egg-info/SOURCES.txt` & `vatis_asr_commons-2.0.2/vatis_asr_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

