# Comparing `tmp/mads_datasets-0.1.5.1.tar.gz` & `tmp/mads_datasets-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.5.1.tar", max compression
+gzip compressed data, was "mads_datasets-0.1.5.2.tar", max compression
```

## Comparing `mads_datasets-0.1.5.1.tar` & `mads_datasets-0.1.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1393 2023-06-07 14:25:34.493117 mads_datasets-0.1.5.1/README.md
--rw-r--r--   0        0        0      164 2023-06-06 09:55:29.933711 mads_datasets-0.1.5.1/mads_datasets/__init__.py
--rw-r--r--   0        0        0    15387 2023-06-06 10:23:56.869646 mads_datasets-0.1.5.1/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.5.1/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5.1/mads_datasets/datatools.py
--rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.5.1/mads_datasets/settings.py
--rw-r--r--   0        0        0     1047 2023-06-12 06:54:35.598288 mads_datasets-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 mads_datasets-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1393 2023-06-07 14:25:34.493117 mads_datasets-0.1.5.2/README.md
+-rw-r--r--   0        0        0      188 2023-06-12 07:06:56.170150 mads_datasets-0.1.5.2/mads_datasets/__init__.py
+-rw-r--r--   0        0        0    15387 2023-06-06 10:23:56.869646 mads_datasets-0.1.5.2/mads_datasets/datasetfactory.py
+-rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.5.2/mads_datasets/datasets.py
+-rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5.2/mads_datasets/datatools.py
+-rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.5.2/mads_datasets/settings.py
+-rw-r--r--   0        0        0      982 2023-06-12 07:06:51.311671 mads_datasets-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mads_datasets-0.1.5.2/PKG-INFO
```

### Comparing `mads_datasets-0.1.5.1/README.md` & `mads_datasets-0.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.1/mads_datasets/datasetfactory.py` & `mads_datasets-0.1.5.2/mads_datasets/datasetfactory.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.1/mads_datasets/datasets.py` & `mads_datasets-0.1.5.2/mads_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.1/mads_datasets/datatools.py` & `mads_datasets-0.1.5.2/mads_datasets/datatools.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.1/mads_datasets/settings.py` & `mads_datasets-0.1.5.2/mads_datasets/settings.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.1/pyproject.toml` & `mads_datasets-0.1.5.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 [tool.poetry]
 name = "mads-datasets"
-version = "0.1.5.1"
+version = "0.1.5.2"
 description = "Datasets for the master applied data science"
 authors = ["Raoul Grouls <Raoul.Grouls@han.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mads_datasets"}]
 
 [tool.poetry.urls]
 GitHub = "https://github.com/raoulg/mads_datasets"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.9.16"
 torch = "^2.0.1"
 tqdm = "^4.65.0"
 requests = "^2.31.0"
 loguru = "^0.7.0"
 numpy = "^1.24.3"
 pydantic = "^1.10.8"
 pillow = "^9.5.0"
-
+torchtext = "^0.15.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pytest = "^7.3.1"
 pep8-naming = "^0.13.3"
 flake8-annotations = "^3.0.1"
 jupyter = "^1.0.0"
 
-
 [tool.poetry.group.tests.dependencies]
 responses = "^0.23.1"
 
-
-[tool.poetry.group.extras.dependencies]
-torchtext = "^0.15.2"
-torchvision = "^0.15.2"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning:jupyter_client.*:",
```

### Comparing `mads_datasets-0.1.5.1/PKG-INFO` & `mads_datasets-0.1.5.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Datasets for the master applied data science
 License: MIT
 Author: Raoul Grouls
 Author-email: Raoul.Grouls@han.nl
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9.16,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: torchtext (>=0.15.2,<0.16.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: GitHub, https://github.com/raoulg/mads_datasets
 Description-Content-Type: text/markdown
 
 # MADS Datasets Library
 
 This library provides the functionality to download, process, and stream several datasets.
```

