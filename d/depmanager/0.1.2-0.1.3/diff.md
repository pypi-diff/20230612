# Comparing `tmp/depmanager-0.1.2.tar.gz` & `tmp/depmanager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depmanager-0.1.2.tar", last modified: Wed May 31 19:17:52 2023, max compression
+gzip compressed data, was "depmanager-0.1.3.tar", last modified: Mon Jun 12 20:23:18 2023, max compression
```

## Comparing `depmanager-0.1.2.tar` & `depmanager-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.389080 depmanager-0.1.2/
--rw-rw-rw-   0        0        0     1085 2023-02-24 16:42:27.000000 depmanager-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    11884 2023-05-31 19:17:52.386079 depmanager-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10030 2023-05-31 18:53:07.000000 depmanager-0.1.2/README.md
--rw-rw-rw-   0        0        0     1054 2023-05-31 19:16:45.000000 depmanager-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 19:17:52.389080 depmanager-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.225079 depmanager-0.1.2/src/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.237080 depmanager-0.1.2/src/depmanager/
--rw-rw-rw-   0        0        0      149 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/depmanager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.285079 depmanager-0.1.2/src/depmanager/api/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/depmanager/api/__init__.py
--rw-rw-rw-   0        0        0     7722 2023-05-23 19:22:43.000000 depmanager-0.1.2/src/depmanager/api/builder.py
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.337079 depmanager-0.1.2/src/depmanager/api/internal/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/depmanager/api/internal/__init__.py
--rw-rw-rw-   0        0        0     4689 2023-04-04 21:53:30.000000 depmanager-0.1.2/src/depmanager/api/internal/common.py
--rw-rw-rw-   0        0        0     6216 2023-05-22 16:16:08.000000 depmanager-0.1.2/src/depmanager/api/internal/database_common.py
--rw-rw-rw-   0        0        0     2382 2023-05-22 18:14:20.000000 depmanager-0.1.2/src/depmanager/api/internal/database_local.py
--rw-rw-rw-   0        0        0     1688 2023-05-22 16:16:08.000000 depmanager-0.1.2/src/depmanager/api/internal/database_remote_folder.py
--rw-rw-rw-   0        0        0     2709 2023-05-22 16:16:08.000000 depmanager-0.1.2/src/depmanager/api/internal/database_remote_ftp.py
--rw-rw-rw-   0        0        0     9859 2023-05-22 19:54:58.000000 depmanager-0.1.2/src/depmanager/api/internal/database_remote_server.py
--rw-rw-rw-   0        0        0    10245 2023-05-22 19:47:09.000000 depmanager-0.1.2/src/depmanager/api/internal/dependency.py
--rw-rw-rw-   0        0        0    10471 2023-05-29 18:25:13.000000 depmanager-0.1.2/src/depmanager/api/internal/system.py
--rw-rw-rw-   0        0        0     1187 2023-05-30 20:57:30.000000 depmanager-0.1.2/src/depmanager/api/local.py
--rw-rw-rw-   0        0        0     6081 2023-05-22 13:45:00.000000 depmanager-0.1.2/src/depmanager/api/package.py
--rw-rw-rw-   0        0        0     1652 2023-05-22 21:20:13.000000 depmanager-0.1.2/src/depmanager/api/recipe.py
--rw-rw-rw-   0        0        0     2730 2023-04-05 20:47:10.000000 depmanager-0.1.2/src/depmanager/api/remotes.py
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.342080 depmanager-0.1.2/src/depmanager/cmake/
--rw-rw-rw-   0        0        0     3259 2023-04-07 21:42:17.000000 depmanager-0.1.2/src/depmanager/cmake/DepManager.cmake
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.382080 depmanager-0.1.2/src/depmanager/command/
--rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/depmanager/command/__init__.py
--rw-rw-rw-   0        0        0     2585 2023-05-22 21:13:04.000000 depmanager-0.1.2/src/depmanager/command/build.py
--rw-rw-rw-   0        0        0      858 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/depmanager/command/get.py
--rw-rw-rw-   0        0        0     1514 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/depmanager/command/info.py
--rw-rw-rw-   0        0        0     4620 2023-05-22 13:40:50.000000 depmanager-0.1.2/src/depmanager/command/pack.py
--rw-rw-rw-   0        0        0     5770 2023-05-18 18:58:14.000000 depmanager-0.1.2/src/depmanager/command/remote.py
--rw-rw-rw-   0        0        0     1770 2023-03-21 22:46:02.000000 depmanager-0.1.2/src/depmanager/manager.py
-drwxrwxrwx   0        0        0        0 2023-05-31 19:17:52.255080 depmanager-0.1.2/src/depmanager.egg-info/
--rw-rw-rw-   0        0        0    11884 2023-05-31 19:17:52.000000 depmanager-0.1.2/src/depmanager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1149 2023-05-31 19:17:52.000000 depmanager-0.1.2/src/depmanager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 19:17:52.000000 depmanager-0.1.2/src/depmanager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-31 19:17:52.000000 depmanager-0.1.2/src/depmanager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-31 19:17:52.000000 depmanager-0.1.2/src/depmanager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-31 19:17:52.000000 depmanager-0.1.2/src/depmanager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.425627 depmanager-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2023-02-24 16:42:27.000000 depmanager-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    12517 2023-06-12 20:23:18.424624 depmanager-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10663 2023-06-12 20:22:31.000000 depmanager-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1056 2023-06-12 20:22:31.000000 depmanager-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 20:23:18.426629 depmanager-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.332627 depmanager-0.1.3/src/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.337627 depmanager-0.1.3/src/depmanager/
+-rw-rw-rw-   0        0        0      149 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.368630 depmanager-0.1.3/src/depmanager/api/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/api/__init__.py
+-rw-rw-rw-   0        0        0     7819 2023-06-03 14:27:48.000000 depmanager-0.1.3/src/depmanager/api/builder.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.399626 depmanager-0.1.3/src/depmanager/api/internal/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/api/internal/__init__.py
+-rw-rw-rw-   0        0        0     4689 2023-04-04 21:53:30.000000 depmanager-0.1.3/src/depmanager/api/internal/common.py
+-rw-rw-rw-   0        0        0     6216 2023-06-03 13:54:25.000000 depmanager-0.1.3/src/depmanager/api/internal/database_common.py
+-rw-rw-rw-   0        0        0     2382 2023-05-22 18:14:20.000000 depmanager-0.1.3/src/depmanager/api/internal/database_local.py
+-rw-rw-rw-   0        0        0     1688 2023-05-22 16:16:08.000000 depmanager-0.1.3/src/depmanager/api/internal/database_remote_folder.py
+-rw-rw-rw-   0        0        0     2709 2023-05-22 16:16:08.000000 depmanager-0.1.3/src/depmanager/api/internal/database_remote_ftp.py
+-rw-rw-rw-   0        0        0    10198 2023-06-12 19:29:09.000000 depmanager-0.1.3/src/depmanager/api/internal/database_remote_server.py
+-rw-rw-rw-   0        0        0    10245 2023-05-22 19:47:09.000000 depmanager-0.1.3/src/depmanager/api/internal/dependency.py
+-rw-rw-rw-   0        0        0    10809 2023-06-12 19:29:00.000000 depmanager-0.1.3/src/depmanager/api/internal/system.py
+-rw-rw-rw-   0        0        0     1187 2023-05-31 20:43:17.000000 depmanager-0.1.3/src/depmanager/api/local.py
+-rw-rw-rw-   0        0        0     6386 2023-06-12 19:57:40.000000 depmanager-0.1.3/src/depmanager/api/package.py
+-rw-rw-rw-   0        0        0     1652 2023-05-22 21:20:13.000000 depmanager-0.1.3/src/depmanager/api/recipe.py
+-rw-rw-rw-   0        0        0     3229 2023-05-31 20:43:17.000000 depmanager-0.1.3/src/depmanager/api/remotes.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.402626 depmanager-0.1.3/src/depmanager/cmake/
+-rw-rw-rw-   0        0        0     3259 2023-04-07 21:42:17.000000 depmanager-0.1.3/src/depmanager/cmake/DepManager.cmake
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.420630 depmanager-0.1.3/src/depmanager/command/
+-rw-rw-rw-   0        0        0        0 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/command/__init__.py
+-rw-rw-rw-   0        0        0     2820 2023-06-03 13:50:57.000000 depmanager-0.1.3/src/depmanager/command/build.py
+-rw-rw-rw-   0        0        0      858 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/command/get.py
+-rw-rw-rw-   0        0        0     1514 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/command/info.py
+-rw-rw-rw-   0        0        0     4735 2023-06-12 19:44:48.000000 depmanager-0.1.3/src/depmanager/command/pack.py
+-rw-rw-rw-   0        0        0     5511 2023-05-31 20:43:17.000000 depmanager-0.1.3/src/depmanager/command/remote.py
+-rw-rw-rw-   0        0        0     1770 2023-03-21 22:46:02.000000 depmanager-0.1.3/src/depmanager/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:23:18.351629 depmanager-0.1.3/src/depmanager.egg-info/
+-rw-rw-rw-   0        0        0    12517 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1149 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-12 20:23:18.000000 depmanager-0.1.3/src/depmanager.egg-info/top_level.txt
```

### Comparing `depmanager-0.1.2/LICENSE` & `depmanager-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/PKG-INFO` & `depmanager-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depmanager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple Dependency manager
 Author-email: Silmaen <genteur.slayer@laposte.net>
 License: MIT License
         
         Copyright (c) 2023 Silmaen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,69 +28,72 @@
 Project-URL: Homepage, https://github.com/Silmaen/DepManager
 Keywords: dependency,setuptools,development
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DepManager
 
