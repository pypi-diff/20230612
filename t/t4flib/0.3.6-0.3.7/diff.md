# Comparing `tmp/t4flib-0.3.6-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.3.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11040 bytes, number of entries: 12
+Zip file size: 11041 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-09 13:22 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
--rw-rw-r--  2.0 unx     6266 b- defN 23-Jun-12 10:26 t4flib/file_helper.py
+-rw-rw-r--  2.0 unx     6276 b- defN 23-Jun-12 12:02 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     5692 b- defN 23-Jun-12 08:53 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     2682 b- defN 23-May-30 14:55 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-30 14:21 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-Jun-12 10:38 t4flib-0.3.6.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 10:38 t4flib-0.3.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-12 10:38 t4flib-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      920 b- defN 23-Jun-12 10:38 t4flib-0.3.6.dist-info/RECORD
-12 files, 27777 bytes uncompressed, 9508 bytes compressed:  65.8%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-Jun-12 12:51 t4flib-0.3.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 12:51 t4flib-0.3.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-12 12:51 t4flib-0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      920 b- defN 23-Jun-12 12:51 t4flib-0.3.7.dist-info/RECORD
+12 files, 27787 bytes uncompressed, 9509 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.3.6.dist-info/METADATA
+Filename: t4flib-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.3.6.dist-info/WHEEL
+Filename: t4flib-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.3.6.dist-info/top_level.txt
+Filename: t4flib-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.3.6.dist-info/RECORD
+Filename: t4flib-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/file_helper.py

```diff
@@ -1,9 +1,9 @@
 import os
-from .log_helper import logger
+from log_helper import logger
 import shutil
 import fnmatch
 import datetime
 import pathlib
 import json
 import zipfile
 import glob
@@ -25,15 +25,15 @@
                 return
             
             for file in files:
                 file_path=str(file.absolute())
             
                 zipf.write(file_path, os.path.relpath(file_path, source_dir))
                 logger('INFO', f'Suppression du dossier source {source_dir}')
-                shutil.rmtree(ignore_errors=True)
+                shutil.rmtree(source_dir,ignore_errors=True)
 
         logger('INFO', f'Le dossier {source_dir} a été zippé avec succès dans {output_filename}')
     except Exception as e:
         logger('ERROR', f'{str(e)}')
         raise
```

## Comparing `t4flib-0.3.6.dist-info/METADATA` & `t4flib-0.3.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.3.6
+Version: 0.3.7
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.3.6.dist-info/RECORD` & `t4flib-0.3.7.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=4kv9YBFa7cwTjxNbBRGgMduVth0VRk05CftWP4Yjexw,1086
 t4flib/data_helper.py,sha256=SdKdv2U1EXtHJcfEff_I8zIlMWv56-xLZqczAw4kOUU,971
-t4flib/file_helper.py,sha256=dzrIOGQwJxwoULjHg3Hkiye-vM3ziaXkECl9zaYcisM,6266
+t4flib/file_helper.py,sha256=CWXPW3bn0EYerEbVtqw-lYOhQSbfhpw8jkpPltU09ao,6276
 t4flib/filetransfer_helper.py,sha256=zYO8sML9ZxsqU7_COVgxTstmKa4KJuwa1kjfdm6jHAY,5692
 t4flib/functional_helper.py,sha256=CfbwrMufVRwCQNg9us9tujS3oeCmxql18vmo7B5lUAI,7420
 t4flib/gcloud_helper.py,sha256=5_5fzYVlivt_2mBs9OBYfRyO-84UsL5gOr5MI8Mt4gQ,2682
 t4flib/log_helper.py,sha256=pu_y3m7iHWpkgYnxLYAlQjWjqknMGDcCDjHV6w4YYDc,876
-t4flib-0.3.6.dist-info/METADATA,sha256=bh5XxEXB1wFDQGf08cXnDWQ71YnhIziNBYbG8D0dnpE,1747
-t4flib-0.3.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.3.6.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.3.6.dist-info/RECORD,,
+t4flib-0.3.7.dist-info/METADATA,sha256=fquQGq9c5hnrryyMbYmaAbk_FOzV5sD6DpCcED-7C80,1747
+t4flib-0.3.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.3.7.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.3.7.dist-info/RECORD,,
```

