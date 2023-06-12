# Comparing `tmp/oexp-0.7.1.tar.gz` & `tmp/oexp-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.7.1.tar", last modified: Mon Jun 12 13:55:02 2023, max compression
+gzip compressed data, was "oexp-0.7.2.tar", last modified: Mon Jun 12 14:01:05 2023, max compression
```

## Comparing `oexp-0.7.1.tar` & `oexp-0.7.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 13:55:02.301936 oexp-0.7.1/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 13:55:02.301763 oexp-0.7.1/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.1/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 13:55:02.300438 oexp-0.7.1/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.1/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    80499 2023-06-12 13:23:43.000000 oexp-0.7.1/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 13:23:43.000000 oexp-0.7.1/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.1/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 13:55:02.301572 oexp-0.7.1/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.1/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2384 2023-06-12 13:53:27.000000 oexp-0.7.1/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.1/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 13:55:02.301183 oexp-0.7.1/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 13:55:02.000000 oexp-0.7.1/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 13:55:02.000000 oexp-0.7.1/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 13:55:02.000000 oexp-0.7.1/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 13:55:02.000000 oexp-0.7.1/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 13:55:02.000000 oexp-0.7.1/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 13:54:57.000000 oexp-0.7.1/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 13:55:02.301995 oexp-0.7.1/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.207837 oexp-0.7.2/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:01:05.207683 oexp-0.7.2/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.7.2/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.206479 oexp-0.7.2/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.7.2/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    80499 2023-06-12 13:23:43.000000 oexp-0.7.2/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-12 13:23:43.000000 oexp-0.7.2/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2011 2023-06-12 01:50:22.000000 oexp-0.7.2/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.207518 oexp-0.7.2/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.7.2/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2384 2023-06-12 13:59:58.000000 oexp-0.7.2/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.7.2/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-12 14:01:05.207143 oexp-0.7.2/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-12 14:01:05.000000 oexp-0.7.2/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-12 14:01:00.000000 oexp-0.7.2/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-12 14:01:05.207880 oexp-0.7.2/setup.cfg
```

### Comparing `oexp-0.7.1/oexp/access.py` & `oexp-0.7.2/oexp/access.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.1/oexp/jbridge.py` & `oexp-0.7.2/oexp/jbridge.py`

 * *Files identical despite different names*

### Comparing `oexp-0.7.1/oexp/util/ops.py` & `oexp-0.7.2/oexp/util/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     data_dir = vals.user_data_dir()
     last_downloaded_jar_path = os.path.join(data_dir, f"last_downloaded_jar.txt")
     jar_path = os.path.join(data_dir, f"oexp-front-0-all.jar")
 
     need_to_download = True
     if os.path.exists(last_downloaded_jar_path):
         with open(last_downloaded_jar_path, 'r') as f:
-            need_to_download = f.read() == gen.JAR_VERSION
+            need_to_download = f.read() != gen.JAR_VERSION
     if need_to_download:
         if os.path.exists(jar_path):
             os.remove(jar_path)
         print("downloading jar...")
         request.urlretrieve(
             access.JAR_URL,
             jar_path
```

### Comparing `oexp-0.7.1/oexp/util/vals.py` & `oexp-0.7.2/oexp/util/vals.py`

 * *Files identical despite different names*

