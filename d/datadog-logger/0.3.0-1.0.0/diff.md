# Comparing `tmp/datadog-logger-0.3.0.tar.gz` & `tmp/datadog_logger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datadog-logger-0.3.0.tar", last modified: Wed Dec  5 14:26:29 2018, max compression
+gzip compressed data, was "datadog_logger-1.0.0.tar", max compression
```

## Comparing `datadog-logger-0.3.0.tar` & `datadog_logger-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2018-12-05 14:26:29.000000 datadog-logger-0.3.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      276 2018-12-05 14:26:23.000000 datadog-logger-0.3.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2018-12-05 14:26:29.000000 datadog-logger-0.3.0/datadog_logger/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      260 2018-12-05 14:26:23.000000 datadog-logger-0.3.0/datadog_logger/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      977 2018-12-05 14:26:23.000000 datadog-logger-0.3.0/datadog_logger/handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      256 2018-12-05 14:26:29.000000 datadog-logger-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-12 15:27:50.021322 datadog_logger-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2340 2023-06-12 15:27:50.021322 datadog_logger-1.0.0/README.md
+-rw-r--r--   0        0        0      414 2023-06-12 15:27:50.021322 datadog_logger-1.0.0/datadog_logger/__init__.py
+-rw-r--r--   0        0        0     1228 2023-06-12 15:27:50.021322 datadog_logger-1.0.0/datadog_logger/handler.py
+-rw-r--r--   0        0        0        0 2023-06-12 15:27:50.021322 datadog_logger-1.0.0/datadog_logger/py.typed
+-rw-r--r--   0        0        0      483 2023-06-12 15:27:50.021322 datadog_logger-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2882 1970-01-01 00:00:00.000000 datadog_logger-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datadog-logger-0.3.0/datadog_logger/handler.py` & `datadog_logger-1.0.0/datadog_logger/handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,45 @@
-import datadog
-
+from collections.abc import Iterable
+from datadog.api.events import Event
 import logging
+from typing import Any, Optional
 
 
 LOG_LEVEL_ALERT_TYPE_MAPPINGS = {
     logging.DEBUG: "info",
     logging.INFO: "info",
     logging.WARNING: "warning",
     logging.ERROR: "error",
     logging.CRITICAL: "error"
 }
 
 
 class DatadogLogHandler(logging.Handler):
-    def __init__(self, tags=None, mentions=None, **kwargs):
+    def __init__(
+        self,
+        tags: Optional[list[str]] = None,
+        mentions: Optional[Iterable[str]] = None,
+        **kwargs: Any
+    ):
         super(DatadogLogHandler, self).__init__(**kwargs)
 
         self.tags = tags
         self.mentions = mentions
 
-    def emit(self, record):
+    def emit(self, record: logging.LogRecord) -> None:
         text = self.format(record)
 
         if self.mentions is not None:
             text = "\n\n".join([text, " ".join(self.mentions)])
 
-        create_args = {
+        create_args: dict[str, object] = {
             "title": record.getMessage(),
             "text": text
         }
 
         if self.tags is not None:
             create_args["tags"] = self.tags
 
         if record.levelno in LOG_LEVEL_ALERT_TYPE_MAPPINGS:
             create_args["alert_type"] = LOG_LEVEL_ALERT_TYPE_MAPPINGS[record.levelno]
 
-        datadog.api.Event.create(**create_args)
+        Event.create(**create_args)  # type: ignore[no-untyped-call]
```

