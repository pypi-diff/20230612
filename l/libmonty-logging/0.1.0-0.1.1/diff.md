# Comparing `tmp/libmonty-logging-0.1.0.tar.gz` & `tmp/libmonty-logging-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmonty-logging-0.1.0.tar", last modified: Mon Jun 12 03:28:53 2023, max compression
+gzip compressed data, was "libmonty-logging-0.1.1.tar", last modified: Mon Jun 12 03:33:45 2023, max compression
```

## Comparing `libmonty-logging-0.1.0.tar` & `libmonty-logging-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2021-06-15 09:06:57.000000 libmonty-logging-0.1.0/LICENSE
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       57 2023-06-12 01:26:45.000000 libmonty-logging-0.1.0/MANIFEST.in
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1577 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      541 2023-06-12 00:32:02.000000 libmonty-logging-0.1.0/README.md
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      104 2021-12-16 04:36:50.000000 libmonty-logging-0.1.0/pyproject.toml
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       23 2023-06-04 22:25:05.000000 libmonty-logging-0.1.0/requirements.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1241 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/setup.cfg
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:28:53.936630 libmonty-logging-0.1.0/src/
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/src/libmonty_logging/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:31:14.000000 libmonty-logging-0.1.0/src/libmonty_logging/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      876 2023-06-12 01:35:21.000000 libmonty-logging-0.1.0/src/libmonty_logging/__main__.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/src/libmonty_logging/config/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-06-05 08:52:12.000000 libmonty-logging-0.1.0/src/libmonty_logging/config/__init__.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/src/libmonty_logging/config/file_and_stream/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-06-05 08:52:12.000000 libmonty-logging-0.1.0/src/libmonty_logging/config/file_and_stream/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1457 2023-06-12 02:40:30.000000 libmonty-logging-0.1.0/src/libmonty_logging/config/file_and_stream/v1.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/src/libmonty_logging/data/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      544 2023-06-12 00:35:24.000000 libmonty-logging-0.1.0/src/libmonty_logging/data/file-and-stream-v1.ini
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1226 2023-06-12 03:03:18.000000 libmonty-logging-0.1.0/src/libmonty_logging/helper.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      758 2023-06-12 03:12:42.000000 libmonty-logging-0.1.0/src/libmonty_logging/message.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      336 2023-06-12 00:49:02.000000 libmonty-logging-0.1.0/src/libmonty_logging/version.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:28:53.940630 libmonty-logging-0.1.0/src/libmonty_logging.egg-info/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1577 2023-06-12 03:28:53.000000 libmonty-logging-0.1.0/src/libmonty_logging.egg-info/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      646 2023-06-12 03:28:53.000000 libmonty-logging-0.1.0/src/libmonty_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2023-06-12 03:28:53.000000 libmonty-logging-0.1.0/src/libmonty_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       21 2023-06-12 03:28:53.000000 libmonty-logging-0.1.0/src/libmonty_logging.egg-info/requires.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       17 2023-06-12 03:28:53.000000 libmonty-logging-0.1.0/src/libmonty_logging.egg-info/top_level.txt
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:33:45.718256 libmonty-logging-0.1.1/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2021-06-15 09:06:57.000000 libmonty-logging-0.1.1/LICENSE
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       57 2023-06-12 01:26:45.000000 libmonty-logging-0.1.1/MANIFEST.in
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1577 2023-06-12 03:33:45.718256 libmonty-logging-0.1.1/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      541 2023-06-12 00:32:02.000000 libmonty-logging-0.1.1/README.md
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      104 2021-12-16 04:36:50.000000 libmonty-logging-0.1.1/pyproject.toml
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       23 2023-06-04 22:25:05.000000 libmonty-logging-0.1.1/requirements.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1241 2023-06-12 03:33:45.718256 libmonty-logging-0.1.1/setup.cfg
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:33:45.714256 libmonty-logging-0.1.1/src/
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:33:45.714256 libmonty-logging-0.1.1/src/libmonty_logging/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2021-12-20 00:31:14.000000 libmonty-logging-0.1.1/src/libmonty_logging/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      876 2023-06-12 01:35:21.000000 libmonty-logging-0.1.1/src/libmonty_logging/__main__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:33:45.718256 libmonty-logging-0.1.1/src/libmonty_logging/config/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-06-05 08:52:12.000000 libmonty-logging-0.1.1/src/libmonty_logging/config/__init__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:33:45.718256 libmonty-logging-0.1.1/src/libmonty_logging/config/file_and_stream/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-06-05 08:52:12.000000 libmonty-logging-0.1.1/src/libmonty_logging/config/file_and_stream/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1457 2023-06-12 02:40:30.000000 libmonty-logging-0.1.1/src/libmonty_logging/config/file_and_stream/v1.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:33:45.718256 libmonty-logging-0.1.1/src/libmonty_logging/data/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      544 2023-06-12 00:35:24.000000 libmonty-logging-0.1.1/src/libmonty_logging/data/file-and-stream-v1.ini
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1226 2023-06-12 03:03:18.000000 libmonty-logging-0.1.1/src/libmonty_logging/helper.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      759 2023-06-12 03:31:23.000000 libmonty-logging-0.1.1/src/libmonty_logging/message.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      336 2023-06-12 03:31:34.000000 libmonty-logging-0.1.1/src/libmonty_logging/version.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-12 03:33:45.718256 libmonty-logging-0.1.1/src/libmonty_logging.egg-info/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1577 2023-06-12 03:33:45.000000 libmonty-logging-0.1.1/src/libmonty_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      646 2023-06-12 03:33:45.000000 libmonty-logging-0.1.1/src/libmonty_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2023-06-12 03:33:45.000000 libmonty-logging-0.1.1/src/libmonty_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       21 2023-06-12 03:33:45.000000 libmonty-logging-0.1.1/src/libmonty_logging.egg-info/requires.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       17 2023-06-12 03:33:45.000000 libmonty-logging-0.1.1/src/libmonty_logging.egg-info/top_level.txt
```

### Comparing `libmonty-logging-0.1.0/LICENSE` & `libmonty-logging-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libmonty-logging-0.1.0/PKG-INFO` & `libmonty-logging-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmonty-logging
-Version: 0.1.0
+Version: 0.1.1
 Summary: libmonty-logging - Python library - logging-related
 Home-page: https://codeberg.org/sunarch/libmonty-logging
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `libmonty-logging-0.1.0/README.md` & `libmonty-logging-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `libmonty-logging-0.1.0/setup.cfg` & `libmonty-logging-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `libmonty-logging-0.1.0/src/libmonty_logging/__main__.py` & `libmonty-logging-0.1.1/src/libmonty_logging/__main__.py`

 * *Files identical despite different names*

