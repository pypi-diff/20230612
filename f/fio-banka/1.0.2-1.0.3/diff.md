# Comparing `tmp/fio_banka-1.0.2.tar.gz` & `tmp/fio_banka-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio_banka-1.0.2.tar", last modified: Sun Jun 11 17:44:34 2023, max compression
+gzip compressed data, was "fio_banka-1.0.3.tar", last modified: Mon Jun 12 19:05:16 2023, max compression
```

## Comparing `fio_banka-1.0.2.tar` & `fio_banka-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:44:34.596285 fio_banka-1.0.2/
--rw-r--r--   0 petr      (1000) petr      (1000)     1069 2023-06-09 11:17:31.000000 fio_banka-1.0.2/LICENSE
--rw-r--r--   0 petr      (1000) petr      (1000)     5588 2023-06-11 17:44:34.595286 fio_banka-1.0.2/PKG-INFO
--rw-r--r--   0 petr      (1000) petr      (1000)     3584 2023-06-11 17:40:12.000000 fio_banka-1.0.2/README.md
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:44:34.595286 fio_banka-1.0.2/fio_banka.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     5588 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/PKG-INFO
--rw-r--r--   0 petr      (1000) petr      (1000)      233 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/SOURCES.txt
--rw-r--r--   0 petr      (1000) petr      (1000)        1 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/dependency_links.txt
--rw-r--r--   0 petr      (1000) petr      (1000)      125 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/requires.txt
--rw-r--r--   0 petr      (1000) petr      (1000)       10 2023-06-11 17:44:34.000000 fio_banka-1.0.2/fio_banka.egg-info/top_level.txt
--rw-r--r--   0 petr      (1000) petr      (1000)    11902 2023-06-09 11:30:08.000000 fio_banka-1.0.2/fio_banka.py
--rw-r--r--   0 petr      (1000) petr      (1000)     2153 2023-06-11 17:40:12.000000 fio_banka-1.0.2/pyproject.toml
--rw-r--r--   0 petr      (1000) petr      (1000)       38 2023-06-11 17:44:34.596285 fio_banka-1.0.2/setup.cfg
-drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-11 17:44:34.595286 fio_banka-1.0.2/tests/
--rw-r--r--   0 petr      (1000) petr      (1000)     9507 2023-06-09 11:30:08.000000 fio_banka-1.0.2/tests/test_fio_banka.py
+drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-12 19:05:16.724821 fio_banka-1.0.3/
+-rw-r--r--   0 petr      (1000) petr      (1000)     1069 2023-06-02 13:39:45.000000 fio_banka-1.0.3/LICENSE
+-rw-r--r--   0 petr      (1000) petr      (1000)     6016 2023-06-12 19:05:16.724821 fio_banka-1.0.3/PKG-INFO
+-rw-r--r--   0 petr      (1000) petr      (1000)     4009 2023-06-12 19:00:13.000000 fio_banka-1.0.3/README.md
+drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-12 19:05:16.723821 fio_banka-1.0.3/fio_banka.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     6016 2023-06-12 19:05:16.000000 fio_banka-1.0.3/fio_banka.egg-info/PKG-INFO
+-rw-r--r--   0 petr      (1000) petr      (1000)      233 2023-06-12 19:05:16.000000 fio_banka-1.0.3/fio_banka.egg-info/SOURCES.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)        1 2023-06-12 19:05:16.000000 fio_banka-1.0.3/fio_banka.egg-info/dependency_links.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)      155 2023-06-12 19:05:16.000000 fio_banka-1.0.3/fio_banka.egg-info/requires.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)       10 2023-06-12 19:05:16.000000 fio_banka-1.0.3/fio_banka.egg-info/top_level.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)    11902 2023-06-12 18:20:12.000000 fio_banka-1.0.3/fio_banka.py
+-rw-r--r--   0 petr      (1000) petr      (1000)     2186 2023-06-12 19:00:13.000000 fio_banka-1.0.3/pyproject.toml
+-rw-r--r--   0 petr      (1000) petr      (1000)       38 2023-06-12 19:05:16.724821 fio_banka-1.0.3/setup.cfg
+drwxr-xr-x   0 petr      (1000) petr      (1000)        0 2023-06-12 19:05:16.724821 fio_banka-1.0.3/tests/
+-rw-r--r--   0 petr      (1000) petr      (1000)     9507 2023-06-12 18:20:12.000000 fio_banka-1.0.3/tests/test_fio_banka.py
```

### Comparing `fio_banka-1.0.2/LICENSE` & `fio_banka-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fio_banka-1.0.2/PKG-INFO` & `fio_banka-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio_banka
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thin wrapper for Fio Banka, a.s. API
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Petr Beranek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,30 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/peberanek/fio-banka
 Keywords: finance,fio,bank,api,czech,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: distribution
 License-File: LICENSE
 
-# Fio Banka API Wrapper
+# Fio Banka API
 
