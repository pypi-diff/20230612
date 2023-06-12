# Comparing `tmp/rds2py-0.2.3.tar.gz` & `tmp/rds2py-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds2py-0.2.3.tar", last modified: Mon Jun  5 17:43:04 2023, max compression
+gzip compressed data, was "rds2py-0.2.4.tar", last modified: Mon Jun 12 19:35:19 2023, max compression
```

## Comparing `rds2py-0.2.3.tar` & `rds2py-0.2.4.tar`

### file list

```diff
@@ -1,324 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.573038 rds2py-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-05 17:42:45.000000 rds2py-0.2.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.537037 rds2py-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-05 17:42:45.000000 rds2py-0.2.3/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 17:42:45.000000 rds2py-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 17:42:45.000000 rds2py-0.2.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-05 17:42:45.000000 rds2py-0.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 17:42:45.000000 rds2py-0.2.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 17:42:45.000000 rds2py-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-05 17:42:45.000000 rds2py-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 17:42:45.000000 rds2py-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 17:42:45.000000 rds2py-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-05 17:43:04.573038 rds2py-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-05 17:42:45.000000 rds2py-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-05 17:42:45.000000 rds2py-0.2.3/docs/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)    15992 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeSystem.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/
--rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    16096 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out
--rw-r--r--   0 runner    (1001) docker     (123)    27834 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile2
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/TargetDirectories.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/cmake.check_cache
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.541038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.545038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/
--r--r--r--   0 runner    (1001) docker     (123)    28232 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx
--r--r--r--   0 runner    (1001) docker     (123)  1112566 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/packed-refs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.549038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108855 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.553038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/CMakeSystem.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeConfigureLog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/TargetDirectories.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate-complete
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/DependInfo.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.make
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.ts
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/progress.make
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/cmake.check_cache
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-build
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-configure
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-done
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-download
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-install
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-mkdir
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-patch
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-test
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-cfgcmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-05 17:42:47.000000 rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/cmake_install.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   109743 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.557038 rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/progress.marks
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/extern/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-05 17:42:48.000000 rds2py-0.2.3/extern/rds2cpp/extern/cmake_install.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.533038 rds2py-0.2.3/extern/rds2cpp/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/Environment.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RObject.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RdsFile.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SEXPType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/StringEncoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/Symbol.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_environment.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_expression.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_language.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_list.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_rds.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_s4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/rds2cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_parse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_write.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_atomic.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_attributes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_builtin.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_expression.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_language.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_list.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_object.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_rds.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_s4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_single_string.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/NAMESPACE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/R/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/R/RcppExports.R
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/R/inspect.R
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/R/namespace.R
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/Makevars
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/RcppExports.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/parse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/src/write.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-altrep.R
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-atomic.R
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-builtin.R
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-environment.R
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-expression.R
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-language.R
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-list.R
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-pairlist.R
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-s4.R
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-symbol.R
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-05 17:42:46.000000 rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat.R
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-05 17:42:45.000000 rds2py-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-05 17:43:04.573038 rds2py-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-05 17:42:45.000000 rds2py-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.537037 rds2py-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.565038 rds2py-0.2.3/src/rds2py/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.569038 rds2py-0.2.3/src/rds2py/lib/
--rw-r--r--   0 runner    (1001) docker     (123)  1002507 2023-06-05 17:43:03.000000 rds2py-0.2.3/src/rds2py/lib/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/lib/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/lib/parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/lib/rds_parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-05 17:42:45.000000 rds2py-0.2.3/src/rds2py/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.569038 rds2py-0.2.3/src/rds2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:43:03.000000 rds2py-0.2.3/src/rds2py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:43:04.000000 rds2py-0.2.3/src/rds2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-05 17:42:45.000000 rds2py-0.2.3/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.569038 rds2py-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:43:04.573038 rds2py-0.2.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/.Rhistory
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_attr.rds
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_chars.rds
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_chars_unicode.rds
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_complex.rds
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_double.rds
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_ints.rds
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_logical.rds
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_logical_wNA.rds
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/atomic_raw.rds
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/generate_files.R
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists.rds
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_df.rds
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_df_rownames.rds
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_nested.rds
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/lists_nested_deep.rds
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_class.rds
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_dense_matrix.rds
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_matrix.rds
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/data/s4_matrix_dgt.rds
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-double.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-int.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_atomic-str.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_interface_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-05 17:42:45.000000 rds2py-0.2.3/tests/test_s4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-05 17:42:45.000000 rds2py-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.807052 rds2py-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-12 19:35:02.000000 rds2py-0.2.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.759051 rds2py-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.767051 rds2py-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-12 19:35:02.000000 rds2py-0.2.4/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 19:35:02.000000 rds2py-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-12 19:35:02.000000 rds2py-0.2.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 19:35:02.000000 rds2py-0.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 19:35:02.000000 rds2py-0.2.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-12 19:35:02.000000 rds2py-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13464 2023-06-12 19:35:02.000000 rds2py-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-12 19:35:02.000000 rds2py-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 19:35:02.000000 rds2py-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-12 19:35:19.807052 rds2py-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-12 19:35:02.000000 rds2py-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-12 19:35:02.000000 rds2py-0.2.4/docs/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.759051 rds2py-0.2.4/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/extern/rds2cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/extern/rds2cpp/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15992 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CMakeSystem.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/
+-rw-r--r--   0 runner    (1001) docker     (123)    26276 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16096 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out
+-rw-r--r--   0 runner    (1001) docker     (123)    27834 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/Makefile.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/Makefile2
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/TargetDirectories.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/cmake.check_cache
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.771051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/CMakeFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/logs/refs/remotes/origin/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.775051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/
+-r--r--r--   0 runner    (1001) docker     (123)    28232 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx
+-r--r--r--   0 runner    (1001) docker     (123)  1112566 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/packed-refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.779051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.779051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/refs/remotes/origin/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.779051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.779051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108855 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.783051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.783051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.783051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.783051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.787051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.787051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/3.26.3/CMakeSystem.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeConfigureLog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/TargetDirectories.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate-complete
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.787051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/DependInfo.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.make
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/compiler_depend.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/progress.make
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/cmake.check_cache
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.763051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.787051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-build
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-configure
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-done
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-download
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-install
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-mkdir
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-patch
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.791051 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-cfgcmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-12 19:35:03.000000 rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/cmake_install.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.791051 rds2py-0.2.4/extern/rds2cpp/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   109743 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.791051 rds2py-0.2.4/extern/rds2cpp/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.791051 rds2py-0.2.4/extern/rds2cpp/extern/CMakeFiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/extern/CMakeFiles/progress.marks
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/extern/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/extern/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-12 19:35:04.000000 rds2py-0.2.4/extern/rds2cpp/extern/cmake_install.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.767051 rds2py-0.2.4/extern/rds2cpp/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.799051 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/Environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/RObject.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/RdsFile.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/SEXPType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/StringEncoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/Symbol.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_expression.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_language.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_list.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_rds.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_s4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/rds2cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/utils_parse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/utils_write.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_atomic.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_attributes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_builtin.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_expression.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_language.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_list.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_object.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_rds.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_s4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_single_string.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.799051 rds2py-0.2.4/extern/rds2cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/NAMESPACE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.799051 rds2py-0.2.4/extern/rds2cpp/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/R/RcppExports.R
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/R/inspect.R
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/R/namespace.R
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.799051 rds2py-0.2.4/extern/rds2cpp/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/src/Makevars
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/src/RcppExports.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/src/parse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/src/write.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.799051 rds2py-0.2.4/extern/rds2cpp/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.799051 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-altrep.R
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-atomic.R
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-builtin.R
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-environment.R
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-expression.R
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-language.R
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-list.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-pairlist.R
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-s4.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-symbol.R
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 19:35:02.000000 rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat.R
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-12 19:35:02.000000 rds2py-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-12 19:35:19.807052 rds2py-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-12 19:35:02.000000 rds2py-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.767051 rds2py-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.799051 rds2py-0.2.4/src/rds2py/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-12 19:35:02.000000 rds2py-0.2.4/src/rds2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7681 2023-06-12 19:35:02.000000 rds2py-0.2.4/src/rds2py/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.803051 rds2py-0.2.4/src/rds2py/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)  1002507 2023-06-12 19:35:18.000000 rds2py-0.2.4/src/rds2py/lib/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-12 19:35:02.000000 rds2py-0.2.4/src/rds2py/lib/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-12 19:35:02.000000 rds2py-0.2.4/src/rds2py/lib/parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-12 19:35:02.000000 rds2py-0.2.4/src/rds2py/lib/rds_parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-12 19:35:02.000000 rds2py-0.2.4/src/rds2py/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-12 19:35:02.000000 rds2py-0.2.4/src/rds2py/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.803051 rds2py-0.2.4/src/rds2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-12 19:35:19.000000 rds2py-0.2.4/src/rds2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-12 19:35:19.000000 rds2py-0.2.4/src/rds2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:35:19.000000 rds2py-0.2.4/src/rds2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:35:18.000000 rds2py-0.2.4/src/rds2py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-12 19:35:19.000000 rds2py-0.2.4/src/rds2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 19:35:19.000000 rds2py-0.2.4/src/rds2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-12 19:35:02.000000 rds2py-0.2.4/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.803051 rds2py-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:35:19.807052 rds2py-0.2.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/.Rhistory
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_attr.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_chars.rds
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_chars_unicode.rds
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_complex.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_double.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_ints.rds
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_logical.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_logical_wNA.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/atomic_raw.rds
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/generate_files.R
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/lists.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/lists_df.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/lists_df_rownames.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/lists_nested.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/lists_nested_deep.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/numpy_dtype.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/s4_class.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/s4_dense_matrix.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/s4_matrix.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/data/s4_matrix_dgt.rds
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_atomic-attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_atomic-bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_atomic-double.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_atomic-int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_atomic-str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_interface_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-12 19:35:02.000000 rds2py-0.2.4/tests/test_s4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-12 19:35:02.000000 rds2py-0.2.4/tox.ini
```

### Comparing `rds2py-0.2.3/.coveragerc` & `rds2py-0.2.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/.github/workflows/pypi-test.yml` & `rds2py-0.2.4/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/.gitignore` & `rds2py-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/CONTRIBUTING.md` & `rds2py-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/LICENSE.txt` & `rds2py-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/PKG-INFO` & `rds2py-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds2py
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parse and read RDS files as Python representations
 Home-page: https://github.com/biocpy/rds2py
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/rds2py/
 Project-URL: Source, https://github.com/biocpy/rds2py
