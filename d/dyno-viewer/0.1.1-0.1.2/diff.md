# Comparing `tmp/dyno_viewer-0.1.1.tar.gz` & `tmp/dyno_viewer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyno_viewer-0.1.1.tar", max compression
+gzip compressed data, was "dyno_viewer-0.1.2.tar", max compression
```

## Comparing `dyno_viewer-0.1.1.tar` & `dyno_viewer-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-06-03 06:45:19.613704 dyno_viewer-0.1.1/LICENSE
--rw-r--r--   0        0        0     3812 2023-06-03 06:45:19.613704 dyno_viewer-0.1.1/README.md
--rw-r--r--   0        0        0       58 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/__main__.py
--rw-r--r--   0        0        0     5875 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/app.py
--rw-r--r--   0        0        0     2256 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/app_workers.py
--rw-r--r--   0        0        0     7792 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/aws/ddb.py
--rw-r--r--   0        0        0      211 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/aws/session.py
--rw-r--r--   0        0        0      612 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/css/query.css
--rw-r--r--   0        0        0       38 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/css/table.css
--rw-r--r--   0        0        0     2233 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/query/filter_query.py
--rw-r--r--   0        0        0     2850 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/query/key_query.py
--rw-r--r--   0        0        0     2057 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/query/sort_key_filter.py
--rw-r--r--   0        0        0      129 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/screens/__init__.py
--rw-r--r--   0        0        0      794 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/screens/error.py
--rw-r--r--   0        0        0      912 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/screens/profile_select.py
--rw-r--r--   0        0        0     5129 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/screens/query.py
--rw-r--r--   0        0        0      857 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/screens/region_select.py
--rw-r--r--   0        0        0     3323 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/screens/table_select.py
--rw-r--r--   0        0        0     1852 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/table.py
--rw-r--r--   0        0        0      181 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/components/types.py
--rw-r--r--   0        0        0       20 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/util/__init__.py
--rw-r--r--   0        0        0      166 2023-06-03 06:45:19.617704 dyno_viewer-0.1.1/dyno_viewer/util/util.py
--rw-r--r--   0        0        0     1045 2023-06-03 06:45:19.621704 dyno_viewer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4371 1970-01-01 00:00:00.000000 dyno_viewer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-12 00:03:14.308979 dyno_viewer-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3909 2023-06-12 00:03:14.308979 dyno_viewer-0.1.2/README.md
+-rw-r--r--   0        0        0       58 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/__main__.py
+-rw-r--r--   0        0        0     5875 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/app.py
+-rw-r--r--   0        0        0     2256 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/app_workers.py
+-rw-r--r--   0        0        0     7792 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/aws/ddb.py
+-rw-r--r--   0        0        0      211 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/aws/session.py
+-rw-r--r--   0        0        0      612 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/css/query.css
+-rw-r--r--   0        0        0       38 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/css/table.css
+-rw-r--r--   0        0        0     2233 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/query/filter_query.py
+-rw-r--r--   0        0        0     2850 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/query/key_query.py
+-rw-r--r--   0        0        0     2057 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/query/sort_key_filter.py
+-rw-r--r--   0        0        0      129 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/error.py
+-rw-r--r--   0        0        0      912 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/profile_select.py
+-rw-r--r--   0        0        0     5129 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/query.py
+-rw-r--r--   0        0        0      857 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/region_select.py
+-rw-r--r--   0        0        0     3323 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/screens/table_select.py
+-rw-r--r--   0        0        0     1852 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/table.py
+-rw-r--r--   0        0        0      181 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/components/types.py
+-rw-r--r--   0        0        0       20 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/util/__init__.py
+-rw-r--r--   0        0        0      166 2023-06-12 00:03:14.312980 dyno_viewer-0.1.2/dyno_viewer/util/util.py
+-rw-r--r--   0        0        0     1119 2023-06-12 00:03:14.316980 dyno_viewer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 dyno_viewer-0.1.2/PKG-INFO
```

### Comparing `dyno_viewer-0.1.1/LICENSE` & `dyno_viewer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/README.md` & `dyno_viewer-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 flatpak install <bundled .flatpak filename>
 ```
 
 ## Dev notes
 
 ### Prerequisites
 
-This repo uses [poetry](https://python-poetry.org/docs/) for package management and needs python 3.10.7 installed either via [pyenv](https://github.com/pyenv/pyenv)
+This repo uses [poetry](https://python-poetry.org/docs/) for package management and needs python 3.10.11 installed either via [pyenv](https://github.com/pyenv/pyenv)
 or [asdf](https://asdf-vm.com/) using the [asdf-community/asdf-python](https://github.com/asdf-community/asdf-python) addon
 
 
 ```bash
