# Comparing `tmp/lifeguard-telegram-1.1.0.tar.gz` & `tmp/lifeguard-telegram-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-telegram-1.1.0.tar", last modified: Tue May 30 19:18:40 2023, max compression
+gzip compressed data, was "lifeguard-telegram-1.1.1.tar", last modified: Mon Jun 12 14:53:49 2023, max compression
```

## Comparing `lifeguard-telegram-1.1.0.tar` & `lifeguard-telegram-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/lifeguard_telegram/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/lifeguard_telegram/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 19:18:40.000000 lifeguard-telegram-1.1.0/lifeguard_telegram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:18:40.905910 lifeguard-telegram-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 19:18:13.000000 lifeguard-telegram-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/lifeguard_telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/setup.py
```

### Comparing `lifeguard-telegram-1.1.0/lifeguard_telegram/__init__.py` & `lifeguard-telegram-1.1.1/lifeguard_telegram/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 import os
 
 from lifeguard.notifications import append_notification_implementation
 from lifeguard.logger import lifeguard_logger as logger
 
 from lifeguard_telegram.bot import init_updater
 from lifeguard_telegram.notifications import TelegramNotificationBase
+from lifeguard_telegram.settings import LIFEGUARD_TELEGRAM_ENABLE_BOTS_LOADER
 
 
 class LifeguardTelegramPlugin:
     """
     Telegram Plugin
     """
 
     def __init__(self, lifeguard_context):
         self.lifeguard_context = lifeguard_context
-        init_updater()
+
+        if LIFEGUARD_TELEGRAM_ENABLE_BOTS_LOADER:
+            init_updater()
 
 
 def init(lifeguard_context):
     append_notification_implementation(TelegramNotificationBase)
     newpid = os.fork()
     if newpid == 0:
         logger.info("starting telegram process")
```

### Comparing `lifeguard-telegram-1.1.0/lifeguard_telegram/bot.py` & `lifeguard-telegram-1.1.1/lifeguard_telegram/bot.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.0/lifeguard_telegram/bot_handlers/builtin_bot_handler.py` & `lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/builtin_bot_handler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.0/lifeguard_telegram/notifications.py` & `lifeguard-telegram-1.1.1/lifeguard_telegram/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.0/setup.py` & `lifeguard-telegram-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-telegram",
-    version="1.1.0",
+    version="1.1.1",
     url="https://github.com/LifeguardSystem/lifeguard-telegram",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with Telegram",
```

