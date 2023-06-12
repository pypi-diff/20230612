# Comparing `tmp/automation_file_dev-0.0.7.tar.gz` & `tmp/automation_file_dev-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file_dev-0.0.7.tar", last modified: Fri Jun  9 03:59:58 2023, max compression
+gzip compressed data, was "automation_file_dev-0.0.8.tar", last modified: Mon Jun 12 07:23:55 2023, max compression
```

## Comparing `automation_file_dev-0.0.7.tar` & `automation_file_dev-0.0.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.497772 automation_file_dev-0.0.7/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1306 2023-06-09 03:59:58.496778 automation_file_dev-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file_dev-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.222350 automation_file_dev-0.0.7/automation_file_dev.egg-info/
--rw-rw-rw-   0        0        0     1306 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2012 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 03:59:58.000000 automation_file_dev-0.0.7/automation_file_dev.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.234372 automation_file_dev-0.0.7/file_automation/
--rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file_dev-0.0.7/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.239369 automation_file_dev-0.0.7/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.7/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.251374 automation_file_dev-0.0.7/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.7/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file_dev-0.0.7/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.266027 automation_file_dev-0.0.7/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.7/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file_dev-0.0.7/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.280993 automation_file_dev-0.0.7/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.7/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-06-08 07:15:08.000000 automation_file_dev-0.0.7/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.286447 automation_file_dev-0.0.7/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.7/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.297843 automation_file_dev-0.0.7/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.307351 automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/delete_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.320163 automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/folder_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.332163 automation_file_dev-0.0.7/file_automation/remote/google_drive/download/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/download/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/download/download_file.py
--rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/driver_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.345661 automation_file_dev-0.0.7/file_automation/remote/google_drive/search/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/search/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/search/search_drive.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.359727 automation_file_dev-0.0.7/file_automation/remote/google_drive/share/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/share/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/share/share_file.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.371732 automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/__init__.py
--rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/upload_to_driver.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.377642 automation_file_dev-0.0.7/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.7/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.387084 automation_file_dev-0.0.7/file_automation/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file_dev-0.0.7/file_automation/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-06-09 03:57:57.000000 automation_file_dev-0.0.7/file_automation/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.416934 automation_file_dev-0.0.7/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.7/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file_dev-0.0.7/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file_dev-0.0.7/file_automation/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.436299 automation_file_dev-0.0.7/file_automation/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.7/file_automation/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-06-09 03:57:57.000000 automation_file_dev-0.0.7/file_automation/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.456850 automation_file_dev-0.0.7/file_automation/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.7/file_automation/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1299 2023-06-08 09:16:50.000000 automation_file_dev-0.0.7/file_automation/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.474202 automation_file_dev-0.0.7/file_automation/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file_dev-0.0.7/file_automation/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      372 2023-06-08 05:31:05.000000 automation_file_dev-0.0.7/file_automation/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:59:58.490770 automation_file_dev-0.0.7/file_automation/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file_dev-0.0.7/file_automation/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 automation_file_dev-0.0.7/file_automation/utils/scheduler/extend_apscheduler.py
--rw-rw-rw-   0        0        0     1008 2023-06-09 03:59:33.000000 automation_file_dev-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 03:59:58.498773 automation_file_dev-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.109984 automation_file_dev-0.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1306 2023-06-12 07:23:55.107828 automation_file_dev-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file_dev-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.678664 automation_file_dev-0.0.8/automation_file_dev.egg-info/
+-rw-rw-rw-   0        0        0     1306 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2012 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 07:23:54.000000 automation_file_dev-0.0.8/automation_file_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.686170 automation_file_dev-0.0.8/file_automation/
+-rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file_dev-0.0.8/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.690159 automation_file_dev-0.0.8/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.8/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.704669 automation_file_dev-0.0.8/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.8/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file_dev-0.0.8/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.719534 automation_file_dev-0.0.8/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.8/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file_dev-0.0.8/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.737631 automation_file_dev-0.0.8/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.8/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-12 07:22:51.000000 automation_file_dev-0.0.8/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.742955 automation_file_dev-0.0.8/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.8/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.758392 automation_file_dev-0.0.8/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.769185 automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.780173 automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.796716 automation_file_dev-0.0.8/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.823542 automation_file_dev-0.0.8/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.842802 automation_file_dev-0.0.8/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.864909 automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.876174 automation_file_dev-0.0.8/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.8/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.909659 automation_file_dev-0.0.8/file_automation/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file_dev-0.0.8/file_automation/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     5297 2023-06-12 07:00:20.000000 automation_file_dev-0.0.8/file_automation/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:54.956895 automation_file_dev-0.0.8/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.8/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file_dev-0.0.8/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file_dev-0.0.8/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.003159 automation_file_dev-0.0.8/file_automation/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.8/file_automation/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     6611 2023-06-12 07:17:42.000000 automation_file_dev-0.0.8/file_automation/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.022084 automation_file_dev-0.0.8/file_automation/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file_dev-0.0.8/file_automation/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1600 2023-06-12 07:17:42.000000 automation_file_dev-0.0.8/file_automation/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.040159 automation_file_dev-0.0.8/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file_dev-0.0.8/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-06-12 07:11:23.000000 automation_file_dev-0.0.8/file_automation/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:23:55.096452 automation_file_dev-0.0.8/file_automation/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file_dev-0.0.8/file_automation/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     7002 2023-06-12 07:17:42.000000 automation_file_dev-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py
+-rw-rw-rw-   0        0        0     1008 2023-06-12 07:23:00.000000 automation_file_dev-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:23:55.120437 automation_file_dev-0.0.8/setup.cfg
```

### Comparing `automation_file_dev-0.0.7/LICENSE` & `automation_file_dev-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/PKG-INFO` & `automation_file_dev-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file_dev
-Version: 0.0.7
+Version: 0.0.8
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.7/README.md` & `automation_file_dev-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/automation_file_dev.egg-info/PKG-INFO` & `automation_file_dev-0.0.8/automation_file_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-file-dev
-Version: 0.0.7
+Version: 0.0.8
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file_dev-0.0.7/automation_file_dev.egg-info/SOURCES.txt` & `automation_file_dev-0.0.8/automation_file_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/__init__.py` & `automation_file_dev-0.0.8/file_automation/__init__.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/local/dir/dir_process.py` & `automation_file_dev-0.0.8/file_automation/local/dir/dir_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/local/file/file_process.py` & `automation_file_dev-0.0.8/file_automation/local/file/file_process.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/local/zip/zip_process.py` & `automation_file_dev-0.0.8/file_automation/local/zip/zip_process.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,9 +94,9 @@
 def set_zip_password(zip_file_path: str, password: bytes):
     current_zip = zipfile.ZipFile(zip_file_path)
     current_zip.setpassword(pwd=password)
     current_zip.close()
     file_automation_logger.info(
         f"Set zip file password, "
         f"zip file: {zip_file_path}, "
-        f"zup password: {password}"
+        f"zip password: {password}"
     )