```

### Comparing `rds2py-0.2.3/README.md` & `rds2py-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/docs/Makefile` & `rds2py-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/docs/conf.py` & `rds2py-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/docs/index.md` & `rds2py-0.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/docs/tutorial.md` & `rds2py-0.2.4/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/.github/workflows/doxygenate.yaml` & `rds2py-0.2.4/extern/rds2cpp/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/.github/workflows/run-tests.yaml` & `rds2py-0.2.4/extern/rds2cpp/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeCache.txt` & `rds2py-0.2.4/extern/rds2cpp/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/3.26.3/CompilerIdCXX/a.out`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/CMakeConfigureLog.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -35,41 +35,41 @@
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerABI.cmake:57 (try_compile)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeTestCXXCompiler.cmake:26 (CMAKE_DETERMINE_COMPILER_ABI)"
       - "CMakeLists.txt:3 (project)"
     checks:
       - "Detecting CXX compiler ABI info"
     directories:
-      source: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL"
-      binary: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL"
+      source: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-wjJAUK"
+      binary: "/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-wjJAUK"
     cmakeVariables:
       CMAKE_CXX_FLAGS: ""
       CMAKE_CXX_FLAGS_DEBUG: "-g"
       CMAKE_EXE_LINKER_FLAGS: ""
     buildResult:
       variable: "CMAKE_CXX_ABI_COMPILED"
       cached: true
       stdout: |
-        Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL
+        Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-wjJAUK
         
-        Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_95e5c/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_95e5c.dir/build.make CMakeFiles/cmTC_95e5c.dir/build
-        gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL'
-        Building CXX object CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o
-        /usr/bin/c++   -v -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp
+        Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_9e310/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_9e310.dir/build.make CMakeFiles/cmTC_9e310.dir/build
+        gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-wjJAUK'
+        Building CXX object CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o
+        /usr/bin/c++   -v -o CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp
         Using built-in specs.
         COLLECT_GCC=/usr/bin/c++
         OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa
         OFFLOAD_TARGET_DEFAULT=1
         Target: x86_64-linux-gnu
         Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c,ada,c++,go,brig,d,fortran,objc,obj-c++,m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32,m64,mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr,amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2
         Thread model: posix
         Supported LTO compression algorithms: zlib zstd
         gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) 
-        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/'
-         /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_95e5c.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/cctDHyu2.s
+        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_9e310.dir/'
+         /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_9e310.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/ccezHvXs.s
         GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)
         	compiled by GNU C version 11.3.0, GMP version 6.2.1, MPFR version 4.1.0, MPC version 1.2.1, isl version isl-0.24-GMP
         
         GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072
         ignoring duplicate directory "/usr/include/x86_64-linux-gnu/c++/11"
         ignoring nonexistent directory "/usr/local/include/x86_64-linux-gnu"
         ignoring nonexistent directory "/usr/lib/gcc/x86_64-linux-gnu/11/include-fixed"
@@ -85,39 +85,39 @@
          /usr/include
         End of search list.
         GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)
         	compiled by GNU C version 11.3.0, GMP version 6.2.1, MPFR version 4.1.0, MPC version 1.2.1, isl version isl-0.24-GMP
         
         GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072
         Compiler executable checksum: 449548cbb29044828dc7ea158b577b98
-        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/'
-         as -v --64 -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o /tmp/cctDHyu2.s
+        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_9e310.dir/'
+         as -v --64 -o CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o /tmp/ccezHvXs.s
         GNU assembler version 2.38 (x86_64-linux-gnu) using BFD version (GNU Binutils for Ubuntu) 2.38
         COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/
         LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/
-        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.'
-        Linking CXX executable cmTC_95e5c
-        /usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_95e5c.dir/link.txt --verbose=1
-        /usr/bin/c++  -v CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_95e5c 
+        COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.'
+        Linking CXX executable cmTC_9e310
+        /usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_9e310.dir/link.txt --verbose=1
+        /usr/bin/c++  -v CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_9e310 
         Using built-in specs.
         COLLECT_GCC=/usr/bin/c++
         COLLECT_LTO_WRAPPER=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper
         OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa
         OFFLOAD_TARGET_DEFAULT=1
         Target: x86_64-linux-gnu
         Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c,ada,c++,go,brig,d,fortran,objc,obj-c++,m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32,m64,mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr,amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2
         Thread model: posix
         Supported LTO compression algorithms: zlib zstd
         gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) 
         COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/
         LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/
-        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_95e5c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_95e5c.'
-         /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccCHBvP6.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_95e5c /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o
-        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_95e5c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_95e5c.'
-        gmake[1]: Leaving directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL'
+        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_9e310' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_9e310.'
+         /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccVPiZN2.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_9e310 /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o
+        COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_9e310' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_9e310.'
+        gmake[1]: Leaving directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-wjJAUK'
         
       exitCode: 0
   -
     kind: "message-v1"
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerABI.cmake:127 (message)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeTestCXXCompiler.cmake:26 (CMAKE_DETERMINE_COMPILER_ABI)"
@@ -149,31 +149,31 @@
     backtrace:
       - "/usr/local/share/cmake-3.26/Modules/CMakeDetermineCompilerABI.cmake:152 (message)"
       - "/usr/local/share/cmake-3.26/Modules/CMakeTestCXXCompiler.cmake:26 (CMAKE_DETERMINE_COMPILER_ABI)"
       - "CMakeLists.txt:3 (project)"
     message: |
       Parsed CXX implicit link information:
         link line regex: [^( *|.*[/\\])(ld|CMAKE_LINK_STARTFILE-NOTFOUND|([^/\\]+-)?ld|collect2)[^/\\]*( |$)]
-        ignore line: [Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL]
+        ignore line: [Change Dir: /home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-wjJAUK]
         ignore line: []
-        ignore line: [Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_95e5c/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_95e5c.dir/build.make CMakeFiles/cmTC_95e5c.dir/build]
-        ignore line: [gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-a24SWL']
-        ignore line: [Building CXX object CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o]
-        ignore line: [/usr/bin/c++   -v -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp]
+        ignore line: [Run Build Command(s):/usr/local/bin/cmake -E env VERBOSE=1 /usr/bin/gmake -f Makefile cmTC_9e310/fast && /usr/bin/gmake  -f CMakeFiles/cmTC_9e310.dir/build.make CMakeFiles/cmTC_9e310.dir/build]
+        ignore line: [gmake[1]: Entering directory '/home/runner/work/rds2py/rds2py/extern/rds2cpp/CMakeFiles/CMakeScratch/TryCompile-wjJAUK']
+        ignore line: [Building CXX object CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o]
+        ignore line: [/usr/bin/c++   -v -o CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o -c /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp]
         ignore line: [Using built-in specs.]
         ignore line: [COLLECT_GCC=/usr/bin/c++]
         ignore line: [OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa]
         ignore line: [OFFLOAD_TARGET_DEFAULT=1]
         ignore line: [Target: x86_64-linux-gnu]
         ignore line: [Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c ada c++ go brig d fortran objc obj-c++ m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32 m64 mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2]
         ignore line: [Thread model: posix]
         ignore line: [Supported LTO compression algorithms: zlib zstd]
         ignore line: [gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) ]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/']
-        ignore line: [ /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_95e5c.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/cctDHyu2.s]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_9e310.dir/']
+        ignore line: [ /usr/lib/gcc/x86_64-linux-gnu/11/cc1plus -quiet -v -imultiarch x86_64-linux-gnu -D_GNU_SOURCE /usr/local/share/cmake-3.26/Modules/CMakeCXXCompilerABI.cpp -quiet -dumpdir CMakeFiles/cmTC_9e310.dir/ -dumpbase CMakeCXXCompilerABI.cpp.cpp -dumpbase-ext .cpp -mtune=generic -march=x86-64 -version -fasynchronous-unwind-tables -fstack-protector-strong -Wformat -Wformat-security -fstack-clash-protection -fcf-protection -o /tmp/ccezHvXs.s]
         ignore line: [GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)]
         ignore line: [	compiled by GNU C version 11.3.0  GMP version 6.2.1  MPFR version 4.1.0  MPC version 1.2.1  isl version isl-0.24-GMP]
         ignore line: []
         ignore line: [GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072]
         ignore line: [ignoring duplicate directory "/usr/include/x86_64-linux-gnu/c++/11"]
         ignore line: [ignoring nonexistent directory "/usr/local/include/x86_64-linux-gnu"]
         ignore line: [ignoring nonexistent directory "/usr/lib/gcc/x86_64-linux-gnu/11/include-fixed"]
@@ -189,42 +189,42 @@
         ignore line: [ /usr/include]
         ignore line: [End of search list.]
         ignore line: [GNU C++17 (Ubuntu 11.3.0-1ubuntu1~22.04) version 11.3.0 (x86_64-linux-gnu)]
         ignore line: [	compiled by GNU C version 11.3.0  GMP version 6.2.1  MPFR version 4.1.0  MPC version 1.2.1  isl version isl-0.24-GMP]
         ignore line: []
         ignore line: [GGC heuristics: --param ggc-min-expand=100 --param ggc-min-heapsize=131072]
         ignore line: [Compiler executable checksum: 449548cbb29044828dc7ea158b577b98]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/']
-        ignore line: [ as -v --64 -o CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o /tmp/cctDHyu2.s]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_9e310.dir/']
+        ignore line: [ as -v --64 -o CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o /tmp/ccezHvXs.s]
         ignore line: [GNU assembler version 2.38 (x86_64-linux-gnu) using BFD version (GNU Binutils for Ubuntu) 2.38]
         ignore line: [COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/]
         ignore line: [LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.']
-        ignore line: [Linking CXX executable cmTC_95e5c]
-        ignore line: [/usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_95e5c.dir/link.txt --verbose=1]
-        ignore line: [/usr/bin/c++  -v CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_95e5c ]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o' '-c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.']
+        ignore line: [Linking CXX executable cmTC_9e310]
+        ignore line: [/usr/local/bin/cmake -E cmake_link_script CMakeFiles/cmTC_9e310.dir/link.txt --verbose=1]
+        ignore line: [/usr/bin/c++  -v CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o -o cmTC_9e310 ]
         ignore line: [Using built-in specs.]
         ignore line: [COLLECT_GCC=/usr/bin/c++]
         ignore line: [COLLECT_LTO_WRAPPER=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper]
         ignore line: [OFFLOAD_TARGET_NAMES=nvptx-none:amdgcn-amdhsa]
         ignore line: [OFFLOAD_TARGET_DEFAULT=1]
         ignore line: [Target: x86_64-linux-gnu]
         ignore line: [Configured with: ../src/configure -v --with-pkgversion='Ubuntu 11.3.0-1ubuntu1~22.04' --with-bugurl=file:///usr/share/doc/gcc-11/README.Bugs --enable-languages=c ada c++ go brig d fortran objc obj-c++ m2 --prefix=/usr --with-gcc-major-version-only --program-suffix=-11 --program-prefix=x86_64-linux-gnu- --enable-shared --enable-linker-build-id --libexecdir=/usr/lib --without-included-gettext --enable-threads=posix --libdir=/usr/lib --enable-nls --enable-bootstrap --enable-clocale=gnu --enable-libstdcxx-debug --enable-libstdcxx-time=yes --with-default-libstdcxx-abi=new --enable-gnu-unique-object --disable-vtable-verify --enable-plugin --enable-default-pie --with-system-zlib --enable-libphobos-checking=release --with-target-system-zlib=auto --enable-objc-gc=auto --enable-multiarch --disable-werror --enable-cet --with-arch-32=i686 --with-abi=m64 --with-multilib-list=m32 m64 mx32 --enable-multilib --with-tune=generic --enable-offload-targets=nvptx-none=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-nvptx/usr amdgcn-amdhsa=/build/gcc-11-xKiWfi/gcc-11-11.3.0/debian/tmp-gcn/usr --without-cuda-driver --enable-checking=release --build=x86_64-linux-gnu --host=x86_64-linux-gnu --target=x86_64-linux-gnu --with-build-config=bootstrap-lto-lean --enable-link-serialization=2]
         ignore line: [Thread model: posix]
         ignore line: [Supported LTO compression algorithms: zlib zstd]
         ignore line: [gcc version 11.3.0 (Ubuntu 11.3.0-1ubuntu1~22.04) ]
         ignore line: [COMPILER_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/]
         ignore line: [LIBRARY_PATH=/usr/lib/gcc/x86_64-linux-gnu/11/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib/:/lib/x86_64-linux-gnu/:/lib/../lib/:/usr/lib/x86_64-linux-gnu/:/usr/lib/../lib/:/usr/lib/gcc/x86_64-linux-gnu/11/../../../:/lib/:/usr/lib/]
-        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_95e5c' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_95e5c.']
-        link line: [ /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccCHBvP6.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_95e5c /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o]
+        ignore line: [COLLECT_GCC_OPTIONS='-v' '-o' 'cmTC_9e310' '-shared-libgcc' '-mtune=generic' '-march=x86-64' '-dumpdir' 'cmTC_9e310.']
+        link line: [ /usr/lib/gcc/x86_64-linux-gnu/11/collect2 -plugin /usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so -plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper -plugin-opt=-fresolution=/tmp/ccVPiZN2.res -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc -plugin-opt=-pass-through=-lc -plugin-opt=-pass-through=-lgcc_s -plugin-opt=-pass-through=-lgcc --build-id --eh-frame-hdr -m elf_x86_64 --hash-style=gnu --as-needed -dynamic-linker /lib64/ld-linux-x86-64.so.2 -pie -z now -z relro -o cmTC_9e310 /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o /usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o -L/usr/lib/gcc/x86_64-linux-gnu/11 -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu -L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib -L/lib/x86_64-linux-gnu -L/lib/../lib -L/usr/lib/x86_64-linux-gnu -L/usr/lib/../lib -L/usr/lib/gcc/x86_64-linux-gnu/11/../../.. CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o -lstdc++ -lm -lgcc_s -lgcc -lc -lgcc_s -lgcc /usr/lib/gcc/x86_64-linux-gnu/11/crtendS.o /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crtn.o]
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/collect2] ==> ignore
           arg [-plugin] ==> ignore
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/liblto_plugin.so] ==> ignore
           arg [-plugin-opt=/usr/lib/gcc/x86_64-linux-gnu/11/lto-wrapper] ==> ignore
-          arg [-plugin-opt=-fresolution=/tmp/ccCHBvP6.res] ==> ignore
+          arg [-plugin-opt=-fresolution=/tmp/ccVPiZN2.res] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc_s] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc] ==> ignore
           arg [-plugin-opt=-pass-through=-lc] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc_s] ==> ignore
           arg [-plugin-opt=-pass-through=-lgcc] ==> ignore
           arg [--build-id] ==> ignore
           arg [--eh-frame-hdr] ==> ignore
@@ -234,27 +234,27 @@
           arg [--as-needed] ==> ignore
           arg [-dynamic-linker] ==> ignore
           arg [/lib64/ld-linux-x86-64.so.2] ==> ignore
           arg [-pie] ==> ignore
           arg [-znow] ==> ignore
           arg [-zrelro] ==> ignore
           arg [-o] ==> ignore
-          arg [cmTC_95e5c] ==> ignore
+          arg [cmTC_9e310] ==> ignore
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o] ==> obj [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o]
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o] ==> obj [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/crti.o]
           arg [/usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o] ==> obj [/usr/lib/gcc/x86_64-linux-gnu/11/crtbeginS.o]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11/../../../../lib]
           arg [-L/lib/x86_64-linux-gnu] ==> dir [/lib/x86_64-linux-gnu]
           arg [-L/lib/../lib] ==> dir [/lib/../lib]
           arg [-L/usr/lib/x86_64-linux-gnu] ==> dir [/usr/lib/x86_64-linux-gnu]
           arg [-L/usr/lib/../lib] ==> dir [/usr/lib/../lib]
           arg [-L/usr/lib/gcc/x86_64-linux-gnu/11/../../..] ==> dir [/usr/lib/gcc/x86_64-linux-gnu/11/../../..]
-          arg [CMakeFiles/cmTC_95e5c.dir/CMakeCXXCompilerABI.cpp.o] ==> ignore
+          arg [CMakeFiles/cmTC_9e310.dir/CMakeCXXCompilerABI.cpp.o] ==> ignore
           arg [-lstdc++] ==> lib [stdc++]
           arg [-lm] ==> lib [m]
           arg [-lgcc_s] ==> lib [gcc_s]
           arg [-lgcc] ==> lib [gcc]
           arg [-lc] ==> lib [c]
           arg [-lgcc_s] ==> lib [gcc_s]
           arg [-lgcc] ==> lib [gcc]
```

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile.cmake` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/CMakeFiles/Makefile2` & `rds2py-0.2.4/extern/rds2cpp/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/LICENSE` & `rds2py-0.2.4/extern/rds2cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/Makefile` & `rds2py-0.2.4/extern/rds2cpp/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/README.md` & `rds2py-0.2.4/extern/rds2cpp/README.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/Makefile` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-build/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/index` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/index`

 * *Files 24% similar despite different names*

