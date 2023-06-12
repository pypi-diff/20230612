# Comparing `tmp/docker-run-cli-0.9.2.tar.gz` & `tmp/docker-run-cli-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/data01/reiher/git/ops/docker-run/docker-run/dist/.tmp-a2_n4ilg/docker-run-cli-0.9.2.tar", last modified: Sat Jun 10 17:15:52 2023, max compression
+gzip compressed data, was "docker-run-cli-0.9.3.tar", last modified: Mon Jun 12 16:20:52 2023, max compression
```

## Comparing `docker-run-cli-0.9.2.tar` & `docker-run-cli-0.9.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1123 2023-05-29 13:04:51.000000 docker-run-cli-0.9.2/LICENSE
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       51 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/MANIFEST.in
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7799 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     5602 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/README.md
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     1420 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/pyproject.toml
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/scripts/
--rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1620 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/scripts/activate-python-docker-run-shell-completion
--rwxrwxr-x   0 reiher   (16171) fb-5     (12389)     1091 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/scripts/docker-run
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       38 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/setup.cfg
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       45 2023-06-10 17:14:01.000000 docker-run-cli-0.9.2/src/docker_run/__init__.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      107 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/__main__.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run/bash_completion.d/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     2886 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/bash_completion.d/docker-run
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     6110 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/core.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run/plugins/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        0 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/plugins/__init__.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     4566 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/plugins/core.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      520 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/plugins/plugin.py
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      758 2023-05-29 13:04:41.000000 docker-run-cli-0.9.2/src/docker_run/utils.py
-drwxrwsr-x   0 reiher   (16171) fb-5     (12389)        0 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)     7799 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/PKG-INFO
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      568 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)        1 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)      151 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/requires.txt
--rw-rw-r--   0 reiher   (16171) fb-5     (12389)       11 2023-06-10 17:15:52.000000 docker-run-cli-0.9.2/src/docker_run_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:52.330391 docker-run-cli-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-12 16:20:52.330391 docker-run-cli-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:52.326391 docker-run-cli-0.9.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/scripts/activate-python-docker-run-shell-completion
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/scripts/docker-run
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:20:52.330391 docker-run-cli-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:52.326391 docker-run-cli-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:52.326391 docker-run-cli-0.9.3/src/docker_run/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:52.326391 docker-run-cli-0.9.3/src/docker_run/bash_completion.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/bash_completion.d/docker-run
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:52.326391 docker-run-cli-0.9.3/src/docker_run/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-12 16:20:42.000000 docker-run-cli-0.9.3/src/docker_run/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:20:52.330391 docker-run-cli-0.9.3/src/docker_run_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-12 16:20:52.000000 docker-run-cli-0.9.3/src/docker_run_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-12 16:20:52.000000 docker-run-cli-0.9.3/src/docker_run_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:20:52.000000 docker-run-cli-0.9.3/src/docker_run_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 16:20:52.000000 docker-run-cli-0.9.3/src/docker_run_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 16:20:52.000000 docker-run-cli-0.9.3/src/docker_run_cli.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `docker-run-cli-0.9.2/LICENSE` & `docker-run-cli-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.2/PKG-INFO` & `docker-run-cli-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.2
+Version: 0.9.3
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -42,17 +42,17 @@
 License-File: LICENSE
 
 <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png" height=130 align="right">
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
 <p align="center">
-  <img src="https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run"/></a>
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
-  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/>
+  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/v/docker-run-cli?label=PyPI"/></a>
+  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
 <p align="center">
   <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.2 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.3 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
@@ -24,17 +24,17 @@
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: POSIX ::
 Linux Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
 Extra: dev Provides-Extra: docker-ros Provides-Extra: plugins Provides-Extra:
 all License-File: LICENSE [https://github.com/ika-rwth-aachen/docker-run/raw/
 main/assets/logo.png] # *docker-run* â ``docker run`` and ``docker exec``
 with useful defaults
-     [https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run]
  [https://img.shields.io/github/license/ika-rwth-aachen/docker-run] [https://
-img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]
+img.shields.io/pypi/v/docker-run-cli?label=PyPI] [https://img.shields.io/pypi/
+             dm/docker-run-cli?color=blue&label=PyPI%20downloads]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
 arguments.
   [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
 While *docker-run* can be used with any Docker image, we recommend to also
 check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
```

