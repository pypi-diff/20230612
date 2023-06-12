# Comparing `tmp/jinaai-0.1.0.tar.gz` & `tmp/jinaai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.1.0.tar", last modified: Fri Jun  9 08:17:53 2023, max compression
+gzip compressed data, was "jinaai-0.1.1.tar", last modified: Mon Jun 12 03:55:38 2023, max compression
```

## Comparing `jinaai-0.1.0.tar` & `jinaai-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-09 08:17:53.063112 jinaai-0.1.0/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      186 2023-06-09 08:17:53.062983 jinaai-0.1.0/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       15 2023-06-09 08:02:58.000000 jinaai-0.1.0/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-09 08:17:53.062264 jinaai-0.1.0/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      383 2023-06-09 08:13:55.000000 jinaai-0.1.0/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-09 08:17:53.062834 jinaai-0.1.0/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      186 2023-06-09 08:17:53.000000 jinaai-0.1.0/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      157 2023-06-09 08:17:53.000000 jinaai-0.1.0/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-09 08:17:53.000000 jinaai-0.1.0/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-09 08:17:53.000000 jinaai-0.1.0/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-09 08:17:53.063151 jinaai-0.1.0/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      307 2023-06-09 08:16:47.000000 jinaai-0.1.0/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 03:55:38.170729 jinaai-0.1.1/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.1.1/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      208 2023-06-12 03:55:38.170535 jinaai-0.1.1/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      627 2023-06-09 08:24:51.000000 jinaai-0.1.1/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 03:55:38.169874 jinaai-0.1.1/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      383 2023-06-09 08:13:55.000000 jinaai-0.1.1/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 03:55:38.170401 jinaai-0.1.1/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      208 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      165 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-12 03:55:38.000000 jinaai-0.1.1/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-12 03:55:38.170768 jinaai-0.1.1/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      307 2023-06-12 03:53:51.000000 jinaai-0.1.1/setup.py
```

