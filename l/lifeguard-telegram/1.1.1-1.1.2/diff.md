# Comparing `tmp/lifeguard-telegram-1.1.1.tar.gz` & `tmp/lifeguard-telegram-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-telegram-1.1.1.tar", last modified: Mon Jun 12 14:53:49 2023, max compression
+gzip compressed data, was "lifeguard-telegram-1.1.2.tar", last modified: Mon Jun 12 15:10:21 2023, max compression
```

## Comparing `lifeguard-telegram-1.1.1.tar` & `lifeguard-telegram-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/lifeguard_telegram/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/lifeguard_telegram/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 14:53:49.000000 lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:53:49.925517 lifeguard-telegram-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-12 14:52:57.000000 lifeguard-telegram-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:21.143137 lifeguard-telegram-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 15:10:21.143137 lifeguard-telegram-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:21.139137 lifeguard-telegram-1.1.2/lifeguard_telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/lifeguard_telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/lifeguard_telegram/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:21.143137 lifeguard-telegram-1.1.2/lifeguard_telegram/bot_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/lifeguard_telegram/bot_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/lifeguard_telegram/bot_handlers/builtin_bot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/lifeguard_telegram/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/lifeguard_telegram/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:10:21.143137 lifeguard-telegram-1.1.2/lifeguard_telegram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-12 15:10:21.000000 lifeguard-telegram-1.1.2/lifeguard_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-12 15:10:21.000000 lifeguard-telegram-1.1.2/lifeguard_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:10:21.000000 lifeguard-telegram-1.1.2/lifeguard_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 15:10:21.000000 lifeguard-telegram-1.1.2/lifeguard_telegram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 15:10:21.000000 lifeguard-telegram-1.1.2/lifeguard_telegram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:10:21.143137 lifeguard-telegram-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-12 15:09:49.000000 lifeguard-telegram-1.1.2/setup.py
```

### Comparing `lifeguard-telegram-1.1.1/PKG-INFO` & `lifeguard-telegram-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-telegram
-Version: 1.1.1
+Version: 1.1.2
 Summary: Lifeguard integration with Telegram
 Home-page: https://github.com/LifeguardSystem/lifeguard-telegram
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-telegram-1.1.1/lifeguard_telegram/__init__.py` & `lifeguard-telegram-1.1.2/lifeguard_telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.1/lifeguard_telegram/bot.py` & `lifeguard-telegram-1.1.2/lifeguard_telegram/bot.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.1/lifeguard_telegram/bot_handlers/builtin_bot_handler.py` & `lifeguard-telegram-1.1.2/lifeguard_telegram/bot_handlers/builtin_bot_handler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.1/lifeguard_telegram/notifications.py` & `lifeguard-telegram-1.1.2/lifeguard_telegram/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.1/lifeguard_telegram/settings.py` & `lifeguard-telegram-1.1.2/lifeguard_telegram/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-telegram-1.1.1/lifeguard_telegram.egg-info/PKG-INFO` & `lifeguard-telegram-1.1.2/lifeguard_telegram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-telegram
-Version: 1.1.1
+Version: 1.1.2
 Summary: Lifeguard integration with Telegram
 Home-page: https://github.com/LifeguardSystem/lifeguard-telegram
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-telegram-1.1.1/setup.py` & `lifeguard-telegram-1.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-telegram",
-    version="1.1.1",
+    version="1.1.2",
     url="https://github.com/LifeguardSystem/lifeguard-telegram",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with Telegram",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["lifeguard", "python-telegram-bot", "telepot"],
+    install_requires=["lifeguard", "python-telegram-bot==13.1", "telepot"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