### Comparing `docker-run-cli-0.9.2/README.md` & `docker-run-cli-0.9.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png" height=130 align="right">
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
 <p align="center">
-  <img src="https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run"/></a>
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
-  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/>
+  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/v/docker-run-cli?label=PyPI"/></a>
+  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
 <p align="center">
   <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png] #
 *docker-run* â ``docker run`` and ``docker exec`` with useful defaults
-     [https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run]
  [https://img.shields.io/github/license/ika-rwth-aachen/docker-run] [https://
-img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]
+img.shields.io/pypi/v/docker-run-cli?label=PyPI] [https://img.shields.io/pypi/
+             dm/docker-run-cli?color=blue&label=PyPI%20downloads]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
 arguments.
   [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
 While *docker-run* can be used with any Docker image, we recommend to also
 check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
```

### Comparing `docker-run-cli-0.9.2/pyproject.toml` & `docker-run-cli-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "docker-run-cli"
-version = "0.9.2"
+version = "0.9.3"
 description = "'docker run' and 'docker exec' with useful defaults"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Lennart Reiher", email = "lennart.reiher@rwth-aachen.de"},
     {name = "Jean-Pierre Busch", email = "jean-pierre.busch@rwth-aachen.de"},
 ]
```

### Comparing `docker-run-cli-0.9.2/scripts/activate-python-docker-run-shell-completion` & `docker-run-cli-0.9.3/scripts/activate-python-docker-run-shell-completion`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.2/scripts/docker-run` & `docker-run-cli-0.9.3/scripts/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.2/src/docker_run/bash_completion.d/docker-run` & `docker-run-cli-0.9.3/src/docker_run/bash_completion.d/docker-run`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.2/src/docker_run/core.py` & `docker-run-cli-0.9.3/src/docker_run/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import argparse
 import importlib
 import os
 import sys
 from typing import Any, Dict, List, Tuple
 
 import docker_run
-from docker_run.utils import log, runCommand
+from docker_run.utils import log, runCommand, validDockerContainerName
 from docker_run.plugins.plugin import Plugin
 
 # automatically load all available plugins inheriting from `Plugin`
 PLUGINS = []
 PLUGINS_DIR = os.path.join(os.path.dirname(__file__), "plugins")
 for file_name in os.listdir(PLUGINS_DIR):
     if file_name.endswith(".py") and file_name != "plugin.py":
         module_name = os.path.splitext(file_name)[0]
         module = importlib.import_module(f"docker_run.plugins.{module_name}")
         for name, cls in module.__dict__.items():
             if isinstance(cls, type) and issubclass(cls, Plugin) and cls is not Plugin:
                 PLUGINS.append(cls)
 
+DEFAULT_CONTAINER_NAME = validDockerContainerName(os.path.basename(os.getcwd()))
 
 def parseArguments() -> Tuple[argparse.Namespace, List[str], List[str]]:
 
     class DockerRunArgumentParser(argparse.ArgumentParser):
 
         def print_help(self, file=None):
             super().print_help(file=sys.stderr if file is None else file)
@@ -41,15 +42,15 @@
                                                  "container removal after exit, interactive tty, current directory name as container name, GPU support, X11 GUI forwarding. "
                                                  "Passes any additional arguments to `docker run`. "
                                                  "Executes `docker exec` instead if a container with the specified name (`--name`) is already running.",
                                      add_help=False)
 
     parser.add_argument("--help", action="help", default=argparse.SUPPRESS, help="show this help message and exit")
     parser.add_argument("--image", help="image name (may also be specified without --image as last argument before command)")
