# Comparing `tmp/talkytrend-1.1.4.tar.gz` & `tmp/talkytrend-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.1.4.tar", max compression
+gzip compressed data, was "talkytrend-1.1.5.tar", max compression
```

## Comparing `talkytrend-1.1.4.tar` & `talkytrend-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-11 11:51:24.342967 talkytrend-1.1.4/LICENSE
--rw-r--r--   0        0        0     2058 2023-06-11 11:51:24.342967 talkytrend-1.1.4/README.md
--rw-r--r--   0        0        0     1669 2023-06-11 11:51:44.938962 talkytrend-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      101 2023-06-11 11:51:44.938962 talkytrend-1.1.4/talkytrend/__init__.py
--rw-r--r--   0        0        0      630 2023-06-11 11:51:24.342967 talkytrend-1.1.4/talkytrend/config.py
--rw-r--r--   0        0        0      769 2023-06-11 11:51:24.342967 talkytrend-1.1.4/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     3730 2023-06-11 11:51:24.342967 talkytrend-1.1.4/talkytrend/main.py
--rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 talkytrend-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-12 15:58:42.228725 talkytrend-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2058 2023-06-12 15:58:42.228725 talkytrend-1.1.5/README.md
+-rw-r--r--   0        0        0     1669 2023-06-12 15:59:00.121294 talkytrend-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-06-12 15:59:00.125295 talkytrend-1.1.5/talkytrend/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-12 15:58:42.228725 talkytrend-1.1.5/talkytrend/config.py
+-rw-r--r--   0        0        0      769 2023-06-12 15:58:42.228725 talkytrend-1.1.5/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     3733 2023-06-12 15:58:42.228725 talkytrend-1.1.5/talkytrend/main.py
+-rw-r--r--   0        0        0     2905 1970-01-01 00:00:00.000000 talkytrend-1.1.5/PKG-INFO
```

### Comparing `talkytrend-1.1.4/LICENSE` & `talkytrend-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.4/README.md` & `talkytrend-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.4/pyproject.toml` & `talkytrend-1.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkytrend"
-version = "1.1.4"
+version = "1.1.5"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.1.4/talkytrend/config.py` & `talkytrend-1.1.5/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.4/talkytrend/default_settings.toml` & `talkytrend-1.1.5/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.1.4/talkytrend/main.py` & `talkytrend-1.1.5/talkytrend/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         while True:
             tasks = [self.check_signal()]
             tasks.append(self.fetch_key_events())
             tasks.append(self.fetch_key_news())
             results = await asyncio.gather(*tasks)
             if results[0] is not None:
                 print("Key signal:", results[0])
-                yield results[0]
+                return results[0]
             if results[1] is not None:
                 print("Key event:", results[1])
-                yield results[1]
+                return results[1]
             if results[2] is not None:
                 print("Key news:", results[2]["title"])
-                yield results[2]
+                return results[2]
             await asyncio.sleep(settings.scanner_frequency)
```

### Comparing `talkytrend-1.1.4/PKG-INFO` & `talkytrend-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.1.4
+Version: 1.1.5
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

