# Comparing `tmp/t4flib-0.3.8-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.3.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11041 bytes, number of entries: 12
+Zip file size: 11132 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-09 13:22 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
--rw-rw-r--  2.0 unx     6277 b- defN 23-Jun-12 13:28 t4flib/file_helper.py
+-rw-rw-r--  2.0 unx     6496 b- defN 23-Jun-12 15:13 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     5692 b- defN 23-Jun-12 08:53 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     2682 b- defN 23-May-30 14:55 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-30 14:21 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-Jun-12 13:40 t4flib-0.3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 13:40 t4flib-0.3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-12 13:40 t4flib-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      920 b- defN 23-Jun-12 13:40 t4flib-0.3.8.dist-info/RECORD
-12 files, 27788 bytes uncompressed, 9509 bytes compressed:  65.8%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-Jun-12 15:24 t4flib-0.3.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 15:24 t4flib-0.3.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-12 15:24 t4flib-0.3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      920 b- defN 23-Jun-12 15:24 t4flib-0.3.9.dist-info/RECORD
+12 files, 28007 bytes uncompressed, 9600 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.3.8.dist-info/METADATA
+Filename: t4flib-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.3.8.dist-info/WHEEL
+Filename: t4flib-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.3.8.dist-info/top_level.txt
+Filename: t4flib-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.3.8.dist-info/RECORD
+Filename: t4flib-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/file_helper.py

```diff
@@ -10,14 +10,18 @@
 import pandas as pd
 import csv
 
 
 def __validate_filemask__(filename, filemask):
     return fnmatch.fnmatch(filename, filemask)
 
+def ignore_extended_attributes(func, filename, exc_info):
+    is_meta_file = os.path.basename(filename).startswith("._")
+    if not (func is os.unlink and is_meta_file):
+        raise
 
 def zip_folder(source_dir, dest_dir, output_filename):
     logger('INFO', f'Zippage du dossier {source_dir}')
     try:
         with zipfile.ZipFile(os.path.join(dest_dir, output_filename), 'w', zipfile.ZIP_DEFLATED) as zipf:
             files=get_all_file_by_filemask(source_dir, '*')
             if len(files) == 0:
@@ -25,15 +29,15 @@
                 return
             
             for file in files:
                 file_path=str(file.absolute())
             
                 zipf.write(file_path, os.path.relpath(file_path, source_dir))
                 logger('INFO', f'Suppression du dossier source {source_dir}')
-                shutil.rmtree(source_dir,ignore_errors=True)
+                shutil.rmtree(source_dir,ignore_errors=True,onerror=ignore_extended_attributes)
 
         logger('INFO', f'Le dossier {source_dir} a été zippé avec succès dans {output_filename}')
     except Exception as e:
         logger('ERROR', f'{str(e)}')
         raise
```

## Comparing `t4flib-0.3.8.dist-info/METADATA` & `t4flib-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.3.8
+Version: 0.3.9
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.3.8.dist-info/RECORD` & `t4flib-0.3.9.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=4kv9YBFa7cwTjxNbBRGgMduVth0VRk05CftWP4Yjexw,1086
 t4flib/data_helper.py,sha256=SdKdv2U1EXtHJcfEff_I8zIlMWv56-xLZqczAw4kOUU,971
-t4flib/file_helper.py,sha256=khrQYRmCK3TbsjpKt18lbGTC5BG0ndqCnCYg_CzRbfw,6277
+t4flib/file_helper.py,sha256=YL1AwDPLbd9AFDU5SUB1G-hFJjkDleamYc4hiVxIkGc,6496
 t4flib/filetransfer_helper.py,sha256=zYO8sML9ZxsqU7_COVgxTstmKa4KJuwa1kjfdm6jHAY,5692
 t4flib/functional_helper.py,sha256=CfbwrMufVRwCQNg9us9tujS3oeCmxql18vmo7B5lUAI,7420
 t4flib/gcloud_helper.py,sha256=5_5fzYVlivt_2mBs9OBYfRyO-84UsL5gOr5MI8Mt4gQ,2682
 t4flib/log_helper.py,sha256=pu_y3m7iHWpkgYnxLYAlQjWjqknMGDcCDjHV6w4YYDc,876
-t4flib-0.3.8.dist-info/METADATA,sha256=XHxsdu7r97GaIKbCmR4tZDUYMKjHNeyyAddWalzGICM,1747
-t4flib-0.3.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.3.8.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.3.8.dist-info/RECORD,,
+t4flib-0.3.9.dist-info/METADATA,sha256=jdYj5M5iaYmwH__e8jkhSEgRxKv19MyrzwcBnEyuSGQ,1747
+t4flib-0.3.9.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.3.9.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.3.9.dist-info/RECORD,,
```

