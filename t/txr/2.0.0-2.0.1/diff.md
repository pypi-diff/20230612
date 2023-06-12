# Comparing `tmp/txr-2.0.0-py3-none-any.whl.zip` & `tmp/txr-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 19511 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    18646 b- defN 23-Jun-12 08:51 txr.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-12 08:51 txr-2.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1873 b- defN 23-Jun-12 08:51 txr-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 08:51 txr-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       33 b- defN 23-Jun-12 08:51 txr-2.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-12 08:51 txr-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      521 b- defN 23-Jun-12 08:51 txr-2.0.0.dist-info/RECORD
-7 files, 56992 bytes uncompressed, 18595 bytes compressed:  67.4%
+Zip file size: 19500 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    18656 b- defN 23-Jun-12 08:54 txr.py
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-12 08:55 txr-2.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1883 b- defN 23-Jun-12 08:55 txr-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 08:55 txr-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       33 b- defN 23-Jun-12 08:55 txr-2.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-12 08:55 txr-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      521 b- defN 23-Jun-12 08:55 txr-2.0.1.dist-info/RECORD
+7 files, 57012 bytes uncompressed, 18584 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: txr.py
 Comment: 
 
-Filename: txr-2.0.0.dist-info/LICENSE
+Filename: txr-2.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: txr-2.0.0.dist-info/METADATA
+Filename: txr-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: txr-2.0.0.dist-info/WHEEL
+Filename: txr-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: txr-2.0.0.dist-info/entry_points.txt
+Filename: txr-2.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: txr-2.0.0.dist-info/top_level.txt
+Filename: txr-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: txr-2.0.0.dist-info/RECORD
+Filename: txr-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## txr.py

```diff
@@ -1,14 +1,14 @@
 __package_name__ = "txr"
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 __author__ = "Idan Miara"
 __author_email__ = "idan@miara.com"
 __license__ = "GPL3"
 __url__ = r"https://github.com/idanmiara/txr"
-__description__ = "Stylish merge/split files (tar-like with txt output)"
+__description__ = "TXR: The teXt aRchiver - archives text as text. and much more."
 
 import csv
 import hashlib
 import json
 import logging
 import os
 import sys
```

## Comparing `txr-2.0.0.dist-info/LICENSE` & `txr-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `txr-2.0.0.dist-info/METADATA` & `txr-2.0.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: txr
-Version: 2.0.0
-Summary: Stylish merge/split files (tar-like with txt output)
+Version: 2.0.1
+Summary: TXR: The teXt aRchiver - archives text as text. and much more.
 Home-page: https://github.com/idanmiara/txr
 Author: Idan Miara
 Author-email: idan@miara.com
 License: GPL3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: crypto
 Requires-Dist: cryptography ; extra == 'crypto'
 
-TXR: The TeXt aRchiver
+TXR: the teXt aRchiver
 ########################
 
 Mainly purposed for archiving text files as text files, but can archive any file and not only as text.
 `txr` was inspired by tar, gzip and gunzip.
 License: GPL v3 or later.
 
 The `txr` format is composed of two files with the following extensions:
```

