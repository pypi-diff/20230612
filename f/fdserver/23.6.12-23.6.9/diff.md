# Comparing `tmp/fdserver-23.6.12.tar.gz` & `tmp/fdserver-23.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdserver-23.6.12.tar", last modified: Mon Jun 12 16:02:17 2023, max compression
+gzip compressed data, was "fdserver-23.6.9.tar", last modified: Fri Jun  9 20:24:51 2023, max compression
```

## Comparing `fdserver-23.6.12.tar` & `fdserver-23.6.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-12 16:02:17.550760 fdserver-23.6.12/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7652 2022-06-28 19:46:07.000000 fdserver-23.6.12/LICENSE.md
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4383 2023-06-12 16:02:17.549760 fdserver-23.6.12/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3603 2023-06-12 16:01:02.000000 fdserver-23.6.12/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-12 16:02:17.544760 fdserver-23.6.12/fdserver/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:00:34.000000 fdserver-23.6.12/fdserver/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34828 2023-06-12 15:58:24.000000 fdserver-23.6.12/fdserver/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-12 16:02:17.548760 fdserver-23.6.12/fdserver/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5445 2023-02-01 20:40:07.000000 fdserver-23.6.12/fdserver/data/k6gte-fdserver-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-02-01 20:38:54.000000 fdserver-23.6.12/fdserver/data/k6gte-fdserver-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2649 2023-02-01 20:39:12.000000 fdserver-23.6.12/fdserver/data/k6gte-fdserver-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      302 2023-02-01 20:41:35.000000 fdserver-23.6.12/fdserver/data/k6gte-fdserver.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13503 2023-02-01 20:40:13.000000 fdserver-23.6.12/fdserver/data/k6gte.fdserver.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1216 2023-05-30 16:06:27.000000 fdserver-23.6.12/fdserver/data/server_preferences.json
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-12 16:02:17.549760 fdserver-23.6.12/fdserver/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:01:16.000000 fdserver-23.6.12/fdserver/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12382 2023-06-09 19:06:47.000000 fdserver-23.6.12/fdserver/lib/server_database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-06-12 16:01:21.000000 fdserver-23.6.12/fdserver/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2022-12-28 03:38:12.000000 fdserver-23.6.12/fdserver/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-12 16:02:17.545760 fdserver-23.6.12/fdserver.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4383 2023-06-12 16:02:17.000000 fdserver-23.6.12/fdserver.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      566 2023-06-12 16:02:17.000000 fdserver-23.6.12/fdserver.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-12 16:02:17.000000 fdserver-23.6.12/fdserver.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-06-12 16:02:17.000000 fdserver-23.6.12/fdserver.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-06-12 16:02:17.000000 fdserver-23.6.12/fdserver.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1000 2023-06-12 16:01:40.000000 fdserver-23.6.12/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-12 16:02:17.550760 fdserver-23.6.12/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.863779 fdserver-23.6.9/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7652 2022-06-28 19:46:07.000000 fdserver-23.6.9/LICENSE.md
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4262 2023-06-09 20:24:51.862779 fdserver-23.6.9/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3483 2023-06-09 20:22:41.000000 fdserver-23.6.9/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.860779 fdserver-23.6.9/fdserver/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:00:34.000000 fdserver-23.6.9/fdserver/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34719 2023-06-09 18:52:22.000000 fdserver-23.6.9/fdserver/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.861779 fdserver-23.6.9/fdserver/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5445 2023-02-01 20:40:07.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-02-01 20:38:54.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2649 2023-02-01 20:39:12.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      302 2023-02-01 20:41:35.000000 fdserver-23.6.9/fdserver/data/k6gte-fdserver.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13503 2023-02-01 20:40:13.000000 fdserver-23.6.9/fdserver/data/k6gte.fdserver.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1216 2023-05-30 16:06:27.000000 fdserver-23.6.9/fdserver/data/server_preferences.json
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.862779 fdserver-23.6.9/fdserver/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-12-28 15:01:16.000000 fdserver-23.6.9/fdserver/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12382 2023-06-09 19:06:47.000000 fdserver-23.6.9/fdserver/lib/server_database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-06-09 20:20:22.000000 fdserver-23.6.9/fdserver/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2022-12-28 03:38:12.000000 fdserver-23.6.9/fdserver/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-09 20:24:51.861779 fdserver-23.6.9/fdserver.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4262 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      566 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       19 2023-06-09 20:24:51.000000 fdserver-23.6.9/fdserver.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      999 2023-06-09 20:20:38.000000 fdserver-23.6.9/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-09 20:24:51.863779 fdserver-23.6.9/setup.cfg
```

### Comparing `fdserver-23.6.12/LICENSE.md` & `fdserver-23.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/PKG-INFO` & `fdserver-23.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdserver
-Version: 23.6.12
+Version: 23.6.9
 Summary: Field Day group logging server
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/fdserver
 Project-URL: Bug Tracker, https://github.com/mbridak/fdserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,15 +30,14 @@
 
 - [Field Day log aggregating server](#field-day-log-aggregating-server)
   - [TOC](#toc)
   - [What is it](#what-is-it)
   - [No really what is it](#no-really-what-is-it)
   - [Screenshot](#screenshot)
   - [Installation](#installation)
-  - [Recent Changes](#recent-changes)
   - [Configuration and first run](#configuration-and-first-run)
 
 ## What is it
 
 [ARRL Field Day](http://field-day.arrl.org/) is a once a year 24hr emergency
 preparidness event for radio amateurs (Hams). During the event, we try and
 make as many radio contacts with other Hams in a 24 hour period. You can find
@@ -72,18 +71,14 @@
 Field Day aggregation server.
 
 options:
   -h, --help  show this help message and exit
   -l, --log   Generate log
 ```
 
-## Recent Changes
-
-- [23.6.12] Merged PR from @wvolz to handle MacOS port reuse.
-
 ## Configuration and first run
 
 When executed for the first time, the server will not find a configuration file.
 When this happens, the server will place a fresh copy in the local directory.
 Press CTRL-C to end the program then edit the configuration file now found at
 `./server_preferences.json`. Unless you have good reason to, don't change the
 multicast settings.
```

### Comparing `fdserver-23.6.12/README.md` & `fdserver-23.6.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 - [Field Day log aggregating server](#field-day-log-aggregating-server)
   - [TOC](#toc)
   - [What is it](#what-is-it)
   - [No really what is it](#no-really-what-is-it)
   - [Screenshot](#screenshot)
   - [Installation](#installation)
-  - [Recent Changes](#recent-changes)
   - [Configuration and first run](#configuration-and-first-run)
 
 ## What is it
 
 [ARRL Field Day](http://field-day.arrl.org/) is a once a year 24hr emergency
 preparidness event for radio amateurs (Hams). During the event, we try and
 make as many radio contacts with other Hams in a 24 hour period. You can find
@@ -53,18 +52,14 @@
 Field Day aggregation server.
 
 options:
   -h, --help  show this help message and exit
   -l, --log   Generate log
 ```
 
-## Recent Changes
-
-- [23.6.12] Merged PR from @wvolz to handle MacOS port reuse.
-
 ## Configuration and first run
 
 When executed for the first time, the server will not find a configuration file.
 When this happens, the server will place a fresh copy in the local directory.
 Press CTRL-C to end the program then edit the configuration file now found at
 `./server_preferences.json`. Unless you have good reason to, don't change the
 multicast settings.
```

### Comparing `fdserver-23.6.12/fdserver/__main__.py` & `fdserver-23.6.9/fdserver/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,19 +274,15 @@
         pulse = b'{"cmd": "PING", "host": "server"}'
         s.sendto(pulse, (MULTICAST_GROUP, MULTICAST_PORT))
         send_xml_score()
         time.sleep(10)
 
 
 s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-if sys.platform.startswith('darwin'):
-    s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
-else:
-    s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-
+s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 s.bind(("", MULTICAST_PORT))
 mreq = socket.inet_aton(MULTICAST_GROUP) + socket.inet_aton(INTERFACE_IP)
 s.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, bytes(mreq))
 
 
 _heartbeat = threading.Thread(
     target=send_pulse,
```

### Comparing `fdserver-23.6.12/fdserver/data/k6gte-fdserver-128.png` & `fdserver-23.6.9/fdserver/data/k6gte-fdserver-128.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/fdserver/data/k6gte-fdserver-32.png` & `fdserver-23.6.9/fdserver/data/k6gte-fdserver-32.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/fdserver/data/k6gte-fdserver-64.png` & `fdserver-23.6.9/fdserver/data/k6gte-fdserver-64.png`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/fdserver/data/k6gte.fdserver.svg` & `fdserver-23.6.9/fdserver/data/k6gte.fdserver.svg`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/fdserver/data/server_preferences.json` & `fdserver-23.6.9/fdserver/data/server_preferences.json`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/fdserver/lib/server_database.py` & `fdserver-23.6.9/fdserver/lib/server_database.py`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/fdserver/lib/versiontest.py` & `fdserver-23.6.9/fdserver/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/fdserver.egg-info/PKG-INFO` & `fdserver-23.6.9/fdserver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdserver
-Version: 23.6.12
+Version: 23.6.9
 Summary: Field Day group logging server
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/fdserver
 Project-URL: Bug Tracker, https://github.com/mbridak/fdserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,15 +30,14 @@
 
 - [Field Day log aggregating server](#field-day-log-aggregating-server)
   - [TOC](#toc)
   - [What is it](#what-is-it)
   - [No really what is it](#no-really-what-is-it)
   - [Screenshot](#screenshot)
   - [Installation](#installation)
-  - [Recent Changes](#recent-changes)
   - [Configuration and first run](#configuration-and-first-run)
 
 ## What is it
 
 [ARRL Field Day](http://field-day.arrl.org/) is a once a year 24hr emergency
 preparidness event for radio amateurs (Hams). During the event, we try and
 make as many radio contacts with other Hams in a 24 hour period. You can find
@@ -72,18 +71,14 @@
 Field Day aggregation server.
 
 options:
   -h, --help  show this help message and exit
   -l, --log   Generate log
 ```
 
-## Recent Changes
-
-- [23.6.12] Merged PR from @wvolz to handle MacOS port reuse.
-
 ## Configuration and first run
 
 When executed for the first time, the server will not find a configuration file.
 When this happens, the server will place a fresh copy in the local directory.
 Press CTRL-C to end the program then edit the configuration file now found at
 `./server_preferences.json`. Unless you have good reason to, don't change the
 multicast settings.
```

### Comparing `fdserver-23.6.12/fdserver.egg-info/SOURCES.txt` & `fdserver-23.6.9/fdserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdserver-23.6.12/pyproject.toml` & `fdserver-23.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdserver" 
-version = "23.6.12"
+version = "23.6.9"
 description = "Field Day group logging server"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

