# Comparing `tmp/SmoobuExtractorFormatter-1.2.5.tar.gz` & `tmp/SmoobuExtractorFormatter-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.2.5.tar", last modified: Mon Jun 12 01:29:53 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.2.6.tar", last modified: Mon Jun 12 01:59:16 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.2.5.tar` & `SmoobuExtractorFormatter-1.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 01:29:53.219438 SmoobuExtractorFormatter-1.2.5/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-12 01:29:53.218433 SmoobuExtractorFormatter-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 01:29:53.196426 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0    11103 2023-06-12 01:29:36.000000 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-12 01:29:53.216444 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-12 01:29:53.000000 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-12 01:29:53.000000 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 01:29:53.000000 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-12 01:29:53.000000 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-12 01:29:53.000000 SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 01:29:53.220436 SmoobuExtractorFormatter-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-12 01:29:43.000000 SmoobuExtractorFormatter-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:59:16.614988 SmoobuExtractorFormatter-1.2.6/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-12 01:59:16.613987 SmoobuExtractorFormatter-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 01:59:16.591986 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0    12102 2023-06-12 01:58:57.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:59:16.611989 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 01:59:16.614988 SmoobuExtractorFormatter-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-12 01:59:06.000000 SmoobuExtractorFormatter-1.2.6/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.2.5/LICENSE.txt` & `SmoobuExtractorFormatter-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.2.5/PKG-INFO` & `SmoobuExtractorFormatter-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.5
+Version: 1.2.6
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 9% similar despite different names*

