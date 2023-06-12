# Comparing `tmp/gulagcleaner-0.6.1.tar.gz` & `tmp/gulagcleaner-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulagcleaner-0.6.1.tar", last modified: Mon Jun 12 19:40:34 2023, max compression
+gzip compressed data, was "gulagcleaner-0.6.2.tar", last modified: Mon Jun 12 19:46:42 2023, max compression
```

## Comparing `gulagcleaner-0.6.1.tar` & `gulagcleaner-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 19:40:34.274349 gulagcleaner-0.6.1/
--rw-rw-rw-   0        0        0    71644 2023-06-12 15:18:46.000000 gulagcleaner-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     3016 2023-06-12 19:40:34.275347 gulagcleaner-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 19:40:34.246346 gulagcleaner-0.6.1/gulagcleaner/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:18:46.000000 gulagcleaner-0.6.1/gulagcleaner/__init__.py
--rw-rw-rw-   0        0        0     3114 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/command_line.py
--rw-rw-rw-   0        0        0      228 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/decrypt.py
--rw-rw-rw-   0        0        0     4688 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/extract.py
--rw-rw-rw-   0        0        0      968 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/metadata.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:40:34.273347 gulagcleaner-0.6.1/gulagcleaner.egg-info/
--rw-rw-rw-   0        0        0     3016 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 15:18:46.000000 gulagcleaner-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0      834 2023-06-12 19:40:34.281348 gulagcleaner-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 19:46:42.747641 gulagcleaner-0.6.2/
+-rw-rw-rw-   0        0        0    71644 2023-06-12 15:18:46.000000 gulagcleaner-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     3072 2023-06-12 19:46:42.747641 gulagcleaner-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2528 2023-06-12 19:45:14.000000 gulagcleaner-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 19:46:42.728641 gulagcleaner-0.6.2/gulagcleaner/
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:18:46.000000 gulagcleaner-0.6.2/gulagcleaner/__init__.py
+-rw-rw-rw-   0        0        0     3115 2023-06-12 19:45:40.000000 gulagcleaner-0.6.2/gulagcleaner/command_line.py
+-rw-rw-rw-   0        0        0      228 2023-06-12 19:36:30.000000 gulagcleaner-0.6.2/gulagcleaner/decrypt.py
+-rw-rw-rw-   0        0        0     4688 2023-06-12 19:36:30.000000 gulagcleaner-0.6.2/gulagcleaner/extract.py
+-rw-rw-rw-   0        0        0      968 2023-06-12 19:36:30.000000 gulagcleaner-0.6.2/gulagcleaner/metadata.py
+drwxrwxrwx   0        0        0        0 2023-06-12 19:46:42.746640 gulagcleaner-0.6.2/gulagcleaner.egg-info/
+-rw-rw-rw-   0        0        0     3072 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 15:18:46.000000 gulagcleaner-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      834 2023-06-12 19:46:42.749641 gulagcleaner-0.6.2/setup.cfg
```

### Comparing `gulagcleaner-0.6.1/LICENSE` & `gulagcleaner-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.6.1/PKG-INFO` & `gulagcleaner-0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.6.1
+Version: 0.6.2
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 
 In addition to removing advertisements, Gulag Cleaner is also capable of extracting metadata, such as the author, subject, university, and more, from the file.
 
 # Web Version
 
 This tool can be used without installation directly from [our website](https://gulagcleaner.com) (in Spanish).
 
-[![Gulag Cleaner webpage](./assets/web_mockup.png)](https://gulagcleaner.com)
+[![Gulag Cleaner webpage](https://raw.githubusercontent.com/YM162/gulagcleaner/main/assets/web_mockup.png)](https://gulagcleaner.com)
 
 # Installation
 
 To install Gulag Cleaner, please [download](https://www.python.org/downloads/) and [install](https://wiki.python.org/moin/BeginnersGuide/Download) Python and then run the following command in your terminal:
 ```
 pip install gulagcleaner
 ```
```

### Comparing `gulagcleaner-0.6.1/README.md` & `gulagcleaner-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 In addition to removing advertisements, Gulag Cleaner is also capable of extracting metadata, such as the author, subject, university, and more, from the file.
 
 # Web Version
 
 This tool can be used without installation directly from [our website](https://gulagcleaner.com) (in Spanish).
 
-[![Gulag Cleaner webpage](./assets/web_mockup.png)](https://gulagcleaner.com)
+[![Gulag Cleaner webpage](https://raw.githubusercontent.com/YM162/gulagcleaner/main/assets/web_mockup.png)](https://gulagcleaner.com)
 
 # Installation
 
 To install Gulag Cleaner, please [download](https://www.python.org/downloads/) and [install](https://wiki.python.org/moin/BeginnersGuide/Download) Python and then run the following command in your terminal:
 ```
 pip install gulagcleaner
 ```
```

### Comparing `gulagcleaner-0.6.1/gulagcleaner/command_line.py` & `gulagcleaner-0.6.2/gulagcleaner/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         print("  -r            Replace the original file with the cleaned file.")
         print("  -o            Use the old cleaning method (for files older than 18/05/2023).")
         print("  -v            Show the version of the program.")
         return
 
     # Check for the -v argument
     if '-v' in sys.argv:
-        print("Actual version: 0.6.1")
+        print("Current version: 0.6.2")
         return
 
     # Get the pdf_path argument
     if len(sys.argv) < 2:
         print('Usage: gulagcleaner [-h] [-r] [-o] [-v] <pdf_path>')
         return
     pdf_path = sys.argv[-1]
```

### Comparing `gulagcleaner-0.6.1/gulagcleaner/extract.py` & `gulagcleaner-0.6.2/gulagcleaner/extract.py`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.6.1/gulagcleaner/metadata.py` & `gulagcleaner-0.6.2/gulagcleaner/metadata.py`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.6.1/gulagcleaner.egg-info/PKG-INFO` & `gulagcleaner-0.6.2/gulagcleaner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.6.1
+Version: 0.6.2
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 
 In addition to removing advertisements, Gulag Cleaner is also capable of extracting metadata, such as the author, subject, university, and more, from the file.
 
 # Web Version
 
 This tool can be used without installation directly from [our website](https://gulagcleaner.com) (in Spanish).
 
-[![Gulag Cleaner webpage](./assets/web_mockup.png)](https://gulagcleaner.com)
+[![Gulag Cleaner webpage](https://raw.githubusercontent.com/YM162/gulagcleaner/main/assets/web_mockup.png)](https://gulagcleaner.com)
 
 # Installation
 
 To install Gulag Cleaner, please [download](https://www.python.org/downloads/) and [install](https://wiki.python.org/moin/BeginnersGuide/Download) Python and then run the following command in your terminal:
 ```
 pip install gulagcleaner
 ```
```

### Comparing `gulagcleaner-0.6.1/setup.cfg` & `gulagcleaner-0.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 756c 6167 636c 6561 6e65 720d   = gulagcleaner.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e36 2e31  .version = 0.6.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e36 2e32  .version = 0.6.2
 00000030: 0d0a 6175 7468 6f72 203d 2059 4d31 3632  ..author = YM162
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2064 6176 6964 2e66 6f6e 7461 6e65 6461   david.fontaneda
 00000060: 3136 4067 6d61 696c 2e63 6f6d 0d0a 6465  16@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4164 2072  scription = Ad r
 00000080: 656d 6f76 616c 2074 6f6f 6c20 666f 7220  emoval tool for 
 00000090: 5044 4673 2077 7269 7474 656e 2069 6e20  PDFs written in
```

