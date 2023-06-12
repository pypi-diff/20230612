# Comparing `tmp/simpgit-0.0.1.tar.gz` & `tmp/simpgit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpgit-0.0.1.tar", last modified: Mon Jun 12 20:17:37 2023, max compression
+gzip compressed data, was "simpgit-0.0.2.tar", last modified: Mon Jun 12 20:19:17 2023, max compression
```

## Comparing `simpgit-0.0.1.tar` & `simpgit-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:17:37.123482 simpgit-0.0.1/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 simpgit-0.0.1/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 simpgit-0.0.1/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1211 2023-06-12 20:17:37.123141 simpgit-0.0.1/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1892 2023-06-12 20:13:37.000000 simpgit-0.0.1/README.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      815 2023-06-09 15:12:38.000000 simpgit-0.0.1/config.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:17:37.121324 simpgit-0.0.1/gitllm/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      122 2023-06-12 20:05:15.000000 simpgit-0.0.1/gitllm/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     5338 2023-06-12 20:15:31.000000 simpgit-0.0.1/gitllm/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3088 2023-06-12 20:01:30.000000 simpgit-0.0.1/gitllm/git.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1526 2023-06-12 19:49:46.000000 simpgit-0.0.1/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 simpgit-0.0.1/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-12 20:17:37.123560 simpgit-0.0.1/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:17:37.122614 simpgit-0.0.1/simpgit.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1211 2023-06-12 20:17:33.000000 simpgit-0.0.1/simpgit.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      330 2023-06-12 20:17:37.000000 simpgit-0.0.1/simpgit.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-12 20:17:33.000000 simpgit-0.0.1/simpgit.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       73 2023-06-12 20:17:33.000000 simpgit-0.0.1/simpgit.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       65 2023-06-12 20:17:33.000000 simpgit-0.0.1/simpgit.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        7 2023-06-12 20:17:33.000000 simpgit-0.0.1/simpgit.egg-info/top_level.txt
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:17:37.122794 simpgit-0.0.1/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 simpgit-0.0.1/tests/__init__.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:19:17.768251 simpgit-0.0.2/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 simpgit-0.0.2/.gitattributes
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 simpgit-0.0.2/.gitignore
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3144 2023-06-12 20:19:17.767921 simpgit-0.0.2/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1892 2023-06-12 20:13:37.000000 simpgit-0.0.2/README.md
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      815 2023-06-09 15:12:38.000000 simpgit-0.0.2/config.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:19:17.766390 simpgit-0.0.2/gitllm/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      122 2023-06-12 20:05:15.000000 simpgit-0.0.2/gitllm/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     5338 2023-06-12 20:15:31.000000 simpgit-0.0.2/gitllm/cli.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3088 2023-06-12 20:01:30.000000 simpgit-0.0.2/gitllm/git.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1547 2023-06-12 20:19:01.000000 simpgit-0.0.2/pyproject.toml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 simpgit-0.0.2/requirements.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-12 20:19:17.768320 simpgit-0.0.2/setup.cfg
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:19:17.767435 simpgit-0.0.2/simpgit.egg-info/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3144 2023-06-12 20:19:14.000000 simpgit-0.0.2/simpgit.egg-info/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      330 2023-06-12 20:19:17.000000 simpgit-0.0.2/simpgit.egg-info/SOURCES.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-12 20:19:14.000000 simpgit-0.0.2/simpgit.egg-info/dependency_links.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       73 2023-06-12 20:19:14.000000 simpgit-0.0.2/simpgit.egg-info/entry_points.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       65 2023-06-12 20:19:14.000000 simpgit-0.0.2/simpgit.egg-info/requires.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        7 2023-06-12 20:19:14.000000 simpgit-0.0.2/simpgit.egg-info/top_level.txt
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-12 20:19:17.767605 simpgit-0.0.2/tests/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 simpgit-0.0.2/tests/__init__.py
```

### Comparing `simpgit-0.0.1/.gitignore` & `simpgit-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `simpgit-0.0.1/README.md` & `simpgit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `simpgit-0.0.1/config.py` & `simpgit-0.0.2/config.py`

 * *Files identical despite different names*

### Comparing `simpgit-0.0.1/gitllm/cli.py` & `simpgit-0.0.2/gitllm/cli.py`

 * *Files identical despite different names*

### Comparing `simpgit-0.0.1/gitllm/git.py` & `simpgit-0.0.2/gitllm/git.py`

 * *Files identical despite different names*

### Comparing `simpgit-0.0.1/pyproject.toml` & `simpgit-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simpgit"
-version = "0.0.1"
+version = "0.0.2"
 description = "A tool to simplfy git operations"
+readme = "README.md"
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
     "git",
     "nlp",
```

