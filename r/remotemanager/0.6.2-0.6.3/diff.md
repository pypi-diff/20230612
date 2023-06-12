# Comparing `tmp/remotemanager-0.6.2.tar.gz` & `tmp/remotemanager-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.6.2.tar", last modified: Fri Jun  2 13:40:16 2023, max compression
+gzip compressed data, was "remotemanager-0.6.3.tar", last modified: Mon Jun 12 10:02:48 2023, max compression
```

## Comparing `remotemanager-0.6.2.tar` & `remotemanager-0.6.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.220122 remotemanager-0.6.2/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-02 13:40:16.220122 remotemanager-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.6.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-30 02:49:50.000000 remotemanager-0.6.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-30 02:49:50.000000 remotemanager-0.6.2/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15541 2023-05-30 02:49:50.000000 remotemanager-0.6.2/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12674 2023-05-31 07:19:00.000000 remotemanager-0.6.2/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.6.2/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.6.2/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.6.2/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.6.2/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    24726 2023-05-26 06:15:35.000000 remotemanager-0.6.2/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    48903 2023-05-25 09:38:01.000000 remotemanager-0.6.2/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22648 2023-06-01 14:41:40.000000 remotemanager-0.6.2/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-25 09:38:01.000000 remotemanager-0.6.2/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4043 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6496 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.6.2/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.6.2/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.6.2/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11552 2023-05-31 11:11:40.000000 remotemanager-0.6.2/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.216122 remotemanager-0.6.2/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.6.2/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.6.2/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9262 2023-06-02 09:40:16.000000 remotemanager-0.6.2/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.220122 remotemanager-0.6.2/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.6.2/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:40:16.212123 remotemanager-0.6.2/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-02 13:40:16.000000 remotemanager-0.6.2/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 13:40:16.220122 remotemanager-0.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-12 10:02:48.095340 remotemanager-0.6.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:45:06.000000 remotemanager-0.6.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-06-06 06:58:31.000000 remotemanager-0.6.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.087339 remotemanager-0.6.3/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-06-06 06:58:31.000000 remotemanager-0.6.3/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15718 2023-06-08 13:33:35.000000 remotemanager-0.6.3/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12674 2023-05-31 07:19:00.000000 remotemanager-0.6.3/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:29:09.000000 remotemanager-0.6.3/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:29:09.000000 remotemanager-0.6.3/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 09:38:01.000000 remotemanager-0.6.3/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:29:09.000000 remotemanager-0.6.3/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    24882 2023-06-08 11:36:38.000000 remotemanager-0.6.3/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    49754 2023-06-12 08:57:29.000000 remotemanager-0.6.3/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    22474 2023-06-12 08:57:29.000000 remotemanager-0.6.3/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-25 09:38:01.000000 remotemanager-0.6.3/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4325 2023-06-08 11:36:38.000000 remotemanager-0.6.3/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-08 11:36:38.000000 remotemanager-0.6.3/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-05-31 11:11:40.000000 remotemanager-0.6.3/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.091339 remotemanager-0.6.3/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.6.3/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2023-05-31 11:11:40.000000 remotemanager-0.6.3/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-06-06 06:58:31.000000 remotemanager-0.6.3/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-06-02 09:40:16.000000 remotemanager-0.6.3/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-02 10:52:35.000000 remotemanager-0.6.3/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9262 2023-06-02 09:40:16.000000 remotemanager-0.6.3/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.095340 remotemanager-0.6.3/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 12:56:19.000000 remotemanager-0.6.3/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 10:02:48.087339 remotemanager-0.6.3/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-12 10:02:48.000000 remotemanager-0.6.3/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 10:02:48.095340 remotemanager-0.6.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.6.3/setup.py
```

### Comparing `remotemanager-0.6.2/LICENSE` & `remotemanager-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/PKG-INFO` & `remotemanager-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.2
+Version: 0.6.3
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.2/README.md` & `remotemanager-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/pyproject.toml` & `remotemanager-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.6.2"
+current_version = "0.6.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.6.2/remotemanager/connection/cmd.py` & `remotemanager-0.6.3/remotemanager/connection/cmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import subprocess
 import getpass
 import time
 import warnings
 
+from remotemanager.utils.uuid import generate_uuid
 from remotemanager.connection.detect_locale_error import detect_locale_error
 from remotemanager.storage.sendablemixin import SendableMixin, Unloaded
 from remotemanager.logging import LoggingMixin
 
 
 def _process_redirect_file(file) -> [str, None]:
     if file is not None:
