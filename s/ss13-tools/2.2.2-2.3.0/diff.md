# Comparing `tmp/ss13_tools-2.2.2.tar.gz` & `tmp/ss13_tools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ss13_tools-2.2.2.tar", max compression
+gzip compressed data, was "ss13_tools-2.3.0.tar", max compression
```

## Comparing `ss13_tools-2.2.2.tar` & `ss13_tools-2.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2301 2023-04-20 17:41:38.728386 ss13_tools-2.2.2/README.md
--rw-r--r--   0        0        0     1008 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      325 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/__main__.py
--rw-r--r--   0        0        0       22 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/__version__.py
--rw-r--r--   0        0        0      438 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/auth/__init__.py
--rw-r--r--   0        0        0      205 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/auth/__main__.py
--rw-r--r--   0        0        0      346 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/auth/constants.py
--rw-r--r--   0        0        0    10698 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/auth/tg.py
--rw-r--r--   0        0        0      182 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/byond/__init__.py
--rw-r--r--   0        0        0      543 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/byond/__main__.py
--rw-r--r--   0        0        0       59 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/byond/constants.py
--rw-r--r--   0        0        0     2424 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/byond/key_tools.py
--rw-r--r--   0        0        0      162 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/centcom/__init__.py
--rw-r--r--   0        0        0     1099 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/centcom/__main__.py
--rw-r--r--   0        0        0      394 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/centcom/ban.py
--rw-r--r--   0        0        0     1492 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/centcom/ban_types.py
--rw-r--r--   0        0        0       68 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/centcom/constants.py
--rw-r--r--   0        0        0      614 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/cli.py
--rw-r--r--   0        0        0      222 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/constants.py
--rw-r--r--   0        0        0    18265 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/log_buddy/README.md
--rw-r--r--   0        0        0      198 2023-04-20 17:41:38.736386 ss13_tools-2.2.2/ss13_tools/log_buddy/__init__.py
--rw-r--r--   0        0        0     5561 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_buddy/__main__.py
--rw-r--r--   0        0        0      732 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_buddy/constants.py
--rw-r--r--   0        0        0      562 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_buddy/expressions.py
--rw-r--r--   0        0        0    50868 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_buddy/log.py
--rw-r--r--   0        0        0    17063 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_buddy/log_magics.py
--rw-r--r--   0        0        0    28400 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_buddy/log_parser.py
--rw-r--r--   0        0        0      554 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_downloader/__init__.py
--rw-r--r--   0        0        0     2011 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_downloader/__main__.py
--rw-r--r--   0        0        0     7393 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_downloader/base.py
--rw-r--r--   0        0        0     4566 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_downloader/ckey.py
--rw-r--r--   0        0        0      517 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_downloader/constants.py
--rw-r--r--   0        0        0     4492 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/log_downloader/round.py
--rw-r--r--   0        0        0    10429 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/menu.py
--rw-r--r--   0        0        0     1247 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/menu_item.py
--rw-r--r--   0        0        0     1880 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/scrubby/CKeyController.py
--rw-r--r--   0        0        0     2341 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/scrubby/RoundController.py
--rw-r--r--   0        0        0      622 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/scrubby/__init__.py
--rw-r--r--   0        0        0      107 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/scrubby/__main__.py
--rw-r--r--   0        0        0      433 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/scrubby/constants.py
--rw-r--r--   0        0        0        0 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/scrubby/investigate.py
--rw-r--r--   0        0        0     1201 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/scrubby/round_data.py
--rw-r--r--   0        0        0      154 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/slur_detector/__init__.py
--rw-r--r--   0        0        0      320 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/slur_detector/__main__.py
--rw-r--r--   0        0        0       21 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/slur_detector/constants.py
--rw-r--r--   0        0        0     2740 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/slur_detector/slur_detector.py
--rw-r--r--   0        0        0      987 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/slur_detector/slur_file.py
--rw-r--r--   0        0        0      201 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/slur_detector/word_detection.py
--rw-r--r--   0        0        0      327 2023-04-20 17:41:38.740386 ss13_tools-2.2.2/ss13_tools/util.py
--rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ss13_tools-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2301 2023-06-12 01:20:17.412910 ss13_tools-2.3.0/README.md
+-rw-r--r--   0        0        0     1008 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/__init__.py
+-rw-r--r--   0        0        0     1175 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/__version__.py
+-rw-r--r--   0        0        0      438 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/auth/__init__.py
+-rw-r--r--   0        0        0      205 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/auth/__main__.py
+-rw-r--r--   0        0        0      346 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/auth/constants.py
+-rw-r--r--   0        0        0    10698 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/auth/tg.py
+-rw-r--r--   0        0        0      182 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/byond/__init__.py
+-rw-r--r--   0        0        0      543 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/byond/__main__.py
+-rw-r--r--   0        0        0       59 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/byond/constants.py
+-rw-r--r--   0        0        0     2424 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/byond/key_tools.py
+-rw-r--r--   0        0        0      162 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/centcom/__init__.py
+-rw-r--r--   0        0        0     1099 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/centcom/__main__.py
+-rw-r--r--   0        0        0      394 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/centcom/ban.py
+-rw-r--r--   0        0        0     1492 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/centcom/ban_types.py
+-rw-r--r--   0        0        0       68 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/centcom/constants.py
+-rw-r--r--   0        0        0      614 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/cli.py
+-rw-r--r--   0        0        0      222 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/constants.py
+-rw-r--r--   0        0        0    18265 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/README.md
+-rw-r--r--   0        0        0      198 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/__init__.py
+-rw-r--r--   0        0        0     5561 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/__main__.py
+-rw-r--r--   0        0        0      768 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/constants.py
+-rw-r--r--   0        0        0      562 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/expressions.py
+-rw-r--r--   0        0        0    52497 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/log.py
+-rw-r--r--   0        0        0    17063 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/log_magics.py
+-rw-r--r--   0        0        0    28437 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_buddy/log_parser.py
+-rw-r--r--   0        0        0      554 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_downloader/__init__.py
+-rw-r--r--   0        0        0     2011 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_downloader/__main__.py
+-rw-r--r--   0        0        0     7393 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_downloader/base.py
+-rw-r--r--   0        0        0     4566 2023-06-12 01:20:17.420911 ss13_tools-2.3.0/ss13_tools/log_downloader/ckey.py
+-rw-r--r--   0        0        0      517 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/log_downloader/constants.py
+-rw-r--r--   0        0        0     4492 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/log_downloader/round.py
+-rw-r--r--   0        0        0    10429 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/menu.py
+-rw-r--r--   0        0        0     1247 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/menu_item.py
+-rw-r--r--   0        0        0     1880 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/scrubby/CKeyController.py
+-rw-r--r--   0        0        0     2341 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/scrubby/RoundController.py
+-rw-r--r--   0        0        0      622 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/scrubby/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/scrubby/__main__.py
+-rw-r--r--   0        0        0      433 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/scrubby/constants.py
+-rw-r--r--   0        0        0        0 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/scrubby/investigate.py
+-rw-r--r--   0        0        0     1201 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/scrubby/round_data.py
+-rw-r--r--   0        0        0      154 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/slur_detector/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/slur_detector/__main__.py
+-rw-r--r--   0        0        0       21 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/slur_detector/constants.py
+-rw-r--r--   0        0        0     2740 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/slur_detector/slur_detector.py
+-rw-r--r--   0        0        0      987 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/slur_detector/slur_file.py
+-rw-r--r--   0        0        0      201 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/slur_detector/word_detection.py
+-rw-r--r--   0        0        0      327 2023-06-12 01:20:17.424911 ss13_tools-2.3.0/ss13_tools/util.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 ss13_tools-2.3.0/PKG-INFO
```

### Comparing `ss13_tools-2.2.2/README.md` & `ss13_tools-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/pyproject.toml` & `ss13_tools-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SS13-tools"
-version = "2.2.2"
+version = "2.3.0"
 description = "Python toolchain for SS13"
 authors = ["RigglePrime <27156122+RigglePrime@users.noreply.github.com>", "tattle <66640614+dragomagol@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/RigglePrime/SS13-tools"
 keywords = ["ss13", "tgstation"]
 
 [tool.poetry.dependencies]
```

### Comparing `ss13_tools-2.2.2/ss13_tools/__main__.py` & `ss13_tools-2.3.0/ss13_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/auth/tg.py` & `ss13_tools-2.3.0/ss13_tools/auth/tg.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/byond/__main__.py` & `ss13_tools-2.3.0/ss13_tools/byond/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/byond/key_tools.py` & `ss13_tools-2.3.0/ss13_tools/byond/key_tools.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/centcom/__main__.py` & `ss13_tools-2.3.0/ss13_tools/centcom/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/centcom/ban_types.py` & `ss13_tools-2.3.0/ss13_tools/centcom/ban_types.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/cli.py` & `ss13_tools-2.3.0/ss13_tools/cli.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_buddy/README.md` & `ss13_tools-2.3.0/ss13_tools/log_buddy/README.md`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_buddy/__main__.py` & `ss13_tools-2.3.0/ss13_tools/log_buddy/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_buddy/constants.py` & `ss13_tools-2.3.0/ss13_tools/log_buddy/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "telecomms.txt",
     "uplink.txt",
     "shuttle.txt"
 ]
 HELP_LINK = "https://github.com/RigglePrime/SS13-tools/blob/master/ss13_tools/log_buddy/README.md"
 SHAMELESS = f"## Created using SS13-Tools LogBuddy {__version__} https://github.com/RigglePrime/SS13-Tools\n"
 ERRORED_FILE = "errored.log"
+MAX_SUPPORTED_LOG_VERSION = "1.0.0"
 
 LOG_COLOUR_SCARLET = 124
 LOG_COLOUR_RED = 167
 LOG_COLOUR_EMERALD = 35
 LOG_COLOUR_PERIWINKLE = 69
 LOG_COLOUR_PINK = 169
 LOG_COLOUR_GRAY = 245
```

### Comparing `ss13_tools-2.2.2/ss13_tools/log_buddy/expressions.py` & `ss13_tools-2.3.0/ss13_tools/log_buddy/expressions.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_buddy/log.py` & `ss13_tools-2.3.0/ss13_tools/log_buddy/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/env python3
 
 from datetime import datetime
 from enum import Enum
 from typing import Annotated, Tuple, Optional
 import re
 from html import unescape as html_unescape
-from colorama import init
+import json
 
+from colorama import init
 from dateutil.parser import isoparse
 
 from ss13_tools.byond import canonicalize
 from ss13_tools.log_buddy.expressions import LOC_REGEX, ADMIN_BUILD_MODE, ADMIN_STAT_CHANGE,\
     HORRIBLE_HREF, GAME_I_LOVE_BOMBS, ADMINPRIVATE_NOTE, ADMINPRIVATE_BAN,\
     LOG_PRETTY_LOC, LOG_PRETTY_STR, LOG_PRETTY_PATH
 from ss13_tools.log_buddy.constants import LOG_COLOUR_SCARLET, LOG_COLOUR_RED, LOG_COLOUR_EMERALD,\
     LOG_COLOUR_PERIWINKLE, LOG_COLOUR_PINK, LOG_COLOUR_GRAY, LOG_COLOUR_PASTEL_CYAN, LOG_COLOUR_SUNSET,\
-    LOG_COLOUR_PASTEL_ORANGE, LOG_COLOUR_AMETHYST, LOG_COLOUR_OCEAN
+    LOG_COLOUR_PASTEL_ORANGE, LOG_COLOUR_AMETHYST, LOG_COLOUR_OCEAN,\
+    MAX_SUPPORTED_LOG_VERSION
 
 
 class LogType(Enum):
     """What type of log file is it?"""
     UNKNOWN = 0
     ACCESS = 1
     GAME = 2
@@ -171,33 +173,47 @@
         raise NotImplementedError("Not yet implemented")
 
 
 class UnknownLogException(Exception):
     """Thrown when a log type is not known. (so unexpected!)"""
 
 
+class UnsupportedSchemaVersionException(Exception):
+    """Thrown when a JSON log schema isn't supported. (so unexpected!)"""
+
+
 class Log:
     """Represents one log entry
 
     Examples:
     log = `Log("log line here")` # NOTE: must be a valid log entry"""
 
     def __init__(self, line: Optional[str] = None) -> None:
-        if not line or line[0] != "[":
-            raise UnknownLogException("Does not start with [")
+        if not line:
+            raise UnknownLogException("Log line empty!")
 
+        self.json_schema = None
         self.time = None
         self.agent = None
         self.patient = None
         self.location = None
         self.location_name = None
         self.text = None
         self.is_dead = None
-
         self.raw_line = line
+
+        if line[0] == "{":
+            self.__json_parse()
+            return
+        if line[0] == "[":
+            self.__parse_old_log()
+            return
+        raise UnknownLogException("Unsupported log")
+
+    def __parse_old_log(self):
         date_time, other = self.raw_line.split("] ", 1)
         self.time = isoparse(date_time[1:])  # Remove starting [
         if other.endswith("VOTE:"):
             other += " "
 
         # Check for TGUI logs
         if ": " not in other and (" in " in other or " (as " in other):
@@ -209,20 +225,39 @@
             # You see, here's the problem. What if we only have a client and no window or context?
             # Is that even possible? I am too lazy to make sure and will assume it's not.
             # If it is, hi! Welcome to hell. Please edit the conditional before to work.
             # Just know that it will catch false positives. What fun world of logging we live in.
             self.parse_tgui(other)
             return
         log_type, other = other.split(": ", 1)
-        self.log_type = LogType.parse_log_type(log_type)
+        self.log_type = LogType.parse_log_type(log_type.replace("GAME-", "", 1))
         # Python go brrrrrrr
         parsing_function = getattr(self, f"parse_{self.log_type.name.lower()}", None)
         if parsing_function:
             parsing_function(other)
 
+    def __json_parse(self):
+        log = json.loads(self.raw_line)
+        if not log['s-ver'].count('.') == 2:
+            raise UnknownLogException("Schema version corrupted")
+        max_supported = tuple(int(x) for x in MAX_SUPPORTED_LOG_VERSION.split('.'))
+        schema_version = tuple(int(x) for x in log['s-ver'].split('.'))
+        for i in range(len(max_supported)):  # pylint: disable=consider-using-enumerate
+            if max_supported[i] > schema_version[i]:
+                break
+            if max_supported[i] < schema_version[i]:
+                raise UnsupportedSchemaVersionException(f"Unsupported schema: {log['s-ver']}")
+        self.json_schema = log['s-ver']
+        self.time = isoparse(log['ts'])
+        self.log_type = LogType.parse_log_type(log['cat'].replace("game-", "", 1))
+        parsing_function = getattr(self, f"parse_{self.log_type.name.lower()}", None)
+        if parsing_function:
+            parsing_function(log['msg'])
+
+    json_schema = Annotated[str, "JSON schema version. None if not a JSON log"]
     time: Annotated[datetime, "Time of logging"]
     agent: Annotated[Optional[Player], "Player performing the action"]
     patient: Annotated[Optional[Player], "Player receiving the action"]
     raw_line: Annotated[str, "Raw, unmodified line"]
     log_type: Annotated[LogType, "Type of the log"]
     location: Annotated[Optional[Tuple[int, int, int]], "X, Y, Y where the action was performed"]
     location_name: Annotated[Optional[str], "Name of the location where the action was performed"]
@@ -1035,14 +1070,16 @@
         return lambda match: f"\033[38;5;{colour}m{html_unescape(match.group(0))}\033[0m"
 
     def __re_pretty(self, colour):
         return lambda match: f"\033[38;5;{colour}m{match.group(0)}\033[0m"
 
     def pretty(self):
         """Return, but with ANSI colour!"""
+        if self.raw_line[0] == "{":
+            return self.__pretty_json()
         to_be_printed = self.raw_line
         to_be_printed = re.sub(LOG_PRETTY_LOC, self.__re_pretty(LOG_COLOUR_PASTEL_CYAN), to_be_printed)
         to_be_printed = re.sub(LOG_PRETTY_PATH, self.__re_pretty(LOG_COLOUR_PASTEL_ORANGE), to_be_printed)
         to_be_printed = re.sub(LOG_PRETTY_STR, self.__re_pretty_htmlescaped(LOG_COLOUR_SUNSET), to_be_printed, 1)
         return to_be_printed.replace("[", "\033[38;5;240m[", 1).replace("]", "]\033[0m", 1)\
                             .replace("ACCESS:", f"\033[38;5;{LOG_COLOUR_GRAY}mACCESS:\033[0m", 1)\
                             .replace("ASSET:", f"\033[38;5;{LOG_COLOUR_GRAY}mASSET:\033[0m", 1)\
@@ -1071,14 +1108,17 @@
                             .replace("SILICON:", f"\033[38;5;{LOG_COLOUR_OCEAN}mSILICON:\033[0m", 1)\
                             \
                             .replace(str(self.agent), f"\033[38;5;{LOG_COLOUR_AMETHYST}m{str(self.agent)}\033[0m")\
                             .replace(str(self.patient), f"\033[38;5;{LOG_COLOUR_AMETHYST}m{str(self.patient)}\033[0m")\
                             .replace(str(self.location_name),
                                      f"\033[38;5;{LOG_COLOUR_PASTEL_CYAN}m{str(self.location_name)}\033[0m")
 
+    def __pretty_json(self):
+        return self.raw_line
+
     def __str__(self):
         """String representation"""
         return self.raw_line
 
     def __repr__(self):
         """Object representation"""
         return self.raw_line
```

### Comparing `ss13_tools-2.2.2/ss13_tools/log_buddy/log_magics.py` & `ss13_tools-2.3.0/ss13_tools/log_buddy/log_magics.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_buddy/log_parser.py` & `ss13_tools-2.3.0/ss13_tools/log_buddy/log_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,16 @@
                 if not quiet:
                     print(f"Could not be parsed: '{line}', with the reason:", exception)
                 if verbose:
                     traceback.print_exc()
                 pbar.display()
         if errored:
             with open(ERRORED_FILE, 'a+', encoding="utf-8") as file:
-                file.write("If you see this, please share it with Riggle.\n")
+                file.write("## If you see this, please share it with Riggle.\n")
+                file.write("## ")
                 file.write(__version__)
                 file.write("\n\n")
                 file.writelines(chain.from_iterable(zip(errored, repeat("\n"))))
 
     def __parse_one_line(self, line: str):
         if line.startswith("-censored"):
             return  # Skip censored lines
```

### Comparing `ss13_tools-2.2.2/ss13_tools/log_downloader/__init__.py` & `ss13_tools-2.3.0/ss13_tools/log_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_downloader/__main__.py` & `ss13_tools-2.3.0/ss13_tools/log_downloader/__main__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_downloader/base.py` & `ss13_tools-2.3.0/ss13_tools/log_downloader/base.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_downloader/ckey.py` & `ss13_tools-2.3.0/ss13_tools/log_downloader/ckey.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_downloader/constants.py` & `ss13_tools-2.3.0/ss13_tools/log_downloader/constants.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/log_downloader/round.py` & `ss13_tools-2.3.0/ss13_tools/log_downloader/round.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/menu.py` & `ss13_tools-2.3.0/ss13_tools/menu.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/menu_item.py` & `ss13_tools-2.3.0/ss13_tools/menu_item.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/scrubby/CKeyController.py` & `ss13_tools-2.3.0/ss13_tools/scrubby/CKeyController.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/scrubby/RoundController.py` & `ss13_tools-2.3.0/ss13_tools/scrubby/RoundController.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/scrubby/__init__.py` & `ss13_tools-2.3.0/ss13_tools/scrubby/__init__.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/scrubby/round_data.py` & `ss13_tools-2.3.0/ss13_tools/scrubby/round_data.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/slur_detector/slur_detector.py` & `ss13_tools-2.3.0/ss13_tools/slur_detector/slur_detector.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/ss13_tools/slur_detector/slur_file.py` & `ss13_tools-2.3.0/ss13_tools/slur_detector/slur_file.py`

 * *Files identical despite different names*

### Comparing `ss13_tools-2.2.2/PKG-INFO` & `ss13_tools-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ss13-tools
-Version: 2.2.2
+Version: 2.3.0
 Summary: Python toolchain for SS13
 Home-page: https://github.com/RigglePrime/SS13-tools
 Keywords: ss13,tgstation
 Author: RigglePrime
 Author-email: 27156122+RigglePrime@users.noreply.github.com
 Requires-Python: >=3.9.1,<3.12
 Classifier: Programming Language :: Python :: 3
```

