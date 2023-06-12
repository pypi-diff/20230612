# Comparing `tmp/mmuxer-0.5.2.tar.gz` & `tmp/mmuxer-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmuxer-0.5.2.tar", last modified: Sat Mar 11 12:18:00 2023, max compression
+gzip compressed data, was "mmuxer-0.5.3.tar", last modified: Mon Jun 12 16:59:49 2023, max compression
```

## Comparing `mmuxer-0.5.2.tar` & `mmuxer-0.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:18:00.739413 mmuxer-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-11 12:17:54.000000 mmuxer-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-11 12:18:00.739413 mmuxer-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-03-11 12:17:54.000000 mmuxer-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:18:00.735413 mmuxer-0.5.2/mmuxer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:18:00.735413 mmuxer-0.5.2/mmuxer/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/cli/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/cli/sieve_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/config_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:18:00.739413 mmuxer-0.5.2/mmuxer/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/script.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/models/sieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-11 12:17:54.000000 mmuxer-0.5.2/mmuxer/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 12:18:00.735413 mmuxer-0.5.2/mmuxer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-11 12:18:00.000000 mmuxer-0.5.2/mmuxer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-11 12:18:00.000000 mmuxer-0.5.2/mmuxer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 12:18:00.000000 mmuxer-0.5.2/mmuxer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-11 12:18:00.000000 mmuxer-0.5.2/mmuxer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-11 12:18:00.000000 mmuxer-0.5.2/mmuxer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-11 12:18:00.000000 mmuxer-0.5.2/mmuxer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-11 12:17:58.000000 mmuxer-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 12:18:00.739413 mmuxer-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-11 12:17:54.000000 mmuxer-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:49.502391 mmuxer-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-12 16:59:42.000000 mmuxer-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 16:59:49.502391 mmuxer-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-12 16:59:42.000000 mmuxer-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:49.502391 mmuxer-0.5.3/mmuxer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:49.502391 mmuxer-0.5.3/mmuxer/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/cli/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/cli/sieve_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/config_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:49.502391 mmuxer-0.5.3/mmuxer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/models/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-12 16:59:42.000000 mmuxer-0.5.3/mmuxer/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:59:49.502391 mmuxer-0.5.3/mmuxer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 16:59:49.000000 mmuxer-0.5.3/mmuxer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-12 16:59:49.000000 mmuxer-0.5.3/mmuxer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:59:49.000000 mmuxer-0.5.3/mmuxer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 16:59:49.000000 mmuxer-0.5.3/mmuxer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 16:59:49.000000 mmuxer-0.5.3/mmuxer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 16:59:49.000000 mmuxer-0.5.3/mmuxer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-12 16:59:46.000000 mmuxer-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:59:49.502391 mmuxer-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 16:59:42.000000 mmuxer-0.5.3/setup.py
```

### Comparing `mmuxer-0.5.2/LICENSE` & `mmuxer-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/PKG-INFO` & `mmuxer-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mmuxer
-Version: 0.5.2
+Version: 0.5.3
 Summary: Manage mail from your server.
 Author-email: Mathias Millet <mathias@mmill.eu>
 License: AGPL-3.0
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: systemd
 License-File: LICENSE
 
 # Mail Muxer
 
 ![cover](assets/cover.png)
 
 Are you tired of managing IMAP filters through cumbersome, slow and unintuive web interfaces ? Then Mail Muxer is here to save you from this pain !
```

### Comparing `mmuxer-0.5.2/README.md` & `mmuxer-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/__main__.py` & `mmuxer-0.5.3/mmuxer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import enum
 import logging
 import os
 from pathlib import Path
+from typing import Optional
 
 import typer
 from rich.logging import RichHandler
 from rich.pretty import pprint
 from typer.core import TyperGroup
 
 from .cli.folder import app as folder_app
@@ -25,16 +26,23 @@
 class LogLevel(enum.Enum):
     DEBUG = "debug"
     INFO = "info"
     WARNING = "warning"
     ERROR = "error"
 
 
-def main_callback(log_level: LogLevel = typer.Option("info", case_sensitive=False)):
-    if os.isatty(0):
+def main_callback(
+    log_level: LogLevel = typer.Option("info", case_sensitive=False),
+    journald_logger: Optional[str] = typer.Option(None, help="Log to journald instead of stdout"),
+):
+    if journald_logger:
+        from cysystemd import journal
+
+        handler = journal.JournaldLogHandler(identifier=journald_logger)
+    elif os.isatty(0):
         handler = RichHandler(
             rich_tracebacks=True, show_time=False, show_path=(log_level == LogLevel.DEBUG)
         )
     else:
         handler = logging.StreamHandler()
         formatter = logging.Formatter("%(levelname)s - %(message)s")
         handler.setFormatter(formatter)
```

### Comparing `mmuxer-0.5.2/mmuxer/cli/folder.py` & `mmuxer-0.5.3/mmuxer/cli/folder.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/cli/run.py` & `mmuxer-0.5.3/mmuxer/cli/run.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/cli/sieve_export.py` & `mmuxer-0.5.3/mmuxer/cli/sieve_export.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/config_state.py` & `mmuxer-0.5.3/mmuxer/config_state.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/models/action.py` & `mmuxer-0.5.3/mmuxer/models/action.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/models/condition.py` & `mmuxer-0.5.3/mmuxer/models/condition.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/models/enums.py` & `mmuxer-0.5.3/mmuxer/models/enums.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/models/rule.py` & `mmuxer-0.5.3/mmuxer/models/rule.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/models/script.py` & `mmuxer-0.5.3/mmuxer/models/script.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/models/settings.py` & `mmuxer-0.5.3/mmuxer/models/settings.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/models/sieve.py` & `mmuxer-0.5.3/mmuxer/models/sieve.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/utils.py` & `mmuxer-0.5.3/mmuxer/utils.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer/workers.py` & `mmuxer-0.5.3/mmuxer/workers.py`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/mmuxer.egg-info/PKG-INFO` & `mmuxer-0.5.3/mmuxer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: mmuxer
-Version: 0.5.2
+Version: 0.5.3
 Summary: Manage mail from your server.
 Author-email: Mathias Millet <mathias@mmill.eu>
 License: AGPL-3.0
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: systemd
 License-File: LICENSE
 
 # Mail Muxer
 
 ![cover](assets/cover.png)
 
 Are you tired of managing IMAP filters through cumbersome, slow and unintuive web interfaces ? Then Mail Muxer is here to save you from this pain !
```

### Comparing `mmuxer-0.5.2/mmuxer.egg-info/SOURCES.txt` & `mmuxer-0.5.3/mmuxer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmuxer-0.5.2/pyproject.toml` & `mmuxer-0.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mmuxer"
-version = "0.5.2"
+version = "0.5.3"
 description = "Manage mail from your server."
 authors = [
     {name = "Mathias Millet", email="mathias@mmill.eu"},
 ]
 license = {text = "AGPL-3.0"}
 readme = "README.md"
 requires-python = ">=3.8"
@@ -37,14 +37,18 @@
 dev = [
     "pytest >= 7.0",
     "pre-commit >= 2.0",
     "pytest-bg-process",
     "pytz",
 ]
 
+systemd = [
+     "cysystemd >= 1.5.0"
+]
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["mmuxer*"]
 
 [tool.pytest.ini_options]
```