@@ -49,29 +50,29 @@
             time to wait before issuing a timeout
         max_timeouts (int):
             number of times to attempt communication in case of a timeout
         force_file (bool):
             always use the fexec method if True
     """
 
-    _temp_file = "tmp_cmd.sh"
-
     _do_not_package = ["_subprocess"]
 
     def __init__(
         self,
         cmd: str,
         asynchronous: bool = False,
         stdout: str = None,
         stderr: str = None,
         timeout: int = 5,
         max_timeouts: int = 3,
         raise_errors: bool = True,
         force_file: bool = False,
     ):
+        self._uuid = generate_uuid(f"{time.time()} {cmd}")
+
         self._cmd = cmd
         self._subprocess = None
         self._async = asynchronous
         self._force_file = force_file
         self._redirect = {
             "stdout": _process_redirect_file(stdout),
             "stderr": _process_redirect_file(stderr),
@@ -105,14 +106,26 @@
         self._pid = None
 
     def __repr__(self):
         stdout = self.stdout if self.stdout is not None else ""
         return stdout
 
     @property
+    def uuid(self):
+        return self._uuid
+
+    @property
+    def short_uuid(self):
+        return self._uuid[:8]
+
+    @property
+    def tempfile(self):
+        return f"{self.short_uuid}.sh"
+
+    @property
     def sent(self) -> str:
         """
         The command passed at initialisation
         """
         return self._cmd.__repr__()
 
     @property
@@ -126,34 +139,19 @@
     def is_redirected(self) -> bool:
         """
         True if the cmd is redirected to a file
         """
         return any([self._redirect["stdout"], self._redirect["stderr"]])
 
     def _get_return_attr(self, attr: str) -> [str, None]:
+        # subprocess objects cannot be serialised, check if we are post-reserialisation
         if isinstance(self._subprocess, Unloaded):
             self._logger.warning(f"broken subprocess, getting attr _{attr}")
             return getattr(self, f"_{attr}")
 
-        poll = self._subprocess.poll()
-        self._logger.info(f"cmd poll returned {poll}")
-        if poll is None or poll < 0:
-            self._logger.info("Falling back to communicate()")
-            return self.communicate()[attr]
-
-        self._logger.info(f"attempting to access the subprocess {attr} attr")
-        out = getattr(self._subprocess, attr, None)
-        if out is not None:
-            try:
-                self._stdout = str(out.read().strip())
-                return self._stdout
-            except ValueError as E:
-                self._logger.info(f"ValueError on read: {str(E)}")
-        self._logger.info("Falling back to communicate()")
-
         return self.communicate()[attr]
 
     @property
     def stdout(self) -> str:
         """
         Directly returns the stdout from the cmd execution. Attempts
         to communicate with the subprocess in the case of an async run.
@@ -162,15 +160,16 @@
 
         Returns (str):
             the stdout from the command execution
         """
         if self._stdout is not None:
             self._logger.info("returning cached stdout")
             return self._stdout
-        return self._get_return_attr("stdout")
+        self._stdout = self._get_return_attr("stdout")
+        return self._stdout
 
     @property
     def stderr(self) -> str:
         """
         Directly returns the stderr from the cmd execution. Attempts
         to communicate with the subprocess in the case of an async run.
 
@@ -178,15 +177,16 @@
 
         Returns (str):
             the stdout from the command execution
         """
         if self._stderr is not None:
             self._logger.info("returning cached stderr")
             return self._stderr
-        return self._get_return_attr("stderr")
+        self._stderr = self._get_return_attr("stderr")
+        return self._stderr
 
     @property
     def pwd(self) -> str:
         """
         Present working directory at command execution
 
         Returns None if the command has not been executed yet.
@@ -226,14 +226,17 @@
         Attempt to retrieve the returncode of the subprocess. This call will
         not disturb an asynchronous run, returning None
 
         Returns (int, None):
                 The exit status of the subprocess, None if it is still running.
                 None otherwise.
         """
+        if self._subprocess is None:
+            self._logger.info("attempted returncode call on non-exec CMD")
+            return None
         self._subprocess.poll()
         return self._subprocess.returncode
 
     @property
     def is_finished(self) -> bool:
         """
         Returns True if this command has finished execution. This will NOT talk