-env PYTHON_CONFIGURE_OPTS="--enable-shared" asdf install python 3.10.7
+env PYTHON_CONFIGURE_OPTS="--enable-shared" asdf install python 3.10.11
 ```
 or if using pyenv:
 
 ```bash
-env PYTHON_CONFIGURE_OPTS="--enable-shared" pyenv install 3.10.7
+env PYTHON_CONFIGURE_OPTS="--enable-shared" pyenv install 3.10.11
 ```
 
 see [how to build cpython with --enable-shared](https://github.com/pyenv/pyenv/wiki#how-to-build-cpython-with---enable-shared) for more info
 
 ### Local dev setup
 
 To install locally run:
@@ -70,42 +70,42 @@
 ### Testing textual notes
 
 See [testing notes doc](docs/testing-textual.md)
 
 
 ### Flatpak notes
 
-This repo supports local flatpak building to make the process easy there is a script that builds the flatpak, Which are loosely created from this really useful [blog post](https://www.loganasherjones.com/2018/05/using-flatpak-with-python/). To run call:
+This repo supports local flatpak building to make the process easy there is a script that builds the flatpak, Which are loosely created from this really useful [blog post](https://www.loganasherjones.com/2018/05/using-flatpak-with-python/). To run call via [poe](https://poethepoet.natn.io/index.html) (a script runner for poetry):
 
 ```bash
-poetry run flatpak_build
+poetry run poe flatpak_build
 ```
 
 This will export the main packages into a requirements file and then build flatpak in the `.flatpak` folder then export that flatpak to a binary file in root called `dyno-viewer.flatpak` which can be installed on another computer via `flatpak install dyno-viewer.flatpak`
 
 It also has support for doing other different options via arguments:
 
 #### Install locally
 
 ``` bash
-poetry run flatpak_build -i 
+poetry run poe flatpak_build -i 
 ```
 
 This will install the flatpak locally instead of exporting it to a file (Useful for dev testing), Which then you can run it via:
 
 ```bash
 flatpak run org.flatpak.dyno-viewer
 ```
 
 #### Gpg key support
 
 You can pass a gpg key for signing a flatpak, Which is best practice (see more on that [here](https://docs.flatpak.org/en/latest/flatpak-builder.html#signing)) via:
 
 ```bash
-poetry run flatpak_build --gpg "<key id>"
+poetry run poe flatpak_build --gpg "<key id>"
 ```
 
 If the gpg key is not in the default directory then you can also add the path to it via this argument:
 
 ```bash 
-poetry run flatpak_build --gpg "<key id>" --gh path/to/gpg/key
+poetry run poe flatpak_build --gpg "<key id>" --gh path/to/gpg/key
 ```
```

### Comparing `dyno_viewer-0.1.1/dyno_viewer/app.py` & `dyno_viewer-0.1.2/dyno_viewer/app.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/app_workers.py` & `dyno_viewer-0.1.2/dyno_viewer/app_workers.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/aws/ddb.py` & `dyno_viewer-0.1.2/dyno_viewer/aws/ddb.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/css/query.css` & `dyno_viewer-0.1.2/dyno_viewer/components/css/query.css`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/query/filter_query.py` & `dyno_viewer-0.1.2/dyno_viewer/components/query/filter_query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/query/key_query.py` & `dyno_viewer-0.1.2/dyno_viewer/components/query/key_query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/query/sort_key_filter.py` & `dyno_viewer-0.1.2/dyno_viewer/components/query/sort_key_filter.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/screens/error.py` & `dyno_viewer-0.1.2/dyno_viewer/components/screens/error.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/screens/profile_select.py` & `dyno_viewer-0.1.2/dyno_viewer/components/screens/profile_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/screens/query.py` & `dyno_viewer-0.1.2/dyno_viewer/components/screens/query.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/screens/region_select.py` & `dyno_viewer-0.1.2/dyno_viewer/components/screens/region_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/screens/table_select.py` & `dyno_viewer-0.1.2/dyno_viewer/components/screens/table_select.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/dyno_viewer/components/table.py` & `dyno_viewer-0.1.2/dyno_viewer/components/table.py`

 * *Files identical despite different names*

### Comparing `dyno_viewer-0.1.1/pyproject.toml` & `dyno_viewer-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 [tool.poetry]
 name = "dyno-viewer"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Rowan Self <piesrule123@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dyno_viewer"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.26.135"
 simplejson = "^3.19.1"
 dynamodb-json = "^1.3"
-textual = "^0.24.1"
+textual = ">=0.24.1,<0.28.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ipykernel = "^6.22.0"
-textual = {extras = ["dev"], version = "^0.24.1"}
+textual = {extras = ["dev"], version = ">=0.24.1,<0.28.0"}
 pytest = "^7.3.1"
 moto = {extras = ["all"], version = "^4.1.9"}
 pytest-aiohttp = "^1.0.4"
 pandas = "^1.5.3"
 pytest-mock = "^3.10.0"
 jupyterlab = "^3.6.3"
 pytest-xdist = "^3.3.0"
 toml = "^0.10.2"
 pyinstaller = {version = "^5.11.0", python = ">=3.9,<3.12"}
