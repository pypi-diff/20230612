# Comparing `tmp/clementine-0.0.3.dev0.tar.gz` & `tmp/clementine-2023.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clementine-0.0.3.dev0.tar", last modified: Mon May 29 01:26:52 2023, max compression
+gzip compressed data, was "clementine-2023.6.12.tar", last modified: Mon Jun 12 19:16:18 2023, max compression
```

## Comparing `clementine-0.0.3.dev0.tar` & `clementine-2023.6.12.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.210205 clementine-0.0.3.dev0/
--rw-r--r--   0 sue        (501) staff       (20)     1394 2023-05-29 01:26:52.210060 clementine-0.0.3.dev0/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      855 2023-05-29 01:24:23.000000 clementine-0.0.3.dev0/README.md
--rw-r--r--   0 sue        (501) staff       (20)      994 2023-05-29 01:04:28.000000 clementine-0.0.3.dev0/pyproject.toml
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-29 01:26:52.210240 clementine-0.0.3.dev0/setup.cfg
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-29 01:07:57.000000 clementine-0.0.3.dev0/setup.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.207232 clementine-0.0.3.dev0/src/
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.208299 clementine-0.0.3.dev0/src/clementine/
--rw-r--r--   0 sue        (501) staff       (20)      108 2023-05-29 00:46:48.000000 clementine-0.0.3.dev0/src/clementine/__init__.py
--rw-r--r--   0 sue        (501) staff       (20)      443 2023-05-29 00:34:22.000000 clementine-0.0.3.dev0/src/clementine/cli.py
--rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-28 14:37:03.000000 clementine-0.0.3.dev0/src/clementine/version.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.209517 clementine-0.0.3.dev0/src/clementine.egg-info/
--rw-r--r--   0 sue        (501) staff       (20)     1394 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      363 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/SOURCES.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/dependency_links.txt
--rw-r--r--   0 sue        (501) staff       (20)       51 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/entry_points.txt
--rw-r--r--   0 sue        (501) staff       (20)      234 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/requires.txt
--rw-r--r--   0 sue        (501) staff       (20)       11 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/top_level.txt
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.209674 clementine-0.0.3.dev0/tests/
--rw-r--r--   0 sue        (501) staff       (20)      101 2023-05-29 00:31:28.000000 clementine-0.0.3.dev0/tests/test_clementine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 19:16:05.000000 clementine-2023.6.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-12 19:16:18.316277 clementine-2023.6.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-12 19:16:05.000000 clementine-2023.6.12/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-12 19:16:05.000000 clementine-2023.6.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:16:18.316277 clementine-2023.6.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 19:16:05.000000 clementine-2023.6.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.312276 clementine-2023.6.12/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/src/clementine/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/blossom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-12 19:16:05.000000 clementine-2023.6.12/src/clementine/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/src/clementine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 19:16:18.000000 clementine-2023.6.12/src/clementine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:16:18.316277 clementine-2023.6.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-12 19:16:05.000000 clementine-2023.6.12/tests/test_blossom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-12 19:16:05.000000 clementine-2023.6.12/tests/test_clementine.py
```