@@ -339,15 +342,15 @@
                 stdout passthrough
             stderr:
                 stderr passthrough
 
         Returns:
             None
         """
-        file = CMD._temp_file
+        file = self.tempfile
         with open(file, "w+") as o:
             o.write(self._cmd)
 
         self._redirect["execfile"] = file
 
         t0 = time.time()
         self._subprocess = subprocess.Popen(
@@ -426,17 +429,20 @@
 
         if self._raise_errors and not ignore_errors and err is not None and err != "":
             if detect_locale_error(err):
                 self._logger.warning(f"locale error detected: {err}")
             else:
                 raise RuntimeError(f"received the following stderr: \n{err}")
 
-        return {"stdout": _clean_output(std), "stderr": _clean_output(err)}
+        self._stdout = _clean_output(std)
+        self._stderr = _clean_output(err)
+
+        return {"stdout": self._stdout, "stderr": self._stderr}
 
-    def _communicate(self):
+    def _communicate(self) -> (str, str):
         """
         Attempt to communicate with the process, handling timeout
 
         Issues a Popen.communicate() with a timeout
         If this fails, will wait for (timeout * number of tries) seconds and
         try again. This continues until max_timeouts has been reached
 
@@ -446,14 +452,18 @@
         timeout = self.timeout
         self._timeout_current_tries += 1
         dt = 0  # accumulate time on each retry, rather than the whole call
         try:
             t0 = time.time()
             stdout, stderr = self._subprocess.communicate(timeout=timeout)
             dt += time.time() - t0
+        except AttributeError as E:
+            self._logger.info("attempted communicate on unexec CMD")
+            self._logger.info(str(E))
+            return None, None
         except subprocess.TimeoutExpired:
             print(
                 f"({self._timeout_current_tries}/{self.max_timeouts}) "
                 f"communication attempt failed after {timeout}s",
                 end="... ",
             )
```

### Comparing `remotemanager-0.6.2/remotemanager/connection/computers/base.py` & `remotemanager-0.6.3/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/connection/computers/example.py` & `remotemanager-0.6.3/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/connection/computers/options.py` & `remotemanager-0.6.3/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/connection/computers/parsers.py` & `remotemanager-0.6.3/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/connection/testing_object.py` & `remotemanager-0.6.3/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/connection/url.py` & `remotemanager-0.6.3/remotemanager/connection/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,15 @@
         stdout: str = None,
         stderr: str = None,
         timeout: int = None,
         max_timeouts: int = None,
         raise_errors: bool = None,
         dry_run: bool = False,
         prepend: bool = False,
+        force_file: bool = False,
     ) -> typing.Union[CMD, str]:
         """
         Creates and executes a command
 
         Args:
             asynchronous (bool):
                 run this command asynchronously
@@ -409,14 +410,16 @@
                 number of times to attempt communication in case of a timeout
             raise_errors (bool):
                 override for global setting. Raise any stderr if encountered
             dry_run (bool):
                 don't exec the command if True, just returns the string
             prepend (bool):
                 always attempt to use ssh_prepend
+            force_file (bool):
+                passthrough for CMD force_file argument
 
         Returns (CMD):
             returned command instance
         """
         _remote_call = False
         if local is not None and not local:
             self._logger.info("forced remote call; appending ssh to cmd")
@@ -450,14 +453,15 @@
             cmd.strip(),
             asynchronous=asynchronous,
             stdout=stdout,
             stderr=stderr,
             timeout=timeout,
             max_timeouts=max_timeouts,
             raise_errors=raise_errors,
+            force_file=force_file,
         )
         thiscmd.exec()
         if not local:
             self._callcount += 1
 
         self._cmd_history.append(thiscmd)
```

### Comparing `remotemanager-0.6.2/remotemanager/dataset/dataset.py` & `remotemanager-0.6.3/remotemanager/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -443,14 +443,15 @@
             dependency_call (bool):
                 True if called via the dependency handler
             verbose (int, Verbose, None):
                 verbose level for this runner (defaults to Dataset level)
             run_args:
                 any extra arguments to pass to runner
         """
+        self._logger.debug("Dataset append_run called")
         Quiet.state = quiet
         if args is None and arguments is not None:
             args = arguments
 
         if verbose is None:
             verbose = self.verbose.value
 
@@ -753,29 +754,38 @@
         out = {}
         for k, v in self.__dict__.items():
             if k not in Dataset.__dict__ and not k.startswith(("_", "~")):
                 out[k] = v
         out.update(self._global_run_args)
         return out
 
-    def _script_sub(self, **sub_args) -> str:
+    def _script_sub(self, avoid_nodes: bool = False, **sub_args) -> str:
         """
         Substitutes run argmuents into the computer script, if it exists
 
         Args:
