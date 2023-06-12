# Comparing `tmp/mads_datasets-0.1.5.tar.gz` & `tmp/mads_datasets-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.5.tar", max compression
+gzip compressed data, was "mads_datasets-0.1.5.1.tar", max compression
```

## Comparing `mads_datasets-0.1.5.tar` & `mads_datasets-0.1.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:06:45.165441 mads_datasets-0.1.5/README.md
--rw-r--r--   0        0        0      164 2023-06-06 09:55:29.933711 mads_datasets-0.1.5/mads_datasets/__init__.py
--rw-r--r--   0        0        0    15387 2023-06-06 10:23:56.869646 mads_datasets-0.1.5/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.5/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5/mads_datasets/datatools.py
--rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.5/mads_datasets/settings.py
--rw-r--r--   0        0        0      974 2023-06-06 10:26:31.136041 mads_datasets-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mads_datasets-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1393 2023-06-07 14:25:34.493117 mads_datasets-0.1.5.1/README.md
+-rw-r--r--   0        0        0      164 2023-06-06 09:55:29.933711 mads_datasets-0.1.5.1/mads_datasets/__init__.py
+-rw-r--r--   0        0        0    15387 2023-06-06 10:23:56.869646 mads_datasets-0.1.5.1/mads_datasets/datasetfactory.py
+-rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.5.1/mads_datasets/datasets.py
+-rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5.1/mads_datasets/datatools.py
+-rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.5.1/mads_datasets/settings.py
+-rw-r--r--   0        0        0     1047 2023-06-12 06:54:35.598288 mads_datasets-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 mads_datasets-0.1.5.1/PKG-INFO
```

### Comparing `mads_datasets-0.1.5/mads_datasets/datasetfactory.py` & `mads_datasets-0.1.5.1/mads_datasets/datasetfactory.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5/mads_datasets/datasets.py` & `mads_datasets-0.1.5.1/mads_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5/mads_datasets/datatools.py` & `mads_datasets-0.1.5.1/mads_datasets/datatools.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5/mads_datasets/settings.py` & `mads_datasets-0.1.5.1/mads_datasets/settings.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5/pyproject.toml` & `mads_datasets-0.1.5.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [tool.poetry]
 name = "mads-datasets"
-version = "0.1.5"
+version = "0.1.5.1"
 description = "Datasets for the master applied data science"
 authors = ["Raoul Grouls <Raoul.Grouls@han.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mads_datasets"}]
 
+[tool.poetry.urls]
+GitHub = "https://github.com/raoulg/mads_datasets"
+
 [tool.poetry.dependencies]
 python = "^3.9"
 torch = "^2.0.1"
 tqdm = "^4.65.0"
 requests = "^2.31.0"
 loguru = "^0.7.0"
 numpy = "^1.24.3"
```

