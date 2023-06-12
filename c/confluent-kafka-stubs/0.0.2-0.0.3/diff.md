# Comparing `tmp/confluent_kafka_stubs-0.0.2.tar.gz` & `tmp/confluent_kafka_stubs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluent_kafka_stubs-0.0.2.tar", max compression
+gzip compressed data, was "confluent_kafka_stubs-0.0.3.tar", max compression
```

## Comparing `confluent_kafka_stubs-0.0.2.tar` & `confluent_kafka_stubs-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11562 2023-06-11 14:52:08.988748 confluent_kafka_stubs-0.0.2/LICENSE
--rw-r--r--   0        0        0     1212 2023-06-12 14:40:44.304323 confluent_kafka_stubs-0.0.2/README.md
--rw-r--r--   0        0        0       40 2023-06-11 18:28:05.626894 confluent_kafka_stubs-0.0.2/confluent_kafka-stubs/__init__.pyi
--rw-r--r--   0        0        0    10833 2023-06-12 13:51:39.568426 confluent_kafka_stubs-0.0.2/confluent_kafka-stubs/cimpl.pyi
--rw-r--r--   0        0        0      743 2023-06-12 14:41:13.417517 confluent_kafka_stubs-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 confluent_kafka_stubs-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11562 2023-06-11 14:52:08.988748 confluent_kafka_stubs-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1346 2023-06-12 14:45:07.689908 confluent_kafka_stubs-0.0.3/README.md
+-rw-r--r--   0        0        0       40 2023-06-11 18:28:05.626894 confluent_kafka_stubs-0.0.3/confluent_kafka-stubs/__init__.pyi
+-rw-r--r--   0        0        0    12251 2023-06-12 15:41:59.200483 confluent_kafka_stubs-0.0.3/confluent_kafka-stubs/cimpl.pyi
+-rw-r--r--   0        0        0      743 2023-06-12 14:44:48.316643 confluent_kafka_stubs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2095 1970-01-01 00:00:00.000000 confluent_kafka_stubs-0.0.3/PKG-INFO
```

### Comparing `confluent_kafka_stubs-0.0.2/LICENSE` & `confluent_kafka_stubs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `confluent_kafka_stubs-0.0.2/README.md` & `confluent_kafka_stubs-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 
 The package can be installed from [PyPI](https://pypi.org/project/confluent-kafka-stubs/), and needs to be installed in a location that tools like `mypy` can access. In my experience, installing it as a user package works well, at least with `neovim` and the official `mypy` package on `Arch Linux`. You can install it as a user package as follows:
 
 ```bash
 pip install --user confluent-kafka-stubs
 ```
 
+## Updating
+
+The package can be updated like any other PyPI package.
+
+```bash
+pip install --user --upgrade confluent-kafka-stubs
+```
+
 ## Status
 
 This package should be considered a work in progress.
 
 In the `cimpl` module, I believe all constants have been ported along with the following classes or functions:
 
 - `KafkaError`: class
```

### Comparing `confluent_kafka_stubs-0.0.2/confluent_kafka-stubs/cimpl.pyi` & `confluent_kafka_stubs-0.0.3/confluent_kafka-stubs/cimpl.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -156,14 +156,77 @@
     UNKNOWN_TOPIC_OR_PART: int
     UNSTABLE_OFFSET_COMMIT: int
     UNSUPPORTED_COMPRESSION_TYPE: int
     UNSUPPORTED_FOR_MESSAGE_FORMAT: int
     UNSUPPORTED_SASL_MECHANISM: int
     UNSUPPORTED_VERSION: int
 
