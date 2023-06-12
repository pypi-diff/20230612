# Comparing `tmp/t4flib-0.3.3-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.3.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11027 bytes, number of entries: 12
+Zip file size: 11017 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-Jun-09 13:22 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
--rw-rw-r--  2.0 unx     5744 b- defN 23-Jun-09 13:22 t4flib/filetransfer_helper.py
+-rw-rw-r--  2.0 unx     5692 b- defN 23-Jun-12 08:53 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
 -rw-rw-r--  2.0 unx     2682 b- defN 23-May-30 14:55 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-30 14:21 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      920 b- defN 23-Jun-09 13:35 t4flib-0.3.3.dist-info/RECORD
-12 files, 27708 bytes uncompressed, 9495 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-Jun-12 09:06 t4flib-0.3.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-12 09:06 t4flib-0.3.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-12 09:06 t4flib-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      920 b- defN 23-Jun-12 09:06 t4flib-0.3.4.dist-info/RECORD
+12 files, 27656 bytes uncompressed, 9485 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.3.3.dist-info/METADATA
+Filename: t4flib-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.3.3.dist-info/WHEEL
+Filename: t4flib-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.3.3.dist-info/top_level.txt
+Filename: t4flib-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.3.3.dist-info/RECORD
+Filename: t4flib-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/filetransfer_helper.py

```diff
@@ -138,13 +138,12 @@
                     ret = None
 
                 if ret in [202, 200]:
 
                     logger("INFO", f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
                     log_f.info(f"Le flux {flow_name} contenant le fichier {str(file)} est parti")
                     log_f.info(f"Suppresssion du fichier {str(file)}")
-                    os.remove(str(file.absolute()))
                 else:
 
                     logger('ERROR', f"Un code erreur API : {ret} a eu lieu")
                     logger('ERROR', f"Erreur lors de l'appel à l'API statut => {ret}")
                     log_f.error(f"Erreur lors de l'appel à l'API statut => {ret}")
```

## Comparing `t4flib-0.3.3.dist-info/METADATA` & `t4flib-0.3.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.3.3
+Version: 0.3.4
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

