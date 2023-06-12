# Comparing `tmp/gulagcleaner-0.5.2.tar.gz` & `tmp/gulagcleaner-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulagcleaner-0.5.2.tar", last modified: Wed May 31 22:42:56 2023, max compression
+gzip compressed data, was "gulagcleaner-0.6.1.tar", last modified: Mon Jun 12 19:40:34 2023, max compression
```

## Comparing `gulagcleaner-0.5.2.tar` & `gulagcleaner-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:42:56.117352 gulagcleaner-0.5.2/
--rw-rw-rw-   0        0        0    71644 2023-02-12 15:01:11.000000 gulagcleaner-0.5.2/LICENSE
--rw-rw-rw-   0        0        0     2437 2023-05-31 22:42:56.117352 gulagcleaner-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2023-05-31 21:58:02.000000 gulagcleaner-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:42:56.087160 gulagcleaner-0.5.2/gulagcleaner/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:01:11.000000 gulagcleaner-0.5.2/gulagcleaner/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-05-31 22:41:03.000000 gulagcleaner-0.5.2/gulagcleaner/command_line.py
--rw-rw-rw-   0        0        0     5926 2023-05-31 22:40:26.000000 gulagcleaner-0.5.2/gulagcleaner/gulagcleaner_extract.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:42:56.115474 gulagcleaner-0.5.2/gulagcleaner.egg-info/
--rw-rw-rw-   0        0        0     2437 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-02-12 15:01:11.000000 gulagcleaner-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0      857 2023-05-31 22:42:56.120348 gulagcleaner-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 19:40:34.274349 gulagcleaner-0.6.1/
+-rw-rw-rw-   0        0        0    71644 2023-06-12 15:18:46.000000 gulagcleaner-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     3016 2023-06-12 19:40:34.275347 gulagcleaner-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2472 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 19:40:34.246346 gulagcleaner-0.6.1/gulagcleaner/
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:18:46.000000 gulagcleaner-0.6.1/gulagcleaner/__init__.py
+-rw-rw-rw-   0        0        0     3114 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/command_line.py
+-rw-rw-rw-   0        0        0      228 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/decrypt.py
+-rw-rw-rw-   0        0        0     4688 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/extract.py
+-rw-rw-rw-   0        0        0      968 2023-06-12 19:36:30.000000 gulagcleaner-0.6.1/gulagcleaner/metadata.py
+drwxrwxrwx   0        0        0        0 2023-06-12 19:40:34.273347 gulagcleaner-0.6.1/gulagcleaner.egg-info/
+-rw-rw-rw-   0        0        0     3016 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-12 19:40:34.000000 gulagcleaner-0.6.1/gulagcleaner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 15:18:46.000000 gulagcleaner-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0      834 2023-06-12 19:40:34.281348 gulagcleaner-0.6.1/setup.cfg
```

### Comparing `gulagcleaner-0.5.2/LICENSE` & `gulagcleaner-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.5.2/PKG-INFO` & `gulagcleaner-0.6.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,79 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.5.2
+Version: 0.6.1
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
-Author: YM162,KosmicKatXV,pgalinanes
+Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # Gulag Cleaner
 
