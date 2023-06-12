# Comparing `tmp/commandeft-0.1.5.tar.gz` & `tmp/commandeft-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandeft-0.1.5.tar", last modified: Mon Jun 12 03:29:50 2023, max compression
+gzip compressed data, was "commandeft-0.2.0.tar", last modified: Mon Jun 12 09:21:31 2023, max compression
```

## Comparing `commandeft-0.1.5.tar` & `commandeft-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1078 2023-06-10 01:12:32.215348 commandeft-0.1.5/LICENSE
--rw-r--r--   0        0        0     3477 2023-06-12 03:13:58.678920 commandeft-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-11 23:37:24.840096 commandeft-0.1.5/commandeft/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009549 commandeft-0.1.5/commandeft/constants/__init__.py
--rw-r--r--   0        0        0     3153 2023-06-11 23:38:27.793749 commandeft-0.1.5/commandeft/constants/consts.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.009834 commandeft-0.1.5/commandeft/core/__init__.py
--rw-r--r--   0        0        0     2557 2023-06-12 03:25:45.776795 commandeft-0.1.5/commandeft/core/cli.py
--rw-r--r--   0        0        0      823 2023-06-11 23:38:27.796254 commandeft-0.1.5/commandeft/core/decision.py
--rw-r--r--   0        0        0     1715 2023-06-11 23:38:27.804139 commandeft-0.1.5/commandeft/core/generation.py
--rw-r--r--   0        0        0     1128 2023-06-12 03:26:22.574486 commandeft-0.1.5/commandeft/main.py
--rw-r--r--   0        0        0        0 2023-06-12 01:40:57.010171 commandeft-0.1.5/commandeft/util/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-11 23:38:27.808831 commandeft-0.1.5/commandeft/util/config_util.py
--rw-r--r--   0        0        0      437 2023-06-11 23:38:27.809677 commandeft-0.1.5/commandeft/util/gen_util.py
--rw-r--r--   0        0        0     2729 2023-06-12 03:13:58.680953 commandeft-0.1.5/commandeft/util/interactive_util.py
--rw-r--r--   0        0        0     1664 2023-06-12 03:29:50.096178 commandeft-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 commandeft-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-12 08:48:28.900375 commandeft-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3477 2023-06-12 08:48:28.901375 commandeft-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 08:48:28.901375 commandeft-0.2.0/commandeft/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:48:28.902375 commandeft-0.2.0/commandeft/constants/__init__.py
+-rw-r--r--   0        0        0     3153 2023-06-12 08:48:28.902375 commandeft-0.2.0/commandeft/constants/consts.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:48:28.902375 commandeft-0.2.0/commandeft/core/__init__.py
+-rw-r--r--   0        0        0     2557 2023-06-12 08:48:28.902375 commandeft-0.2.0/commandeft/core/cli.py
+-rw-r--r--   0        0        0      823 2023-06-12 08:48:28.903375 commandeft-0.2.0/commandeft/core/decision.py
+-rw-r--r--   0        0        0     1715 2023-06-12 08:48:28.903375 commandeft-0.2.0/commandeft/core/generation.py
+-rw-r--r--   0        0        0     1128 2023-06-12 08:48:28.903375 commandeft-0.2.0/commandeft/main.py
+-rw-r--r--   0        0        0        0 2023-06-12 08:48:28.904376 commandeft-0.2.0/commandeft/util/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-12 08:48:28.904376 commandeft-0.2.0/commandeft/util/config_util.py
+-rw-r--r--   0        0        0      624 2023-06-12 09:16:04.009413 commandeft-0.2.0/commandeft/util/gen_util.py
+-rw-r--r--   0        0        0     2729 2023-06-12 08:48:28.905376 commandeft-0.2.0/commandeft/util/interactive_util.py
+-rw-r--r--   0        0        0     1664 2023-06-12 09:21:31.508371 commandeft-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 commandeft-0.2.0/PKG-INFO
```

### Comparing `commandeft-0.1.5/LICENSE` & `commandeft-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/README.md` & `commandeft-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/constants/consts.py` & `commandeft-0.2.0/commandeft/constants/consts.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/core/cli.py` & `commandeft-0.2.0/commandeft/core/cli.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/core/decision.py` & `commandeft-0.2.0/commandeft/core/decision.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/core/generation.py` & `commandeft-0.2.0/commandeft/core/generation.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/main.py` & `commandeft-0.2.0/commandeft/main.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/util/config_util.py` & `commandeft-0.2.0/commandeft/util/config_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/commandeft/util/interactive_util.py` & `commandeft-0.2.0/commandeft/util/interactive_util.py`

 * *Files identical despite different names*

### Comparing `commandeft-0.1.5/pyproject.toml` & `commandeft-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "commandeft"
-version = "0.1.5"
+version = "0.2.0"
 description = "CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models."
 readme = "README.md"
 authors = [
     { name = "Petros Sidirokastritis", email = "sidirope@gmail.com" },
 ]
 requires-python = ">=3.8.1, <=3.11.4"
 dependencies = [
```

### Comparing `commandeft-0.1.5/PKG-INFO` & `commandeft-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandeft
-Version: 0.1.5
+Version: 0.2.0
 Summary: CommanDeft is a CLI tool that converts natural language prompts into executable commands or scripts using OpenAI's chat models.
 Author-Email: Petros Sidirokastritis <sidirope@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Ferrum-Citadel/commandeft
 Requires-Python: <=3.11.4,>=3.8.1
 Requires-Dist: PyJWT==2.7.0
 Requires-Dist: Pygments==2.15.1
```

