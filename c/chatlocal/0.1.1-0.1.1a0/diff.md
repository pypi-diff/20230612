# Comparing `tmp/chatlocal-0.1.1.tar.gz` & `tmp/chatlocal-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlocal-0.1.1.tar", max compression
+gzip compressed data, was "chatlocal-0.1.1a0.tar", max compression
```

## Comparing `chatlocal-0.1.1.tar` & `chatlocal-0.1.1a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6301 2023-06-12 10:21:34.138117 chatlocal-0.1.1/README.md
--rw-r--r--   0        0        0      250 2023-06-12 10:31:15.664533 chatlocal-0.1.1/chatlocal/__init__.py
--rw-r--r--   0        0        0     2631 2023-06-12 08:58:42.125242 chatlocal-0.1.1/chatlocal/dataloader.py
--rw-r--r--   0        0        0     1326 2023-06-12 10:02:15.849512 chatlocal-0.1.1/chatlocal/settings.py
--rw-r--r--   0        0        0     3294 2023-06-12 09:07:55.665877 chatlocal-0.1.1/chatlocal/vectorstore.py
--rw-r--r--   0        0        0      746 2023-06-12 10:31:05.994683 chatlocal-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 chatlocal-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6301 2023-06-12 10:21:34.138117 chatlocal-0.1.1a0/README.md
+-rw-r--r--   0        0        0      256 2023-06-12 10:25:00.450423 chatlocal-0.1.1a0/chatlocal/__init__.py
+-rw-r--r--   0        0        0     2631 2023-06-12 08:58:42.125242 chatlocal-0.1.1a0/chatlocal/dataloader.py
+-rw-r--r--   0        0        0     1326 2023-06-12 10:02:15.849512 chatlocal-0.1.1a0/chatlocal/settings.py
+-rw-r--r--   0        0        0     3294 2023-06-12 09:07:55.665877 chatlocal-0.1.1a0/chatlocal/vectorstore.py
+-rw-r--r--   0        0        0      752 2023-06-12 10:24:45.829345 chatlocal-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0     7096 1970-01-01 00:00:00.000000 chatlocal-0.1.1a0/PKG-INFO
```

### Comparing `chatlocal-0.1.1/README.md` & `chatlocal-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `chatlocal-0.1.1/chatlocal/dataloader.py` & `chatlocal-0.1.1a0/chatlocal/dataloader.py`

 * *Files identical despite different names*

### Comparing `chatlocal-0.1.1/chatlocal/settings.py` & `chatlocal-0.1.1a0/chatlocal/settings.py`

 * *Files identical despite different names*

### Comparing `chatlocal-0.1.1/chatlocal/vectorstore.py` & `chatlocal-0.1.1a0/chatlocal/vectorstore.py`

 * *Files identical despite different names*

### Comparing `chatlocal-0.1.1/pyproject.toml` & `chatlocal-0.1.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatlocal"
-version = "0.1.1"
+version = "0.1.1-alpha"
 description = "chat with your local files"
 authors = ["Raoul Grouls <Raoul.Grouls@han.nl>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.urls]
 GitHub = "https://github.com/raoulg/chatlocal"
```

### Comparing `chatlocal-0.1.1/PKG-INFO` & `chatlocal-0.1.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlocal
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: chat with your local files
 License: MIT
 Author: Raoul Grouls
 Author-email: Raoul.Grouls@han.nl
 Requires-Python: >=3.9.16,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

