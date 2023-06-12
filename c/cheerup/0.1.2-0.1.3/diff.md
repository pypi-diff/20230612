# Comparing `tmp/cheerup-0.1.2.tar.gz` & `tmp/cheerup-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheerup-0.1.2.tar", last modified: Sun Jun 11 12:15:11 2023, max compression
+gzip compressed data, was "cheerup-0.1.3.tar", last modified: Mon Jun 12 12:59:57 2023, max compression
```

## Comparing `cheerup-0.1.2.tar` & `cheerup-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.887266 cheerup-0.1.2/
--rw-r--r--   0 tyamamiya   (501) staff       (20)     1072 2023-06-11 06:23:09.000000 cheerup-0.1.2/LICENSE
--rw-r--r--   0 tyamamiya   (501) staff       (20)     2700 2023-06-11 12:15:11.887049 cheerup-0.1.2/PKG-INFO
--rw-r--r--   0 tyamamiya   (501) staff       (20)     2172 2023-06-11 09:51:06.000000 cheerup-0.1.2/README.md
--rw-r--r--   0 tyamamiya   (501) staff       (20)      680 2023-06-11 12:09:45.000000 cheerup-0.1.2/pyproject.toml
--rw-r--r--   0 tyamamiya   (501) staff       (20)       38 2023-06-11 12:15:11.887332 cheerup-0.1.2/setup.cfg
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.884411 cheerup-0.1.2/src/
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.885757 cheerup-0.1.2/src/cheerup/
--rw-r--r--   0 tyamamiya   (501) staff       (20)     4021 2023-06-11 10:01:39.000000 cheerup-0.1.2/src/cheerup/__init__.py
-drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-11 12:15:11.886747 cheerup-0.1.2/src/cheerup.egg-info/
--rw-r--r--   0 tyamamiya   (501) staff       (20)     2700 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/PKG-INFO
--rw-r--r--   0 tyamamiya   (501) staff       (20)      268 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/SOURCES.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)        1 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/dependency_links.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)       41 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/entry_points.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)       44 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/requires.txt
--rw-r--r--   0 tyamamiya   (501) staff       (20)        8 2023-06-11 12:15:11.000000 cheerup-0.1.2/src/cheerup.egg-info/top_level.txt
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-12 12:59:57.494819 cheerup-0.1.3/
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     1072 2023-06-12 01:13:28.000000 cheerup-0.1.3/LICENSE
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     2700 2023-06-12 12:59:57.494535 cheerup-0.1.3/PKG-INFO
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     2172 2023-06-12 01:13:28.000000 cheerup-0.1.3/README.md
+-rw-r--r--   0 tyamamiya   (501) staff       (20)      680 2023-06-12 12:57:32.000000 cheerup-0.1.3/pyproject.toml
+-rw-r--r--   0 tyamamiya   (501) staff       (20)       38 2023-06-12 12:59:57.494908 cheerup-0.1.3/setup.cfg
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-12 12:59:57.490797 cheerup-0.1.3/src/
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-12 12:59:57.492234 cheerup-0.1.3/src/cheerup/
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     4077 2023-06-12 12:55:50.000000 cheerup-0.1.3/src/cheerup/__init__.py
+drwxr-xr-x   0 tyamamiya   (501) staff       (20)        0 2023-06-12 12:59:57.494166 cheerup-0.1.3/src/cheerup.egg-info/
+-rw-r--r--   0 tyamamiya   (501) staff       (20)     2700 2023-06-12 12:59:57.000000 cheerup-0.1.3/src/cheerup.egg-info/PKG-INFO
+-rw-r--r--   0 tyamamiya   (501) staff       (20)      268 2023-06-12 12:59:57.000000 cheerup-0.1.3/src/cheerup.egg-info/SOURCES.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)        1 2023-06-12 12:59:57.000000 cheerup-0.1.3/src/cheerup.egg-info/dependency_links.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)       41 2023-06-12 12:59:57.000000 cheerup-0.1.3/src/cheerup.egg-info/entry_points.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)       44 2023-06-12 12:59:57.000000 cheerup-0.1.3/src/cheerup.egg-info/requires.txt
+-rw-r--r--   0 tyamamiya   (501) staff       (20)        8 2023-06-12 12:59:57.000000 cheerup-0.1.3/src/cheerup.egg-info/top_level.txt
```

### Comparing `cheerup-0.1.2/LICENSE` & `cheerup-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cheerup-0.1.2/PKG-INFO` & `cheerup-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheerup
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cheer on your command-line expertise!
 Author-email: Takashi Yamamiya <tak@metatoys.org>
 Project-URL: Homepage, https://github.com/propella/cheerup
 Project-URL: Bug Tracker, https://github.com/propella/cheerup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cheerup-0.1.2/README.md` & `cheerup-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cheerup-0.1.2/pyproject.toml` & `cheerup-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cheerup"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "Takashi Yamamiya", email = "tak@metatoys.org" }]
 description = "Cheer on your command-line expertise!"
 readme = "README.md"
 requires-python = ">=3.9"
 
 dependencies = [
     "openai",
```

### Comparing `cheerup-0.1.2/src/cheerup/__init__.py` & `cheerup-0.1.3/src/cheerup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         jsondata = json.dumps(history, indent=2)
         file.write(jsondata)
 
 
 def chat(cmd: str, locale: Optional[str] = None) -> str:
     """Print response from OpenAI API."""
 
-    prompt = "You are an AI assistant adept at complimenting programmers. Please provide verbose compliments on the user's Unix command inputs."
+    prompt = "You are an AI assistant adept at complimenting programmers. Please provide verbose compliments with many emojis on the user's Unix command inputs."
     if locale:
         prompt += f" Use the language in the locale: {locale}."
     history = get_history()
 
     query = {"role": "user", "content": cmd}
     messages = messages = [
         *history,
@@ -47,14 +47,15 @@
             "role": "system",
             "content": prompt,
         },
         query,
     ]
     # pprint(messages)
 
+    print("🤖 ", end="", flush=True)
     try:
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=messages,
             stream=True,
         )
     except openai.error.AuthenticationError:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cheerup-0.1.2/src/cheerup.egg-info/PKG-INFO` & `cheerup-0.1.3/src/cheerup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheerup
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cheer on your command-line expertise!
 Author-email: Takashi Yamamiya <tak@metatoys.org>
 Project-URL: Homepage, https://github.com/propella/cheerup
 Project-URL: Bug Tracker, https://github.com/propella/cheerup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

