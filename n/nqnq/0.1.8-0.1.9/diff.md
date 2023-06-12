# Comparing `tmp/nqnq-0.1.8.tar.gz` & `tmp/nqnq-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nqnq-0.1.8.tar", last modified: Mon Aug 29 09:52:17 2022, max compression
+gzip compressed data, was "nqnq-0.1.9.tar", last modified: Fri Sep 23 09:37:53 2022, max compression
```

## Comparing `nqnq-0.1.8.tar` & `nqnq-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-08-29 09:52:17.137482 nqnq-0.1.8/
--rw-r--r--   0 nanangqq   (501) staff       (20)     1074 2022-04-23 04:32:14.000000 nqnq-0.1.8/LICENSE
--rw-r--r--   0 nanangqq   (501) staff       (20)       54 2022-06-12 01:38:29.000000 nqnq-0.1.8/MANIFEST.in
--rw-r--r--   0 nanangqq   (501) staff       (20)      477 2022-08-29 09:52:17.137302 nqnq-0.1.8/PKG-INFO
--rw-r--r--   0 nanangqq   (501) staff       (20)      148 2022-06-12 01:25:25.000000 nqnq-0.1.8/README.md
--rw-r--r--   0 nanangqq   (501) staff       (20)       84 2022-04-23 04:32:14.000000 nqnq-0.1.8/pyproject.toml
--rw-r--r--   0 nanangqq   (501) staff       (20)       57 2022-06-12 02:00:33.000000 nqnq-0.1.8/requirements.txt
--rw-r--r--   0 nanangqq   (501) staff       (20)       38 2022-08-29 09:52:17.137531 nqnq-0.1.8/setup.cfg
--rw-r--r--   0 nanangqq   (501) staff       (20)      886 2022-08-29 09:51:54.000000 nqnq-0.1.8/setup.py
-drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-08-29 09:52:17.123957 nqnq-0.1.8/src/
-drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-08-29 09:52:17.127269 nqnq-0.1.8/src/nq/
--rw-r--r--   0 nanangqq   (501) staff       (20)        0 2022-04-23 04:32:14.000000 nqnq-0.1.8/src/nq/__init__.py
-drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-08-29 09:52:17.130620 nqnq-0.1.8/src/nq/data/
--rw-r--r--   0 nanangqq   (501) staff       (20)      371 2022-08-23 06:27:29.000000 nqnq-0.1.8/src/nq/data/__init__.py
--rw-r--r--   0 nanangqq   (501) staff       (20)  2024216 2022-06-12 00:56:55.000000 nqnq-0.1.8/src/nq/data/bjd_20220401.pkl
--rw-r--r--   0 nanangqq   (501) staff       (20)  2017709 2022-08-23 05:56:21.000000 nqnq-0.1.8/src/nq/data/bjd_20220701.pkl
--rw-r--r--   0 nanangqq   (501) staff       (20)      473 2022-06-08 07:15:45.000000 nqnq-0.1.8/src/nq/hwp.py
--rw-r--r--   0 nanangqq   (501) staff       (20)      329 2022-04-23 04:36:37.000000 nqnq-0.1.8/src/nq/kk.py
--rw-r--r--   0 nanangqq   (501) staff       (20)     6042 2022-08-29 09:47:46.000000 nqnq-0.1.8/src/nq/pnu.py
--rw-r--r--   0 nanangqq   (501) staff       (20)     4085 2022-07-20 09:37:27.000000 nqnq-0.1.8/src/nq/rates.py
--rw-r--r--   0 nanangqq   (501) staff       (20)       63 2022-06-12 00:27:08.000000 nqnq-0.1.8/src/nq/sql.py
--rw-r--r--   0 nanangqq   (501) staff       (20)      458 2022-08-23 06:29:30.000000 nqnq-0.1.8/src/nq/test.py
--rw-r--r--   0 nanangqq   (501) staff       (20)     3457 2022-06-08 09:15:33.000000 nqnq-0.1.8/src/nq/vid.py
-drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-08-29 09:52:17.137118 nqnq-0.1.8/src/nqnq.egg-info/
--rw-r--r--   0 nanangqq   (501) staff       (20)      477 2022-08-29 09:52:17.000000 nqnq-0.1.8/src/nqnq.egg-info/PKG-INFO
--rw-r--r--   0 nanangqq   (501) staff       (20)      430 2022-08-29 09:52:17.000000 nqnq-0.1.8/src/nqnq.egg-info/SOURCES.txt
--rw-r--r--   0 nanangqq   (501) staff       (20)        1 2022-08-29 09:52:17.000000 nqnq-0.1.8/src/nqnq.egg-info/dependency_links.txt
--rw-r--r--   0 nanangqq   (501) staff       (20)       26 2022-08-29 09:52:17.000000 nqnq-0.1.8/src/nqnq.egg-info/requires.txt
--rw-r--r--   0 nanangqq   (501) staff       (20)        3 2022-08-29 09:52:17.000000 nqnq-0.1.8/src/nqnq.egg-info/top_level.txt
+drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-09-23 09:37:53.752128 nqnq-0.1.9/
+-rw-r--r--   0 nanangqq   (501) staff       (20)     1074 2022-04-23 04:32:14.000000 nqnq-0.1.9/LICENSE
+-rw-r--r--   0 nanangqq   (501) staff       (20)       54 2022-06-12 01:38:29.000000 nqnq-0.1.9/MANIFEST.in
+-rw-r--r--   0 nanangqq   (501) staff       (20)      477 2022-09-23 09:37:53.751983 nqnq-0.1.9/PKG-INFO
+-rw-r--r--   0 nanangqq   (501) staff       (20)      148 2022-06-12 01:25:25.000000 nqnq-0.1.9/README.md
+-rw-r--r--   0 nanangqq   (501) staff       (20)       84 2022-04-23 04:32:14.000000 nqnq-0.1.9/pyproject.toml
+-rw-r--r--   0 nanangqq   (501) staff       (20)       57 2022-06-12 02:00:33.000000 nqnq-0.1.9/requirements.txt
+-rw-r--r--   0 nanangqq   (501) staff       (20)       38 2022-09-23 09:37:53.752175 nqnq-0.1.9/setup.cfg
+-rw-r--r--   0 nanangqq   (501) staff       (20)      886 2022-09-23 09:37:42.000000 nqnq-0.1.9/setup.py
+drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-09-23 09:37:53.740390 nqnq-0.1.9/src/
+drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-09-23 09:37:53.743139 nqnq-0.1.9/src/nq/
+-rw-r--r--   0 nanangqq   (501) staff       (20)        0 2022-04-23 04:32:14.000000 nqnq-0.1.9/src/nq/__init__.py
+drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-09-23 09:37:53.746769 nqnq-0.1.9/src/nq/data/
+-rw-r--r--   0 nanangqq   (501) staff       (20)      371 2022-08-23 06:27:29.000000 nqnq-0.1.9/src/nq/data/__init__.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)  2024216 2022-06-12 00:56:55.000000 nqnq-0.1.9/src/nq/data/bjd_20220401.pkl
+-rw-r--r--   0 nanangqq   (501) staff       (20)  2017709 2022-08-23 05:56:21.000000 nqnq-0.1.9/src/nq/data/bjd_20220701.pkl
+-rw-r--r--   0 nanangqq   (501) staff       (20)      473 2022-06-08 07:15:45.000000 nqnq-0.1.9/src/nq/hwp.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)      329 2022-04-23 04:36:37.000000 nqnq-0.1.9/src/nq/kk.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)     6042 2022-08-29 09:47:46.000000 nqnq-0.1.9/src/nq/pnu.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)     4085 2022-07-20 09:37:27.000000 nqnq-0.1.9/src/nq/rates.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)      728 2022-09-23 09:37:09.000000 nqnq-0.1.9/src/nq/sb.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)       63 2022-06-12 00:27:08.000000 nqnq-0.1.9/src/nq/sql.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)      458 2022-08-23 06:29:30.000000 nqnq-0.1.9/src/nq/test.py
+-rw-r--r--   0 nanangqq   (501) staff       (20)     3457 2022-06-08 09:15:33.000000 nqnq-0.1.9/src/nq/vid.py
+drwxr-xr-x   0 nanangqq   (501) staff       (20)        0 2022-09-23 09:37:53.751799 nqnq-0.1.9/src/nqnq.egg-info/
+-rw-r--r--   0 nanangqq   (501) staff       (20)      477 2022-09-23 09:37:53.000000 nqnq-0.1.9/src/nqnq.egg-info/PKG-INFO
+-rw-r--r--   0 nanangqq   (501) staff       (20)      443 2022-09-23 09:37:53.000000 nqnq-0.1.9/src/nqnq.egg-info/SOURCES.txt
+-rw-r--r--   0 nanangqq   (501) staff       (20)        1 2022-09-23 09:37:53.000000 nqnq-0.1.9/src/nqnq.egg-info/dependency_links.txt
+-rw-r--r--   0 nanangqq   (501) staff       (20)       26 2022-09-23 09:37:53.000000 nqnq-0.1.9/src/nqnq.egg-info/requires.txt
+-rw-r--r--   0 nanangqq   (501) staff       (20)        3 2022-09-23 09:37:53.000000 nqnq-0.1.9/src/nqnq.egg-info/top_level.txt
```

### Comparing `nqnq-0.1.8/LICENSE` & `nqnq-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nqnq-0.1.8/setup.py` & `nqnq-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     running_idx = lines.index("# running")
     requirements = lines[running_idx + 1 :]
     print(requirements)
 
 
 setuptools.setup(
     name="nqnq",
-    version="0.1.8",
+    version="0.1.9",
     author="nanangqq",
     author_email="gingggg@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `nqnq-0.1.8/src/nq/data/bjd_20220401.pkl` & `nqnq-0.1.9/src/nq/data/bjd_20220401.pkl`

 * *Files identical despite different names*

### Comparing `nqnq-0.1.8/src/nq/data/bjd_20220701.pkl` & `nqnq-0.1.9/src/nq/data/bjd_20220701.pkl`

 * *Files identical despite different names*

### Comparing `nqnq-0.1.8/src/nq/pnu.py` & `nqnq-0.1.9/src/nq/pnu.py`

 * *Files identical despite different names*

### Comparing `nqnq-0.1.8/src/nq/rates.py` & `nqnq-0.1.9/src/nq/rates.py`

 * *Files identical despite different names*

### Comparing `nqnq-0.1.8/src/nq/vid.py` & `nqnq-0.1.9/src/nq/vid.py`

 * *Files identical despite different names*