+    # Private class constants
+    _ALL_BROKERS_DOWN: int
+    _APPLICATION: int
+    _ASSIGNMENT_LOST: int
+    _ASSIGN_PARTITIONS: int
+    _AUTHENTICATION: int
+    _AUTO_OFFSET_RESET: int
+    _BAD_COMPRESSION: int
+    _BAD_MSG: int
+    _CONFLICT: int
+    _CRIT_SYS_RESOURCE: int
+    _DESTROY: int
+    _EXISTING_SUBSCRIPTION: int
+    _FAIL: int
+    _FATAL: int
+    _FENCED: int
+    _FS: int
+    _GAPLESS_GUARANTEE: int
+    _INCONSISTENT: int
+    _INTR: int
+    _INVALID_ARG: int
+    _INVALID_TYPE: int
+    _IN_PROGRESS: int
+    _ISR_INSUFF: int
+    _KEY_DESERIALIZATION: int
+    _KEY_SERIALIZATION: int
+    _LOG_TRUNCATION: int
+    _MAX_POLL_EXCEEDED: int
+    _MSG_TIMED_OUT: int
+    _NODE_UPDATE: int
+    _NOENT: int
+    _NOOP: int
+    _NOT_CONFIGURED: int
+    _NOT_IMPLEMENTED: int
+    _NO_OFFSET: int
+    _OUTDATED: int
+    _PARTIAL: int
+    _PARTITION_EOF: int
+    _PREV_IN_PROGRESS: int
+    _PURGE_INFLIGHT: int
+    _PURGE_QUEUE: int
+    _QUEUE_FULL: int
+    _READ_ONLY: int
+    _RESOLVE: int
+    _RETRY: int
+    _REVOKE_PARTITIONS: int
+    _SSL: int
+    _STATE: int
+    _TIMED_OUT: int
+    _TIMED_OUT_QUEUE: int
+    _TRANSPORT: int
+    _UNDERFLOW: int
+    _UNKNOWN_BROKER: int
+    _UNKNOWN_GROUP: int
+    _UNKNOWN_PARTITION: int
+    _UNKNOWN_PROTOCOL: int
+    _UNKNOWN_TOPIC: int
+    _UNSUPPORTED_FEATURE: int
+    _VALUE_DESERIALIZATION: int
+    _VALUE_SERIALIZATION: int
+    _WAIT_CACHE: int
+    _WAIT_COORD: int
+
     def __init__(
         self,
         error_code: int,
         reason: Optional[str] = None,
         fatal: bool = False,
         retriable: bool = False,
         txn_requires_abort: bool = False,
```

### Comparing `confluent_kafka_stubs-0.0.2/pyproject.toml` & `confluent_kafka_stubs-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confluent-kafka-stubs"
-version = "0.0.2"
+version = "0.0.3"
 description = "Stub files for confluent-kafka."
 authors = ["The Epic <theepic.dev.83@gmail.com>"]
 readme = "README.md"
 packages = [{include = "confluent_kafka-stubs"}]
 license = "Apache-2.0"
 repository = "https://gitlab.com/theepic-dev/confluent-kafka-stubs"
 keywords = ["kafka", "stubs", "types"]
```

### Comparing `confluent_kafka_stubs-0.0.2/PKG-INFO` & `confluent_kafka_stubs-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confluent-kafka-stubs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Stub files for confluent-kafka.
 Home-page: https://gitlab.com/theepic-dev/confluent-kafka-stubs
 License: Apache-2.0
 Keywords: kafka,stubs,types
 Author: The Epic
 Author-email: theepic.dev.83@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -28,14 +28,22 @@
 
 The package can be installed from [PyPI](https://pypi.org/project/confluent-kafka-stubs/), and needs to be installed in a location that tools like `mypy` can access. In my experience, installing it as a user package works well, at least with `neovim` and the official `mypy` package on `Arch Linux`. You can install it as a user package as follows:
 
 ```bash
 pip install --user confluent-kafka-stubs
 ```
 
+## Updating
+
+The package can be updated like any other PyPI package.
+
+```bash
+pip install --user --upgrade confluent-kafka-stubs
+```
+
 ## Status
 
 This package should be considered a work in progress.
 
 In the `cimpl` module, I believe all constants have been ported along with the following classes or functions:
 
 - `KafkaError`: class
```