```

### Comparing `automation_file_dev-0.0.7/file_automation/remote/google_drive/delete/delete_manager.py` & `automation_file_dev-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/remote/google_drive/dir/folder_manager.py` & `automation_file_dev-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/remote/google_drive/download/download_file.py` & `automation_file_dev-0.0.8/file_automation/remote/google_drive/download/download_file.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/remote/google_drive/driver_instance.py` & `automation_file_dev-0.0.8/file_automation/remote/google_drive/driver_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/remote/google_drive/search/search_drive.py` & `automation_file_dev-0.0.8/file_automation/remote/google_drive/search/search_drive.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/remote/google_drive/share/share_file.py` & `automation_file_dev-0.0.8/file_automation/remote/google_drive/share/share_file.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/remote/google_drive/upload/upload_to_driver.py` & `automation_file_dev-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/utils/callback/callback_function_executor.py` & `automation_file_dev-0.0.8/file_automation/utils/callback/callback_function_executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing
-from sys import stderr
 
 from file_automation.local.dir.dir_process import copy_dir, create_dir, remove_dir_tree
 from file_automation.local.file.file_process import copy_file, remove_file, rename_file, copy_specify_extension_file, \
     copy_all_file_to_dir
 from file_automation.local.zip.zip_process import zip_dir, zip_file, zip_info, zip_file_info, set_zip_password, \
     read_zip_file, unzip_file, unzip_all
 from file_automation.remote.google_drive.delete.delete_manager import delete_file
@@ -14,14 +13,15 @@
     search_all_file, search_field, search_file_mimetype
 from file_automation.remote.google_drive.share.share_file import \
     share_file_to_anyone, share_file_to_domain, share_file_to_user
 from file_automation.remote.google_drive.upload.upload_to_driver import \
     upload_dir_to_folder, upload_to_folder, upload_dir_to_drive, upload_to_drive
 from file_automation.utils.exception.exception_tags import get_bad_trigger_function, get_bad_trigger_method
 from file_automation.utils.exception.exceptions import CallbackExecutorException
