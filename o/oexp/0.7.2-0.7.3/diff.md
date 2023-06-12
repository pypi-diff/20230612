# Comparing `tmp/oexp-0.7.2.tar.gz` & `tmp/oexp-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.7.2.tar", last modified: Mon Jun 12 14:01:05 2023, max compression
+gzip compressed data, was "oexp-0.7.3.tar", last modified: Mon Jun 12 14:11:30 2023, max compression
```

## Comparing `oexp-0.7.2.tar` & `oexp-0.7.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.207837 oexp-0.7.2/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:01:05.207683 oexp-0.7.2/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.2/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.206479 oexp-0.7.2/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.2/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    80499 2023-06-12 13:23:43.000000 oexp-0.7.2/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 13:23:43.000000 oexp-0.7.2/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.2/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.207518 oexp-0.7.2/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.2/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2384 2023-06-12 13:59:58.000000 oexp-0.7.2/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.2/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.207143 oexp-0.7.2/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 14:01:00.000000 oexp-0.7.2/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 14:01:05.207880 oexp-0.7.2/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.203868 oexp-0.7.3/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:11:30.203629 oexp-0.7.3/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.3/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.202061 oexp-0.7.3/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.3/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    80499 2023-06-12 13:23:43.000000 oexp-0.7.3/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 13:23:43.000000 oexp-0.7.3/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.3/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.203232 oexp-0.7.3/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.3/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.7.3/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.3/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:11:30.202816 oexp-0.7.3/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 14:11:30.000000 oexp-0.7.3/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 14:11:25.000000 oexp-0.7.3/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 14:11:30.203933 oexp-0.7.3/setup.cfg
```

### Comparing `oexp-0.7.2/oexp/access.py` & `oexp-0.7.3/oexp/access.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.2/oexp/jbridge.py` & `oexp-0.7.3/oexp/jbridge.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.2/oexp/util/ops.py` & `oexp-0.7.3/oexp/util/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 import subprocess
 import os
 import socket
 import urllib.request as request
+from distutils.util import strtobool
+
 from oexp import gen, access
 from oexp.util import vals
 
 
+def strtobool_none_is_false(val):
+    if val is None:
+        return False
+    else:
+        return strtobool(val)
+
+
+VERBOSE = strtobool_none_is_false(os.getenv('VERBOSE'))
+
+
+def verbose(s):
+    if VERBOSE:
+        print(s)
+
+
 def server_socket(next_port_to_try):
     # _java_sock.connect(("localhost", int(access.PORT)))
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     did_bind = False
     while next_port_to_try <= vals._last_port_to_try:
         try:
             sock.bind((vals._HOST, next_port_to_try))
             did_bind = True
             break
         except socket.error:
-            print(f"port {next_port_to_try} is being used, trying for port {next_port_to_try + 1} ")
+            verbose(f"port {next_port_to_try} is being used, trying for port {next_port_to_try + 1} ")
             next_port_to_try += 1
     if not did_bind:
         raise Exception("could not bind socket")
     sock.listen()
     return sock, next_port_to_try
```

### Comparing `oexp-0.7.2/oexp/util/vals.py` & `oexp-0.7.3/oexp/util/vals.py`

 * *Files identical despite different names*