+            avoid_nodes (bool):
+                ignore submission scripts if True
             **sub_args:
                 jobscript arguments
 
         Returns:
             (str):
                 jobscript
         """
+        if avoid_nodes:
+            self._logger.info("creating a jobscript for the login nodes")
+            return self._script
         if not self._computer:
+            self._logger.info("not a computer, returning base script")
             return self._script
         if "name" not in sub_args:
+            self._logger.info(
+                f"name not found in args, " f"appending self name {self.name}"
+            )
             sub_args["name"] = self.name
         return self.url.script(**sub_args)
 
     @property
     def script(self, **sub_args) -> str:
         """
         Currently stored run script
@@ -1008,28 +1018,33 @@
         return all([r == state for r in self.get_all_runner_states()])
 
     def run(
         self,
         force: bool = False,
         dry_run: bool = False,
         quiet: bool = False,
+        avoid_nodes: bool = False,
         **run_args,
     ):
         """
         Run the functions
 
         Args:
             force (bool):
                 force all runs to go through, ignoring checks
             dry_run (bool):
                 create files, but do not run
+            avoid_nodes (bool):
+                if True, will attempt to avoid running on avoid_nodes using a standard
+                'bash' submission
             run_args:
                 any arguments to pass to the runners during this run.
                 will override any "global" arguments set at Dataset init
         """
+        self._logger.debug("Dataset run called")
         Quiet.state = quiet
 
         if os.name == "nt" and self.url.is_local:
             raise RuntimeError(localwinerror)
         if self.is_parent:
             self._logger.warning(f"dataset {self} is a parent, " f"skipping run")
             Quiet.state = quiet
@@ -1040,27 +1055,36 @@
                 f"dataset {self} is a part of a dependency "
                 f"chain, calling from there"
             )
             self.dependency.run(force=force, dry_run=dry_run, **run_args)
             Quiet.state = quiet
             return
 
-        self._run(force, dry_run, **run_args)
+        self._run(force, dry_run, avoid_nodes, **run_args)
         Quiet.state = quiet
 
-    def _run(self, force: bool = False, dry_run: bool = False, **run_args) -> None:
+    def _run(
+        self,
+        force: bool = False,
+        dry_run: bool = False,
+        avoid_nodes: bool = False,
+        **run_args,
+    ) -> None:
         """
         Seperation of run and _run allows for dependency runs. Any
         functionality intended for run that does not interact with
         dependencies should be placed here
         """
+        self._logger.debug("Dataset _run called")
         self._run_cmds = []
         self._repo_files = []
         self._master_scripts = []
         # initial run args
+        if len(run_args) != 0:
+            self._logger.info(f"extra run args: {format_iterable(run_args)}")
         temp_args = {"force": force}
         temp_args.update(run_args)
 
         runners_to_update = []
         master_scripts = {}
         any_file_written = False
         asynchronous = None
@@ -1071,24 +1095,28 @@
             runner.state = Runner._submit_status["initial"]
             runner._write_runfile(self)
             any_file_written = True
 
             self._logger.info("writing script with run args:")
             self._logger.info(format_iterable(runner.run_args))
 
-            script = self._script_sub(**runner.run_args)
+            script = self._script_sub(avoid_nodes, **runner.run_args)
             runner._write_script(self.url.python, script)
 
             self.transport.queue_for_push(
                 [runner.jobscript.name, runner.runfile.name],
                 runner.local_dir,
                 runner.remote_dir,
             )
 
-            runline = f"{self.url.submitter} {runner.jobscript.name}"
+            if avoid_nodes:
+                submitter = getattr(self, "submitter", "bash")
+            else:
+                submitter = self.url.submitter
+            runline = f"{submitter} {runner.jobscript.name}"
 
             asynchronous = runner.run_option("asynchronous", True)
             if asynchronous and self.url.submitter == "bash":
                 self._logger.debug('appending "&" for async run')
                 runline += f" 2>> {self.stderr_dump} &"
 
             if runner.remote_dir not in master_scripts:
