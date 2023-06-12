# Comparing `tmp/enderchest-0.1.1rc1.tar.gz` & `tmp/enderchest-0.1.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enderchest-0.1.1rc1.tar", last modified: Fri Jun  9 22:57:09 2023, max compression
+gzip compressed data, was "enderchest-0.1.1rc2.tar", last modified: Mon Jun 12 18:12:10 2023, max compression
```

## Comparing `enderchest-0.1.1rc1.tar` & `enderchest-0.1.1rc2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/enderchest/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/enderchest/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    31260 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/enderchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    29630 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/shulker_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/sync/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/sync/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_craft.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    27683 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.840967 enderchest-0.1.1rc1/enderchest/test/testing_files/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/enderchest.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/instgroups.json
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/launcher_profiles.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/options.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/testing_files/version_manifest_v2.json
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/enderchest/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 22:57:09.836967 enderchest-0.1.1rc1/enderchest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 22:57:09.000000 enderchest-0.1.1rc1/enderchest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 22:57:09.844967 enderchest-0.1.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-06-09 22:57:02.000000 enderchest-0.1.1rc1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:12:10.254337 enderchest-0.1.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-12 18:12:10.258337 enderchest-0.1.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:12:10.258337 enderchest-0.1.1rc2/enderchest/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-12 18:12:10.258337 enderchest-0.1.1rc2/enderchest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31260 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/enderchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29632 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/shulker_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:12:10.254337 enderchest-0.1.1rc2/enderchest/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/sync/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/sync/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/sync/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:12:10.254337 enderchest-0.1.1rc2/enderchest/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15993 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/test_craft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27683 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/test_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:12:10.254337 enderchest-0.1.1rc2/enderchest/test/testing_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/testing_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/testing_files/enderchest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/testing_files/instgroups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/testing_files/launcher_profiles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/testing_files/options.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/testing_files/version_manifest_v2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/enderchest/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:12:10.254337 enderchest-0.1.1rc2/enderchest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-12 18:12:10.000000 enderchest-0.1.1rc2/enderchest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-12 18:12:10.000000 enderchest-0.1.1rc2/enderchest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:12:10.000000 enderchest-0.1.1rc2/enderchest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 18:12:10.000000 enderchest-0.1.1rc2/enderchest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-12 18:12:10.000000 enderchest-0.1.1rc2/enderchest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 18:12:10.000000 enderchest-0.1.1rc2/enderchest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 18:12:10.258337 enderchest-0.1.1rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83196 2023-06-12 18:12:01.000000 enderchest-0.1.1rc2/versioneer.py
```

### Comparing `enderchest-0.1.1rc1/LICENSE` & `enderchest-0.1.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/PKG-INFO` & `enderchest-0.1.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.1rc1
+Version: 0.1.1rc2
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.1rc1/README.md` & `enderchest-0.1.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/cli.py` & `enderchest-0.1.1rc2/enderchest/cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/config.py` & `enderchest-0.1.1rc2/enderchest/config.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/craft.py` & `enderchest-0.1.1rc2/enderchest/craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/enderchest.py` & `enderchest-0.1.1rc2/enderchest/enderchest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/filesystem.py` & `enderchest-0.1.1rc2/enderchest/filesystem.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/gather.py` & `enderchest-0.1.1rc2/enderchest/gather.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
     )
 
     matches = [
         instance for instance in chest.instances if shulker_box.matches(instance)
     ]
 
     if len(matches) == 0:
-        report = "is not link to by any registered instances"
+        report = "is not linked to by any registered instances"
     else:
         report = "is linked to by the following instances:\n" + "\n".join(
             f"  - {_render_instance(instance)}" for instance in matches
         )
 
     GATHER_LOGGER.info(f"The shulker box {_render_shulker_box(shulker_box)} {report}")
```

### Comparing `enderchest-0.1.1rc1/enderchest/instance.py` & `enderchest-0.1.1rc2/enderchest/instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/loggers.py` & `enderchest-0.1.1rc2/enderchest/loggers.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/place.py` & `enderchest-0.1.1rc2/enderchest/place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/prompt.py` & `enderchest-0.1.1rc2/enderchest/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Utilities for helping build interactive prompts"""
 
-CURSOR = "==>"
+CURSOR = "\x1b[35;1m==>\x1b[0m"
 
 # https://stackoverflow.com/a/18472142
 YES = ("y", "yes", "t", "true", "on", "1")
 
 NO = ("n", "no", "f", "false", "off", "0")
 
 
@@ -28,17 +28,17 @@
     - The output will be stripped of trailing and leading whitespace, but no
       other validation or processing will be used.
     - Regardless of whether a suggestion is provided, if the user provides an
       empty input, this method will return an empty string. To reiterate: the
       suggestion *does not serve* as a default / fallback value.
     """
     lines = message.splitlines() + [""]
-    message = "\n".join(f"{CURSOR} {line}" for line in lines)
+    message = "\n".join(f"{CURSOR}\x1b[1m {line}\x1b[0m" for line in lines)
     if suggestion is not None:
-        message += f"[{suggestion}] "
+        message += f"\x1b[35;1m[{suggestion}]\x1b[0m "
     return input(message)
 
 
 def confirm(default: bool) -> bool:
     """Confirm that the user wishes to continue
 
     Parameters
```

### Comparing `enderchest-0.1.1rc1/enderchest/remote.py` & `enderchest-0.1.1rc2/enderchest/remote.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/shulker_box.py` & `enderchest-0.1.1rc2/enderchest/shulker_box.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/__init__.py` & `enderchest-0.1.1rc2/enderchest/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/file.py` & `enderchest-0.1.1rc2/enderchest/sync/file.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/rsync.py` & `enderchest-0.1.1rc2/enderchest/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/sync/utils.py` & `enderchest-0.1.1rc2/enderchest/sync/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/conftest.py` & `enderchest-0.1.1rc2/enderchest/test/conftest.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_cli.py` & `enderchest-0.1.1rc2/enderchest/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_config.py` & `enderchest-0.1.1rc2/enderchest/test/test_config.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_craft.py` & `enderchest-0.1.1rc2/enderchest/test/test_craft.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_gather.py` & `enderchest-0.1.1rc2/enderchest/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_instance.py` & `enderchest-0.1.1rc2/enderchest/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_place.py` & `enderchest-0.1.1rc2/enderchest/test/test_place.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/test_sync.py` & `enderchest-0.1.1rc2/enderchest/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/testing_files/enderchest.cfg` & `enderchest-0.1.1rc2/enderchest/test/testing_files/enderchest.cfg`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/testing_files/launcher_profiles.json` & `enderchest-0.1.1rc2/enderchest/test/testing_files/launcher_profiles.json`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest/test/utils.py` & `enderchest-0.1.1rc2/enderchest/test/utils.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/enderchest.egg-info/PKG-INFO` & `enderchest-0.1.1rc2/enderchest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enderchest
-Version: 0.1.1rc1
+Version: 0.1.1rc2
 Summary: syncing and linking for all your Minecraft instances
 Home-page: https://github.com/OpenBagTwo/EnderChest
 Author: Gili "OpenBagTwo" Barlev
 License: GPL v3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `enderchest-0.1.1rc1/enderchest.egg-info/SOURCES.txt` & `enderchest-0.1.1rc2/enderchest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/setup.py` & `enderchest-0.1.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `enderchest-0.1.1rc1/versioneer.py` & `enderchest-0.1.1rc2/versioneer.py`

 * *Files identical despite different names*