### Comparing `libmonty-logging-0.1.0/src/libmonty_logging/config/file_and_stream/v1.py` & `libmonty-logging-0.1.1/src/libmonty_logging/config/file_and_stream/v1.py`

 * *Files identical despite different names*

### Comparing `libmonty-logging-0.1.0/src/libmonty_logging/data/file-and-stream-v1.ini` & `libmonty-logging-0.1.1/src/libmonty_logging/data/file-and-stream-v1.ini`

 * *Files identical despite different names*

### Comparing `libmonty-logging-0.1.0/src/libmonty_logging/helper.py` & `libmonty-logging-0.1.1/src/libmonty_logging/helper.py`

 * *Files identical despite different names*

### Comparing `libmonty-logging-0.1.0/src/libmonty_logging/message.py` & `libmonty-logging-0.1.1/src/libmonty_logging/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
     if len(underliner) != 1:
         raise ValueError(f'Argument "underliner" must be 1 character long: "{underliner}"')
 
     header = f'{program_name}'
     
     if program_version is not None:
-        header += f'{program_version}'
+        header += f' {program_version}'
 
     logging.info(header)
     logging.info('-' * len(header))
```

### Comparing `libmonty-logging-0.1.0/src/libmonty_logging.egg-info/PKG-INFO` & `libmonty-logging-0.1.1/src/libmonty_logging.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmonty-logging
-Version: 0.1.0
+Version: 0.1.1
 Summary: libmonty-logging - Python library - logging-related
 Home-page: https://codeberg.org/sunarch/libmonty-logging
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `libmonty-logging-0.1.0/src/libmonty_logging.egg-info/SOURCES.txt` & `libmonty-logging-0.1.1/src/libmonty_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

