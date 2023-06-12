# Comparing `tmp/OpenFintech-0.0.3.tar.gz` & `tmp/OpenFintech-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFintech-0.0.3.tar", last modified: Thu Jun  8 19:27:11 2023, max compression
+gzip compressed data, was "OpenFintech-0.0.4.tar", last modified: Mon Jun 12 04:24:11 2023, max compression
```

## Comparing `OpenFintech-0.0.3.tar` & `OpenFintech-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-08 19:27:11.013448 OpenFintech-0.0.3/
--rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.3/LICENSE
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-08 19:27:11.011991 OpenFintech-0.0.3/OpenFintech/
--rw-r--r--   0 harri      (501) staff       (20)     2514 2023-06-08 19:24:31.000000 OpenFintech-0.0.3/OpenFintech/FinMongo.py
--rw-r--r--   0 harri      (501) staff       (20)       30 2023-06-08 17:08:02.000000 OpenFintech-0.0.3/OpenFintech/__init__.py
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-08 19:27:11.013019 OpenFintech-0.0.3/OpenFintech.egg-info/
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-08 19:27:10.000000 OpenFintech-0.0.3/OpenFintech.egg-info/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)      214 2023-06-08 19:27:10.000000 OpenFintech-0.0.3/OpenFintech.egg-info/SOURCES.txt
--rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-08 19:27:10.000000 OpenFintech-0.0.3/OpenFintech.egg-info/dependency_links.txt
--rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-08 19:27:10.000000 OpenFintech-0.0.3/OpenFintech.egg-info/top_level.txt
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-08 19:27:11.013274 OpenFintech-0.0.3/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)       14 2023-06-05 19:27:30.000000 OpenFintech-0.0.3/README.md
--rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-08 19:27:11.013499 OpenFintech-0.0.3/setup.cfg
--rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-08 19:25:35.000000 OpenFintech-0.0.3/setup.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-12 04:24:11.009088 OpenFintech-0.0.4/
+-rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.4/LICENSE
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-12 04:24:11.007758 OpenFintech-0.0.4/OpenFintech/
+-rw-r--r--   0 harri      (501) staff       (20)     6459 2023-06-12 04:23:26.000000 OpenFintech-0.0.4/OpenFintech/FinMongo.py
+-rw-r--r--   0 harri      (501) staff       (20)     1284 2023-06-12 04:23:25.000000 OpenFintech-0.0.4/OpenFintech/User.py
+-rw-r--r--   0 harri      (501) staff       (20)       53 2023-06-08 20:01:22.000000 OpenFintech-0.0.4/OpenFintech/__init__.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-12 04:24:11.008671 OpenFintech-0.0.4/OpenFintech.egg-info/
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)      234 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/SOURCES.txt
+-rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/dependency_links.txt
+-rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/top_level.txt
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-12 04:24:11.008910 OpenFintech-0.0.4/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)       14 2023-06-05 19:27:30.000000 OpenFintech-0.0.4/README.md
+-rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-12 04:24:11.009142 OpenFintech-0.0.4/setup.cfg
+-rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-12 04:21:45.000000 OpenFintech-0.0.4/setup.py
```

### Comparing `OpenFintech-0.0.3/LICENSE` & `OpenFintech-0.0.4/LICENSE`

 * *Files identical despite different names*