@@ -1099,15 +1127,15 @@
                 self.transport.queue_for_push(
                     os.path.split(file)[1], os.path.split(file)[0], runner.remote_dir
                 )
 
             runners_to_update.append(runner.uuid)
 
         if not any_file_written:
-            self._run_finalise()
+            return self._run_finalise()
 
         cmds = []
         i = 0
         for remote, lines in master_scripts.items():
             scriptname = f"{i}-{self.master_script}"
             i += 1
             _scriptfile = TrackedFile(self.local_dir, remote, scriptname)
@@ -1480,20 +1508,14 @@
     def all_finished(self) -> bool:
         """
         Check if `all` runners have finished
 
         Returns (bool):
             True if all runners have completed their runs
         """
-        for cmd in self._run_cmds:
-            if cmd.stderr and cmd.stderr != "":
-                if detect_locale_error(cmd.stderr):
-                    self._logger.warning(f"locale error detected: {cmd.stderr}")
-                else:
-                    raise RuntimeError(cmd.stderr)
         return all(self.is_finished)
 
     def wait(
         self, interval: int = 10, timeout: int = None, verbose: bool = False
     ) -> None:
         """
         Block run until completion, checking every `interval` seconds
```

### Comparing `remotemanager-0.6.2/remotemanager/dataset/dependency.py` & `remotemanager-0.6.3/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/dataset/runner.py` & `remotemanager-0.6.3/remotemanager/dataset/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 
 from remotemanager.storage.database import Database
 from remotemanager.storage import SendableMixin, TrackedFile
 from remotemanager.storage.sendablemixin import SERIALISED_STORAGE_KEY
 from remotemanager.logging.utils import format_iterable
 from remotemanager.utils.uuid import generate_uuid
-from remotemanager.utils import object_from_uuid, _time_format
+from remotemanager.utils import object_from_uuid, _time_format, ensure_list
 from remotemanager.logging import LoggingMixin
 from remotemanager.logging.verbosity import Verbosity
 
 from datetime import datetime
 
 localwinerror = """Local runs on windows machines are not supported.
 Please use a URL which connects to a non-windows machine or consider using
@@ -196,62 +196,54 @@
     def name(self) -> str:
         return self._id
 
     @property
     def identifier(self) -> str:
         return self._identifier
 
-    def _format_filename(self, identifier: str, ftype: str, ext: str) -> str:
+    def _format_filename(self, ftype: str, ext: str) -> str:
         """
         Formats internal file names consistently.
 
         Args:
-            identifier (str):
-                dataset name and runner id as string
             ftype (str):
                 file type. Jobscript, result file, etc.
             ext (str):
                 file extension
 
         Returns:
             str: formatted filename
         """
-        self._logger.info(
-            f"creating filename for content {identifier}, "
-            f"filetype {ftype} and "
-            f"extension {ext}"
-        )
-        return f"{identifier}-{ftype}{ext}"
+        self._logger.info(f"creating filename for {ftype} and " f"extension {ext}")
+        return f"{self.identifier}-{ftype}{ext}"
 
     @property
     def runfile(self) -> TrackedFile:
         """
         Filename of the python runfile
         """
-        base_name = self._format_filename(self.identifier, "run", ".py")
+        base_name = self._format_filename("run", ".py")
 
         return TrackedFile(self.local_dir, self.remote_dir, base_name)
 
     @property
     def jobscript(self) -> TrackedFile:
         """
         Filename of the run script
         """
-        base_name = self._format_filename(self.identifier, "jobscript", ".sh")
+        base_name = self._format_filename("jobscript", ".sh")
 
         return TrackedFile(self.local_dir, self.remote_dir, base_name)
 
     @property
     def resultfile(self) -> TrackedFile:
         """
         Result file name
         """
-        base_name = self._format_filename(
-            self.identifier, "result", f".{self.result_extension}"
-        )
+        base_name = self._format_filename("result", f".{self.result_extension}")
 
         paths = [self.remote_dir]
         if self.run_dir != self.remote_dir and self.run_dir is not None:
             paths.append(self.run_dir)
         joined = "/".join(paths)
 
         return TrackedFile(self.local_dir, joined, base_name)
@@ -522,17 +514,18 @@
         base_timekey = self.format_time(t)
         idx = 0
         timekey = f"{base_timekey}/{idx}"
         while timekey in self._history:
             idx += 1
 
             timekey = f"{base_timekey}/{idx}"
-            self._logger.info(f"timekey updated to {timekey}")
 
