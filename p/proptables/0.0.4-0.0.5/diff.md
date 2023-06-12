# Comparing `tmp/proptables-0.0.4.tar.gz` & `tmp/proptables-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proptables-0.0.4.tar", last modified: Sun Jun 11 10:33:48 2023, max compression
+gzip compressed data, was "proptables-0.0.5.tar", last modified: Mon Jun 12 09:44:08 2023, max compression
```

## Comparing `proptables-0.0.4.tar` & `proptables-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 10:33:48.304926 proptables-0.0.4/
--rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0       62 2023-06-11 10:30:34.000000 proptables-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2452 2023-06-11 10:33:48.304926 proptables-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-06-07 09:25:23.000000 proptables-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 10:33:47.932711 proptables-0.0.4/proptables/
-drwxrwxrwx   0        0        0        0 2023-06-11 10:33:47.958985 proptables-0.0.4/proptables/R134a/
--rw-rw-rw-   0        0        0     2379 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/R134a_PresSat.csv
--rw-rw-rw-   0        0        0      239 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/R134a_SupPreSat.csv
--rw-rw-rw-   0        0        0     9904 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/R134a_Super.csv
--rw-rw-rw-   0        0        0     3782 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/R134a_TempSat.csv
--rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/__init__.py
--rw-rw-rw-   0        0        0     4503 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/calSatData.py
--rw-rw-rw-   0        0        0     5043 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/calSuperHeatData.py
--rw-rw-rw-   0        0        0      574 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/import_data.py
--rw-rw-rw-   0        0        0      113 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/interpolate.py
--rw-rw-rw-   0        0        0     1389 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/main.py
--rw-rw-rw-   0        0        0     5652 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/superheated.py
--rw-rw-rw-   0        0        0     2068 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/R134a/test.py
--rw-rw-rw-   0        0        0       88 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:33:47.974614 proptables-0.0.4/proptables/water/
--rw-rw-rw-   0        0        0     3388 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/H2O_Compressed.csv
--rw-rw-rw-   0        0        0     3894 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/H2O_PresSat.csv
--rw-rw-rw-   0        0        0    15532 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/H2O_Super.csv
--rw-rw-rw-   0        0        0     4185 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/H2O_TempSat.csv
--rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/calwatercompressed.py
--rw-rw-rw-   0        0        0     4462 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/calwatersat.py
--rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/calwatersuperheat.py
--rw-rw-rw-   0        0        0      419 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/import_data_water.py
--rw-rw-rw-   0        0        0      794 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/main.py
--rw-rw-rw-   0        0        0      161 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/mainwater.py
--rw-rw-rw-   0        0        0      956 2023-06-11 10:30:34.000000 proptables-0.0.4/proptables/water/test.py
-drwxrwxrwx   0        0        0        0 2023-06-11 10:33:47.943581 proptables-0.0.4/proptables.egg-info/
--rw-rw-rw-   0        0        0     2452 2023-06-11 10:33:47.000000 proptables-0.0.4/proptables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2023-06-11 10:33:47.000000 proptables-0.0.4/proptables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 10:33:47.000000 proptables-0.0.4/proptables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 10:33:47.000000 proptables-0.0.4/proptables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-06-11 10:33:48.323120 proptables-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 09:44:08.166547 proptables-0.0.5/
+-rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       62 2023-06-11 10:30:34.000000 proptables-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2452 2023-06-12 09:44:08.166547 proptables-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-06-07 09:25:23.000000 proptables-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 09:44:07.829018 proptables-0.0.5/proptables/
+drwxrwxrwx   0        0        0        0 2023-06-12 09:44:07.849117 proptables-0.0.5/proptables/R134a/
+-rw-rw-rw-   0        0        0     2379 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_PresSat.csv
+-rw-rw-rw-   0        0        0      239 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_SupPreSat.csv
+-rw-rw-rw-   0        0        0     9904 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_Super.csv
+-rw-rw-rw-   0        0        0     3782 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_TempSat.csv
+-rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/__init__.py
+-rw-rw-rw-   0        0        0     4503 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/calSatData.py
+-rw-rw-rw-   0        0        0     4210 2023-06-12 08:12:48.000000 proptables-0.0.5/proptables/R134a/calSuperHeatData.py
+-rw-rw-rw-   0        0        0      574 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/import_data.py
+-rw-rw-rw-   0        0        0      113 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/interpolate.py
+-rw-rw-rw-   0        0        0     1389 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/main.py
+-rw-rw-rw-   0        0        0     7288 2023-06-12 08:12:48.000000 proptables-0.0.5/proptables/R134a/superheated.py
+-rw-rw-rw-   0        0        0     2068 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/test.py
+-rw-rw-rw-   0        0        0       88 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:44:08.166547 proptables-0.0.5/proptables/water/
+-rw-rw-rw-   0        0        0     3388 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_Compressed.csv
+-rw-rw-rw-   0        0        0     3894 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_PresSat.csv
+-rw-rw-rw-   0        0        0    15532 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_Super.csv
+-rw-rw-rw-   0        0        0     4185 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_TempSat.csv
+-rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/calwatercompressed.py
+-rw-rw-rw-   0        0        0     4462 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/calwatersat.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/calwatersuperheat.py
+-rw-rw-rw-   0        0        0      419 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/import_data_water.py
+-rw-rw-rw-   0        0        0      794 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/main.py
+-rw-rw-rw-   0        0        0      161 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/mainwater.py
+-rw-rw-rw-   0        0        0      956 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/test.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:44:07.839037 proptables-0.0.5/proptables.egg-info/
+-rw-rw-rw-   0        0        0     2452 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-06-12 09:44:08.175644 proptables-0.0.5/setup.cfg
```

### Comparing `proptables-0.0.4/LICENCE.txt` & `proptables-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/PKG-INFO` & `proptables-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.4
+Version: 0.0.5
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proptables-0.0.4/README.md` & `proptables-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/R134a/R134a_PresSat.csv` & `proptables-0.0.5/proptables/R134a/R134a_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/R134a/R134a_Super.csv` & `proptables-0.0.5/proptables/R134a/R134a_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/R134a/R134a_TempSat.csv` & `proptables-0.0.5/proptables/R134a/R134a_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/R134a/calSatData.py` & `proptables-0.0.5/proptables/R134a/calSatData.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/R134a/calSuperHeatData.py` & `proptables-0.0.5/proptables/R134a/calSuperHeatData.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,18 @@
 from proptables.R134a.import_data import data_path_SupPreSat
 
 class HeatedCalculater:
     def __init__(self):
         self.dfSupSat=pd.read_csv(data_path_SupPreSat)
 
     def superheatedTable(self,Pressure):