-    parser.add_argument("--name", default=os.path.basename(os.getcwd()), help="container name; generates `docker exec` command if already running")
+    parser.add_argument("--name", default=DEFAULT_CONTAINER_NAME, help="container name; generates `docker exec` command if already running")
     parser.add_argument("--no-name", action="store_true", help="disable automatic container name (current directory)")
     parser.add_argument("--verbose", action="store_true", help="print generated command")
     parser.add_argument("--version", action="store_true", help="show program's version number and exit")
 
     # plugin args
     for plugin in PLUGINS:
         plugin.addArguments(parser)
@@ -84,22 +85,27 @@
     Returns:
         str: executable `docker run` or `docker exec` command
     """
 
     # check for running container
     if args["no_name"]:
         args["name"] = None
-    new_container = False
-    running_containers = runCommand('docker ps --format "{{.Names}}"')[0].split('\n')
-    new_container = not (args["name"] in running_containers)
+        new_container = True
+    else:
+        new_container = False
+        running_containers = runCommand('docker ps --format "{{.Names}}"')[0].split('\n')
+        new_container = not (args["name"] in running_containers)
+        if not new_container and args["image"] is not None and len(args["image"]) > 0:
+            args["name"] = None if args["name"] == DEFAULT_CONTAINER_NAME else args["name"]
+            new_container = True
 
     if new_container: # docker run
 
         log_msg = f"Starting new container "
-        if not args["no_name"]:
+        if args["name"] is not None:
             log_msg += f"'{args['name']}'"
         log(log_msg + " ...")
         docker_cmd = ["docker", "run"]
 
         # name
         if args["name"] is not None and len(args["name"]) > 0:
             docker_cmd += [f"--name {args['name']}"]
```

### Comparing `docker-run-cli-0.9.2/src/docker_run/plugins/core.py` & `docker-run-cli-0.9.3/src/docker_run/plugins/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,26 +88,29 @@
 
     @classmethod
     def x11GuiForwardingFlags(cls, docker_network: str = "bridge") -> List[str]:
 
         display = os.environ.get("DISPLAY")
         if display is None:
             return []
+        
+        if cls.OS == "Darwin":
+            runCommand(f"xhost +local:")
 
         xsock = "/tmp/.X11-unix"
         xauth = tempfile.NamedTemporaryFile(prefix='.docker.xauth.', delete=False).name
         xauth_display = display if cls.OS != "Darwin" else runCommand("ifconfig en0 | grep 'inet '")[0].split()[1] + ":0"
         xauth_output = "ffff" + runCommand(f"xauth nlist {xauth_display}")[0][4:]
         runCommand(f"xauth -f {xauth} nmerge - 2>/dev/null", input=xauth_output.encode())
         os.chmod(xauth, 0o777)
 
         if docker_network != "host" and not display.startswith(":"):
-            display="172.17.0.1:" + display.split(":")[1]
+            display = "172.17.0.1:" + display.split(":")[1]
         if cls.OS == "Darwin":
-            display="host.docker.internal:" + display.split(":")[1]
+            display = "host.docker.internal:" + display.split(":")[1]
 
         flags = []
         flags.append(f"--env DISPLAY={display}")
         flags.append(f"--env XAUTHORITY={xauth}")
         flags.append(f"--env QT_X11_NO_MITSHM=1")
         flags.append(f"--volume {xauth}:{xauth}")
         flags.append(f"--volume {xsock}:{xsock}")
```

### Comparing `docker-run-cli-0.9.2/src/docker_run/plugins/plugin.py` & `docker-run-cli-0.9.3/src/docker_run/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `docker-run-cli-0.9.2/src/docker_run/utils.py` & `docker-run-cli-0.9.3/src/docker_run/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import subprocess
 import sys
 from typing import Tuple
 
 
 def log(msg: str, *args, **kwargs):
     """Log message to stderr.
