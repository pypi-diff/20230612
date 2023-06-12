# Comparing `tmp/eqalert-3.5.4.tar.gz` & `tmp/eqalert-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqalert-3.5.4.tar", last modified: Sun Jun 11 19:18:44 2023, max compression
+gzip compressed data, was "eqalert-3.5.5.tar", last modified: Mon Jun 12 10:29:31 2023, max compression
```

## Comparing `eqalert-3.5.4.tar` & `eqalert-3.5.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.736483 eqalert-3.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-11 19:18:44.736483 eqalert-3.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-11 19:18:29.000000 eqalert-3.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.732483 eqalert-3.5.4/eqa/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    60671 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/eqalert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.732483 eqalert-3.5.4/eqa/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125764 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/action.py
--rw-r--r--   0 runner    (1001) docker     (123)   580215 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    82457 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/encounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)   488202 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/lib/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.736483 eqalert-3.5.4/eqa/sound/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/sound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/sound/tick.wav
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-11 19:18:29.000000 eqalert-3.5.4/eqa/sound/tock.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 19:18:44.736483 eqalert-3.5.4/eqalert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-11 19:18:44.000000 eqalert-3.5.4/eqalert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-11 19:18:44.736483 eqalert-3.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-11 19:18:29.000000 eqalert-3.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:31.934272 eqalert-3.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-12 10:29:31.934272 eqalert-3.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-12 10:29:16.000000 eqalert-3.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:31.926272 eqalert-3.5.5/eqa/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60671 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/eqalert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:31.934272 eqalert-3.5.5/eqa/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125764 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)   580215 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82457 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31830 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)   488202 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/lib/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:31.934272 eqalert-3.5.5/eqa/sound/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/sound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/sound/tick.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-06-12 10:29:16.000000 eqalert-3.5.5/eqa/sound/tock.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:29:31.934272 eqalert-3.5.5/eqalert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-06-12 10:29:31.000000 eqalert-3.5.5/eqalert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-12 10:29:31.000000 eqalert-3.5.5/eqalert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:29:31.000000 eqalert-3.5.5/eqalert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 10:29:31.000000 eqalert-3.5.5/eqalert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 10:29:31.000000 eqalert-3.5.5/eqalert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 10:29:31.000000 eqalert-3.5.5/eqalert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 10:29:31.934272 eqalert-3.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-12 10:29:16.000000 eqalert-3.5.5/setup.py
```

### Comparing `eqalert-3.5.4/PKG-INFO` & `eqalert-3.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.4
+Version: 3.5.5
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
```

### Comparing `eqalert-3.5.4/README.md` & `eqalert-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/eqalert.py` & `eqalert-3.5.5/eqa/eqalert.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/action.py` & `eqalert-3.5.5/eqa/lib/action.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/config.py` & `eqalert-3.5.5/eqa/lib/config.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/curses.py` & `eqalert-3.5.5/eqa/lib/curses.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/encounter.py` & `eqalert-3.5.5/eqa/lib/encounter.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/keys.py` & `eqalert-3.5.5/eqa/lib/keys.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/log.py` & `eqalert-3.5.5/eqa/lib/log.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/parser.py` & `eqalert-3.5.5/eqa/lib/parser.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/settings.py` & `eqalert-3.5.5/eqa/lib/settings.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/sound.py` & `eqalert-3.5.5/eqa/lib/sound.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/state.py` & `eqalert-3.5.5/eqa/lib/state.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/struct.py` & `eqalert-3.5.5/eqa/lib/struct.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/lib/timer.py` & `eqalert-3.5.5/eqa/lib/timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,14 +351,15 @@
 
 
 def consolidate_spell_timers(expired_timer, timers, sound_q, display_q):
     """Consolidate like spell timers"""
 
     try:
         new_timers = []
+        payload = expired_timer.payload
         for timer_event in timers:
             if timer_event.type == "spell":
                 if expired_timer.spell == timer_event.spell:
                     if int((timer_event.time - expired_timer.time).total_seconds()) < 3:
                         if expired_timer.payload.endswith(" has worn off"):
                             payload = (
                                 expired_timer.spell.replace("_", " ")
```

### Comparing `eqalert-3.5.4/eqa/lib/watch.py` & `eqalert-3.5.5/eqa/lib/watch.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/sound/tick.wav` & `eqalert-3.5.5/eqa/sound/tick.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqa/sound/tock.wav` & `eqalert-3.5.5/eqa/sound/tock.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/eqalert.egg-info/PKG-INFO` & `eqalert-3.5.5/eqalert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.4
+Version: 3.5.5
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
```

### Comparing `eqalert-3.5.4/eqalert.egg-info/SOURCES.txt` & `eqalert-3.5.5/eqalert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.4/setup.py` & `eqalert-3.5.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="eqalert",
-    version="3.5.4",
+    version="3.5.5",
     author="M Geitz",
     author_email="git@geitz.xyz",
     install_requires=[
         "playsound>=1.3.0",
         "gtts>=2.3.1",
     ],
     python_requires=">=3.9.2",
```