-        result=superheatedtable(Pressure)
-        result=result.reset_index(drop=True)
-        result=result.set_axis(["Temp","v","energy","enthalpy","entropy"],axis=1)
-        if Pressure in self.dfSupSat["Pressure"].values:
-            indexing=self.dfSupSat[self.dfSupSat["Pressure"].values==Pressure].index.values
-            result["Temp"].values[1]=self.dfSupSat["SaturatedTemperature"].values[indexing][0]
-        return result
-
+        return superheatedtable(Pressure)
 
     def findsuperTemp(self,Pressure,Temperature):
-        ans=self.superheatedTable(Pressure)
-        ans=ans.loc[1:]
-        ans=ans.reset_index(drop=True)
-        ans=ans.apply(pd.to_numeric)
+        ans=superheatedtable(Pressure)
         if Temperature in ans["Temp"].values:
             indexing=ans[ans["Temp"].values==Temperature].index.values
             row=ans.iloc[indexing]
             return row
         else:
             nearest=ans["Temp"].sub(Temperature).abs().argsort()[:2]
             result=ans.iloc[nearest]
@@ -38,18 +28,15 @@
             result.drop([0],inplace=True)
             result=result.reset_index(drop=True)
             result.drop([1],inplace=True)
             result=result.reset_index(drop=True)
             return result
         
     def findsuperEnthalpy(self,Pressure,Enthalpy):
