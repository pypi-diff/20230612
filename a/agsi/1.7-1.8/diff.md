# Comparing `tmp/agsi-1.7.tar.gz` & `tmp/agsi-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.7.tar", last modified: Mon Jun 12 08:25:29 2023, max compression
+gzip compressed data, was "agsi-1.8.tar", last modified: Mon Jun 12 10:15:33 2023, max compression
```

## Comparing `agsi-1.7.tar` & `agsi-1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:25:29.621582 agsi-1.7/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-1.7/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 08:25:29.621582 agsi-1.7/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-1.7/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:25:29.621582 agsi-1.7/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-1.7/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:25:29.621582 agsi-1.7/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    15761 2023-06-12 08:25:13.000000 agsi-1.7/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-1.7/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     5980 2023-05-25 15:09:48.000000 agsi-1.7/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075103 2023-06-12 08:02:57.000000 agsi-1.7/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-1.7/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-1.7/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 08:25:29.621582 agsi-1.7/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 08:25:29.000000 agsi-1.7/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-12 08:25:29.000000 agsi-1.7/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-12 08:25:29.000000 agsi-1.7/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-12 08:25:29.000000 agsi-1.7/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-12 08:25:29.000000 agsi-1.7/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-12 08:25:29.621582 agsi-1.7/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-12 08:25:25.000000 agsi-1.7/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-1.8/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:15:33.143444 agsi-1.8/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-1.8/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-1.8/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15761 2023-06-12 08:25:13.000000 agsi-1.8/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-1.8/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     8953 2023-06-12 10:08:03.000000 agsi-1.8/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075103 2023-06-12 08:02:57.000000 agsi-1.8/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-1.8/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-1.8/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:15:33.143444 agsi-1.8/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-12 10:15:33.000000 agsi-1.8/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-12 10:15:33.143444 agsi-1.8/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-12 10:15:25.000000 agsi-1.8/setup.py
```

### Comparing `agsi-1.7/agsi/data/FarmData.py` & `agsi-1.8/agsi/data/FarmData.py`

 * *Files identical despite different names*

### Comparing `agsi-1.7/agsi/demo_V2.ipynb` & `agsi-1.8/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