#### Comparing `/tmp/diffoscope_jivnv5ke_/tmpfwfb9j8y_TarContainer/0/82` & `/tmp/diffoscope_jivnv5ke_/tmp_pnoqw_u_TarContainer/0/82`

```diff
@@ -5,430 +5,430 @@
 
 Path:      b'.github/workflows/doxygenate.yaml'
 SHA:       ab5e795d0df07f68ed319a8f7f022a4422fb8ba5
 Size:      772
 Flags:     0b100001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785656
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103966
+Device ID: (8, 1)
 
 Path:      b'.github/workflows/run-tests.yaml'
 SHA:       ac1c43ef8042fe89775c24a02234b92c410a9a79
 Size:      755
 Flags:     0b100000
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785657
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103967
+Device ID: (8, 1)
 
 Path:      b'.gitignore'
 SHA:       a599f0596ad4d7fcd6f1b3f478a0c2be80cb7ede
 Size:      33
 Flags:     0b1010
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785658
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103968
+Device ID: (8, 1)
 
 Path:      b'CMakeLists.txt'
 SHA:       0deb491827b473102d5f559769ac403e7bb3cf21
 Size:      368
 Flags:     0b1110
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785659
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103969
+Device ID: (8, 1)
 
 Path:      b'LICENSE'
 SHA:       9eecbc1fb139fed45c8625623d5948aa7a6a9200
 Size:      1066
 Flags:     0b111
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785660
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103970
+Device ID: (8, 1)
 
 Path:      b'README.md'
 SHA:       0596300dc65eefd2a0f27830f2fefcbf57e9e1b7
 Size:      2781
 Flags:     0b1001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785661
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103971
+Device ID: (8, 1)
 
 Path:      b'docs/Doxyfile'
 SHA:       e2a33dbbd5f4374fd7267c07066b3e23ff5cdfd5
 Size:      108855
 Flags:     0b1101
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785663
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103973
+Device ID: (8, 1)
 
 Path:      b'include/byteme/GzipFileReader.hpp'
 SHA:       a3a3c0e9c42d3f4f8e17c7020bba0f889767d147
 Size:      1586
 Flags:     0b100001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785666
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103976
+Device ID: (8, 1)
 
 Path:      b'include/byteme/GzipFileWriter.hpp'
 SHA:       e2215ff44b09f4b219a2f5cfc0b71271add49fff
 Size:      1949
 Flags:     0b100001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785667
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103977
+Device ID: (8, 1)
 
 Path:      b'include/byteme/IstreamReader.hpp'
 SHA:       612aff8a1f80e699db9dab33579031c4dc9135f7
 Size:      1349
 Flags:     0b100000
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785668
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103978
+Device ID: (8, 1)
 
 Path:      b'include/byteme/OstreamWriter.hpp'
 SHA:       54cfa24f802d888139b036b4347e98f2db61a584
 Size:      1071
 Flags:     0b100000
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785669
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103979
+Device ID: (8, 1)
 
 Path:      b'include/byteme/PerByte.hpp'
 SHA:       512b382a3e3fca2ddf4e857412e4e7afc9ed77fa
 Size:      4758
 Flags:     0b11010
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785670
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103980
+Device ID: (8, 1)
 
 Path:      b'include/byteme/RawBufferReader.hpp'
 SHA:       2d278bbad6deb2e0f4d9ddcc8d0cedf441e80f68
 Size:      1039
 Flags:     0b100010
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785671
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103981
+Device ID: (8, 1)
 
 Path:      b'include/byteme/RawBufferWriter.hpp'
 SHA:       0d4c55a572ff79d41688c2dad54898c9176d95cf
 Size:      845
 Flags:     0b100010
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785672
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103982
+Device ID: (8, 1)
 
 Path:      b'include/byteme/RawFileReader.hpp'
 SHA:       3bc82c5a165051a81d620ece874a72f648cd879e
 Size:      1920
 Flags:     0b100000
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785673
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103983
+Device ID: (8, 1)
 
 Path:      b'include/byteme/RawFileWriter.hpp'
 SHA:       471698f29c7fea0d394d46303f1c797a9f4f76de
 Size:      1764
 Flags:     0b100000
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785674
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103984
+Device ID: (8, 1)
 
 Path:      b'include/byteme/Reader.hpp'
 SHA:       65e83f517d44059125ea1fff440899152ca749c8
 Size:      1145
 Flags:     0b11001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785675
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103985
+Device ID: (8, 1)
 
 Path:      b'include/byteme/SelfClosingFILE.hpp'
 SHA:       b6e4a59997eff7b4847b694deddf66ffe5648add
 Size:      905
 Flags:     0b100010
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785676
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103986
+Device ID: (8, 1)
 
 Path:      b'include/byteme/SelfClosingGzFile.hpp'
 SHA:       7d4b1785548294c15a1afd4c645af05e286577b7
 Size:      878
 Flags:     0b100100
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785677
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103987
+Device ID: (8, 1)
 
 Path:      b'include/byteme/SomeBufferReader.hpp'
 SHA:       5b6357164ffb46a95d7b9cef5c5adf7cedeaa003
 Size:      1670
 Flags:     0b100011
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785678
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103988
+Device ID: (8, 1)
 
 Path:      b'include/byteme/SomeFileReader.hpp'
 SHA:       93a2a70c2b0e57b1e1a11cc4ad9a787c76172bb9
 Size:      1777
 Flags:     0b100001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.172338084
-Modified:  1685986968.172338084
-Inode:     785679
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103989
+Device ID: (8, 1)
 
 Path:      b'include/byteme/Writer.hpp'
 SHA:       49c6e5164407f752572031140a22a53d88cff9f8
 Size:      957
 Flags:     0b11001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785680
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103990
+Device ID: (8, 1)
 
 Path:      b'include/byteme/ZlibBufferReader.hpp'
 SHA:       5251fcdbce3c0e4df68afe921223cd162a32d1b1
 Size:      3832
 Flags:     0b100011
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785681
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103991
+Device ID: (8, 1)
 
 Path:      b'include/byteme/ZlibBufferWriter.hpp'
 SHA:       c8e30753186dcadf3457c7c446257af218e47a53
 Size:      3361
 Flags:     0b100011
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785682
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103992
+Device ID: (8, 1)
 
 Path:      b'include/byteme/magic_numbers.hpp'
 SHA:       315d1e2b8fd0cd3b10b1c89a107b225b14174633
 Size:      841
 Flags:     0b100000
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785683
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103993
+Device ID: (8, 1)
 
 Path:      b'include/byteme/temp_file_path.hpp'
 SHA:       df667f1c8be59a8d476014030cc74e5f38b7ab26
 Size:      1839
 Flags:     0b100001
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785684
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103994
+Device ID: (8, 1)
 
 Path:      b'tests/CMakeLists.txt'
 SHA:       b4df64f6acee6963aba316fc19b958cb6f91b09a
 Size:      1063
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785686
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103996
+Device ID: (8, 1)
 
 Path:      b'tests/src/GzipFileReader.cpp'
 SHA:       a143a1d7748ba54557b651bbea5f73b779e7a8f1
 Size:      2182
 Flags:     0b11100
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785688
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103998
+Device ID: (8, 1)
 
 Path:      b'tests/src/GzipFileWriter.cpp'
 SHA:       e5a557b7719cd5641ade76f65b560c648bb462b2
 Size:      2485
 Flags:     0b11100
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785689
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1103999
+Device ID: (8, 1)
 
 Path:      b'tests/src/IstreamReader.cpp'
 SHA:       79f468752a09d1d6a375c0f8e7763cbf2c46a99f
 Size:      1553
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785690
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104000
+Device ID: (8, 1)
 
 Path:      b'tests/src/OstreamWriter.cpp'
 SHA:       cee2cfaa3980cee3bf1440547319c18e8ed608cc
 Size:      1920
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785691
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104001
+Device ID: (8, 1)
 
 Path:      b'tests/src/PerByte.cpp'
 SHA:       c4cc8734ccf342dc14c97c875d4863299ad6e6f1
 Size:      2970
 Flags:     0b10101
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785692
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104002
+Device ID: (8, 1)
 
 Path:      b'tests/src/RawBufferReader.cpp'
 SHA:       702299273b3cb06c2728e1767e7e1ac7d490dae2
 Size:      2035
 Flags:     0b11101
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785693
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104003
+Device ID: (8, 1)
 
 Path:      b'tests/src/RawBufferWriter.cpp'
 SHA:       0eb7d04c5e9f5bc4f60669ea8e937ab53663ce8f
 Size:      1584
 Flags:     0b11101
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785694
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104004
+Device ID: (8, 1)
 
 Path:      b'tests/src/RawFileReader.cpp'
 SHA:       09426f3e5b6560522f9b24c89c19c4d0789c79f8
 Size:      2030
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785695
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104005
+Device ID: (8, 1)
 
 Path:      b'tests/src/RawFileWriter.cpp'
 SHA:       8c814cf5d7d52863a91d63f3ad5c05680ae861f2
 Size:      2160
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785696
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104006
+Device ID: (8, 1)
 
 Path:      b'tests/src/ZlibBufferReader.cpp'
 SHA:       bce71d0ad2566e09b363bada7ad972b798293c37
 Size:      2619
 Flags:     0b11110
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785697
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104007
+Device ID: (8, 1)
 
 Path:      b'tests/src/ZlibBufferWriter.cpp'
 SHA:       9e1d8ba51507c9259b5a0dc5e6a18bf12e332b3d
 Size:      3347
 Flags:     0b11110
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785698
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104008
+Device ID: (8, 1)
 
 Path:      b'tests/src/read_lines.h'
 SHA:       f1833fdf8d5069dbd933d51bc958b1d4084be20b
 Size:      1416
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1685986968.176338128
-Modified:  1685986968.176338128
-Inode:     785699
-Device ID: (8, 17)
+Created:   1686598504.142833652
+Modified:  1686598504.142833652
+Inode:     1104009
+Device ID: (8, 1)
```

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.idx`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.git/objects/pack/pack-7240a34dedb6cbf1d892766b378b45d8ae1a08b4.pack`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/LICENSE` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/LICENSE`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/README.md` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/README.md`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/GzipFileWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/IstreamReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/OstreamWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/PerByte.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawBufferWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/RawFileWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/Reader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingFILE.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SelfClosingGzFile.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeBufferReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/SomeFileReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/Writer.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferReader.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/ZlibBufferWriter.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/magic_numbers.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/include/byteme/temp_file_path.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/GzipFileWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/IstreamReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/OstreamWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/PerByte.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawBufferWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/RawFileWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferReader.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/ZlibBufferWriter.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-src/tests/src/read_lines.h`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/CMakeRuleHashes.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.json`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/Labels.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/build.make`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeFiles/byteme-populate.dir/cmake_clean.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/Makefile` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitclone-lastrun.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/src/byteme-populate-stamp/byteme-populate-gitinfo.txt`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitclone.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-gitupdate.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/byteme-populate-prefix/tmp/byteme-populate-mkdirs.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake` & `rds2py-0.2.4/extern/rds2cpp/_deps/byteme-subbuild/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/cmake_install.cmake` & `rds2py-0.2.4/extern/rds2cpp/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/docs/Doxyfile` & `rds2py-0.2.4/extern/rds2cpp/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake` & `rds2py-0.2.4/extern/rds2cpp/extern/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/extern/Makefile` & `rds2py-0.2.4/extern/rds2cpp/extern/Makefile`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/extern/cmake_install.cmake` & `rds2py-0.2.4/extern/rds2cpp/extern/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/Environment.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/Environment.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/ExternalPointer.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RObject.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/RObject.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/RdsFile.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/RdsFile.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SEXPType.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/SEXPType.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/SharedParseInfo.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/SharedWriteInfo.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_altrep.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_atomic.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_attributes.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_builtin.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_environment.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_environment.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_expression.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_expression.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_external_pointer.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_language.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_language.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_list.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_list.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_object.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_object.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_pairlist.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_rds.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_rds.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_s4.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_s4.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_single_string.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/parse_symbol.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_parse.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/utils_parse.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/utils_write.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/utils_write.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_atomic.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_atomic.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_attributes.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_attributes.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_builtin.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_builtin.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_expression.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_expression.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_language.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_language.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_list.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_list.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_object.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_object.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_pairlist.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_rds.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_rds.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_s4.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_s4.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/include/rds2cpp/write_single_string.hpp` & `rds2py-0.2.4/extern/rds2cpp/include/rds2cpp/write_single_string.hpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/src/RcppExports.cpp` & `rds2py-0.2.4/extern/rds2cpp/tests/src/RcppExports.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/src/parse.cpp` & `rds2py-0.2.4/extern/rds2cpp/tests/src/parse.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/src/write.cpp` & `rds2py-0.2.4/extern/rds2cpp/tests/src/write.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-altrep.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-altrep.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-atomic.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-atomic.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-builtin.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-builtin.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-environment.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-environment.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-expression.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-expression.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-external-pointer.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-language.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-language.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-list.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-list.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-pairlist.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-pairlist.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-s4.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-s4.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/extern/rds2cpp/tests/tests/testthat/test-symbol.R` & `rds2py-0.2.4/extern/rds2cpp/tests/tests/testthat/test-symbol.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/setup.cfg` & `rds2py-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/setup.py` & `rds2py-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/src/rds2py/__init__.py` & `rds2py-0.2.4/src/rds2py/__init__.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/src/rds2py/interface.py` & `rds2py-0.2.4/src/rds2py/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     cls = get_class(robj)
 
     if cls not in ["densematrix"]:
         raise TypeError(f"obj is not a supported dense matrix format, but is `{cls}`")
 
     return np.ndarray(
         shape=tuple(robj["attributes"]["dim"]["data"].tolist()),
+        dtype=robj["data"].dtype,
         buffer=robj["data"],
         order=order,
     )
 
 
 def as_SCE(robj: MutableMapping) -> np.ndarray:
     """Convert a realized R object to a python `SingleCellExperiment` or `SummarizedExperiment` representation.
```

### Comparing `rds2py-0.2.3/src/rds2py/lib/parser.cpp` & `rds2py-0.2.4/src/rds2py/lib/parser.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 /* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "src/rds2py/lib/rds_parser.cpp"
         ],
         "extra_compile_args": [
             "-std=c++17"
         ],
         "extra_link_args": [
             "-lz"
         ],
         "include_dirs": [
             "src/rds2py/lib",
             "extern/rds2cpp/include",
             "extern/rds2cpp/_deps/byteme-src/include",
-            "/tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "rds2py.core",
         "sources": [
             "src/rds2py/lib/parser.pyx",
             "src/rds2py/lib/rds_parser.cpp"
         ]
@@ -1164,195 +1164,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1385,42 +1385,42 @@
 struct __pyx_obj_6rds2py_4core_PyParsedObject;
 struct __pyx_obj_6rds2py_4core_PyRObject;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -6178,15 +6178,15 @@
   __Pyx_AddTraceback("rds2py.core.PyRObject.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6195,29 +6195,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6228,15 +6228,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6245,29 +6245,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6278,15 +6278,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6295,29 +6295,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6328,15 +6328,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6345,29 +6345,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6378,15 +6378,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6395,29 +6395,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6428,212 +6428,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6649,15 +6649,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6665,53 +6665,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -6719,30 +6719,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6757,15 +6757,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6781,15 +6781,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6797,53 +6797,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -6851,30 +6851,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6889,15 +6889,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6913,15 +6913,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6929,53 +6929,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -6983,30 +6983,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7021,176 +7021,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21892,26 +21892,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../../../tmp/build-env-09c6s9qs/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-4_iz5gzi/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 950, __pyx_L1_error)
```

### Comparing `rds2py-0.2.3/src/rds2py/lib/parser.pxd` & `rds2py-0.2.4/src/rds2py/lib/parser.pxd`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/src/rds2py/lib/parser.pyx` & `rds2py-0.2.4/src/rds2py/lib/parser.pyx`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/src/rds2py/lib/rds_parser.cpp` & `rds2py-0.2.4/src/rds2py/lib/rds_parser.cpp`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/src/rds2py/parser.py` & `rds2py-0.2.4/src/rds2py/parser.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/src/rds2py/pdf.py` & `rds2py-0.2.4/src/rds2py/pdf.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/src/rds2py.egg-info/PKG-INFO` & `rds2py-0.2.4/src/rds2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds2py
-Version: 0.2.3
+Version: 0.2.4
 Summary: Parse and read RDS files as Python representations
 Home-page: https://github.com/biocpy/rds2py
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/rds2py/
 Project-URL: Source, https://github.com/biocpy/rds2py
```

### Comparing `rds2py-0.2.3/src/rds2py.egg-info/SOURCES.txt` & `rds2py-0.2.4/src/rds2py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -252,11 +252,12 @@
 tests/data/atomic_raw.rds
 tests/data/generate_files.R
 tests/data/lists.rds
 tests/data/lists_df.rds
 tests/data/lists_df_rownames.rds
 tests/data/lists_nested.rds
 tests/data/lists_nested_deep.rds
+tests/data/numpy_dtype.rds
 tests/data/s4_class.rds
 tests/data/s4_dense_matrix.rds
 tests/data/s4_matrix.rds
 tests/data/s4_matrix_dgt.rds
```

### Comparing `rds2py-0.2.3/test.py` & `rds2py-0.2.4/test.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/data/.Rhistory` & `rds2py-0.2.4/tests/data/.Rhistory`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/data/atomic_attr.rds` & `rds2py-0.2.4/tests/data/atomic_attr.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/data/atomic_complex.rds` & `rds2py-0.2.4/tests/data/atomic_complex.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/data/atomic_double.rds` & `rds2py-0.2.4/tests/data/atomic_double.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/data/generate_files.R` & `rds2py-0.2.4/tests/data/generate_files.R`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/data/s4_matrix.rds` & `rds2py-0.2.4/tests/data/s4_matrix.rds`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/test_atomic-attr.py` & `rds2py-0.2.4/tests/test_atomic-attr.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/test_atomic-bool.py` & `rds2py-0.2.4/tests/test_atomic-bool.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/test_atomic-str.py` & `rds2py-0.2.4/tests/test_atomic-str.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/test_interface_matrix.py` & `rds2py-0.2.4/tests/test_interface_matrix.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,7 +20,14 @@
 
 def test_read_s4_matrix_dgt():
     parsed_obj = read_rds("tests/data/s4_matrix_dgt.rds")
     array = as_sparse_matrix(parsed_obj)
 
     assert array is not None
     assert isinstance(array, sp.spmatrix)
+
+def test_read_dense_numpy_dtype():
+    parsed_obj = read_rds("tests/data/numpy_dtype.rds")
+    array = as_dense_matrix(parsed_obj)
+
+    assert array is not None
+    assert isinstance(array, np.ndarray)
```

### Comparing `rds2py-0.2.3/tests/test_list.py` & `rds2py-0.2.4/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tests/test_s4.py` & `rds2py-0.2.4/tests/test_s4.py`

 * *Files identical despite different names*

### Comparing `rds2py-0.2.3/tox.ini` & `rds2py-0.2.4/tox.ini`

 * *Files identical despite different names*