-        ans=self.superheatedTable(Pressure)
-        ans=ans.loc[1:]
-        ans=ans.reset_index(drop=True)
-        ans=ans.apply(pd.to_numeric)
+        ans=superheatedtable(Pressure)
         if Enthalpy in ans["enthalpy"].values:
             indexing=ans[ans["enthalpy"].values==Enthalpy].index.values
             row=ans.iloc[indexing]
             return row
         else:
             nearest=ans["enthalpy"].sub(Enthalpy).abs().argsort()[:2]
             result=ans.iloc[nearest]
@@ -63,18 +50,15 @@
             result.drop([0],inplace=True)
             result=result.reset_index(drop=True)
             result.drop([1],inplace=True)
             result=result.reset_index(drop=True)
             return result
     
     def findsuperEntropy(self,Pressure,Entropy):
-        ans=self.superheatedTable(Pressure)
-        ans=ans.loc[1:]
-        ans=ans.reset_index(drop=True)
-        ans=ans.apply(pd.to_numeric)
+        ans=superheatedtable(Pressure)
         if Entropy in ans["entropy"].values:
             indexing=ans[ans["entropy"].values==Entropy].index.values
             row=ans.iloc[indexing]
             return row
         else:
             nearest=ans["entropy"].sub(Entropy).abs().argsort()[:2]
             result=ans.iloc[nearest]
@@ -88,18 +72,15 @@
             result.drop([0],inplace=True)
             result=result.reset_index(drop=True)
             result.drop([1],inplace=True)
             result=result.reset_index(drop=True)
             return result
         
     def findsuperspecificvolume(self,Pressure,specificvolume):
-        ans=self.superheatedTable(Pressure)
-        ans=ans.loc[1:]
-        ans=ans.reset_index(drop=True)
-        ans=ans.apply(pd.to_numeric)
+        ans=superheatedtable(Pressure)
         if specificvolume in ans["v"].values:
             indexing=ans[ans["v"].values==specificvolume].index.values
             row=ans.iloc[indexing]
             return row
         else:
             nearest=ans["v"].sub(specificvolume).abs().argsort()[:2]
             result=ans.iloc[nearest]
```

### Comparing `proptables-0.0.4/proptables/R134a/import_data.py` & `proptables-0.0.5/proptables/R134a/import_data.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/R134a/main.py` & `proptables-0.0.5/proptables/R134a/main.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/R134a/test.py` & `proptables-0.0.5/proptables/R134a/test.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/water/H2O_Compressed.csv` & `proptables-0.0.5/proptables/water/H2O_Compressed.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/water/H2O_PresSat.csv` & `proptables-0.0.5/proptables/water/H2O_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/water/H2O_Super.csv` & `proptables-0.0.5/proptables/water/H2O_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/water/H2O_TempSat.csv` & `proptables-0.0.5/proptables/water/H2O_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/water/calwatersat.py` & `proptables-0.0.5/proptables/water/calwatersat.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/water/main.py` & `proptables-0.0.5/proptables/water/main.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables/water/test.py` & `proptables-0.0.5/proptables/water/test.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/proptables.egg-info/PKG-INFO` & `proptables-0.0.5/proptables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.4
+Version: 0.0.5
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proptables-0.0.4/proptables.egg-info/SOURCES.txt` & `proptables-0.0.5/proptables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proptables-0.0.4/setup.cfg` & `proptables-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7074 6162 6c65 730d 0a76   = proptables..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e34 0d0a  ersion = 0.0.4..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e35 0d0a  ersion = 0.0.5..
 00000030: 6175 7468 6f72 203d 2042 7564 6468 6920  author = Buddhi 
 00000040: 5769 6a65 6e61 7961 6b65 0d0a 6175 7468  Wijenayake..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696a 656e  or_email = wijen
 00000060: 6179 616b 6562 7564 6468 6933 3438 3032  ayakebuddhi34802
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 466f 7220 6765  ription = For ge
 00000090: 6e65 7261 7469 6e67 2070 726f 7065 7274  nerating propert
```