+
+[![Twitter](https://a11ybadges.com/badge?logo=twitter)](https://twitter.com/gulagcleaner)
+[![Instagram](https://a11ybadges.com/badge?logo=instagram)](https://www.instagram.com/gulagcleaner/)
+[![Ko-fi](https://a11ybadges.com/badge?logo=kofi)](https://ko-fi.com/L3L86VEX9)
+
+
 Gulag Cleaner is a tool designed to remove advertisements from PDFs, making it easier to read and navigate documents without being disrupted by unwanted ads.
 
 This tool does not just crop the ads out of the PDF, instead, we extract the original file without ads by manipulating the internal structure of the PDF, ensuring maximum quality.
 
 In addition to removing advertisements, Gulag Cleaner is also capable of extracting metadata, such as the author, subject, university, and more, from the file.
 
-## Installation
+# Web Version
 
-To install Gulag Cleaner, simply run the following command in your terminal:
+This tool can be used without installation directly from [our website](https://gulagcleaner.com) (in Spanish).
+
+[![Gulag Cleaner webpage](./assets/web_mockup.png)](https://gulagcleaner.com)
+
+# Installation
+
+To install Gulag Cleaner, please [download](https://www.python.org/downloads/) and [install](https://wiki.python.org/moin/BeginnersGuide/Download) Python and then run the following command in your terminal:
 ```
 pip install gulagcleaner
 ```
 
-## Usage
+# Usage
 
 Gulag Cleaner can be used through both a Command Line Interface (CLI) and in your code.
 
-### Command Line Interface
+## Command Line Interface
 
 To use Gulag Cleaner through the CLI, simply run the following command, replacing `<filename>` with the name of your PDF file:
 
 ```
 gulagcleaner [-r] [-h] [-o] [-v] <filename>
 ```
 
-### Code
+## Options
 
-To use Gulag Cleaner in your code, you can use the following code snippet:
+Gulag Cleaner provides several options for its usage:
 
-```python
-from gulagcleaner.gulagcleaner_extract import deembed
+> * '-r': Replace the original file with the cleaned version.
+> * '-o': Use the old cleaning method (for files older than 18/05/2023).
+> * '-h': Display the help message, providing information on how to use Gulag Cleaner.
+> * '-v': Display the current version of Gulag Cleaner.
 
-return_msg = deembed("file.pdf")
-```
+## Code
 
-## Options
+To use Gulag Cleaner in your code, you can use the following code snippet:
 
-Gulag Cleaner provides several options for it's usage:
+```python
+from gulagcleaner.extract import clean_pdf
 
-> * '-r': Replaces the original file with the cleaned version.
-> * '-o': Uses the old deembeding method (for files older than 18/05/2023).
-> * '-h': Displays the help message, providing information on how to use Gulag Cleaner.
-> * '-v': Displays the current version of Gulag Cleaner.
+return_msg = clean_pdf("file.pdf")
+```
 
-## License
+# License
 Gulag Cleaner is distributed under the GPL-3 license, which means it's open-source and free to use.
 
-## Contributing
+# Contributing
 We're always looking for ways to improve Gulag Cleaner, and we welcome contributions from the community. If you have ideas for improvements or bug fixes, please feel free to submit a pull request.
```

### Comparing `gulagcleaner-0.5.2/gulagcleaner/gulagcleaner_extract.py` & `gulagcleaner-0.6.1/gulagcleaner/extract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,11 @@
-import os
-import pikepdf
-from pdfminer.high_level import extract_text
 from pdfrw import PdfReader, PdfWriter
 from pdfrw.findobjs import wrap_object, find_objects
 from pdfrw.objects import PdfName
 
-def extract_metadata(pdf_path):
-    """
-    Extract metadata from a PDF file, including the author, subject, course and grade, faculty, and university.
-
-    Args:
-        pdf_path (str): The path to the pdf file.
-
-    Returns:
-        metadict (dict): A dictionary with the following keys and values:
-            "Archivo": (str) File name.
-            "Autor": (str) Author of the file.
-            "Asignatura": (str) Subject.
-            "Curso y Grado": (str) Course and degree.
-            "Facultad": (str) Faculty.
-            "Universidad": (str) University.
-    """
-    text = extract_text(pdf_path, maxpages=1)
-    metalist = list(filter(None, text.splitlines()))
-    return {
-        "Archivo": metalist[0],
-        "Autor": metalist[1],
-        "Asignatura": metalist[2],
-        "Curso y Grado": metalist[3],
-        "Facultad": metalist[4],
-        "Universidad": metalist[5]
-    }
-
 def find_iobj_pairs(first_page, second_page):
     """
     Finds the indirect objects that repeat between pages.
 
     Args:
         first_page (PDFPage): The first page.
         second_page (PDFPage): The second page.
@@ -47,68 +17,59 @@
     """
     comunes = tuple(set(first_page).intersection(second_page))
     if first_page.index(comunes[0]) < first_page.index(comunes[1]):
         return (first_page,first_page.index(comunes[0]))
     else:
         return (first_page,first_page.index(comunes[1]))
     
-def deembed(pdf_path, replace=False, method="new"):
+def clean_pdf(pdf_path, output_path="", method="new"):
     """
     De-embeds the PDF file and creates a new PDF file in the same folder with each embedded page in a new page.
 
     Args:
         pdf_path (str): The path to the PDF file.
-        replace (bool, optional): If set to True, the original file will be replaced by the de-embedded file.
-            Default is False.
-        method (str, optional): Defines what strategy will be used to deembed the pdf file. Can be "old" or "new".
-            Default if "new".
+        output_path (str): The path to the output PDF file.
+        method (str, optional): Defines what strategy will be used to clean the pdf file. Can be "new", "old" or "naive".
+            Default is "new".
 
     Returns:
         return_msg (dict): A dictionary with the following keys:
             success (bool): Indicates whether the de-embedding process was successful.
             return_path (str): The path to the de-embedded file if successful.
             error (str): An error description if the process was unsuccessful.
-            meta (dict): Information about the file including "Archivo", "Autor", "Asignatura", "Curso y Grado", "Facultad", and "Universidad".
     """
+
     if not pdf_path.endswith(".pdf"):
         return {
             "Success": False,
             "return_path": "",
             "Error": "File is not a .pdf file.",
-            "Meta": {}
         }
 
-    intermediate_pdf_path = pdf_path[:-4] + "_inter.pdf"
-    try:
-        # We remove the decryption in the pdf streams 
-        # This is not always necesary, maybe add a check to see if the file is encrypted?
-        with pikepdf.Pdf.open(pdf_path) as pdf:
-            pdf.save(intermediate_pdf_path)
-
-        metadict = {}
-        try:
-            metadict = extract_metadata(pdf_path)
-        except Exception as e:
-            print("Failed to extract metadata:", e)
+    if output_path == "":
+        output_path = pdf_path[:-4] + "_clean.pdf"
 
-        pdf = PdfReader(intermediate_pdf_path)
+    try:
+        pdf = PdfReader(pdf_path)
 
+        # Old method, for files older than 18/05/2023. Works by finding the embedded pages and creating new pages with them.
         if method=="old":
-            xobjs = list(find_objects(pdf.pages, valid_subtypes=(PdfName.Form, PdfName.Dummy)))
+            xobjs = []
+            for page in pdf.pages:
+                xobjs.extend([page.Resources.XObject[object] for object in page.Resources.XObject if "EmbeddedPdfPage" in str(object)])
             newpages = [wrap_object(item, 1000, 0.5 * 72) for item in xobjs]
 
             if not xobjs:
-                os.remove(intermediate_pdf_path)
                 return {
                     "Success": False,
                     "return_path": "",
-                    "Error": "No embedded pages found.",
-                    "Meta": metadict
+                    "Error": "No embedded pages found."
                 }
             
+        # New method, for files newer than 18/05/2023. Works by finding the repeating indirect objects between pages and creating new pages with them.
         elif method=="new":
             content_list = []
             for page in pdf.pages:
                 content = [content.indirect for content in page.Contents]
                 if len(content)>1:
                     content_list.append(content)
 
@@ -122,37 +83,37 @@
 
             newpages = []
             for i,page in enumerate([page for page in pdf.pages if len(page.Contents)>1]):
                 newpage = page.copy()
                 newpage.Contents = [pdf.indirect_objects[iobj] for iobj in new_contents[i]]
                 newpage.Annots = []
                 newpages.append(newpage)
+
+        #Naive method. Just detects the pages with ads and crops them. THIS METHOD IS NOT RECOMENDED AT ALL. It is very unreliable and when copying text from the outputed pdf the ads and watermaks are copied as well, because we are just "hiding" them from the user, not truly removing them.
+        elif method=="naive":
+            #Not yet implemented.
+            newpages = []
+
         else:
-            os.remove(intermediate_pdf_path)
             return {
                 "Success": False,
                 "return_path": "",
-                "Error": "Deembeding method not found.",
-                "Meta": metadict
+                "Error": "Cleaning method not found."
             }
         
-        output = pdf_path[:-4] + (".pdf" if replace else "_clean.pdf")
-        writer = PdfWriter(output)
+        writer = PdfWriter(output_path)
         writer.addpages(newpages)
         writer.write()
 
-        os.rename(output, output.replace('wuolah-free-', ''))
-        os.remove(intermediate_pdf_path)
-
         return {
             "Success": True,
-            "return_path": output,
-            "Error": "",
-            "Meta": metadict
-        }
+            "return_path": output_path,
+            "Error": ""
+            }
+    
     except Exception as e:
         return {
             "Success": False,
             "return_path": "",
             "Error": str(e),
             "Meta": {}
         }
```

### Comparing `gulagcleaner-0.5.2/gulagcleaner.egg-info/PKG-INFO` & `gulagcleaner-0.6.1/gulagcleaner.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,79 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.5.2
+Version: 0.6.1
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
-Author: YM162,KosmicKatXV,pgalinanes
+Author: YM162
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # Gulag Cleaner
 
+
+[![Twitter](https://a11ybadges.com/badge?logo=twitter)](https://twitter.com/gulagcleaner)
+[![Instagram](https://a11ybadges.com/badge?logo=instagram)](https://www.instagram.com/gulagcleaner/)
+[![Ko-fi](https://a11ybadges.com/badge?logo=kofi)](https://ko-fi.com/L3L86VEX9)
+
+
 Gulag Cleaner is a tool designed to remove advertisements from PDFs, making it easier to read and navigate documents without being disrupted by unwanted ads.
 
 This tool does not just crop the ads out of the PDF, instead, we extract the original file without ads by manipulating the internal structure of the PDF, ensuring maximum quality.
 
 In addition to removing advertisements, Gulag Cleaner is also capable of extracting metadata, such as the author, subject, university, and more, from the file.
 
-## Installation
+# Web Version
 
-To install Gulag Cleaner, simply run the following command in your terminal:
+This tool can be used without installation directly from [our website](https://gulagcleaner.com) (in Spanish).
+
+[![Gulag Cleaner webpage](./assets/web_mockup.png)](https://gulagcleaner.com)
+
+# Installation
+
+To install Gulag Cleaner, please [download](https://www.python.org/downloads/) and [install](https://wiki.python.org/moin/BeginnersGuide/Download) Python and then run the following command in your terminal:
 ```
 pip install gulagcleaner
 ```
 
-## Usage
+# Usage
 
 Gulag Cleaner can be used through both a Command Line Interface (CLI) and in your code.
 
-### Command Line Interface
+## Command Line Interface
 
 To use Gulag Cleaner through the CLI, simply run the following command, replacing `<filename>` with the name of your PDF file:
 
 ```
 gulagcleaner [-r] [-h] [-o] [-v] <filename>
 ```
 
-### Code
+## Options
 
-To use Gulag Cleaner in your code, you can use the following code snippet:
+Gulag Cleaner provides several options for its usage:
 
-```python
-from gulagcleaner.gulagcleaner_extract import deembed
+> * '-r': Replace the original file with the cleaned version.
+> * '-o': Use the old cleaning method (for files older than 18/05/2023).
+> * '-h': Display the help message, providing information on how to use Gulag Cleaner.
+> * '-v': Display the current version of Gulag Cleaner.
 
-return_msg = deembed("file.pdf")
-```
+## Code
 
-## Options
+To use Gulag Cleaner in your code, you can use the following code snippet:
 
-Gulag Cleaner provides several options for it's usage:
+```python
+from gulagcleaner.extract import clean_pdf
 
-> * '-r': Replaces the original file with the cleaned version.
-> * '-o': Uses the old deembeding method (for files older than 18/05/2023).
-> * '-h': Displays the help message, providing information on how to use Gulag Cleaner.
-> * '-v': Displays the current version of Gulag Cleaner.
+return_msg = clean_pdf("file.pdf")
+```
 
-## License
+# License
 Gulag Cleaner is distributed under the GPL-3 license, which means it's open-source and free to use.
 
-## Contributing
+# Contributing
 We're always looking for ways to improve Gulag Cleaner, and we welcome contributions from the community. If you have ideas for improvements or bug fixes, please feel free to submit a pull request.
```

### Comparing `gulagcleaner-0.5.2/setup.cfg` & `gulagcleaner-0.6.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 756c 6167 636c 6561 6e65 720d   = gulagcleaner.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e32  .version = 0.5.2
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e36 2e31  .version = 0.6.1
 00000030: 0d0a 6175 7468 6f72 203d 2059 4d31 3632  ..author = YM162
-00000040: 2c4b 6f73 6d69 634b 6174 5856 2c70 6761  ,KosmicKatXV,pga
-00000050: 6c69 6e61 6e65 730d 0a61 7574 686f 725f  linanes..author_
-00000060: 656d 6169 6c20 3d20 6461 7669 642e 666f  email = david.fo
-00000070: 6e74 616e 6564 6131 3640 676d 6169 6c2e  ntaneda16@gmail.
-00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
-00000090: 203d 2041 6420 7265 6d6f 7661 6c20 746f   = Ad removal to
-000000a0: 6f6c 2066 6f72 2050 4446 7320 7772 6974  ol for PDFs writ
-000000b0: 7465 6e20 696e 2070 7974 686f 6e2e 0d0a  ten in python...
-000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000d0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000e0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-000000f0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000100: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000110: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
-00000120: 2f67 6974 6875 622e 636f 6d2f 594d 3136  /github.com/YM16
-00000130: 322f 6775 6c61 672d 636c 6561 6e65 722d  2/gulag-cleaner-
-00000140: 636c 690d 0a70 726f 6a65 6374 5f75 726c  cli..project_url
-00000150: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000160: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-00000170: 6875 622e 636f 6d2f 594d 3136 322f 6775  hub.com/YM162/gu
-00000180: 6c61 672d 636c 6561 6e65 722d 636c 692f  lag-cleaner-cli/
-00000190: 6973 7375 6573 0d0a 636c 6173 7369 6669  issues..classifi
-000001a0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
-000001b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001c0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
-000001d0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001e0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001f0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-00000200: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000210: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
-00000220: 7074 696f 6e73 5d0d 0a69 6e73 7461 6c6c  ptions]..install
-00000230: 5f72 6571 7569 7265 7320 3d20 0d0a 0970  _requires = ...p
-00000240: 6466 7277 3e3d 302e 340d 0a09 7069 6b65  dfrw>=0.4...pike
-00000250: 7064 663e 3d35 2e31 2e32 0d0a 0970 6466  pdf>=5.1.2...pdf
-00000260: 6d69 6e65 722e 7369 783e 3d32 3032 3230  miner.six>=20220
-00000270: 3532 340d 0a70 6163 6b61 6765 7320 3d20  524..packages = 
-00000280: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000290: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
-000002a0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002b0: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
-000002c0: 6465 203d 200d 0a09 7465 7374 730d 0a0d  de = ...tests...
-000002d0: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-000002e0: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
-000002f0: 5f73 6372 6970 7473 203d 200d 0a09 6775  _scripts = ...gu
-00000300: 6c61 6763 6c65 616e 6572 203d 2067 756c  lagcleaner = gul
-00000310: 6167 636c 6561 6e65 722e 636f 6d6d 616e  agcleaner.comman
-00000320: 645f 6c69 6e65 3a6d 6169 6e0d 0a0d 0a5b  d_line:main....[
-00000330: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000340: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000350: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000050: 2064 6176 6964 2e66 6f6e 7461 6e65 6461   david.fontaneda
+00000060: 3136 4067 6d61 696c 2e63 6f6d 0d0a 6465  16@gmail.com..de
+00000070: 7363 7269 7074 696f 6e20 3d20 4164 2072  scription = Ad r
+00000080: 656d 6f76 616c 2074 6f6f 6c20 666f 7220  emoval tool for 
+00000090: 5044 4673 2077 7269 7474 656e 2069 6e20  PDFs written in 
+000000a0: 7079 7468 6f6e 2e0d 0a6c 6f6e 675f 6465  python...long_de
+000000b0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+000000c0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+000000d0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000000e0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+000000f0: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
+00000100: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000110: 2e63 6f6d 2f59 4d31 3632 2f67 756c 6167  .com/YM162/gulag
+00000120: 2d63 6c65 616e 6572 2d63 6c69 0d0a 7072  -cleaner-cli..pr
+00000130: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+00000140: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
+00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000160: 2f59 4d31 3632 2f67 756c 6167 2d63 6c65  /YM162/gulag-cle
+00000170: 616e 6572 2d63 6c69 2f69 7373 7565 730d  aner-cli/issues.
+00000180: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000190: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001b0: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+000001c0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001d0: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+000001e0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000001f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000200: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+00000210: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000220: 6573 203d 200d 0a09 7064 6672 773e 3d30  es = ...pdfrw>=0
+00000230: 2e34 0d0a 0970 696b 6570 6466 3e3d 352e  .4...pikepdf>=5.
+00000240: 312e 320d 0a09 7064 666d 696e 6572 2e73  1.2...pdfminer.s
+00000250: 6978 3e3d 3230 3232 3035 3234 0d0a 7061  ix>=20220524..pa
+00000260: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000270: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000280: 3d20 3e3d 332e 360d 0a0d 0a5b 6f70 7469  = >=3.6....[opti
+00000290: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000002a0: 645d 0d0a 6578 636c 7564 6520 3d20 0d0a  d]..exclude = ..
+000002b0: 0974 6573 7473 0d0a 0d0a 5b6f 7074 696f  .tests....[optio
+000002c0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
+000002d0: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
+000002e0: 7320 3d20 0d0a 0967 756c 6167 636c 6561  s = ...gulagclea
+000002f0: 6e65 7220 3d20 6775 6c61 6763 6c65 616e  ner = gulagclean
+00000300: 6572 2e63 6f6d 6d61 6e64 5f6c 696e 653a  er.command_line:
+00000310: 6d61 696e 0d0a 0d0a 5b65 6767 5f69 6e66  main....[egg_inf
+00000320: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000330: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000340: 0d0a                                     ..
```

