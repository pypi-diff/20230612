# Comparing `tmp/gulagcleaner-0.6.2.tar.gz` & `tmp/gulagcleaner-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulagcleaner-0.6.2.tar", last modified: Mon Jun 12 19:46:42 2023, max compression
+gzip compressed data, was "gulagcleaner-0.6.3.tar", last modified: Mon Jun 12 19:58:04 2023, max compression
```

## Comparing `gulagcleaner-0.6.2.tar` & `gulagcleaner-0.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 19:46:42.747641 gulagcleaner-0.6.2/
--rw-rw-rw-   0        0        0    71644 2023-06-12 15:18:46.000000 gulagcleaner-0.6.2/LICENSE
--rw-rw-rw-   0        0        0     3072 2023-06-12 19:46:42.747641 gulagcleaner-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     2528 2023-06-12 19:45:14.000000 gulagcleaner-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 19:46:42.728641 gulagcleaner-0.6.2/gulagcleaner/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:18:46.000000 gulagcleaner-0.6.2/gulagcleaner/__init__.py
--rw-rw-rw-   0        0        0     3115 2023-06-12 19:45:40.000000 gulagcleaner-0.6.2/gulagcleaner/command_line.py
--rw-rw-rw-   0        0        0      228 2023-06-12 19:36:30.000000 gulagcleaner-0.6.2/gulagcleaner/decrypt.py
--rw-rw-rw-   0        0        0     4688 2023-06-12 19:36:30.000000 gulagcleaner-0.6.2/gulagcleaner/extract.py
--rw-rw-rw-   0        0        0      968 2023-06-12 19:36:30.000000 gulagcleaner-0.6.2/gulagcleaner/metadata.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:46:42.746640 gulagcleaner-0.6.2/gulagcleaner.egg-info/
--rw-rw-rw-   0        0        0     3072 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 19:46:42.000000 gulagcleaner-0.6.2/gulagcleaner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 15:18:46.000000 gulagcleaner-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      834 2023-06-12 19:46:42.749641 gulagcleaner-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 19:58:04.316753 gulagcleaner-0.6.3/
+-rw-rw-rw-   0        0        0    71644 2023-06-12 15:18:46.000000 gulagcleaner-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0     3072 2023-06-12 19:58:04.317758 gulagcleaner-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2528 2023-06-12 19:45:14.000000 gulagcleaner-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 19:58:04.294753 gulagcleaner-0.6.3/gulagcleaner/
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:18:46.000000 gulagcleaner-0.6.3/gulagcleaner/__init__.py
+-rw-rw-rw-   0        0        0     3147 2023-06-12 19:57:03.000000 gulagcleaner-0.6.3/gulagcleaner/command_line.py
+-rw-rw-rw-   0        0        0      228 2023-06-12 19:36:30.000000 gulagcleaner-0.6.3/gulagcleaner/decrypt.py
+-rw-rw-rw-   0        0        0     4688 2023-06-12 19:36:30.000000 gulagcleaner-0.6.3/gulagcleaner/extract.py
+-rw-rw-rw-   0        0        0      968 2023-06-12 19:36:30.000000 gulagcleaner-0.6.3/gulagcleaner/metadata.py
+drwxrwxrwx   0        0        0        0 2023-06-12 19:58:04.315753 gulagcleaner-0.6.3/gulagcleaner.egg-info/
+-rw-rw-rw-   0        0        0     3072 2023-06-12 19:58:04.000000 gulagcleaner-0.6.3/gulagcleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-06-12 19:58:04.000000 gulagcleaner-0.6.3/gulagcleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 19:58:04.000000 gulagcleaner-0.6.3/gulagcleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-12 19:58:04.000000 gulagcleaner-0.6.3/gulagcleaner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-06-12 19:58:04.000000 gulagcleaner-0.6.3/gulagcleaner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 19:58:04.000000 gulagcleaner-0.6.3/gulagcleaner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 15:18:46.000000 gulagcleaner-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0      834 2023-06-12 19:58:04.318755 gulagcleaner-0.6.3/setup.cfg
```

### Comparing `gulagcleaner-0.6.2/LICENSE` & `gulagcleaner-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.6.2/PKG-INFO` & `gulagcleaner-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.6.2
+Version: 0.6.3
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gulagcleaner-0.6.2/README.md` & `gulagcleaner-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.6.2/gulagcleaner/command_line.py` & `gulagcleaner-0.6.3/gulagcleaner/command_line.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         print("  -r            Replace the original file with the cleaned file.")
         print("  -o            Use the old cleaning method (for files older than 18/05/2023).")
         print("  -v            Show the version of the program.")
         return
 
     # Check for the -v argument
     if '-v' in sys.argv:
-        print("Current version: 0.6.2")
+        print("Current version: 0.6.3")
         return
 
     # Get the pdf_path argument
     if len(sys.argv) < 2:
         print('Usage: gulagcleaner [-h] [-r] [-o] [-v] <pdf_path>')
         return
     pdf_path = sys.argv[-1]
@@ -60,19 +60,18 @@
      # Check if the -o argument is present
     if '-o' in sys.argv:
         method = "old"
         pdf_path = decrypt_pdf(pdf_path)
         intermediate = True
     else:
         method = "new"
+        intermediate = False
     
     # Call the cleaning function
     return_msg = clean_pdf(pdf_path, output_path, method)
-    if intermediate:
-        os.remove(pdf_path)
 
     if return_msg["Success"]:
         print("Cleaning successful. File saved in", return_msg["return_path"])
         try:
             metadict = extract_metadata(pdf_path)
             print("Metadata:")
             print("Archivo: " + metadict["Archivo"])
@@ -82,9 +81,12 @@
             print("Facultad: " + metadict["Facultad"])
             print("Universidad: " + metadict["Universidad"])
         except Exception as e:
             print("Failed to extract metadata:", e)            
     else:
         print("Error:", return_msg["Error"])
 
+    if intermediate:
+        os.remove(pdf_path)
+
 if __name__ == "__main__":
     print('Call from the "gulagcleaner" command.')
```

### Comparing `gulagcleaner-0.6.2/gulagcleaner/extract.py` & `gulagcleaner-0.6.3/gulagcleaner/extract.py`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.6.2/gulagcleaner/metadata.py` & `gulagcleaner-0.6.3/gulagcleaner/metadata.py`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.6.2/gulagcleaner.egg-info/PKG-INFO` & `gulagcleaner-0.6.3/gulagcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.6.2
+Version: 0.6.3
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gulagcleaner-0.6.2/setup.cfg` & `gulagcleaner-0.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 756c 6167 636c 6561 6e65 720d   = gulagcleaner.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e36 2e32  .version = 0.6.2
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e36 2e33  .version = 0.6.3
 00000030: 0d0a 6175 7468 6f72 203d 2059 4d31 3632  ..author = YM162
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2064 6176 6964 2e66 6f6e 7461 6e65 6461   david.fontaneda
 00000060: 3136 4067 6d61 696c 2e63 6f6d 0d0a 6465  16@gmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4164 2072  scription = Ad r
 00000080: 656d 6f76 616c 2074 6f6f 6c20 666f 7220  emoval tool for 
 00000090: 5044 4673 2077 7269 7474 656e 2069 6e20  PDFs written in
```