```diff
@@ -169,16 +169,14 @@
                 #bookings.rename(columns = table, inplace = True)
                 
                 columns = bookings.columns 
                 dict = {}
 
                 bookings.rename(columns = table, inplace = True)
                 
-                del bookings[names['name_addon']]
-                
                 columns_exist = {}
                 columns_notexist = []
                 
                 for name in table.keys():
                     if name in columns :
                         columns_exist[name] = True
                     else :
@@ -187,86 +185,111 @@
                 
                 
                 number_menage = bookings[names['name_menage']].shape[0]
                 number_sejour = bookings[names['name_taxe']].shape[0]
                 
                 # merging every columns into one : baseprice
                 
-                '''bookings['basePrice_'] = bookings[names['name_baseprice']].apply(lambda x: [val for val in x if pd.notna(val)], axis = 1)
-                
-                lens1 = bookings['basePrice_'].apply(len_value)
-                
-                del bookings[names['name_baseprice']]
-                
-                bookings['basePrice_'] = bookings['basePrice_'].apply(one_value)'''
+                try :
+                    bookings['basePrice_'] = bookings[names['name_baseprice']].apply(lambda x: [val for val in x if pd.notna(val)], axis = 1)
+                    
+                    lens1 = bookings['basePrice_'].apply(len_value)
+                    
+                    del bookings[names['name_baseprice']]
+                    
+                    bookings['basePrice_'] = bookings['basePrice_'].apply(one_value)
+                except :
+                    print("multiple baseprice not found")
                 
                 
                 # merging every columns into one : frais de menage
                 
-                bookings['frais_menage_'] = bookings[names['name_menage']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
-                
+                try : 
+                    bookings['frais_menage_'] = bookings[names['name_menage']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                    
 
-                lens = bookings['frais_menage_'].apply(len_value)
-                
-                del bookings[names['name_menage']]
-                
-                bookings['frais_menage_'] = bookings['frais_menage_'].apply(one_value)
-                
+                    lens = bookings['frais_menage_'].apply(len_value)
+                    
+                    del bookings[names['name_menage']]
+                    
+                    bookings['frais_menage_'] = bookings['frais_menage_'].apply(one_value)
                 
+                except : 
+                    print("multiple frais de menage not found")
                 # merging every columns into one : taxe de sejour
             
             
                 print(bookings[names['name_taxe']].head())
-                bookings['taxe_sejour_'] = bookings[names['name_taxe']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
-                lens2 = bookings['taxe_sejour_'].apply(len_value)
                 
-                del bookings[names['name_taxe']]
+                try : 
                 
-                bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
+                    bookings['taxe_sejour_'] = bookings[names['name_taxe']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                    lens2 = bookings['taxe_sejour_'].apply(len_value)
+                    
+                    del bookings[names['name_taxe']]
+                    
+                    bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
+                    
+                except : 
+                    print("multiple taxe de sejour not found")
                 
                 # merge every column into one : commission 
                 
-                bookings['commission_'] = bookings[names['name_commission']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                try : 
+                    bookings['commission_'] = bookings[names['name_commission']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
 
-                lens3 = bookings['commission_'].apply(len_value)
-                
-                del bookings[names['name_commission']]
-                
-                bookings['commission_'] = bookings['commission_'].apply(one_value)
+                    lens3 = bookings['commission_'].apply(len_value)
+                    
+                    del bookings[names['name_commission']]
+                    
+                    bookings['commission_'] = bookings['commission_'].apply(one_value)
+                except :
+                    print("multiple commission not found")
                 
                 # merge evry column into one : gestion 
+            
+                try : 
                 
-                bookings['frais_gestion_'] = bookings[names['name_gestion']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
-                
-                lens4 = bookings['frais_gestion_'].apply(len_value)
-                
-                del bookings[names['name_gestion']]
+                    bookings['frais_gestion_'] = bookings[names['name_gestion']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                    
+                    lens4 = bookings['frais_gestion_'].apply(len_value)
+                    
+                    del bookings[names['name_gestion']]
+                    
+                    bookings['frais_gestion_'] = bookings['frais_gestion_'].apply(one_value)
                 
-                bookings['frais_gestion_'] = bookings['frais_gestion_'].apply(one_value)
+                except : 
+                    print("multiple frais de gestion not found")
                 
                 # merge every column into one : frais_electricite
                 
-                bookings['frais_electricite_'] = bookings[names['name_electricite']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
-                
-                lens5 = bookings['frais_electricite_'].apply(len_value)
-                
-                del bookings[names['name_electricite']]
-                
-                bookings['frais_electricite_'] = bookings['frais_electricite_'].apply(one_value)
+                try : 
+                    bookings['frais_electricite_'] = bookings[names['name_electricite']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                    
+                    lens5 = bookings['frais_electricite_'].apply(len_value)
+                    
+                    del bookings[names['name_electricite']]
+                    
+                    bookings['frais_electricite_'] = bookings['frais_electricite_'].apply(one_value)
+                except :
+                    print("multiple frais d'electricite not found")
                 
                 
                 # sum every column into one : linge de lit et serviettes 
                 
-                bookings['frais_linge_serviettes_'] = bookings[names['name_linge']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
-                
-                lens6 = bookings['frais_linge_serviettes_'].apply(len_value)
-                
-                del bookings[names['name_linge']]
-                
-                bookings['frais_linge_serviettes_'] = bookings['frais_linge_serviettes_'].apply(sum_value)
+                try : 
+                    bookings['frais_linge_serviettes_'] = bookings[names['name_linge']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                    
+                    lens6 = bookings['frais_linge_serviettes_'].apply(len_value)
+                    
+                    del bookings[names['name_linge']]
+                    
+                    bookings['frais_linge_serviettes_'] = bookings['frais_linge_serviettes_'].apply(sum_value)
+                except : 
+                    print("multiple frais de linge et serviettes not found")
                 
                 # delete all the cancel columns 
                 
                 # Find keys containing "cancel" and store them in the list
                 keys_to_delete = []
                 for key in bookings.keys():
                     if 'cancel' in key:
```

### Comparing `SmoobuExtractorFormatter-1.2.5/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.5
+Version: 1.2.6
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.5/setup.py` & `SmoobuExtractorFormatter-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.2.5',
+    version='1.2.6',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

