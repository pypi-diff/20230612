# Comparing `tmp/SMjour-0.0.4.tar.gz` & `tmp/SMjour-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SMjour-0.0.4.tar", last modified: Mon Jun 12 17:54:39 2023, max compression
+gzip compressed data, was "SMjour-0.0.5.tar", last modified: Mon Jun 12 18:34:42 2023, max compression
```

## Comparing `SMjour-0.0.4.tar` & `SMjour-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 17:54:39.157000 SMjour-0.0.4/
--rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      448 2023-06-12 17:54:39.147000 SMjour-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 17:54:39.030000 SMjour-0.0.4/SMjour/
--rw-rw-rw-   0        0        0     6462 2023-06-12 17:54:13.000000 SMjour-0.0.4/SMjour/SMjour.py
--rw-rw-rw-   0        0        0        0 2023-06-12 13:07:40.000000 SMjour-0.0.4/SMjour/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:54:39.132000 SMjour-0.0.4/SMjour.egg-info/
--rw-rw-rw-   0        0        0      448 2023-06-12 17:54:38.000000 SMjour-0.0.4/SMjour.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-12 17:54:38.000000 SMjour-0.0.4/SMjour.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 17:54:38.000000 SMjour-0.0.4/SMjour.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-12 17:54:38.000000 SMjour-0.0.4/SMjour.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 17:54:38.000000 SMjour-0.0.4/SMjour.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      660 2023-06-12 17:54:39.155000 SMjour-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 18:34:42.539000 SMjour-0.0.5/
+-rw-rw-rw-   0        0        0     1097 2023-06-12 13:17:40.000000 SMjour-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      448 2023-06-12 18:34:42.528000 SMjour-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:00.000000 SMjour-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 18:34:42.442000 SMjour-0.0.5/SMjour/
+-rw-rw-rw-   0        0        0     6475 2023-06-12 18:34:14.000000 SMjour-0.0.5/SMjour/SMjour.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 13:07:40.000000 SMjour-0.0.5/SMjour/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 18:34:42.519000 SMjour-0.0.5/SMjour.egg-info/
+-rw-rw-rw-   0        0        0      448 2023-06-12 18:34:42.000000 SMjour-0.0.5/SMjour.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-12 18:34:42.000000 SMjour-0.0.5/SMjour.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 18:34:42.000000 SMjour-0.0.5/SMjour.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-12 18:34:42.000000 SMjour-0.0.5/SMjour.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 18:34:42.000000 SMjour-0.0.5/SMjour.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 14:12:44.000000 SMjour-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      660 2023-06-12 18:34:42.538000 SMjour-0.0.5/setup.cfg
```

### Comparing `SMjour-0.0.4/LICENSE` & `SMjour-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SMjour-0.0.4/SMjour/SMjour.py` & `SMjour-0.0.5/SMjour/SMjour.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     else:
         raise ValueError('Format Not Found')
     try:
       df=df.drop("Unnamed: 0",axis=1)
     except:
        pass
     try:
-       df["Weeks"]=pd.to_datetime(df["Weeks"])
+      df["Weeks"]=pd.to_datetime(df["Weeks"])
     except:
-       pass
+      pass
     
     return df
 #"G:\Shared drives\Team members\Agustin\merk\00Q3\1websls\data.csv"
 ###########################################################################################################################################################
 
 
 def to_sav(option='default'):
@@ -76,14 +76,15 @@
     randomo=random.randint(100000, 1000000)
     try:
       pyspssio.write_sav(newpath+f"/data_{randomo}.sav", df)
     except:
       pyreadstat.write_sav(df, newpath+f"/data_{randomo}.sav")
     print(f'Saved as data_{randomo}')
     print('Wait some minutes, the Google Drive is updating')
+    return df
 
 def fix_csv(option='default'):
     #import drive
     drive.mount("/content/drive")
     newpath=input_path('Input path:')
     if (newpath.split("/")[-1].split(".")[-1] == "xlsx") or (newpath.split("/")[-1].split(".")[-1] == "xls"):
         df=pd.read_excel(newpath)
```

### Comparing `SMjour-0.0.4/setup.cfg` & `SMjour-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 4d6a 6f75 720d 0a76 6572 7369   = SMjour..versi
-00000020: 6f6e 203d 2030 2e30 2e34 0d0a 6175 7468  on = 0.0.4..auth
+00000020: 6f6e 203d 2030 2e30 2e35 0d0a 6175 7468  on = 0.0.5..auth
 00000030: 6f72 203d 2041 6775 7374 696e 2042 7573  or = Agustin Bus
 00000040: 746f 7320 4261 7274 6f6e 0d0a 6175 7468  tos Barton..auth
 00000050: 6f72 5f65 6d61 696c 203d 2061 6775 7374  or_email = agust
 00000060: 696e 6275 7374 6f73 6261 7274 6f6e 4067  inbustosbarton@g
 00000070: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000080: 7074 696f 6e20 3d20 696e 7665 7374 6967  ption = investig
 00000090: 6174 696f 6e20 6a6f 7572 6e61 6c0d 0a6c  ation journal..l
```