-        self._logger.info(f"updating runner {self.short_uuid} state -> " f"{newstate}")
+        self._logger.info(
+            f"({timekey}) updating runner {self.short_uuid} state -> " f"{newstate}"
+        )
         self._history[timekey] = newstate
 
     def run(self, dry_run: bool = False, **kwargs) -> None:
         """
         Perform a manual run
 
         .. warning::
@@ -582,16 +575,19 @@
         else:
             parent.transport.wipe_transfers()
             self._logger.important(f"launch command: {cmd}")
             self.state = "dry run"
 
     def _assess_run(self, **kwargs) -> bool:
 
-        self._extra_files["send"] += kwargs.pop("extra_files_send", [])
-        self._extra_files["recv"] += kwargs.pop("extra_files_recv", [])
+        send_extra = kwargs.pop("extra_files_send", [])
+        self._extra_files["send"] += ensure_list(send_extra)
+
+        recv_extra = kwargs.pop("extra_files_recv", [])
+        self._extra_files["recv"] += ensure_list(recv_extra)
 
         self._run_options.update(kwargs)
 
         self._logger.important(f"assessing run for runner {self}", end="... ")
         self._logger.info("\nrun args:")
         self._logger.info(format_iterable(self.run_args))
         self._logger.info(f"current state is {self.state}")
```

### Comparing `remotemanager-0.6.2/remotemanager/jupyter/magic.py` & `remotemanager-0.6.3/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/logging/__init__.py` & `remotemanager-0.6.3/remotemanager/logging/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,31 +21,31 @@
     This class inserts itself between the logging Logger and the
     _logobj used
     """
 
     def __init__(self, logger: str, parent):
         self._logger = logging.getLogger(logger)
 
-        self._add_logging_level("runtime", 15)
-        self._add_logging_level("important", 25)
+        self._add_logging_level("RUNTIME", 15)
+        self._add_logging_level("IMPORTANT", 25)
 
         self._parent = parent
 
     def _add_logging_level(self, name, level):
         def loglevel(self, message, *args, **kwargs):
             if self.isEnabledFor(level):
                 self._log(level, message, args, **kwargs)
 
         def logroot(message, *args, **kwargs):
             logging.log(level, message, *args, **kwargs)
 
         logging.addLevelName(level, name)
-        setattr(logging, name, level)
-        setattr(logging.getLoggerClass(), name, loglevel)
-        setattr(logging, name, logroot)
+        setattr(logging, name.lower(), level)
+        setattr(logging.getLoggerClass(), name.lower(), loglevel)
+        setattr(logging, name.lower(), logroot)
 
     @property
     def verbose(self):
         try:
             return self._parent._verbose
         except AttributeError:
             return None
@@ -56,104 +56,109 @@
             return
         try:
             self.verbose.print(msg, lvl, end)
         except AttributeError:
             # usually raised if the stored _verbose is None
             pass
 
+    def add_uuid(self, msg):
+        if hasattr(self._parent, "short_uuid"):
+            return f"({self._parent.short_uuid}) {msg}"
+        return msg
+
     def debug(
         self,
         msg: str,
         silent: bool = False,
         prepend: str = "",
         append: str = "",
         end: str = "\n",
         *args,
         **kwargs,
     ):
-        self._logger.debug(msg, *args, **kwargs)
+        self._logger.debug(self.add_uuid(msg), *args, **kwargs)
         if not silent:
             self._print(prepend + str(msg) + append, 1, end=end)
 
     def runtime(
         self,
         msg: str,
         silent: bool = False,
         prepend: str = "",
         append: str = "",
         end: str = "\n",
         *args,
         **kwargs,
     ):
-        self._logger.runtime(msg, *args, **kwargs)
+        self._logger.runtime(self.add_uuid(msg), *args, **kwargs)
         if not silent:
             self._print(prepend + str(msg) + append, 2, end=end)
 
     def info(
         self,
         msg: str,
         silent: bool = False,
         prepend: str = "",
         append: str = "",
         end: str = "\n",
         *args,
         **kwargs,
     ):
-        self._logger.info(msg, *args, **kwargs)
+        self._logger.info(self.add_uuid(msg), *args, **kwargs)
         if not silent:
             self._print(prepend + str(msg) + append, 3, end=end)
 
     def important(
         self,
         msg: str,
         silent: bool = False,
         prepend: str = "",
         append: str = "",
         end: str = "\n",
         *args,
         **kwargs,
     ):
