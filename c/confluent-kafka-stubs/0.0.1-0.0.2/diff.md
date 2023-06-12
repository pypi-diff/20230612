# Comparing `tmp/confluent_kafka_stubs-0.0.1.tar.gz` & `tmp/confluent_kafka_stubs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluent_kafka_stubs-0.0.1.tar", max compression
+gzip compressed data, was "confluent_kafka_stubs-0.0.2.tar", max compression
```

## Comparing `confluent_kafka_stubs-0.0.1.tar` & `confluent_kafka_stubs-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11562 2023-06-11 14:52:08.988748 confluent_kafka_stubs-0.0.1/LICENSE
--rw-r--r--   0        0        0      791 2023-06-12 13:59:22.939382 confluent_kafka_stubs-0.0.1/README.md
--rw-r--r--   0        0        0       40 2023-06-11 18:28:05.626894 confluent_kafka_stubs-0.0.1/confluent_kafka-stubs/__init__.pyi
--rw-r--r--   0        0        0    10833 2023-06-12 13:51:39.568426 confluent_kafka_stubs-0.0.1/confluent_kafka-stubs/cimpl.pyi
--rw-r--r--   0        0        0      743 2023-06-12 14:09:51.140170 confluent_kafka_stubs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 confluent_kafka_stubs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11562 2023-06-11 14:52:08.988748 confluent_kafka_stubs-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1212 2023-06-12 14:40:44.304323 confluent_kafka_stubs-0.0.2/README.md
+-rw-r--r--   0        0        0       40 2023-06-11 18:28:05.626894 confluent_kafka_stubs-0.0.2/confluent_kafka-stubs/__init__.pyi
+-rw-r--r--   0        0        0    10833 2023-06-12 13:51:39.568426 confluent_kafka_stubs-0.0.2/confluent_kafka-stubs/cimpl.pyi
+-rw-r--r--   0        0        0      743 2023-06-12 14:41:13.417517 confluent_kafka_stubs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 confluent_kafka_stubs-0.0.2/PKG-INFO
```

### Comparing `confluent_kafka_stubs-0.0.1/LICENSE` & `confluent_kafka_stubs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `confluent_kafka_stubs-0.0.1/confluent_kafka-stubs/cimpl.pyi` & `confluent_kafka_stubs-0.0.2/confluent_kafka-stubs/cimpl.pyi`

 * *Files identical despite different names*

### Comparing `confluent_kafka_stubs-0.0.1/pyproject.toml` & `confluent_kafka_stubs-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confluent-kafka-stubs"
-version = "0.0.1"
+version = "0.0.2"
 description = "Stub files for confluent-kafka."
 authors = ["The Epic <theepic.dev.83@gmail.com>"]
 readme = "README.md"
 packages = [{include = "confluent_kafka-stubs"}]
 license = "Apache-2.0"
 repository = "https://gitlab.com/theepic-dev/confluent-kafka-stubs"
 keywords = ["kafka", "stubs", "types"]
```

### Comparing `confluent_kafka_stubs-0.0.1/PKG-INFO` & `confluent_kafka_stubs-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluent-kafka-stubs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Stub files for confluent-kafka.
 Home-page: https://gitlab.com/theepic-dev/confluent-kafka-stubs
 License: Apache-2.0
 Keywords: kafka,stubs,types
 Author: The Epic
 Author-email: theepic.dev.83@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -20,14 +20,22 @@
 
 # confluent-kafka-stubs
 
 This package only contains type hints for the `confluent-kafka` python package. It may be useful to add type checking for `mypy`, or autocompletion in your *language server*.
 
 This package is not endorsed by Confluent.
 
+## Installation
+
+The package can be installed from [PyPI](https://pypi.org/project/confluent-kafka-stubs/), and needs to be installed in a location that tools like `mypy` can access. In my experience, installing it as a user package works well, at least with `neovim` and the official `mypy` package on `Arch Linux`. You can install it as a user package as follows:
+
+```bash
+pip install --user confluent-kafka-stubs
+```
+
 ## Status
 
 This package should be considered a work in progress.
 
 In the `cimpl` module, I believe all constants have been ported along with the following classes or functions:
 
 - `KafkaError`: class
```

