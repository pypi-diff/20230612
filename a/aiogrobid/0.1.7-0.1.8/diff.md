# Comparing `tmp/aiogrobid-0.1.7.tar.gz` & `tmp/aiogrobid-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogrobid-0.1.7.tar", last modified: Fri May 26 08:01:18 2023, max compression
+gzip compressed data, was "aiogrobid-0.1.8.tar", last modified: Mon Jun 12 18:03:33 2023, max compression
```

## Comparing `aiogrobid-0.1.7.tar` & `aiogrobid-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 08:01:18.346362 aiogrobid-0.1.7/
--rw-r--r--   0 pasha      (501) staff       (20)     1063 2022-10-25 06:23:08.000000 aiogrobid-0.1.7/LICENSE
--rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-05-26 08:01:18.346496 aiogrobid-0.1.7/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)     2910 2022-10-25 06:23:08.000000 aiogrobid-0.1.7/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 08:01:18.343148 aiogrobid-0.1.7/aiogrobid/
--rw-r--r--   0 pasha      (501) staff       (20)       61 2022-10-25 06:23:08.000000 aiogrobid-0.1.7/aiogrobid/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)      397 2023-05-26 07:44:21.000000 aiogrobid-0.1.7/aiogrobid/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     3742 2023-05-26 08:01:05.000000 aiogrobid-0.1.7/aiogrobid/client.py
--rw-r--r--   0 pasha      (501) staff       (20)       91 2022-10-25 06:23:08.000000 aiogrobid-0.1.7/aiogrobid/exceptions.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-05-26 08:01:18.346061 aiogrobid-0.1.7/aiogrobid.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-05-26 08:01:18.000000 aiogrobid-0.1.7/aiogrobid.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      325 2023-05-26 08:01:18.000000 aiogrobid-0.1.7/aiogrobid.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-05-26 08:01:18.000000 aiogrobid-0.1.7/aiogrobid.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       50 2023-05-26 08:01:18.000000 aiogrobid-0.1.7/aiogrobid.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       59 2023-05-26 08:01:18.000000 aiogrobid-0.1.7/aiogrobid.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)       10 2023-05-26 08:01:18.000000 aiogrobid-0.1.7/aiogrobid.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiogrobid-0.1.7/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      613 2023-05-26 08:01:18.347146 aiogrobid-0.1.7/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:03:33.800284 aiogrobid-0.1.8/
+-rw-r--r--   0 pasha      (501) staff       (20)     1063 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/LICENSE
+-rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-06-12 18:03:33.800583 aiogrobid-0.1.8/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)     2910 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:03:33.796749 aiogrobid-0.1.8/aiogrobid/
+-rw-r--r--   0 pasha      (501) staff       (20)       61 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/aiogrobid/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)      396 2023-05-29 06:48:15.000000 aiogrobid-0.1.8/aiogrobid/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     3765 2023-06-12 17:59:03.000000 aiogrobid-0.1.8/aiogrobid/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)       91 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/aiogrobid/exceptions.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-06-12 18:03:33.799919 aiogrobid-0.1.8/aiogrobid.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     3142 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      325 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       50 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       59 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       10 2023-06-12 18:03:33.000000 aiogrobid-0.1.8/aiogrobid.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       89 2022-10-25 06:23:08.000000 aiogrobid-0.1.8/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      613 2023-06-12 18:03:33.801494 aiogrobid-0.1.8/setup.cfg
```

### Comparing `aiogrobid-0.1.7/LICENSE` & `aiogrobid-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogrobid-0.1.7/PKG-INFO` & `aiogrobid-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogrobid
-Version: 0.1.7
+Version: 0.1.8
 Home-page: https://github.com/izihawa/aiogrobid
 Author: Pasha Podolsky
 License: MIT
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogrobid-0.1.7/README.md` & `aiogrobid-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aiogrobid-0.1.7/aiogrobid/client.py` & `aiogrobid-0.1.8/aiogrobid/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from aiobaseclient import BaseClient
 from lxml import etree
 
-from .exceptions import BadRequestError
+from exceptions import BadRequestError
 
 
 class GrobidClient(BaseClient):
     def __init__(self, base_url):
         super().__init__(base_url=base_url)
 
     def _get_text_for_one(self, root, name):
@@ -52,17 +52,17 @@
             if pers_name is not None:
                 surname = pers_name.find('.//{http://www.tei-c.org/ns/1.0}surname')
                 forename = pers_name.find('.//{http://www.tei-c.org/ns/1.0}forename')
                 name = None
                 if surname is not None and forename is not None:
                     name = f"{surname.text.strip()}, {forename.text.strip()}"
                 else:
-                    if surname:
+                    if surname is not None:
                         name = surname.text.strip()
-                    if forename:
+                    if forename is not None:
                         name = forename.text.strip()
                 if name:
                     authors.append(name)
         return authors
 
     async def process_fulltext_document(self, pdf_file):
         return await self.post(
```

### Comparing `aiogrobid-0.1.7/aiogrobid.egg-info/PKG-INFO` & `aiogrobid-0.1.8/aiogrobid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogrobid
-Version: 0.1.7
+Version: 0.1.8
 Home-page: https://github.com/izihawa/aiogrobid
 Author: Pasha Podolsky
 License: MIT
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aiogrobid-0.1.7/setup.cfg` & `aiogrobid-0.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 classifiers = 
 	Topic :: Utilities
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = aiogrobid
 python_requires = '>=3.8',
-version = 0.1.7
+version = 0.1.8
 url = https://github.com/izihawa/aiogrobid
 
 [options]
 packages = find:
 install_requires = 
 	aiobaseclient >= 0.2.4
 	fire >= 0.3.1
```