-        self._logger.important(msg, *args, **kwargs)
+        self._logger.important(self.add_uuid(msg), *args, **kwargs)
         if not silent:
             self._print(prepend + str(msg) + append, 4, end=end)
 
     def warning(
         self,
         msg: str,
         silent: bool = False,
         prepend: str = "",
         append: str = "",
         end: str = "\n",
         *args,
         **kwargs,
     ):
-        self._logger.warning(msg, *args, **kwargs)
+        self._logger.warning(self.add_uuid(msg), *args, **kwargs)
         if not silent:
             self._print(prepend + str(msg) + append, 5, end=end)
 
     def error(
         self,
         msg: str,
         silent: bool = False,
         prepend: str = "",
         append: str = "",
         end: str = "\n",
         *args,
         **kwargs,
     ):
-        self._logger.error(msg, *args, **kwargs)
+        self._logger.error(self.add_uuid(msg), *args, **kwargs)
         if not silent:
             self._print(prepend + str(msg) + append, 6, end=end)
 
     def critical(
         self,
         msg: str,
         silent: bool = False,
         prepend: str = "",
         append: str = "",
         end: str = "\n",
         *args,
         **kwargs,
     ):
-        self._logger.critical(msg, *args, **kwargs)
+        self._logger.critical(self.add_uuid(msg), *args, **kwargs)
         if not silent:
             self._print(prepend + str(msg) + append, 7, end=end)
```

### Comparing `remotemanager-0.6.2/remotemanager/logging/log.py` & `remotemanager-0.6.3/remotemanager/logging/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,16 +162,16 @@
         """
         refresh handlers attached to the logger
         """
         for handler in self._base.handlers:
             self._base.removeHandler(handler)
         file_handler = logging.FileHandler(self._path, mode=self._mode)
         formatter = logging.Formatter(
-            "%(asctime)s - " "%(levelname)s - " "%(name)s.%(funcName)s: " "%(message)s",
-            datefmt="%Y-%m-%d %H-%M-%S",
+            "%(asctime)s " "%(levelname)-9s " "%(name)s.%(funcName)s: " "%(message)s",
+            datefmt="%Y%m%d%H%M%S",
         )
 
         file_handler.setFormatter(formatter)
         self._base.addHandler(file_handler)
 
     # TODO(lbeal) can this be made more pythonic?
```

### Comparing `remotemanager-0.6.2/remotemanager/logging/utils.py` & `remotemanager-0.6.3/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/logging/verbosity.py` & `remotemanager-0.6.3/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/serialisation/serial.py` & `remotemanager-0.6.3/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.6.3/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.6.3/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/storage/database.py` & `remotemanager-0.6.3/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/storage/function.py` & `remotemanager-0.6.3/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/storage/remotefunction.py` & `remotemanager-0.6.3/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/storage/sendablemixin.py` & `remotemanager-0.6.3/remotemanager/storage/sendablemixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections.abc
 import importlib
+import json
 import logging
 import os.path
 from collections import deque
 
 import yaml
 
 CLASS_STORAGE_KEY = "~serialisedclass~"
@@ -366,18 +367,15 @@
 
 
 def get_mro_classnames(obj) -> list:
     return [subobj.__name__ for subobj in obj.__class__.__mro__]
 
 
 def basic_available(obj):
-    # attempt a serialisation, if it does not have a yaml constructor tag
-    # we're probably safe to skip any further processing
+    # attempt a base json serialisation, which will fail fast if we can't dump
     try:
-        basic = yaml.dump(obj)
-        if not basic.startswith("!!"):
-            return True
+        json.dumps(obj)
+        return True
     except Exception as E:
         if hasattr(obj, "_logger"):
             obj._logger.error(str(E))
         return False
-    return False
```

### Comparing `remotemanager-0.6.2/remotemanager/storage/trackedfile.py` & `remotemanager-0.6.3/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/transport/cp.py` & `remotemanager-0.6.3/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/transport/rsync.py` & `remotemanager-0.6.3/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/transport/scp.py` & `remotemanager-0.6.3/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/transport/transport.py` & `remotemanager-0.6.3/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/utils/__init__.py` & `remotemanager-0.6.3/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/utils/flags.py` & `remotemanager-0.6.3/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager/utils/version.py` & `remotemanager-0.6.3/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.2/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.6.3/remotemanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.2
+Version: 0.6.3
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.2/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.6.3/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

