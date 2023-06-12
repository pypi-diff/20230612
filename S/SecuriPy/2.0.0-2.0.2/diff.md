# Comparing `tmp/SecuriPy-2.0.0.tar.gz` & `tmp/SecuriPy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-2.0.0.tar", last modified: Mon Jun 12 07:38:13 2023, max compression
+gzip compressed data, was "SecuriPy-2.0.2.tar", last modified: Mon Jun 12 17:42:47 2023, max compression
```

## Comparing `SecuriPy-2.0.0.tar` & `SecuriPy-2.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:38:13.889252 SecuriPy-2.0.0/
--rw-rw-rw-   0        0        0     2266 2023-06-12 07:38:13.888251 SecuriPy-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1647 2023-06-12 07:35:35.000000 SecuriPy-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 07:38:13.883247 SecuriPy-2.0.0/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     2266 2023-06-12 07:38:13.000000 SecuriPy-2.0.0/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-06-12 07:38:13.000000 SecuriPy-2.0.0/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:38:13.000000 SecuriPy-2.0.0/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 07:38:13.000000 SecuriPy-2.0.0/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6866 2023-06-12 07:29:34.000000 SecuriPy-2.0.0/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 07:38:13.890249 SecuriPy-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-06-12 07:37:49.000000 SecuriPy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:47.191832 SecuriPy-2.0.2/
+-rw-rw-rw-   0        0        0     2266 2023-06-12 17:42:47.189534 SecuriPy-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1647 2023-06-12 07:35:35.000000 SecuriPy-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:47.188122 SecuriPy-2.0.2/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     2266 2023-06-12 17:42:46.000000 SecuriPy-2.0.2/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-06-12 17:42:46.000000 SecuriPy-2.0.2/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 17:42:46.000000 SecuriPy-2.0.2/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 17:42:46.000000 SecuriPy-2.0.2/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6857 2023-06-12 17:41:55.000000 SecuriPy-2.0.2/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 17:42:47.191832 SecuriPy-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-06-12 17:42:31.000000 SecuriPy-2.0.2/setup.py
```

### Comparing `SecuriPy-2.0.0/PKG-INFO` & `SecuriPy-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 2.0.0
+Version: 2.0.2
 Summary: Encrypter and Decrypter of all types of human-readable file formats Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-2.0.0/README.md` & `SecuriPy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-2.0.0/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-2.0.2/SecuriPy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 2.0.0
+Version: 2.0.2
 Summary: Encrypter and Decrypter of all types of human-readable file formats Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-2.0.0/SecuriPy.py` & `SecuriPy-2.0.2/SecuriPy.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
         key = Text.pwd(message, password)
         encrypted_text = []
         for i in range(len(message)):
             x = (ord(message[i]) +ord(key[i]) + 1000)
             encrypted_text.append(chr(x))
         encrypted_text = ("" . join(encrypted_text))
         key = ("".join(key))
-        return encrypted_text + "\x00" + key
+        return encrypted_text + " " + key
 
     @staticmethod
     def decrypt(text, password):
         """Figures out the key from the encrypted text and decryptes it with respect to the key"""
         orig_text = []
-        encrypted_text = text.split("\x00")[0]
+        encrypted_text = text.split(" ")[0]
         key = Text.pwd(encrypted_text, password)
-        if key == text.split("\x00")[1]:
+        if key == text.split(" ")[1]:
             for i in range(len(encrypted_text)):
                 x = (ord(encrypted_text[i]) -ord(key[i]) - 1000)
                 orig_text.append(chr(x))
             orig_text = ("" . join(orig_text))
             return orig_text[:-1]
         else:
             return "Message is corrupt or Password is incorrect"
```

### Comparing `SecuriPy-2.0.0/setup.py` & `SecuriPy-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="2.0.0",
+    version="2.0.2",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of all types of human-readable file formats Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

