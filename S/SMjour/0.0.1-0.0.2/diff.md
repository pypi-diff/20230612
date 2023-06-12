# Comparing `tmp/SMjour-0.0.1.tar.gz` & `tmp/SMjour-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjour-0.0.1.tar", last modified: Mon Jun 12 14:51:52 2023, max compression
+gzip compressed data, was "SMjour-0.0.2.tar", last modified: Mon Jun 12 15:21:32 2023, max compression
```

## Comparing `SMjour-0.0.1.tar` & `SMjour-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:51:52.029000 SMjour-0.0.1/
--rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      448 2023-06-12 14:51:52.017000 SMjour-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 14:51:51.895000 SMjour-0.0.1/SMjour/
--rw-rw-rw-   0        0        0     6312 2023-06-12 14:30:30.000000 SMjour-0.0.1/SMjour/SMjour.py
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:40.000000 SMjour-0.0.1/SMjour/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:51:52.005000 SMjour-0.0.1/SMjour.egg-info/
--rw-rw-rw-   0        0        0      448 2023-06-12 14:51:51.000000 SMjour-0.0.1/SMjour.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-12 14:51:51.000000 SMjour-0.0.1/SMjour.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:51:51.000000 SMjour-0.0.1/SMjour.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-12 14:51:51.000000 SMjour-0.0.1/SMjour.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 14:51:51.000000 SMjour-0.0.1/SMjour.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      660 2023-06-12 14:51:52.028000 SMjour-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 15:21:32.950000 SMjour-0.0.2/
+-rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-06-12 15:21:32.939000 SMjour-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 15:21:32.849000 SMjour-0.0.2/SMjour/
+-rw-rw-rw-   0        0        0     6392 2023-06-12 15:21:08.000000 SMjour-0.0.2/SMjour/SMjour.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:40.000000 SMjour-0.0.2/SMjour/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:21:32.928000 SMjour-0.0.2/SMjour.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-06-12 15:21:32.000000 SMjour-0.0.2/SMjour.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-12 15:21:32.000000 SMjour-0.0.2/SMjour.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:21:32.000000 SMjour-0.0.2/SMjour.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-12 15:21:32.000000 SMjour-0.0.2/SMjour.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 15:21:32.000000 SMjour-0.0.2/SMjour.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      660 2023-06-12 15:21:32.948000 SMjour-0.0.2/setup.cfg
```

### Comparing `SMjour-0.0.1/LICENSE` & `SMjour-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjour-0.0.1/SMjour/SMjour.py` & `SMjour-0.0.2/SMjour/SMjour.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,30 @@
     return df
 #"G:\Shared drives\Team members\Agustin\merk\00Q3\1websls\data.csv"
 ###########################################################################################################################################################
 
 
 def to_sav(option='default'):
     #import drive
-    
+    drive.mount("/content/drive")
     newpath=input_path('Input path:')
     if (newpath.split("/")[-1].split(".")[-1] == "xlsx") or (newpath.split("/")[-1].split(".")[-1] == "xls"):
         df=pd.read_excel(newpath)
     elif (newpath.split("/")[-1].split(".")[-1] == "csv"):
         if option=='default':
           df=pd.read_csv(newpath)
         elif option == 1:
           with open(newpath, "r", newline="") as fp:
             # you can use verbose=True to see what CleverCSV does
             dialect = clevercsv.Sniffer().sniff(fp.read(), verbose=False)
             fp.seek(0)
             reader = clevercsv.reader(fp, dialect)
             rows = list(reader)
           df=pd.DataFrame(rows)
+          df.columns=[str(i) for i in df.columns]
         elif option==2:
           df = clevercsv.read_dataframe(newpath)
         elif option==3:
           rows = clevercsv.read_table(newpath)
           df=pd.DataFrame(rows)  
     else:
         raise ValueError('Format Not Found')
```

### Comparing `SMjour-0.0.1/setup.cfg` & `SMjour-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 4d6a 6f75 720d 0a76 6572 7369   = SMjour..versi
-00000020: 6f6e 203d 2030 2e30 2e31 0d0a 6175 7468  on = 0.0.1..auth
+00000020: 6f6e 203d 2030 2e30 2e32 0d0a 6175 7468  on = 0.0.2..auth
 00000030: 6f72 203d 2041 6775 7374 696e 2042 7573  or = Agustin Bus
 00000040: 746f 7320 4261 7274 6f6e 0d0a 6175 7468  tos Barton..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6775 7374  or_email = agust
 00000060: 696e 6275 7374 6f73 6261 7274 6f6e 4067  inbustosbarton@g
 00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000080: 7074 696f 6e20 3d20 696e 7665 7374 6967  ption = investig
 00000090: 6174 696f 6e20 6a6f 7572 6e61 6c0d 0a6c  ation journal..l
```