+[![image](https://img.shields.io/pypi/v/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://img.shields.io/pypi/l/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://img.shields.io/pypi/pyversions/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://github.com/peberanek/fio-banka/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/fio-banka/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/fio-banka/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/fio-banka/main)
 
 Thin wrapper for [Fio Banka, a.s. API](https://www.fio.cz/bank-services/internetbanking-api). Inspired by Honza Javorek's [fiobank](https://github.com/honzajavorek/fiobank).
 
 ## Description
 
 This wrapper is intentionally simple. It does not limit the user by any specific data processing, data structures or error handling. Instead, it returns data as-is, i.e. in a text or a binary format. So the user can handle the processing, errors, data validation or more complex stuff (like caching) according to their needs. A couple of helper functions for data extraction are included nonetheless (see the [Usage](#usage) section below).
```

### Comparing `fio_banka-1.0.2/README.md` & `fio_banka-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-# Fio Banka API Wrapper
+# Fio Banka API
 
+[![image](https://img.shields.io/pypi/v/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://img.shields.io/pypi/l/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://img.shields.io/pypi/pyversions/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://github.com/peberanek/fio-banka/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/fio-banka/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/fio-banka/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/fio-banka/main)
 
 Thin wrapper for [Fio Banka, a.s. API](https://www.fio.cz/bank-services/internetbanking-api). Inspired by Honza Javorek's [fiobank](https://github.com/honzajavorek/fiobank).
 
 ## Description
 
 This wrapper is intentionally simple. It does not limit the user by any specific data processing, data structures or error handling. Instead, it returns data as-is, i.e. in a text or a binary format. So the user can handle the processing, errors, data validation or more complex stuff (like caching) according to their needs. A couple of helper functions for data extraction are included nonetheless (see the [Usage](#usage) section below).
```

### Comparing `fio_banka-1.0.2/fio_banka.egg-info/PKG-INFO` & `fio_banka-1.0.3/fio_banka.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-banka
-Version: 1.0.2
+Version: 1.0.3
 Summary: Thin wrapper for Fio Banka, a.s. API
 Author-email: Petr Beranek <petrberanek.mail@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Petr Beranek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,26 +26,30 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/peberanek/fio-banka
 Keywords: finance,fio,bank,api,czech,wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: distribution
 License-File: LICENSE
 
-# Fio Banka API Wrapper
+# Fio Banka API
 
+[![image](https://img.shields.io/pypi/v/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://img.shields.io/pypi/l/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://img.shields.io/pypi/pyversions/fio-banka)](https://pypi.org/project/fio-banka/)
+[![image](https://github.com/peberanek/fio-banka/actions/workflows/tests.yml/badge.svg)](https://github.com/peberanek/fio-banka/actions/workflows/tests.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/peberanek/fio-banka/main.svg)](https://results.pre-commit.ci/latest/github/peberanek/fio-banka/main)
 
 Thin wrapper for [Fio Banka, a.s. API](https://www.fio.cz/bank-services/internetbanking-api). Inspired by Honza Javorek's [fiobank](https://github.com/honzajavorek/fiobank).
 
 ## Description
 
 This wrapper is intentionally simple. It does not limit the user by any specific data processing, data structures or error handling. Instead, it returns data as-is, i.e. in a text or a binary format. So the user can handle the processing, errors, data validation or more complex stuff (like caching) according to their needs. A couple of helper functions for data extraction are included nonetheless (see the [Usage](#usage) section below).
```

### Comparing `fio_banka-1.0.2/fio_banka.py` & `fio_banka-1.0.3/fio_banka.py`

 * *Files identical despite different names*

### Comparing `fio_banka-1.0.2/pyproject.toml` & `fio_banka-1.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fio_banka"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name = "Petr Beranek", email = "petrberanek.mail@gmail.com" },
 ]
 description = "Thin wrapper for Fio Banka, a.s. API"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 keywords = ["finance", "fio", "bank", "api", "czech", "wrapper"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Intended Audience :: Financial and Insurance Industry",
-  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Topic :: Communications",
   "Topic :: Office/Business :: Financial",
 ]
 dependencies = [
-  "requests==2.31.0",
+  "requests>=2.31.0,<3.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/peberanek/fio-banka"
 
 [project.optional-dependencies]
 development = [
-  "pre-commit==3.3.1",
-  "pytest==7.3.1",
-  "pytest-cov==4.1.0",
+  "pre-commit>=3.3.1,<4.0",
+  "pytest>=7.3.1,<8.0",
+  "pytest-cov>=4.1.0,<5.0",
 ]
 distribution = [
-  "build==0.10.0",
-  "twine==4.0.2",
+  "build>=0.10.0,<1.0",
+  "twine>=4.0.2,<5.0",
 ]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--cov=fio_banka --cov-report term-missing"
 
 [tool.ruff]
```

### Comparing `fio_banka-1.0.2/tests/test_fio_banka.py` & `fio_banka-1.0.3/tests/test_fio_banka.py`

 * *Files identical despite different names*