+poethepoet = "^0.20.0"
 
 
 
 [tool.poetry.group.build.dependencies]
 
+[tool.poe.tasks]
+build_local.script = 'scripts.commands:build_local'
+flatpak_build.script = 'scripts.commands:build_flatpak'
+
+
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = ["tests"]
 
 [tool.poetry.scripts]
 dyno-viewer  = 'dyno_viewer.app:run'
-build_local = 'scripts.commands:build_local'
-flatpak_build = 'scripts.commands:build_flatpak'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dyno_viewer-0.1.1/PKG-INFO` & `dyno_viewer-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dyno-viewer
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Rowan Self
 Author-email: piesrule123@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.135,<2.0.0)
 Requires-Dist: dynamodb-json (>=1.3,<2.0)
 Requires-Dist: simplejson (>=3.19.1,<4.0.0)
-Requires-Dist: textual (>=0.24.1,<0.25.0)
+Requires-Dist: textual (>=0.24.1,<0.28.0)
 Description-Content-Type: text/markdown
 
 ![screenshot](dyno-viewer-screenshot.png)
 # Dyno-viewer
 
 Dyno-viewer is dynamodb table viewer for your terminal build using [textual](https://github.com/Textualize/textual). 
 
@@ -54,25 +54,25 @@
 flatpak install <bundled .flatpak filename>
 ```
 
 ## Dev notes
 
 ### Prerequisites
 
-This repo uses [poetry](https://python-poetry.org/docs/) for package management and needs python 3.10.7 installed either via [pyenv](https://github.com/pyenv/pyenv)
+This repo uses [poetry](https://python-poetry.org/docs/) for package management and needs python 3.10.11 installed either via [pyenv](https://github.com/pyenv/pyenv)
 or [asdf](https://asdf-vm.com/) using the [asdf-community/asdf-python](https://github.com/asdf-community/asdf-python) addon
 
 
 ```bash
-env PYTHON_CONFIGURE_OPTS="--enable-shared" asdf install python 3.10.7
+env PYTHON_CONFIGURE_OPTS="--enable-shared" asdf install python 3.10.11
 ```
 or if using pyenv:
 
 ```bash
-env PYTHON_CONFIGURE_OPTS="--enable-shared" pyenv install 3.10.7
+env PYTHON_CONFIGURE_OPTS="--enable-shared" pyenv install 3.10.11
 ```
 
 see [how to build cpython with --enable-shared](https://github.com/pyenv/pyenv/wiki#how-to-build-cpython-with---enable-shared) for more info
 
 ### Local dev setup
 
 To install locally run:
@@ -87,43 +87,43 @@
 ### Testing textual notes
 
 See [testing notes doc](docs/testing-textual.md)
 
 
 ### Flatpak notes
 
-This repo supports local flatpak building to make the process easy there is a script that builds the flatpak, Which are loosely created from this really useful [blog post](https://www.loganasherjones.com/2018/05/using-flatpak-with-python/). To run call:
+This repo supports local flatpak building to make the process easy there is a script that builds the flatpak, Which are loosely created from this really useful [blog post](https://www.loganasherjones.com/2018/05/using-flatpak-with-python/). To run call via [poe](https://poethepoet.natn.io/index.html) (a script runner for poetry):
 
 ```bash
-poetry run flatpak_build
+poetry run poe flatpak_build
 ```
 
 This will export the main packages into a requirements file and then build flatpak in the `.flatpak` folder then export that flatpak to a binary file in root called `dyno-viewer.flatpak` which can be installed on another computer via `flatpak install dyno-viewer.flatpak`
 
 It also has support for doing other different options via arguments:
 
 #### Install locally
 
 ``` bash
-poetry run flatpak_build -i 
+poetry run poe flatpak_build -i 
 ```
 
 This will install the flatpak locally instead of exporting it to a file (Useful for dev testing), Which then you can run it via:
 
 ```bash
 flatpak run org.flatpak.dyno-viewer
 ```
 
 #### Gpg key support
 
 You can pass a gpg key for signing a flatpak, Which is best practice (see more on that [here](https://docs.flatpak.org/en/latest/flatpak-builder.html#signing)) via:
 
 ```bash
-poetry run flatpak_build --gpg "<key id>"
+poetry run poe flatpak_build --gpg "<key id>"
 ```
 
 If the gpg key is not in the default directory then you can also add the path to it via this argument:
 
 ```bash 
-poetry run flatpak_build --gpg "<key id>" --gh path/to/gpg/key
+poetry run poe flatpak_build --gpg "<key id>" --gh path/to/gpg/key
 ```
```