-Depmanager is a minimalistic tool to manage dependencies (also known as third-party 
+Depmanager is a minimalistic tool to manage dependencies (also known as third-party
 libraries) of a C++ Project. It works closely with cmake tool.
 
 It allow to store dependencies in a distant repository to share builds with other and
 have a local cache project-independent.
 
 ## Installation
 
-Depmanager is written in python so in the following we assume you have a 
+Depmanager is written in python so in the following we assume you have a
 working python installation designated as `<python>` with `pip` installed.
 
 ### pip
 
 To install dep manager simply use `<python> -m pip  install depmanager`
 
+See the page on Pypi: [depmanager](https://pypi.org/project/depmanager/).
+
 ### From source
 
 Prerequisite: python module 'build' install it with `<python> -m pip install build`
 
-Clone the github repository.
+Clone the gitHub repository.
 
 In the source root do:
+
 ```powershell
 <python> -m build
 <python> -m pip install dist/depmanager-x.y.z-py3-none-any.whl
 ```
 
 ## Commandline use
 
 ### Get help
 
-For any command or sub-command adding `--help` or `-h` to get help 
+For any command or sub-command adding `--help` or `-h` to get help
 on parameters or usage.
 
 ### Generalities
 
 In the base commande you can find:
 
 | command | subcommands                 | description                        |
 |---------|-----------------------------|------------------------------------|
 | info    | basedir, cmakedir, version  | info on local instance             |
 | get     |                             | Get the config package             |
 | pack    | pull, push, add, del, query | Manage packages                    |
 | remote  | list, add, del              | Manage the list of distant servers |
 | build   |                             | Build a new package                |
 
-In the following we will desigate `<query>` as something representing the description
-of a dependency. The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
- <type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
+In the following, `<query>` designate something representing the dependency's description.
+The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
+<type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
 
 Valid values for `type`: `shared`, `static`, `header`.
 
 Valid values for `os` : `Windows`, `Linux` (default: host os)
 
 Valid values for `arch` : `x86_64`, `aarch64` (default: host arch)
 
@@ -104,43 +107,44 @@
 If the name does not exist, it will fall back to default then to local.
 
 ## Base commands
 
 ### info
 
 subcommands:
- * `version` gives the version of the local manager.
- * `basedir` gives the path to the local data of the manager
- * `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
+
+* `version` gives the version of the local manager.
+* `basedir` gives the path to the local data of the manager
+* `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
 
 ### get
 
 `depmanager get <query>`
 
-Get path to cmake config of the 'best' package given the query information.
+Get path to cmake config of the 'best' package given by the query information.
 
 The command will only search in the local cache. This does not intent for human use but more for
 cmake integration.
 
 ### pack
 
 Actions on packages.
 
 #### query
 
-`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if 
+`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if
 nothing given) and print the result.
 
 #### add, del
 
 `depmanager pack add <location>` Will add a package to the local database. `<location>` can be a
 folder, then it must contain a properly formatted `edp.info` file. Or an archive (.zip, .tgz or .tar.gz
 file format allowed). The uncompressed archive must contain a properly formatted `edp.info` file.
 
-`depmanager pack del <query>` Will remove from local cache all package matching the query
+`depmanager pack del <query>` Will remove from local cache all package matching the query.
 
 #### push, pull
 
 `depmanager pack [push|pull] <query> <remote> [--force(-f)]` will synchronize Local cache with the remote.
 The `query` must be precise enough to match one and only one package. `remote` must be valid.
 
 `push` will look for the package in local cache that match the query and send it to the given remote.
@@ -149,30 +153,40 @@
 
 If `--force` is given, The transfert occurs even if the package already exists in the destination.
 
 ### remote
 
 Manage the list of remote servers
 subcommands:
- * `list` lists the defined remote server.
- * `add` adds a new remote to the list.
-   * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
-   * Name is mandatory. if the name already exist it will modify the existing one.
-   * Allowed proto are:
-     * `ftp` supports login
-     * `folder` a folder of your computer (mostly for debug or testing)
-     * `srv` a dedicated server see [github](https://github.com/Silmaen/DepManagerServer)
-     * `srvs` a dedicated server with secure connexion see [github](https://github.com/Silmaen/DepManagerServer)
-   * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
- * `del <remote>` remove the designated remote if exists.
- * `sync <remote>` push to remote all local package that does not already exist on remote.
+
+* `list` lists the defined remote server.
+* `add` adds a new remote to the list.
+    * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
+    * Mandatory. If name already exists it will modify the existing one.
+    * Allowed proto are:
+        * `ftp` supports login
+        * `folder` a folder of your computer (mostly for debug or testing)
+        * `srv` a dedicated server see [gitHub](https://github.com/Silmaen/DepManagerServer)
+        * `srvs` a dedicated server with secure connexion see [gitHub](https://github.com/Silmaen/DepManagerServer)
+    * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
+* `del <remote>` remove the designated remote if exists.
+* `sync <remote>` push to remote all local package that does not already exist on remote.
 
 ### build
 
-`depmanager build <location>` will search for recipe in the given location and build them.
+`depmanager build [OPTIONS] <location>` will search for recipe in the given location and build them.
+
+Some option can be passed to the build system:
+
+* `--single-thread`: on some low-end devices (such as RaspberryPi) single thread build is recommended.
+* `--force`, `-f`: Force the build even if the dependency already exists
+* `--cross-c`: redefine the C compiler
+* `--cross-cxx`: redefine the C++ compiler
+* `--cross-arch`: redefine the architecture
+* `--cross-os`: redefine the OS
 
 ## Using package with cmake
 
 ### Include depmanager to cmake
 
 To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
 to the cmake folder of this installation.
@@ -191,50 +205,51 @@
     list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
     include(DepManager)
 endif()
 ```
 
 ### Find packages
 
-With depmanager initialized in cmake, it provide an alternative to classical `find_package`
+With depmanager initialized in cmake, it provides an alternative to classical `find_package`
 of cmake by `dm_find_package`
 
 ```cmake
 dm_find_package(
    package
    [QUIET] [TRACE] [REQUIRED]
    [VERSION version]
    [KIND kind]
    [ARCH target_arch]
    [OS target_os]
    [COMPILER target_compiler]
 )
 ```
+
 `package` is the package name to find.
 
 `version` is the exact version to match (wildcard are allowed). By default, find the
 latest one.
 
 `kind` is used to force library kind (`shared`, `static`, `header`). By default it return
 the first found.
 
-If `REQUIRED` set, the function will give an error if no package found. 
+If `REQUIRED` set, the function will give an error if no package found.
 (same as original `find_package`)
 
 If `QUIET` set, only errors are written. (same as original `find_package`). In opposition,
 if `TRACE` set, many more debug message displayed.
 
 `target_arch`, `target_os`, `target_compiler` are used in the query. If not set, default
 values are `CMAKE_SYSTEM_PROCESSOR`, `CMAKE_SYSTEM_NAME` and `CMAKE_CXX_COMPILER_ID`
 
-**LIMITATION:** it require the library name is the package name. So no multi lib or lib with different name.
+**LIMITATION:** it requires the library name is the package name. So no multi lib or lib with different name.
 
 ### Load package
 
-This command is similar to the previous one, but does not directly do a cmake's `find_package`. 
+This command is similar to the previous one, but does not directly do a cmake's `find_package`.
 It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
 
 ```cmake
 dm_load_package(
    package
    [QUIET] [TRACE]
    [VERSION version]
@@ -245,57 +260,59 @@
 )
 ```
 
 After call this command, the cmake user has to call for needed `find_package`.
 
 ## Create you own package
 
-Depmanager allow you to create your own packages by defining recipes. Then run 
+Depmanager allow you to create your own packages by defining recipes. Then run
 `depmanager build <location of recipes>`
 The program will then build and add dependencies to the local cache.
 
 The location can contain as many recipe in any number of files.
 
 ### The recipe
 
 During build, Depmanager will look in all `.py` file for class that inherits from
 depmanager.api.recipe.Recipe.
 
 As for dependency usage, build also rely on cmake for building.
 
 The builder will use the provided recipe in the following workflow:
 
- * Init recipe
- * Call `recipe.source()`
- * Call `recipe.configure()`
- * Initialize options based on recipe data
- * Run cmake configure
- * For all configuration (mostly 'Debug', 'Release')
-   * build target `install`
- * Call `recipe.install()`
- * Generate edp.info file
- * Import into local cache
- * Clean Temporary
+* Init recipe
+* Call `recipe.source()`
+* Call `recipe.configure()`
+* Initialize options based on recipe data
+* Run cmake configure
+* For all configuration (mostly 'Debug', 'Release')
+    * build target `install`
+* Call `recipe.install()`
+* Generate edp.info file
+* Import into local cache
+* Clean Temporary
 
 Here is a small example
 
 ```python
 """
 Small recipe example
 """
 from depmanager.api.recipe import Recipe
 
+
 class MyAwesomeLib(Recipe):
     """
     Awesome lib
     """
     name = "awesome_lib"  # lib name
-    version = "0.0.1.foo" # lib version
-    source_dir = "src"    # where to fine the sources (especially) the CmakeList.txt
-    kind = "static"       # the lib's kind
+    version = "0.0.1.foo"  # lib version
+    source_dir = "src"  # where to fine the sources (especially) the CmakeList.txt
+    kind = "static"  # the lib's kind
+
 
 class AnotherAwesomeLib(MyAwesomeLib):
     """
     Shared version of previous one
     """
     kind = "shared"
 ```
@@ -303,29 +320,32 @@
 ## Roadmap
 
 First of all in the roadmap is to use this tool in C++ project to get feedback.
 
 Among things:
 
 * version 0.2.0
-  * [ ] Do query across multiple source (local then remote)
-  * [ ] Add a sorting order for remotes
-  * [ ] Auto-pull if not in local
-    * [ ] Auto build recipe if neither local or remote found
-  * [ ] Add concept of toolset
-    * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one
-    * [ ] Use toolset in build
-    * [ ] use toolset in queries
+    * [ ] Do query across multiple source (local then remote).
+    * [ ] Add a sorting order for remotes.
+    * [ ] Auto-pull if not in local.
+        * [ ] Auto build recipe if neither local nor remote found.
+    * [ ] Add concept of toolset.
+        * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
+        * [ ] Use toolset in build.
+        * [ ] use toolset in queries.
+* version 0.1.4
+    * [ ] Add build Date in package properties.
+    * [ ] Allow to force push/pull.
+    * [ ] Allow to sync with remote.
+        * [ ] Allow to pull local package that have newer version.
+        * [ ] Allow to push local package newer than remote or not existing in remote.
 * version 0.1.3
-  * [ ] omit -d in push/pull command
-  * [ ] add progressbass in push/pull command
-  * [ ] Add build Date in package properties
-  * [ ] Allow to force push/pull
-  * [ ] Allow to sync with remote
-    * [ ] Allow to pull local package that have newer version
-    * [ ] Allow to push local package newer than remote or not existing in remote
+    * [X] Update internal statuses when using API.
+    * [X] omit -d in push/pull command.
+    * [X] add progress bar in push/pull command.
+    * [X] Allow single thread in build.
 * version 0.1.2
-  * [X] Add possibility to force os, arch and compiler for cross compiling
-  * [X] Adapt build system to search dependency in the forced environment.
+    * [X] Add possibility to force os, arch and compiler for cross compiling.
+    * [X] Adapt build system to search dependency in the forced environment.
 * version 0.1.1
-  * [X] Add remote Type of 'srv': a dedicated dependency server
-  * [X] Add remote Type of 'srvs': a dedicated dependency server with secure connexion
+    * [X] Add remote 'srv' Type: a dedicated dependency server.
+    * [X] Add remote 'srvs' Type: a dedicated dependency server with secure connexion.
```

### Comparing `depmanager-0.1.2/README.md` & `depmanager-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 # DepManager
 
-Depmanager is a minimalistic tool to manage dependencies (also known as third-party 
+Depmanager is a minimalistic tool to manage dependencies (also known as third-party
 libraries) of a C++ Project. It works closely with cmake tool.
 
 It allow to store dependencies in a distant repository to share builds with other and
 have a local cache project-independent.
 
 ## Installation
 
-Depmanager is written in python so in the following we assume you have a 
+Depmanager is written in python so in the following we assume you have a
 working python installation designated as `<python>` with `pip` installed.
 
 ### pip
 
 To install dep manager simply use `<python> -m pip  install depmanager`
 
+See the page on Pypi: [depmanager](https://pypi.org/project/depmanager/).
+
 ### From source
 
 Prerequisite: python module 'build' install it with `<python> -m pip install build`
 
-Clone the github repository.
+Clone the gitHub repository.
 
 In the source root do:
+
 ```powershell
 <python> -m build
 <python> -m pip install dist/depmanager-x.y.z-py3-none-any.whl
 ```
 
 ## Commandline use
 
 ### Get help
 
-For any command or sub-command adding `--help` or `-h` to get help 
+For any command or sub-command adding `--help` or `-h` to get help
 on parameters or usage.
 
 ### Generalities
 
 In the base commande you can find:
 
 | command | subcommands                 | description                        |
 |---------|-----------------------------|------------------------------------|
 | info    | basedir, cmakedir, version  | info on local instance             |
 | get     |                             | Get the config package             |
 | pack    | pull, push, add, del, query | Manage packages                    |
 | remote  | list, add, del              | Manage the list of distant servers |
 | build   |                             | Build a new package                |
 
-In the following we will desigate `<query>` as something representing the description
-of a dependency. The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
- <type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
+In the following, `<query>` designate something representing the dependency's description.
+The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
+<type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
 
 Valid values for `type`: `shared`, `static`, `header`.
 
 Valid values for `os` : `Windows`, `Linux` (default: host os)
 
 Valid values for `arch` : `x86_64`, `aarch64` (default: host arch)
 
@@ -66,43 +69,44 @@
 If the name does not exist, it will fall back to default then to local.
 
 ## Base commands
 
 ### info
 
 subcommands:
- * `version` gives the version of the local manager.
- * `basedir` gives the path to the local data of the manager
- * `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
+
+* `version` gives the version of the local manager.
+* `basedir` gives the path to the local data of the manager
+* `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
 
 ### get
 
 `depmanager get <query>`
 
-Get path to cmake config of the 'best' package given the query information.
+Get path to cmake config of the 'best' package given by the query information.
 
 The command will only search in the local cache. This does not intent for human use but more for
 cmake integration.
 
 ### pack
 
 Actions on packages.
 
 #### query
 
-`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if 
+`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if
 nothing given) and print the result.
 
 #### add, del
 
 `depmanager pack add <location>` Will add a package to the local database. `<location>` can be a
 folder, then it must contain a properly formatted `edp.info` file. Or an archive (.zip, .tgz or .tar.gz
 file format allowed). The uncompressed archive must contain a properly formatted `edp.info` file.
 
-`depmanager pack del <query>` Will remove from local cache all package matching the query
+`depmanager pack del <query>` Will remove from local cache all package matching the query.
 
 #### push, pull
 
 `depmanager pack [push|pull] <query> <remote> [--force(-f)]` will synchronize Local cache with the remote.
 The `query` must be precise enough to match one and only one package. `remote` must be valid.
 
 `push` will look for the package in local cache that match the query and send it to the given remote.
@@ -111,30 +115,40 @@
 
 If `--force` is given, The transfert occurs even if the package already exists in the destination.
 
 ### remote
 
 Manage the list of remote servers
 subcommands:
- * `list` lists the defined remote server.
- * `add` adds a new remote to the list.
-   * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
-   * Name is mandatory. if the name already exist it will modify the existing one.
-   * Allowed proto are:
-     * `ftp` supports login
-     * `folder` a folder of your computer (mostly for debug or testing)
-     * `srv` a dedicated server see [github](https://github.com/Silmaen/DepManagerServer)
-     * `srvs` a dedicated server with secure connexion see [github](https://github.com/Silmaen/DepManagerServer)
-   * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
- * `del <remote>` remove the designated remote if exists.
- * `sync <remote>` push to remote all local package that does not already exist on remote.
+
+* `list` lists the defined remote server.
+* `add` adds a new remote to the list.
+    * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
+    * Mandatory. If name already exists it will modify the existing one.
+    * Allowed proto are:
+        * `ftp` supports login
+        * `folder` a folder of your computer (mostly for debug or testing)
+        * `srv` a dedicated server see [gitHub](https://github.com/Silmaen/DepManagerServer)
+        * `srvs` a dedicated server with secure connexion see [gitHub](https://github.com/Silmaen/DepManagerServer)
+    * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
+* `del <remote>` remove the designated remote if exists.
+* `sync <remote>` push to remote all local package that does not already exist on remote.
 
 ### build
 
-`depmanager build <location>` will search for recipe in the given location and build them.
+`depmanager build [OPTIONS] <location>` will search for recipe in the given location and build them.
+
+Some option can be passed to the build system:
+
+* `--single-thread`: on some low-end devices (such as RaspberryPi) single thread build is recommended.
+* `--force`, `-f`: Force the build even if the dependency already exists
+* `--cross-c`: redefine the C compiler
+* `--cross-cxx`: redefine the C++ compiler
+* `--cross-arch`: redefine the architecture
+* `--cross-os`: redefine the OS
 
 ## Using package with cmake
 
 ### Include depmanager to cmake
 
 To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
 to the cmake folder of this installation.
@@ -153,50 +167,51 @@
     list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
     include(DepManager)
 endif()
 ```
 
 ### Find packages
 
-With depmanager initialized in cmake, it provide an alternative to classical `find_package`
+With depmanager initialized in cmake, it provides an alternative to classical `find_package`
 of cmake by `dm_find_package`
 
 ```cmake
 dm_find_package(
    package
    [QUIET] [TRACE] [REQUIRED]
    [VERSION version]
    [KIND kind]
    [ARCH target_arch]
    [OS target_os]
    [COMPILER target_compiler]
 )
 ```
+
 `package` is the package name to find.
 
 `version` is the exact version to match (wildcard are allowed). By default, find the
 latest one.
 
 `kind` is used to force library kind (`shared`, `static`, `header`). By default it return
 the first found.
 
-If `REQUIRED` set, the function will give an error if no package found. 
+If `REQUIRED` set, the function will give an error if no package found.
 (same as original `find_package`)
 
 If `QUIET` set, only errors are written. (same as original `find_package`). In opposition,
 if `TRACE` set, many more debug message displayed.
 
 `target_arch`, `target_os`, `target_compiler` are used in the query. If not set, default
 values are `CMAKE_SYSTEM_PROCESSOR`, `CMAKE_SYSTEM_NAME` and `CMAKE_CXX_COMPILER_ID`
 
-**LIMITATION:** it require the library name is the package name. So no multi lib or lib with different name.
+**LIMITATION:** it requires the library name is the package name. So no multi lib or lib with different name.
 
 ### Load package
 
-This command is similar to the previous one, but does not directly do a cmake's `find_package`. 
+This command is similar to the previous one, but does not directly do a cmake's `find_package`.
 It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
 
 ```cmake
 dm_load_package(
    package
    [QUIET] [TRACE]
    [VERSION version]
@@ -207,57 +222,59 @@
 )
 ```
 
 After call this command, the cmake user has to call for needed `find_package`.
 
 ## Create you own package
 
-Depmanager allow you to create your own packages by defining recipes. Then run 
+Depmanager allow you to create your own packages by defining recipes. Then run
 `depmanager build <location of recipes>`
 The program will then build and add dependencies to the local cache.
 
 The location can contain as many recipe in any number of files.
 
 ### The recipe
 
 During build, Depmanager will look in all `.py` file for class that inherits from
 depmanager.api.recipe.Recipe.
 
 As for dependency usage, build also rely on cmake for building.
 
 The builder will use the provided recipe in the following workflow:
 
- * Init recipe
- * Call `recipe.source()`
- * Call `recipe.configure()`
- * Initialize options based on recipe data
- * Run cmake configure
- * For all configuration (mostly 'Debug', 'Release')
-   * build target `install`
- * Call `recipe.install()`
- * Generate edp.info file
- * Import into local cache
- * Clean Temporary
+* Init recipe
+* Call `recipe.source()`
+* Call `recipe.configure()`
+* Initialize options based on recipe data
+* Run cmake configure
+* For all configuration (mostly 'Debug', 'Release')
+    * build target `install`
+* Call `recipe.install()`
+* Generate edp.info file
+* Import into local cache
+* Clean Temporary
 
 Here is a small example
 
 ```python
 """
 Small recipe example
 """
 from depmanager.api.recipe import Recipe
 
+
 class MyAwesomeLib(Recipe):
     """
     Awesome lib
     """
     name = "awesome_lib"  # lib name
-    version = "0.0.1.foo" # lib version
-    source_dir = "src"    # where to fine the sources (especially) the CmakeList.txt
-    kind = "static"       # the lib's kind
+    version = "0.0.1.foo"  # lib version
+    source_dir = "src"  # where to fine the sources (especially) the CmakeList.txt
+    kind = "static"  # the lib's kind
+
 
 class AnotherAwesomeLib(MyAwesomeLib):
     """
     Shared version of previous one
     """
     kind = "shared"
 ```
@@ -265,29 +282,32 @@
 ## Roadmap
 
 First of all in the roadmap is to use this tool in C++ project to get feedback.
 
 Among things:
 
 * version 0.2.0
-  * [ ] Do query across multiple source (local then remote)
-  * [ ] Add a sorting order for remotes
-  * [ ] Auto-pull if not in local
-    * [ ] Auto build recipe if neither local or remote found
-  * [ ] Add concept of toolset
-    * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one
-    * [ ] Use toolset in build
-    * [ ] use toolset in queries
+    * [ ] Do query across multiple source (local then remote).
+    * [ ] Add a sorting order for remotes.
+    * [ ] Auto-pull if not in local.
+        * [ ] Auto build recipe if neither local nor remote found.
+    * [ ] Add concept of toolset.
+        * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
+        * [ ] Use toolset in build.
+        * [ ] use toolset in queries.
+* version 0.1.4
+    * [ ] Add build Date in package properties.
+    * [ ] Allow to force push/pull.
+    * [ ] Allow to sync with remote.
+        * [ ] Allow to pull local package that have newer version.
+        * [ ] Allow to push local package newer than remote or not existing in remote.
 * version 0.1.3
-  * [ ] omit -d in push/pull command
-  * [ ] add progressbass in push/pull command
-  * [ ] Add build Date in package properties
-  * [ ] Allow to force push/pull
-  * [ ] Allow to sync with remote
-    * [ ] Allow to pull local package that have newer version
-    * [ ] Allow to push local package newer than remote or not existing in remote
+    * [X] Update internal statuses when using API.
+    * [X] omit -d in push/pull command.
+    * [X] add progress bar in push/pull command.
+    * [X] Allow single thread in build.
 * version 0.1.2
-  * [X] Add possibility to force os, arch and compiler for cross compiling
-  * [X] Adapt build system to search dependency in the forced environment.
+    * [X] Add possibility to force os, arch and compiler for cross compiling.
+    * [X] Adapt build system to search dependency in the forced environment.
 * version 0.1.1
-  * [X] Add remote Type of 'srv': a dedicated dependency server
-  * [X] Add remote Type of 'srvs': a dedicated dependency server with secure connexion
+    * [X] Add remote 'srv' Type: a dedicated dependency server.
+    * [X] Add remote 'srvs' Type: a dedicated dependency server with secure connexion.
```

### Comparing `depmanager-0.1.2/pyproject.toml` & `depmanager-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "depmanager"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
-    {name = "Silmaen", email = "genteur.slayer@laposte.net"}
+    { name = "Silmaen", email = "genteur.slayer@laposte.net" }
 ]
 description = "Simple Dependency manager"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 classifiers = [
     # How mature is this project? Common values are
     #   3 - Alpha
     #   4 - Beta
     #   5 - Production/Stable
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `depmanager-0.1.2/src/depmanager/api/builder.py` & `depmanager-0.1.3/src/depmanager/api/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,16 @@
 
             #
             #
             # build & install
             if cont:
                 for conf in rec.config:
                     cmd = F"cmake --build {self.temp / 'build'} --target install --config {conf}"
+                    if self.cross_info["SINGLE_THREAD"]:
+                        cmd += F" -j 1"
                     cont = try_run(cmd)
                     if not cont:
                         break
 
             #
             #
             # create the info file
```

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/common.py` & `depmanager-0.1.3/src/depmanager/api/internal/common.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/database_common.py` & `depmanager-0.1.3/src/depmanager/api/internal/database_common.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/database_local.py` & `depmanager-0.1.3/src/depmanager/api/internal/database_local.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/database_remote_folder.py` & `depmanager-0.1.3/src/depmanager/api/internal/database_remote_folder.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/database_remote_ftp.py` & `depmanager-0.1.3/src/depmanager/api/internal/database_remote_ftp.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/database_remote_server.py` & `depmanager-0.1.3/src/depmanager/api/internal/database_remote_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """
 Remote FTP database
 """
 from datetime import datetime
-from sys import stderr, stdout
 from pathlib import Path
-from requests.auth import HTTPBasicAuth
-from requests import get as httpget, post as httppost
-from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
+from sys import stderr, stdout
 
 from depmanager.api.internal.database_common import __RemoteDatabase
 from depmanager.api.internal.dependency import Dependency
+from requests import get as httpget, post as httppost
+from requests.auth import HTTPBasicAuth
+from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
 
 class RemoteDatabaseServer(__RemoteDatabase):
     """
     Remote database using server protocol.
     """
 
-    def __init__(self, destination: str, port: int = -1, secure: bool = False, default: bool = False, user: str = "", cred: str = "", verbosity:int  = 0):
+    def __init__(self, destination: str, port: int = -1, secure: bool = False, default: bool = False, user: str = "",
+                 cred: str = "", verbosity: int = 0):
         self.port = port
         if self.port == -1:
             if secure:
                 self.port = 443
             else:
                 self.port = 80
         self.secure = secure
-        self.kind = ["srv","srvs"][secure]
-        true_destination = f"http{['','s'][secure]}://{destination}"
+        self.kind = ["srv", "srvs"][secure]
+        true_destination = f"http{['', 's'][secure]}://{destination}"
         if secure:
             if self.port != 443:
                 true_destination += f":{self.port}"
         else:
             if self.port != 80:
                 true_destination += f":{self.port}"
-        super().__init__(destination=true_destination, default=default, user=user, cred=cred, kind = self.kind, verbosity=verbosity)
+        super().__init__(destination=true_destination, default=default, user=user, cred=cred, kind=self.kind,
+                         verbosity=verbosity)
 
     def connect(self):
         """
         Initialize the connection to remote host.
         TO IMPLEMENT IN DERIVED CLASS.
         """
         pass
@@ -47,20 +49,22 @@
         Get a list of string describing dependency from the server.
         """
         try:
             basic = HTTPBasicAuth(self.user, self.cred)
             resp = httpget(f"{self.destination}/api", auth=basic)
             if resp.status_code != 200:
                 self.valid_shape = False
-                print(f"ERROR connecting to server: {self.destination}: {resp.status_code}: {resp.reason}")
+                print(f"ERROR connecting to server: {self.destination}: {resp.status_code}: {resp.reason}", file=stderr)
+                print(f"  Response from server:\n{resp.text}", file=stderr)
+                print(f"--request--: {resp.request}")
                 return
             data = resp.text.splitlines(keepends=False)
             self.deps_from_strings(data)
         except Exception as err:
-            print(f"ERROR Exception during server connexion: {self.destination}: {err}")
+            print(f"ERROR Exception during server connexion: {self.destination}: {err}", file=stderr)
             return
 
     def dep_to_code(self, dep: Dependency):
         data = {}
         if dep.properties.name not in ["", None]:
             data["name"] = dep.properties.name
         if dep.properties.version not in ["", None]:
@@ -116,30 +120,32 @@
 
             if resp.status_code != 200:
                 self.valid_shape = False
                 print(f"ERROR connecting to server: {self.destination}: {resp.status_code}: {resp.reason}", file=stderr)
                 print(f"      Server Data: {resp.text}", file=stderr)
                 return
             data = resp.text.strip()
-            filename = data.rsplit("/",1)[-1]
+            filename = data.rsplit("/", 1)[-1]
             if filename.startswith(dep.properties.name):
                 filename = filename.replace(dep.properties.name, "")
             fname = destination / filename
             resp = httpget(f"{self.destination}{data}", auth=basic)
             if resp.status_code != 200:
                 self.valid_shape = False
-                print(f"ERROR retrieving file {data} from server {self.destination}: {resp.status_code}: {resp.reason}, see error.log", file=stderr)
+                print(
+                        f"ERROR retrieving file {data} from server {self.destination}: {resp.status_code}: {resp.reason}, see error.log",
+                        file=stderr)
                 with open("error.log", "ab") as fp:
                     fp.write(f"---- ERROR: {datetime.now()} ---- \n".encode('utf8'))
                     fp.write(resp.content)
                 return
             with open(fname, "wb") as fp:
                 fp.write(resp.content)
         except Exception as err:
-            print(f"ERROR Exception during server pull: {self.destination}: {err}")
+            print(f"ERROR Exception during server pull: {self.destination}: {err}", file=stderr)
             return
 
     def create_callback(self, encoder):
         """
         Create a callback for the given encoder.
         :param encoder: The encoder.
         :return: A monitor call back.
@@ -185,15 +191,17 @@
                 post_data["package"] = (file.name, open(file, "rb"), "application/octet-stream")
                 encoder = MultipartEncoder(fields=post_data)
                 monitor = MultipartEncoderMonitor(encoder)
                 headers = {"Content-Type": monitor.content_type}
                 resp = httppost(f"{self.destination}/api", auth=basic, data=monitor, headers=headers)
                 if resp.status_code != 200:
                     self.valid_shape = False
-                    print(f"ERROR connecting to server: {self.destination}: {resp.status_code}: {resp.reason}, see error.log", file=stderr)
+                    print(
+                            f"ERROR connecting to server: {self.destination}: {resp.status_code}: {resp.reason}, see error.log",
+                            file=stderr)
                     with open("error.log", "ab") as fp:
                         fp.write(f"---- ERROR: {datetime.now()} ---- \n".encode('utf8'))
                         fp.write(resp.content)
                     return
             else:
                 basic = HTTPBasicAuth(self.user, self.cred)
                 post_data = {"action": "push"} | self.dep_to_code(dep)
@@ -201,22 +209,22 @@
                 encoder = MultipartEncoder(fields=post_data)
                 monitor = MultipartEncoderMonitor(encoder, callback=self.create_callback(encoder))
                 headers = {"Content-Type": monitor.content_type}
                 resp = httppost(f"{self.destination}/upload", auth=basic, data=monitor, headers=headers)
                 if resp.status_code != 200:
                     self.valid_shape = False
                     print(
-                        f"ERROR connecting to server: {self.destination}: {resp.status_code}: {resp.reason}, see error.log",
-                        file=stderr)
+                            f"ERROR connecting to server: {self.destination}: {resp.status_code}: {resp.reason}, see error.log",
+                            file=stderr)
                     with open("error.log", "ab") as fp:
                         fp.write(f"---- ERROR: {datetime.now()} ---- \n".encode('utf8'))
                         fp.write(resp.content)
                     return
         except Exception as err:
-            print(f"ERROR Exception during server push: {self.destination}: {err}")
+            print(f"ERROR Exception during server push: {self.destination}: {err}", file=stderr)
             return
 
     def get_file(self, distant_name: str, destination: Path):
         """
         Download a file.
         TO IMPLEMENT IN DERIVED CLASS.
         :param distant_name: Name in the distant location.
```

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/dependency.py` & `depmanager-0.1.3/src/depmanager/api/internal/dependency.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/api/internal/system.py` & `depmanager-0.1.3/src/depmanager/api/internal/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Everything needed for database.
 """
 from pathlib import Path
 from shutil import rmtree
 from sys import stderr
 from time import sleep
 
-from depmanager.api.internal.dependency import Props
 from depmanager.api.internal.database_local import LocalDatabase
-from depmanager.api.internal.database_remote_ftp import RemoteDatabaseFtp
 from depmanager.api.internal.database_remote_folder import RemoteDatabaseFolder
+from depmanager.api.internal.database_remote_ftp import RemoteDatabaseFtp
 from depmanager.api.internal.database_remote_server import RemoteDatabaseServer
+from depmanager.api.internal.dependency import Props
 
 
 class LocalSystem:
     """
     System manager.
     """
     supported_remote = ["srv", "srvs", "ftp", "folder"]
@@ -183,15 +183,19 @@
                 login = data["login"]
             else:
                 login = ""
             if "passwd" in data:
                 passwd = data["passwd"]
             else:
                 passwd = ""
-            self.remote_database[name] = RemoteDatabaseServer(url, port, default, login, passwd)
+            self.remote_database[name] = RemoteDatabaseServer(destination=url, port=port, secure=kind == "srvs",
+                                                              default=default, user=login, cred=passwd)
+            if not self.remote_database[name].valid_shape:
+                print("Error: cannot add the remote!", file=stderr)
+                return False
             self.config["remotes"][name] = {
                 "url"    : url,
                 "port"   : port,
                 "default": default,
                 "kind"   : kind
             }
             if ("port" != 80 and kind == "srv") or ("port" != 443 and kind == "srvs"):
@@ -267,14 +271,16 @@
         """
         from shutil import copytree
         p = Props()
         p.from_edp_file(source / "edp.info")
         destination_folder = self.local_database.base_path / f"{p.name}{p.hash()}"
         rmtree(destination_folder, ignore_errors=True)
         copytree(source, destination_folder)
+        self.clear_tmp()
+        self.local_database.reload()
 
     def remove_local(self, pack):
         """
         Remove from local database.
         :param pack: Package's query to remove.
         """
         self.local_database.delete(pack)
```

### Comparing `depmanager-0.1.2/src/depmanager/api/local.py` & `depmanager-0.1.3/src/depmanager/api/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 
 class LocalManager:
     """
     Local manager.
     """
-    version = "0.1.2"
+    version = "0.1.3"
 
     def __init__(self, system=None):
         from depmanager.api.internal.system import LocalSystem
         if isinstance(system, LocalSystem):
             self.__sys = system
         else:
             self.__sys = LocalSystem()
```

### Comparing `depmanager-0.1.2/src/depmanager/api/package.py` & `depmanager-0.1.3/src/depmanager/api/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class PackageManager:
     """
     Manager fo package.
     """
 
-    def __init__(self, system=None, verbosity:int = 0):
+    def __init__(self, system=None, verbosity: int = 0):
         from depmanager.api.internal.system import LocalSystem
         from depmanager.api.local import LocalManager
         self.verbosity = verbosity
         if isinstance(system, LocalSystem):
             self.__sys = system
         elif isinstance(system, LocalManager):
             self.__sys = system.get_sys()
@@ -65,20 +65,24 @@
                 suffixes = [source.suffixes[-1]]
                 if suffixes == [".gz"] and len(source.suffixes) > 1:
                     suffixes = [source.suffixes[-2], source.suffixes[-1]]
             if suffixes == ["zip"]:
                 from zipfile import ZipFile
                 destination_dir = self.__sys.temp_path / "pack"
                 destination_dir.mkdir(parents=True)
+                if self.verbosity > 2:
+                    print(f"PackageManager::add_from_location - Extract ZIP from {source} to {destination_dir}")
                 with ZipFile(source) as archive:
                     archive.extractall(destination_dir)
             elif suffixes in [[".tgz"], [".tar", ".gz"]]:
                 import tarfile
                 destination_dir = self.__sys.temp_path / "pack"
                 destination_dir.mkdir(parents=True)
+                if self.verbosity > 2:
+                    print(f"PackageManager::add_from_location - Extract TGZ from {source} to {destination_dir}")
                 with tarfile.open(str(source), "r|gz") as archive:
                     archive.extractall(destination_dir)
             else:
                 print(f"WARNING: File {source} has unsupported format.", file=stderr)
                 return
             if destination_dir is not None:
                 if not (destination_dir / "edp.info").exists():
```

### Comparing `depmanager-0.1.2/src/depmanager/api/recipe.py` & `depmanager-0.1.3/src/depmanager/api/recipe.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/api/remotes.py` & `depmanager-0.1.3/src/depmanager/api/remotes.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,29 @@
     def get_supported_remotes(self):
         """
         Get lit of supported remote kind.
         :return: Supported remotes.
         """
         return self.__sys.supported_remote
 
+    def get_safe_remote(self, name, default:bool = False):
+        """
+        Get remote or default or None (only if no default exists)
+        :param name: Remote name
+        :param default: to force using default
+        :return: the remote
+        """
+        if default or type(name) != str or name in ["", None]:
+            remote =  None
+        else:
+            remote = self.get_remote(name)
+        if remote is None:
+            return self.get_default_remote()
+        return remote
+
     def get_remote(self, name: str):
         """
         Access to remote with given name.
         :param name: Name of the remote.
         :return: The remote or None.
         """
         if name not in self.__sys.remote_database:
```

### Comparing `depmanager-0.1.2/src/depmanager/cmake/DepManager.cmake` & `depmanager-0.1.3/src/depmanager/cmake/DepManager.cmake`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/command/build.py` & `depmanager-0.1.3/src/depmanager/command/build.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         cross_info["C_COMPILER"] = args.cross_c
     if args.cross_cxx not in ["", None]:
         cross_info["CXX_COMPILER"] = args.cross_cxx
     if args.cross_arch not in ["", None]:
         cross_info["CROSS_ARCH"] = args.cross_arch
     if args.cross_os not in ["", None]:
         cross_info["CROSS_OS"] = args.cross_os
+    cross_info["SINGLE_THREAD"] = args.single_thread
     builder = Builder(location, local=system, cross_info =cross_info)
     if not builder.has_recipes():
         print(f"ERROR: no recipe found in {location}", file=stderr)
         exit(-666)
     print(f"found {len(builder.recipes)} in the given source folder")
     for rep in builder.recipes:
         print(f" - {rep.to_str()}")
@@ -73,8 +74,14 @@
             help="Define the cross archi.")
     build_parser.add_argument(
             "--cross-os",
             type=str,
             default="",
             help="Define the cross OS."
     )
+    build_parser.add_argument(
+            "--single-thread", "-s",
+            action="store_true",
+            default="",
+            help="Force the use of single thread."
+    )
     build_parser.set_defaults(func=build)
```

### Comparing `depmanager-0.1.2/src/depmanager/command/get.py` & `depmanager-0.1.3/src/depmanager/command/get.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/command/info.py` & `depmanager-0.1.3/src/depmanager/command/info.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager/command/pack.py` & `depmanager-0.1.3/src/depmanager/command/pack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Pack command
 """
-from sys import stderr
 from pathlib import Path
+from sys import stderr
 
 possible_info = ["pull", "push", "add", "del", "query"]
 
 
 def pack(args, system=None):
     """
     Entry point for pack command.
@@ -27,16 +27,19 @@
             print("WARNING: No Remotes defined.", file=stderr)
         if args.name not in [None, ""]:
             print(f"WARNING: Remotes '{args.name}' not in remotes lists.", file=stderr)
     if args.what in ["add", "del"] and remote_name != "":
         print(f"ERROR: {args.what} command only work on local database. please do not defined remote.", file=stderr)
         exit(-666)
     if args.what in ["push", "pull"] and remote_name == "":
-        print(f"ERROR: {args.what} command work by linking to a remote, please define a remote.", file=stderr)
-        exit(-666)
+        args.default = True
+        remote_name = pacman.remote_name(args)
+        if remote_name == "":
+            print(f"ERROR: {args.what} command work by linking to a remote, please define a remote.", file=stderr)
+            exit(-666)
     if args.what == "add":
         if args.source in [None, ""]:
             print(f"ERROR: please provide a source for package adding.", file=stderr)
             exit(-666)
         source_path = Path(args.source).resolve()
         if not source_path.exists():
             print(f"ERROR: source path {source_path} does not exists.", file=stderr)
@@ -64,18 +67,18 @@
         deps = pacman.query(query, remote_name)
     if args.what == "query":
         for dep in deps:
             print(f"{dep.properties.get_as_str()}")
         return
     if args.what in ["del", "pull", "push"]:
         if len(deps) == 0:
-            print("WARNING: No package mathing the query.", file=stderr)
+            print("WARNING: No package matching the query.", file=stderr)
             return
         if len(deps) > 1:
-            print("WARNING: More than one package math the query, please precise:", file=stderr)
+            print("WARNING: More than one package match the query, please precise:", file=stderr)
             for dep in deps:
                 print(f"{dep.properties.get_as_str()}")
             return
         dep = deps[0]
         if args.what == "del":
             pacman.remove_package(dep)
         elif args.what == "pull":
```

### Comparing `depmanager-0.1.2/src/depmanager/command/remote.py` & `depmanager-0.1.3/src/depmanager/command/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,21 +71,15 @@
 
     def sync(self, name: str, default: bool = False):
         """
         Synchronize local with given remote (push to server all unexisting package).
         :param name: Remote's name.
         :param default: If using default remote
         """
-        if default:
-            remote_db = self.remote_instance.get_default_remote()
-        else:
-            if type(name) != str or name in ["", None]:
-                print(f"ERROR please give a name for syncing a remote.", file=stderr)
-                exit(-666)
-            remote_db = self.remote_instance.get_remote(name)
+        remote_db = self.remote_instance.get_safe_remote(name, default)
         if remote_db is None:
             print(f"ERROR remote {name} not found.", file=stderr)
             exit(-666)
         local_db = self.remote_instance.get_local()
         all_local = local_db.query({
             "name": "*",
             "version": "*",
```

### Comparing `depmanager-0.1.2/src/depmanager/manager.py` & `depmanager-0.1.3/src/depmanager/manager.py`

 * *Files identical despite different names*

### Comparing `depmanager-0.1.2/src/depmanager.egg-info/PKG-INFO` & `depmanager-0.1.3/src/depmanager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depmanager
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple Dependency manager
 Author-email: Silmaen <genteur.slayer@laposte.net>
 License: MIT License
         
         Copyright (c) 2023 Silmaen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,69 +28,72 @@
 Project-URL: Homepage, https://github.com/Silmaen/DepManager
 Keywords: dependency,setuptools,development
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DepManager
 
-Depmanager is a minimalistic tool to manage dependencies (also known as third-party 
+Depmanager is a minimalistic tool to manage dependencies (also known as third-party
 libraries) of a C++ Project. It works closely with cmake tool.
 
 It allow to store dependencies in a distant repository to share builds with other and
 have a local cache project-independent.
 
 ## Installation
 
-Depmanager is written in python so in the following we assume you have a 
+Depmanager is written in python so in the following we assume you have a
 working python installation designated as `<python>` with `pip` installed.
 
 ### pip
 
 To install dep manager simply use `<python> -m pip  install depmanager`
 
+See the page on Pypi: [depmanager](https://pypi.org/project/depmanager/).
+
 ### From source
 
 Prerequisite: python module 'build' install it with `<python> -m pip install build`
 
-Clone the github repository.
+Clone the gitHub repository.
 
 In the source root do:
+
 ```powershell
 <python> -m build
 <python> -m pip install dist/depmanager-x.y.z-py3-none-any.whl
 ```
 
 ## Commandline use
 
 ### Get help
 
-For any command or sub-command adding `--help` or `-h` to get help 
+For any command or sub-command adding `--help` or `-h` to get help
 on parameters or usage.
 
 ### Generalities
 
 In the base commande you can find:
 
 | command | subcommands                 | description                        |
 |---------|-----------------------------|------------------------------------|
 | info    | basedir, cmakedir, version  | info on local instance             |
 | get     |                             | Get the config package             |
 | pack    | pull, push, add, del, query | Manage packages                    |
 | remote  | list, add, del              | Manage the list of distant servers |
 | build   |                             | Build a new package                |
 
-In the following we will desigate `<query>` as something representing the description
-of a dependency. The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
- <type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
+In the following, `<query>` designate something representing the dependency's description.
+The syntax reads:  `--predicate(-p) <name>:<version> --type(-t)
+<type> --os(-o) <os> --arch(-a) <arch> --compiler(-c) <compiler>`
 
 Valid values for `type`: `shared`, `static`, `header`.
 
 Valid values for `os` : `Windows`, `Linux` (default: host os)
 
 Valid values for `arch` : `x86_64`, `aarch64` (default: host arch)
 
@@ -104,43 +107,44 @@
 If the name does not exist, it will fall back to default then to local.
 
 ## Base commands
 
 ### info
 
 subcommands:
- * `version` gives the version of the local manager.
- * `basedir` gives the path to the local data of the manager
- * `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
+
+* `version` gives the version of the local manager.
+* `basedir` gives the path to the local data of the manager
+* `cmakedir` gives the path to add to `CMAKE_MODULE_PATH` before include `ExternalDependencyManager`
 
 ### get
 
 `depmanager get <query>`
 
-Get path to cmake config of the 'best' package given the query information.
+Get path to cmake config of the 'best' package given by the query information.
 
 The command will only search in the local cache. This does not intent for human use but more for
 cmake integration.
 
 ### pack
 
 Actions on packages.
 
 #### query
 
-`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if 
+`depmanager pack query <query> <remote>` Simply do a search in the given remote (in local if
 nothing given) and print the result.
 
 #### add, del
 
 `depmanager pack add <location>` Will add a package to the local database. `<location>` can be a
 folder, then it must contain a properly formatted `edp.info` file. Or an archive (.zip, .tgz or .tar.gz
 file format allowed). The uncompressed archive must contain a properly formatted `edp.info` file.
 
-`depmanager pack del <query>` Will remove from local cache all package matching the query
+`depmanager pack del <query>` Will remove from local cache all package matching the query.
 
 #### push, pull
 
 `depmanager pack [push|pull] <query> <remote> [--force(-f)]` will synchronize Local cache with the remote.
 The `query` must be precise enough to match one and only one package. `remote` must be valid.
 
 `push` will look for the package in local cache that match the query and send it to the given remote.
@@ -149,30 +153,40 @@
 
 If `--force` is given, The transfert occurs even if the package already exists in the destination.
 
 ### remote
 
 Manage the list of remote servers
 subcommands:
- * `list` lists the defined remote server.
- * `add` adds a new remote to the list.
-   * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
-   * Name is mandatory. if the name already exist it will modify the existing one.
-   * Allowed proto are:
-     * `ftp` supports login
-     * `folder` a folder of your computer (mostly for debug or testing)
-     * `srv` a dedicated server see [github](https://github.com/Silmaen/DepManagerServer)
-     * `srvs` a dedicated server with secure connexion see [github](https://github.com/Silmaen/DepManagerServer)
-   * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
- * `del <remote>` remove the designated remote if exists.
- * `sync <remote>` push to remote all local package that does not already exist on remote.
+
+* `list` lists the defined remote server.
+* `add` adds a new remote to the list.
+    * `--name(-n) <name> --url(-u) <proto>://<url[:port]> [--default(-d)]`.
+    * Mandatory. If name already exists it will modify the existing one.
+    * Allowed proto are:
+        * `ftp` supports login
+        * `folder` a folder of your computer (mostly for debug or testing)
+        * `srv` a dedicated server see [gitHub](https://github.com/Silmaen/DepManagerServer)
+        * `srvs` a dedicated server with secure connexion see [gitHub](https://github.com/Silmaen/DepManagerServer)
+    * Login can be defined with: `--login(-l) <login> --passwd(-p) <passwd>`.
+* `del <remote>` remove the designated remote if exists.
+* `sync <remote>` push to remote all local package that does not already exist on remote.
 
 ### build
 
-`depmanager build <location>` will search for recipe in the given location and build them.
+`depmanager build [OPTIONS] <location>` will search for recipe in the given location and build them.
+
+Some option can be passed to the build system:
+
+* `--single-thread`: on some low-end devices (such as RaspberryPi) single thread build is recommended.
+* `--force`, `-f`: Force the build even if the dependency already exists
+* `--cross-c`: redefine the C compiler
+* `--cross-cxx`: redefine the C++ compiler
+* `--cross-arch`: redefine the architecture
+* `--cross-os`: redefine the OS
 
 ## Using package with cmake
 
 ### Include depmanager to cmake
 
 To initialize depmanager into cmake you need to add to `CMAKE_MODULE_PATH` the path
 to the cmake folder of this installation.
@@ -191,50 +205,51 @@
     list(PREPEND CMAKE_MODULE_PATH ${depmanager_path})
     include(DepManager)
 endif()
 ```
 
 ### Find packages
 
-With depmanager initialized in cmake, it provide an alternative to classical `find_package`
+With depmanager initialized in cmake, it provides an alternative to classical `find_package`
 of cmake by `dm_find_package`
 
 ```cmake
 dm_find_package(
    package
    [QUIET] [TRACE] [REQUIRED]
    [VERSION version]
    [KIND kind]
    [ARCH target_arch]
    [OS target_os]
    [COMPILER target_compiler]
 )
 ```
+
 `package` is the package name to find.
 
 `version` is the exact version to match (wildcard are allowed). By default, find the
 latest one.
 
 `kind` is used to force library kind (`shared`, `static`, `header`). By default it return
 the first found.
 
-If `REQUIRED` set, the function will give an error if no package found. 
+If `REQUIRED` set, the function will give an error if no package found.
 (same as original `find_package`)
 
 If `QUIET` set, only errors are written. (same as original `find_package`). In opposition,
 if `TRACE` set, many more debug message displayed.
 
 `target_arch`, `target_os`, `target_compiler` are used in the query. If not set, default
 values are `CMAKE_SYSTEM_PROCESSOR`, `CMAKE_SYSTEM_NAME` and `CMAKE_CXX_COMPILER_ID`
 
-**LIMITATION:** it require the library name is the package name. So no multi lib or lib with different name.
+**LIMITATION:** it requires the library name is the package name. So no multi lib or lib with different name.
 
 ### Load package
 
-This command is similar to the previous one, but does not directly do a cmake's `find_package`. 
+This command is similar to the previous one, but does not directly do a cmake's `find_package`.
 It only adds to the `CMAKE_PREFIX_PATH` list the folders of given package.
 
 ```cmake
 dm_load_package(
    package
    [QUIET] [TRACE]
    [VERSION version]
@@ -245,57 +260,59 @@
 )
 ```
 
 After call this command, the cmake user has to call for needed `find_package`.
 
 ## Create you own package
 
-Depmanager allow you to create your own packages by defining recipes. Then run 
+Depmanager allow you to create your own packages by defining recipes. Then run
 `depmanager build <location of recipes>`
 The program will then build and add dependencies to the local cache.
 
 The location can contain as many recipe in any number of files.
 
 ### The recipe
 
 During build, Depmanager will look in all `.py` file for class that inherits from
 depmanager.api.recipe.Recipe.
 
 As for dependency usage, build also rely on cmake for building.
 
 The builder will use the provided recipe in the following workflow:
 
- * Init recipe
- * Call `recipe.source()`
- * Call `recipe.configure()`
- * Initialize options based on recipe data
- * Run cmake configure
- * For all configuration (mostly 'Debug', 'Release')
-   * build target `install`
- * Call `recipe.install()`
- * Generate edp.info file
- * Import into local cache
- * Clean Temporary
+* Init recipe
+* Call `recipe.source()`
+* Call `recipe.configure()`
+* Initialize options based on recipe data
+* Run cmake configure
+* For all configuration (mostly 'Debug', 'Release')
+    * build target `install`
+* Call `recipe.install()`
+* Generate edp.info file
+* Import into local cache
+* Clean Temporary
 
 Here is a small example
 
 ```python
 """
 Small recipe example
 """
 from depmanager.api.recipe import Recipe
 
+
 class MyAwesomeLib(Recipe):
     """
     Awesome lib
     """
     name = "awesome_lib"  # lib name
-    version = "0.0.1.foo" # lib version
-    source_dir = "src"    # where to fine the sources (especially) the CmakeList.txt
-    kind = "static"       # the lib's kind
+    version = "0.0.1.foo"  # lib version
+    source_dir = "src"  # where to fine the sources (especially) the CmakeList.txt
+    kind = "static"  # the lib's kind
+
 
 class AnotherAwesomeLib(MyAwesomeLib):
     """
     Shared version of previous one
     """
     kind = "shared"
 ```
@@ -303,29 +320,32 @@
 ## Roadmap
 
 First of all in the roadmap is to use this tool in C++ project to get feedback.
 
 Among things:
 
 * version 0.2.0
-  * [ ] Do query across multiple source (local then remote)
-  * [ ] Add a sorting order for remotes
-  * [ ] Auto-pull if not in local
-    * [ ] Auto build recipe if neither local or remote found
-  * [ ] Add concept of toolset
-    * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one
-    * [ ] Use toolset in build
-    * [ ] use toolset in queries
+    * [ ] Do query across multiple source (local then remote).
+    * [ ] Add a sorting order for remotes.
+    * [ ] Auto-pull if not in local.
+        * [ ] Auto build recipe if neither local nor remote found.
+    * [ ] Add concept of toolset.
+        * [ ] Tool set defines arch, os and compilers; stored in config.ini; with a default one.
+        * [ ] Use toolset in build.
+        * [ ] use toolset in queries.
+* version 0.1.4
+    * [ ] Add build Date in package properties.
+    * [ ] Allow to force push/pull.
+    * [ ] Allow to sync with remote.
+        * [ ] Allow to pull local package that have newer version.
+        * [ ] Allow to push local package newer than remote or not existing in remote.
 * version 0.1.3
-  * [ ] omit -d in push/pull command
-  * [ ] add progressbass in push/pull command
-  * [ ] Add build Date in package properties
-  * [ ] Allow to force push/pull
-  * [ ] Allow to sync with remote
-    * [ ] Allow to pull local package that have newer version
-    * [ ] Allow to push local package newer than remote or not existing in remote
+    * [X] Update internal statuses when using API.
+    * [X] omit -d in push/pull command.
+    * [X] add progress bar in push/pull command.
+    * [X] Allow single thread in build.
 * version 0.1.2
-  * [X] Add possibility to force os, arch and compiler for cross compiling
-  * [X] Adapt build system to search dependency in the forced environment.
+    * [X] Add possibility to force os, arch and compiler for cross compiling.
+    * [X] Adapt build system to search dependency in the forced environment.
 * version 0.1.1
-  * [X] Add remote Type of 'srv': a dedicated dependency server
-  * [X] Add remote Type of 'srvs': a dedicated dependency server with secure connexion
+    * [X] Add remote 'srv' Type: a dedicated dependency server.
+    * [X] Add remote 'srvs' Type: a dedicated dependency server with secure connexion.
```

### Comparing `depmanager-0.1.2/src/depmanager.egg-info/SOURCES.txt` & `depmanager-0.1.3/src/depmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

