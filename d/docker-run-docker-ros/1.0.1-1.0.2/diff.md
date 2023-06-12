# Comparing `tmp/docker-run-docker-ros-1.0.1.tar.gz` & `tmp/docker-run-docker-ros-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run-docker-ros/dist/.tmp-mbix80ld/docker-run-docker-ros-1.0.1.tar", last modified: Tue May 30 10:52:45 2023, max compression
+gzip compressed data, was "docker-run-docker-ros-1.0.2.tar", last modified: Mon Jun 12 16:21:04 2023, max compression
```

## Comparing `docker-run-docker-ros-1.0.1.tar` & `docker-run-docker-ros-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-docker-ros-1.0.1/LICENSE
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     3983 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1862 2023-05-29 13:04:41.000000 docker-run-docker-ros-1.0.1/README.md
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1058 2023-05-30 10:50:48.000000 docker-run-docker-ros-1.0.1/pyproject.toml
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/setup.cfg
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run/
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run/plugins/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1608 2023-05-30 10:50:42.000000 docker-run-docker-ros-1.0.1/src/docker_run/plugins/docker_ros.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     3983 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      313 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/SOURCES.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/dependency_links.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       22 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/requires.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-05-30 10:52:45.000000 docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:21:04.392393 docker-run-docker-ros-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-12 16:20:45.000000 docker-run-docker-ros-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-12 16:21:04.392393 docker-run-docker-ros-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-12 16:20:45.000000 docker-run-docker-ros-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-12 16:20:45.000000 docker-run-docker-ros-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:21:04.392393 docker-run-docker-ros-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:21:04.388393 docker-run-docker-ros-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:21:04.388393 docker-run-docker-ros-1.0.2/src/docker_run/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:21:04.388393 docker-run-docker-ros-1.0.2/src/docker_run/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-12 16:20:45.000000 docker-run-docker-ros-1.0.2/src/docker_run/plugins/docker_ros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:21:04.392393 docker-run-docker-ros-1.0.2/src/docker_run_docker_ros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-12 16:21:04.000000 docker-run-docker-ros-1.0.2/src/docker_run_docker_ros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-12 16:21:04.000000 docker-run-docker-ros-1.0.2/src/docker_run_docker_ros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:21:04.000000 docker-run-docker-ros-1.0.2/src/docker_run_docker_ros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 16:21:04.000000 docker-run-docker-ros-1.0.2/src/docker_run_docker_ros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 16:21:04.000000 docker-run-docker-ros-1.0.2/src/docker_run_docker_ros.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `docker-run-docker-ros-1.0.1/LICENSE` & `docker-run-docker-ros-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.1/PKG-INFO` & `docker-run-docker-ros-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.1
+Version: 1.0.2
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

### Comparing `docker-run-docker-ros-1.0.1/README.md` & `docker-run-docker-ros-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `docker-run-docker-ros-1.0.1/pyproject.toml` & `docker-run-docker-ros-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-docker-ros"
-version = "1.0.1"
+version = "1.0.2"
 description = "docker-run plugin for Docker images built by docker-ros"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
```

### Comparing `docker-run-docker-ros-1.0.1/src/docker_run/plugins/docker_ros.py` & `docker-run-docker-ros-1.0.2/src/docker_run/plugins/docker_ros.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from typing import Any, Dict, List
 
 from docker_run.utils import runCommand
 from docker_run.plugins.plugin import Plugin
 
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 
 class DockerRosPlugin(Plugin):
 
     TARGET_MOUNT = "/docker-ros/ws/src/target"
 
     @classmethod
@@ -29,15 +29,17 @@
         if args["mws"]:
             flags += cls.currentDirMountWorkspaceFlags()
         return flags
 
     @classmethod
     def getExecFlags(cls, args: Dict[str, Any], unknown_args: List[str]) -> List[str]:
         flags = []
-        if not args["no_user"] and runCommand(f"docker exec {args['name']} sh -c 'echo $DOCKER_ROS'")[0][:-1] == "1":
+        is_docker_ros = (runCommand(f"docker exec {args['name']} printenv DOCKER_ROS")[0][:-1] == "1")
+        is_non_root = (len(runCommand(f"docker exec {args['name']} printenv DOCKER_UID")[0][:-1]) > 0)
+        if not args["no_user"] and is_docker_ros and is_non_root:
             flags += cls.userExecFlags()
         return flags
 
     @classmethod
     def userFlags(cls) -> List[str]:
         return [f"--env DOCKER_UID={os.getuid()}", f"--env DOCKER_GID={os.getgid()}"]
```

### Comparing `docker-run-docker-ros-1.0.1/src/docker_run_docker_ros.egg-info/PKG-INFO` & `docker-run-docker-ros-1.0.2/src/docker_run_docker_ros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-docker-ros
-Version: 1.0.1
+Version: 1.0.2
 Summary: docker-run plugin for Docker images built by docker-ros
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
```

