# Comparing `tmp/omero-demo-cleanup-0.2.0.tar.gz` & `tmp/omero-demo-cleanup-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-demo-cleanup-0.2.0.tar", last modified: Tue May 30 11:36:24 2023, max compression
+gzip compressed data, was "omero-demo-cleanup-0.2.1.tar", last modified: Mon Jun 12 10:51:01 2023, max compression
```

## Comparing `omero-demo-cleanup-0.2.0.tar` & `omero-demo-cleanup-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-05-30 11:36:19.000000 omero-demo-cleanup-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-30 11:36:19.000000 omero-demo-cleanup-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-30 11:36:20.000000 omero-demo-cleanup-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-30 11:36:20.000000 omero-demo-cleanup-0.2.0/src/omero/plugins/democleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:36:20.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-05-30 11:36:20.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12245 2023-05-30 11:36:20.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:36:24.239723 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-30 11:36:24.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-30 11:36:24.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:36:24.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 11:36:24.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 11:36:24.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:36:24.000000 omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-12 10:50:54.000000 omero-demo-cleanup-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-12 10:50:54.000000 omero-demo-cleanup-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-12 10:50:54.000000 omero-demo-cleanup-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-12 10:50:54.000000 omero-demo-cleanup-0.2.1/src/omero/plugins/democleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 10:50:54.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-12 10:50:54.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12291 2023-06-12 10:50:54.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:51:01.124536 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-12 10:51:01.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-12 10:51:01.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:51:01.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 10:51:01.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-12 10:51:01.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:51:01.000000 omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/zip-safe
```

### Comparing `omero-demo-cleanup-0.2.0/LICENSE.txt` & `omero-demo-cleanup-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-demo-cleanup-0.2.0/PKG-INFO` & `omero-demo-cleanup-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-demo-cleanup
-Version: 0.2.0
+Version: 0.2.1
 Summary: Plugin for managing the disk space on the demo server.
 Home-page: https://github.com/ome/omero-demo-cleanup/
 Author: The Open Microscopy Team
 Author-email: 
 Keywords: OMERO.CLI,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `omero-demo-cleanup-0.2.0/README.rst` & `omero-demo-cleanup-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `omero-demo-cleanup-0.2.0/setup.py` & `omero-demo-cleanup-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     return long_description
 
 
 long_description = get_long_description()
 
 setup(
     name="omero-demo-cleanup",
-    version="0.2.0",
+    version="0.2.1",
     packages=["omero_demo_cleanup", "omero.plugins"],
     package_dir={"": "src"},
     description="Plugin for managing the disk space on the demo server.",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
```

### Comparing `omero-demo-cleanup-0.2.0/src/omero_demo_cleanup/cli.py` & `omero-demo-cleanup-0.2.1/src/omero_demo_cleanup/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     all services of the Blitzgateway are closed again.
     """
 
     @wraps(func)
     def _wrapper(self: Any, *args: Any, **kwargs: Any) -> Callable:
         self.client = self.ctx.conn(*args)
         self.gateway = BlitzGateway(client_obj=self.client)
+        self.gateway.SERVICE_OPTS.setOmeroGroup("-1")
 
         try:
             return func(self, *args, **kwargs)
         finally:
             if self.gateway is not None:
                 self.gateway.close(hard=False)
                 self.gateway = None
```

### Comparing `omero-demo-cleanup-0.2.0/src/omero_demo_cleanup/library.py` & `omero-demo-cleanup-0.2.1/src/omero_demo_cleanup/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,14 +359,15 @@
         )
         delete_data(conn, user.id, dry_run=dry_run)
 
 
 def main() -> None:
     with omero.cli.cli_login() as cli:
         conn = omero.gateway.BlitzGateway(client_obj=cli.get_client())
+        conn.SERVICE_OPTS.setOmeroGroup("-1")
         try:
             perform_delete(conn)
         except KeyboardInterrupt:
             pass  # ignore
         finally:
             conn.close()
```

### Comparing `omero-demo-cleanup-0.2.0/src/omero_demo_cleanup.egg-info/PKG-INFO` & `omero-demo-cleanup-0.2.1/src/omero_demo_cleanup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-demo-cleanup
-Version: 0.2.0
+Version: 0.2.1
 Summary: Plugin for managing the disk space on the demo server.
 Home-page: https://github.com/ome/omero-demo-cleanup/
 Author: The Open Microscopy Team
 Author-email: 
 Keywords: OMERO.CLI,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