@@ -24,7 +25,25 @@
 
     try:
         output = subprocess.run(cmd, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, *args, **kwargs)
     except subprocess.CalledProcessError as exc:
         raise RuntimeError(f"System command '{cmd}' failed: {exc.stderr.decode()}")
 
     return output.stdout.decode(), output.stderr.decode()
+
+
+def validDockerContainerName(name: str) -> str:
+    """Cleans a string such that it is a valid Docker container name.
+
+    [a-zA-Z0-9][a-zA-Z0-9_.-]
+
+    Args:
+        name (str): raw name
+
+    Returns:
+        str: valid container name
+    """
+    
+    name = re.sub('[^a-zA-Z0-9_.-]', '-', name)
+    name = re.sub('^[^a-zA-Z0-9]+', '', name)
+    
+    return name
```

### Comparing `docker-run-cli-0.9.2/src/docker_run_cli.egg-info/PKG-INFO` & `docker-run-cli-0.9.3/src/docker_run_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-run-cli
-Version: 0.9.2
+Version: 0.9.3
 Summary: 'docker run' and 'docker exec' with useful defaults
 Author-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 Maintainer-email: Lennart Reiher <lennart.reiher@rwth-aachen.de>, Jean-Pierre Busch <jean-pierre.busch@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Institute for Automotive Engineering (ika), RWTH Aachen University
         
@@ -42,17 +42,17 @@
 License-File: LICENSE
 
 <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/logo.png" height=130 align="right">
 
 # *docker-run* – ``docker run`` and ``docker exec`` with useful defaults
 
 <p align="center">
-  <img src="https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run"/></a>
   <img src="https://img.shields.io/github/license/ika-rwth-aachen/docker-run"/>
-  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/>
+  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/v/docker-run-cli?label=PyPI"/></a>
+  <a href="https://pypi.org/project/docker-run-cli/"><img src="https://img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads"/></a>
 </p>
 
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use it to easily start and attach to Docker containers with useful predefined arguments.
 
 <p align="center">
   <img src="https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png" width=550>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.2 Summary: 'docker run'
+Metadata-Version: 2.1 Name: docker-run-cli Version: 0.9.3 Summary: 'docker run'
 and 'docker exec' with useful defaults Author-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> Maintainer-email: Lennart Reiher
 reiher@rwth-aachen.de>, Jean-Pierre Busch
 busch@rwth-aachen.de> License: MIT License Copyright (c) 2023 Institute for
 Automotive Engineering (ika), RWTH Aachen University Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
@@ -24,17 +24,17 @@
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: POSIX ::
 Linux Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-
 Extra: dev Provides-Extra: docker-ros Provides-Extra: plugins Provides-Extra:
 all License-File: LICENSE [https://github.com/ika-rwth-aachen/docker-run/raw/
 main/assets/logo.png] # *docker-run* â ``docker run`` and ``docker exec``
 with useful defaults
-     [https://img.shields.io/github/v/release/ika-rwth-aachen/docker-run]
  [https://img.shields.io/github/license/ika-rwth-aachen/docker-run] [https://
-img.shields.io/pypi/dm/docker-run-cli?color=blue&label=PyPI%20downloads]
+img.shields.io/pypi/v/docker-run-cli?label=PyPI] [https://img.shields.io/pypi/
+             dm/docker-run-cli?color=blue&label=PyPI%20downloads]
 *docker-run* is a CLI tool for simplified interaction with Docker images. Use
 it to easily start and attach to Docker containers with useful predefined
 arguments.
   [https://github.com/ika-rwth-aachen/docker-run/raw/main/assets/teaser.png]
 While *docker-run* can be used with any Docker image, we recommend to also
 check out our other tools for Docker and ROS. - [*docker-ros*](https://
 github.com/ika-rwth-aachen/docker-ros) automatically builds minimal container
```

### Comparing `docker-run-cli-0.9.2/src/docker_run_cli.egg-info/SOURCES.txt` & `docker-run-cli-0.9.3/src/docker_run_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

