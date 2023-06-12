# Comparing `tmp/audible-series-1.0.2.tar.gz` & `tmp/audible_series-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audible-series-1.0.2.tar", max compression
+gzip compressed data, was "audible_series-1.0.3.tar", max compression
```

## Comparing `audible-series-1.0.2.tar` & `audible_series-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1158 2021-08-01 05:53:21.530056 audible-series-1.0.2/README.md
--rw-r--r--   0        0        0       22 2021-07-08 00:10:28.983999 audible-series-1.0.2/audible_series/__init__.py
--rw-r--r--   0        0        0     2892 2021-08-01 05:11:26.248056 audible-series-1.0.2/audible_series/cmd_series.py
--rw-r--r--   0        0        0     1542 2021-08-01 05:31:49.070056 audible-series-1.0.2/audible_series/configfile.py
--rw-r--r--   0        0        0     6372 2021-08-01 05:08:39.691056 audible-series-1.0.2/audible_series/seriesutil.py
--rw-r--r--   0        0        0      732 2021-08-01 05:53:54.418056 audible-series-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2068 2021-08-01 05:54:54.691055 audible-series-1.0.2/setup.py
--rw-r--r--   0        0        0     1850 2021-08-01 05:54:54.691055 audible-series-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 04:09:11.245701 audible_series-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1053 2023-06-12 04:33:00.773702 audible_series-1.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-12 04:09:11.245701 audible_series-1.0.3/audible_series/__init__.py
+-rw-r--r--   0        0        0     2892 2023-06-12 04:09:11.245701 audible_series-1.0.3/audible_series/cmd_series.py
+-rw-r--r--   0        0        0     1542 2023-06-12 04:09:11.245701 audible_series-1.0.3/audible_series/configfile.py
+-rw-r--r--   0        0        0     6372 2023-06-12 04:09:11.249701 audible_series-1.0.3/audible_series/seriesutil.py
+-rw-r--r--   0        0        0      718 2023-06-12 04:34:30.157702 audible_series-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 audible_series-1.0.3/PKG-INFO
```

### Comparing `audible-series-1.0.2/README.md` & `audible_series-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 # Audible Series Command
 
 ## Installation
 
 ```
 pip3 install audible
+pip3 install audible-cli
 pip3 install audible-series
 ```
 
-Sadly the audible-cli tool is not in pypi but is packaged, it's easiest to
-install via git:
-
-```
-git clone https://github.com/mkb79/audible-cli
-pip3 install ./audible-cli
-```
-
 ## Usage
 
 The command will work on an exported library file:
 
 ```
 audible library export
 audible series -l $PWD/library.csv -c $PWD/config.yaml
@@ -35,13 +28,14 @@
 
 This project uses poetry which wraps a bunch of tools like virtualenv.  The
 easiest way to run it for development is to clone this repository then run a
 poetry shell.
 
 ```
 poetry shell
+set -x AUDIBLE_PLUGIN_DIR $PWD/audible_series
 audible library export
 audible series -l $PWD/library.csv -c $PWD/config.yaml
 ```
 
 When developing the `--only_series` flag may be useful since it will filter the
 library to a single series.
```

### Comparing `audible-series-1.0.2/audible_series/cmd_series.py` & `audible_series-1.0.3/audible_series/cmd_series.py`

 * *Files identical despite different names*

### Comparing `audible-series-1.0.2/audible_series/configfile.py` & `audible_series-1.0.3/audible_series/configfile.py`

 * *Files identical despite different names*

### Comparing `audible-series-1.0.2/audible_series/seriesutil.py` & `audible_series-1.0.3/audible_series/seriesutil.py`

 * *Files identical despite different names*

### Comparing `audible-series-1.0.2/pyproject.toml` & `audible_series-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "audible-series"
-version = "1.0.2"
+version = "1.0.3"
 description = "Adds a command to audible-cli that looks for new series releases in a user's library."
 authors = ["Alex Lusco <alex.lusco@gmail.com>"]
 homepage = "https://github.com/luscoma/audible-series"
 repository = "https://github.com/luscoma/audible-series"
 readme="README.md"
 keywords = ["audible"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-audible = "^0.5.4"
-PyYAML = "^5.4.1"
+python = ">=3"
+audible = ">=0.5.4, <1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 autopep8 = "^1.5.7"
 pylint = "^2.9.3"
 parameterized = "^0.8.1"
```

### Comparing `audible-series-1.0.2/PKG-INFO` & `audible_series-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: audible-series
-Version: 1.0.2
+Version: 1.0.3
 Summary: Adds a command to audible-cli that looks for new series releases in a user's library.
 Home-page: https://github.com/luscoma/audible-series
 Keywords: audible
 Author: Alex Lusco
 Author-email: alex.lusco@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
-Requires-Dist: audible (>=0.5.4,<0.6.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: audible (>=0.5.4,<1)
 Project-URL: Repository, https://github.com/luscoma/audible-series
 Description-Content-Type: text/markdown
 
 # Audible Series Command
 
 ## Installation
 
 ```
 pip3 install audible
+pip3 install audible-cli
 pip3 install audible-series
 ```
 
-Sadly the audible-cli tool is not in pypi but is packaged, it's easiest to
-install via git:
-
-```
-git clone https://github.com/mkb79/audible-cli
-pip3 install ./audible-cli
-```
-
 ## Usage
 
 The command will work on an exported library file:
 
 ```
 audible library export
 audible series -l $PWD/library.csv -c $PWD/config.yaml
@@ -53,14 +50,15 @@
 
 This project uses poetry which wraps a bunch of tools like virtualenv.  The
 easiest way to run it for development is to clone this repository then run a
 poetry shell.
 
 ```
 poetry shell
+set -x AUDIBLE_PLUGIN_DIR $PWD/audible_series
 audible library export
 audible series -l $PWD/library.csv -c $PWD/config.yaml
 ```
 
 When developing the `--only_series` flag may be useful since it will filter the
 library to a single series.
```