+from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
 class CallbackFunctionExecutor(object):
 
     def __init__(self):
         self.event_dict: dict = {
             "copy_file": copy_file,
@@ -72,24 +72,31 @@
         :param callback_param_method: what type param will use on callback function only accept kwargs and args
         :param kwargs: trigger_function's param
         :return: trigger_function_name return value
         """
         try:
             if trigger_function_name not in self.event_dict.keys():
                 raise CallbackExecutorException(get_bad_trigger_function)
+            file_automation_logger.info(f"Callback trigger {trigger_function_name} with param {kwargs}")
             execute_return_value = self.event_dict.get(trigger_function_name)(**kwargs)
             if callback_function_param is not None:
                 if callback_param_method not in ["kwargs", "args"]:
                     raise CallbackExecutorException(get_bad_trigger_method)
                 if callback_param_method == "kwargs":
                     callback_function(**callback_function_param)
+                    file_automation_logger.info(
+                        f"Callback function {callback_function} with param {callback_function_param}")
                 else:
                     callback_function(*callback_function_param)
+                    file_automation_logger.info(
+                        f"Callback function {callback_function} with param {callback_function_param}")
             else:
                 callback_function()
+                file_automation_logger.info(f"Callback function {callback_function}")
             return execute_return_value
         except Exception as error:
-            print(repr(error), file=stderr)
+            file_automation_logger.error(
+                f"Callback function failed. {repr(error)}")
 
 
 callback_executor = CallbackFunctionExecutor()
```

### Comparing `automation_file_dev-0.0.7/file_automation/utils/exception/exception_tags.py` & `automation_file_dev-0.0.8/file_automation/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/utils/exception/exceptions.py` & `automation_file_dev-0.0.8/file_automation/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.7/file_automation/utils/executor/action_executor.py` & `automation_file_dev-0.0.8/file_automation/utils/executor/action_executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     share_file_to_anyone, share_file_to_domain, share_file_to_user
 from file_automation.remote.google_drive.upload.upload_to_driver import \
     upload_dir_to_folder, upload_to_folder, upload_dir_to_drive, upload_to_drive
 from file_automation.utils.exception.exception_tags import add_command_exception, executor_list_error, \
     action_is_null_error, cant_execute_action_error
 from file_automation.utils.exception.exceptions import ExecuteActionException, AddCommandException
 from file_automation.utils.json.json_file import read_action_json
+from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
 class Executor(object):
 
     def __init__(self):
         self.event_dict: dict = {
             "copy_file": copy_file,
@@ -89,28 +90,31 @@
         execute_record_dict = dict()
         try:
             if len(action_list) > 0 or isinstance(action_list, list):
                 pass
             else:
                 raise ExecuteActionException(action_is_null_error)
         except Exception as error:
-            print(repr(error), file=sys.stderr, flush=True)
+            file_automation_logger.error(
+                f"Execute {action_list} failed. {repr(error)}"
+            )
         for action in action_list:
             try:
                 event_response = self._execute_event(action)
                 execute_record = "execute: " + str(action)
+                file_automation_logger.info(
+                    f"Execute {action}"
+                )
                 execute_record_dict.update({execute_record: event_response})
             except Exception as error:
-                print(repr(error), file=sys.stderr, flush=True)
-                print(action, file=sys.stderr, flush=True)
+                file_automation_logger.error(
+                    f"Execute {action} failed. {repr(error)}"
+                )
                 execute_record = "execute: " + str(action)
                 execute_record_dict.update({execute_record: repr(error)})
-        for key, value in execute_record_dict.items():
-            print(key, flush=True)
-            print(value, flush=True)
         return execute_record_dict
 
     def execute_files(self, execute_files_list: list) -> list:
         """
         :param execute_files_list: list include execute files path
         :return: every execute detail as list
         """
@@ -123,14 +127,17 @@
 executor = Executor()
 
 
 def add_command_to_executor(command_dict: dict):
     """
     :param command_dict: dict include command we want to add to event_dict
     """
+    file_automation_logger.info(
+        f"Add command to executor {command_dict}"
+    )
     for command_name, command in command_dict.items():
         if isinstance(command, (types.MethodType, types.FunctionType)):
             executor.event_dict.update({command_name: command})
         else:
             raise AddCommandException(add_command_exception)
```

### Comparing `automation_file_dev-0.0.7/file_automation/utils/json/json_file.py` & `automation_file_dev-0.0.8/file_automation/utils/json/json_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import json
 from pathlib import Path
 from threading import Lock
 
-from file_automation.utils.exception.exception_tags import cant_find_json_error
+from file_automation.utils.exception.exception_tags import cant_find_json_error, cant_save_json_error
 from file_automation.utils.exception.exceptions import JsonActionException
+from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 _lock = Lock()
 
 
 def read_action_json(json_file_path: str) -> list:
     """
     use to read action file
     :param json_file_path json file's path to read
     """
     _lock.acquire()
     try:
         file_path = Path(json_file_path)
         if file_path.exists() and file_path.is_file():
+            file_automation_logger.info(
+                f"Read json file {json_file_path}"
+            )
             with open(json_file_path) as read_file:
                 return json.loads(read_file.read())
     except JsonActionException:
         raise JsonActionException(cant_find_json_error)
     finally:
         _lock.release()
 
@@ -29,13 +33,16 @@
     """
     use to save action file
     :param json_save_path  json save path
     :param action_json the json str include action to write
     """
     _lock.acquire()
     try:
+        file_automation_logger.info(
+            f"Write {action_json} as file {json_save_path}"
+        )
         with open(json_save_path, "w+") as file_to_write:
             file_to_write.write(json.dumps(action_json, indent=4))
-    except AutoControlJsonActionException:
-        raise AutoControlJsonActionException(cant_save_json_error)
+    except JsonActionException:
+        raise JsonActionException(cant_save_json_error)
     finally:
         _lock.release()
```

### Comparing `automation_file_dev-0.0.7/file_automation/utils/scheduler/extend_apscheduler.py` & `automation_file_dev-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Callable
 
 from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.schedulers.blocking import BlockingScheduler
 from apscheduler.util import undefined
 
+from file_automation.utils.logging.loggin_instance import file_automation_logger
+
 
 class SchedulerManager(object):
 
     def __init__(self):
         self._blocking_schedulers: BlockingScheduler = BlockingScheduler()
         self._background_schedulers: BackgroundScheduler = BackgroundScheduler()
 
@@ -34,17 +36,23 @@
     def get_blocking_scheduler(self):
         return self._blocking_schedulers
 
     def get_nonblocking_scheduler(self):
         return self._background_schedulers
 
     def start_block_scheduler(self, *args, **kwargs):
+        file_automation_logger.info(
+            f"Start blocking scheduler with {args}, {kwargs}"
+        )
         self._blocking_schedulers.start(*args, **kwargs)
 
     def start_nonblocking_scheduler(self, *args, **kwargs):
+        file_automation_logger.info(
+            f"Start background scheduler with {args}, {kwargs}"
+        )
         self._background_schedulers.start(*args, **kwargs)
 
     def start_all_scheduler(self, *args, **kwargs):
         self._blocking_schedulers.start(*args, **kwargs)
         self._background_schedulers.start(*args, **kwargs)
 
     def add_interval_blocking_secondly(
@@ -112,17 +120,29 @@
         self.add_blocking_job(func=function, id=id, trigger="cron", **trigger_args)
 
     def add_cron_nonblocking(
             self, function: Callable, id: str = None, **trigger_args):
         self.add_nonblocking_job(func=function, id=id, trigger="cron", **trigger_args)
 
     def remove_blocking_job(self, id: str, jobstore: str = 'default'):
+        file_automation_logger.info(
+            f"Remove blocking job {id}, store on {jobstore}"
+        )
         self._blocking_schedulers.remove_job(job_id=id, jobstore=jobstore)
 
     def remove_nonblocking_job(self, id: str, jobstore: str = 'default'):
+        file_automation_logger.info(
+            f"Remove nonblocking job {id}, store on {jobstore}"
+        )
         self._background_schedulers.remove_job(job_id=id, jobstore=jobstore)
 
     def shutdown_blocking_scheduler(self, wait: bool = False):
+        file_automation_logger.info(
+            f"Shutdown blocking scheduler wait = {wait}"
+        )
         self._blocking_schedulers.shutdown(wait=wait)
 
     def shutdown_nonblocking_scheduler(self, wait: bool = False):
+        file_automation_logger.info(
+            f"Shutdown nonblocking scheduler wait = {wait}"
+        )
         self._background_schedulers.shutdown(wait=wait)
```

### Comparing `automation_file_dev-0.0.7/pyproject.toml` & `automation_file_dev-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file_dev"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

