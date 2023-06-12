# Comparing `tmp/SmoobuExtractorFormatter-1.2.6.tar.gz` & `tmp/SmoobuExtractorFormatter-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.2.6.tar", last modified: Mon Jun 12 01:59:16 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.2.7.tar", last modified: Mon Jun 12 02:06:50 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.2.6.tar` & `SmoobuExtractorFormatter-1.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 01:59:16.614988 SmoobuExtractorFormatter-1.2.6/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-12 01:59:16.613987 SmoobuExtractorFormatter-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 01:59:16.591986 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0    12102 2023-06-12 01:58:57.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-12 01:59:16.611989 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-12 01:59:16.000000 SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 01:59:16.614988 SmoobuExtractorFormatter-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-12 01:59:06.000000 SmoobuExtractorFormatter-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:06:50.555551 SmoobuExtractorFormatter-1.2.7/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-12 02:06:50.555551 SmoobuExtractorFormatter-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:06:50.535550 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0    12872 2023-06-12 02:06:36.000000 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:06:50.553552 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-12 02:06:50.000000 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-12 02:06:50.000000 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:06:50.000000 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-12 02:06:50.000000 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-12 02:06:50.000000 SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 02:06:50.556553 SmoobuExtractorFormatter-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-12 02:06:46.000000 SmoobuExtractorFormatter-1.2.7/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.2.6/LICENSE.txt` & `SmoobuExtractorFormatter-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.2.6/PKG-INFO` & `SmoobuExtractorFormatter-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.6
+Version: 1.2.7
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 5% similar despite different names*

```diff
@@ -194,14 +194,15 @@
                     
                     lens1 = bookings['basePrice_'].apply(len_value)
                     
                     del bookings[names['name_baseprice']]
                     
                     bookings['basePrice_'] = bookings['basePrice_'].apply(one_value)
                 except :
+                    bookings.rename(columns = {'basePrice_':'basePrice'}, inplace = True)
                     print("multiple baseprice not found")
                 
                 
                 # merging every columns into one : frais de menage
                 
                 try : 
                     bookings['frais_menage_'] = bookings[names['name_menage']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
@@ -210,43 +211,46 @@
                     lens = bookings['frais_menage_'].apply(len_value)
                     
                     del bookings[names['name_menage']]
                     
                     bookings['frais_menage_'] = bookings['frais_menage_'].apply(one_value)
                 
                 except : 
+                    bookings.rename(columns = {'frais_menage_':'frais_menage'}, inplace = True)
                     print("multiple frais de menage not found")
                 # merging every columns into one : taxe de sejour
             
             
-                print(bookings[names['name_taxe']].head())
+                #print(bookings[names['name_taxe']].head())
                 
                 try : 
                 
                     bookings['taxe_sejour_'] = bookings[names['name_taxe']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
                     lens2 = bookings['taxe_sejour_'].apply(len_value)
                     
                     del bookings[names['name_taxe']]
                     
                     bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
                     
                 except : 
+                    bookings.rename(columns = {'taxe_sejour_':'taxe_sejour'}, inplace = True)
                     print("multiple taxe de sejour not found")
                 
                 # merge every column into one : commission 
                 
                 try : 
                     bookings['commission_'] = bookings[names['name_commission']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
 
                     lens3 = bookings['commission_'].apply(len_value)
                     
                     del bookings[names['name_commission']]
                     
                     bookings['commission_'] = bookings['commission_'].apply(one_value)
                 except :
+                    bookings.rename(columns = {'commission_':'commission'}, inplace = True)
                     print("multiple commission not found")
                 
                 # merge evry column into one : gestion 
             
                 try : 
                 
                     bookings['frais_gestion_'] = bookings[names['name_gestion']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
@@ -254,27 +258,30 @@
                     lens4 = bookings['frais_gestion_'].apply(len_value)
                     
                     del bookings[names['name_gestion']]
                     
                     bookings['frais_gestion_'] = bookings['frais_gestion_'].apply(one_value)
                 
                 except : 
+                    bookings.rename(columns = {'frais_gestion_':'frais_gestion'}, inplace = True)
                     print("multiple frais de gestion not found")
                 
                 # merge every column into one : frais_electricite
                 
                 try : 
                     bookings['frais_electricite_'] = bookings[names['name_electricite']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
                     
                     lens5 = bookings['frais_electricite_'].apply(len_value)
                     
                     del bookings[names['name_electricite']]
                     
                     bookings['frais_electricite_'] = bookings['frais_electricite_'].apply(one_value)
                 except :
+                    
+                    bookings.rename(columns = {'frais_electricite_':'frais_electricite'}, inplace = True)
                     print("multiple frais d'electricite not found")
                 
                 
                 # sum every column into one : linge de lit et serviettes 
                 
                 try : 
                     bookings['frais_linge_serviettes_'] = bookings[names['name_linge']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
@@ -300,36 +307,41 @@
                     del bookings[key]
                     
                 # delete the columns that are on the paramater 
                 
                 for key in to_drop:
                     if key in bookings.keys():
                         del bookings[key]
+                        
+                try : 
+                    del bookings['addon']
+                except :
+                    print("addon not found")
 
 
                 # New column
                 payé_voyageur_calculated = ['basePrice_', 'frais_menage_', 'taxe_sejour_', 'frais_gestion_', 'frais_linge_serviettes_','frais_electricite_']
                 bookings['payé-voyageur_calculated'] = 0.0
 
                 for frais in payé_voyageur_calculated:
                     if frais in bookings.columns:
                         bookings['payé-voyageur_calculated'] += bookings[frais].fillna(0.0)
 
                 try:
-                    bookings['delta'] = (abs(bookings['total-price'] - bookings['payé-voyageur_calculated']))
+                    bookings['delta'] = (abs(bookings['total_price'] - bookings['payé-voyageur_calculated']))
                     bookings = bookings.round(2)  # to avoid rounding errors
                     bookings['Added-Taxes'] = np.where(bookings['taxe_sejour_'] == bookings['delta'], True, False)
-                    bookings['Equals-Prices'] = np.where(bookings['total-price'] == bookings['payé-voyageur_calculated'], True, False)
+                    bookings['Equals-Prices'] = np.where(bookings['total_price'] == bookings['payé-voyageur_calculated'], True, False)
 
                     del bookings['delta']
                 except KeyError as error:
                     _, _, tb = sys.exc_info()
                     line_number = traceback.extract_tb(tb)[-1][1]       
                     print(f"Error occurred on line {line_number}: {error}")
-                    print("\nThere is a problem with the columns: total-price and payé-voyageur_calculated\n")
+                    print("\nThere is a problem with the columns: total_price and payé-voyageur_calculated\n")
 
                 # newly formated data to excel
                 bookings = bookings.round(2)
                 bookings.to_excel( path_output +"/Smoobu_"+file_name.split("/")[-1] + ".xlsx", index = False)
                 
                 print("\nSmoobu file created \n")
                 for file in os.listdir():
```

### Comparing `SmoobuExtractorFormatter-1.2.6/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.2.7/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.6
+Version: 1.2.7
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.6/setup.py` & `SmoobuExtractorFormatter-1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.2.6',
+    version='1.2.7',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

