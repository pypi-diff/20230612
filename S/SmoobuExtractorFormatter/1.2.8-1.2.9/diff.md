# Comparing `tmp/SmoobuExtractorFormatter-1.2.8.tar.gz` & `tmp/SmoobuExtractorFormatter-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.2.8.tar", last modified: Mon Jun 12 02:11:26 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.2.9.tar", last modified: Mon Jun 12 02:14:05 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.2.8.tar` & `SmoobuExtractorFormatter-1.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 02:11:26.772614 SmoobuExtractorFormatter-1.2.8/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-12 02:11:26.771617 SmoobuExtractorFormatter-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 02:11:26.751613 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0    12989 2023-06-12 02:11:07.000000 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-12 02:11:26.768617 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-12 02:11:26.000000 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-12 02:11:26.000000 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 02:11:26.000000 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-12 02:11:26.000000 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-12 02:11:26.000000 SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 02:11:26.772614 SmoobuExtractorFormatter-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-12 02:11:14.000000 SmoobuExtractorFormatter-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:14:05.657243 SmoobuExtractorFormatter-1.2.9/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-12 02:14:05.656243 SmoobuExtractorFormatter-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 02:14:05.639241 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0    12996 2023-06-12 02:13:43.000000 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-12 02:14:05.654241 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-12 02:14:05.000000 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-12 02:14:05.000000 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 02:14:05.000000 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-12 02:14:05.000000 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-12 02:14:05.000000 SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 02:14:05.657243 SmoobuExtractorFormatter-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-12 02:13:50.000000 SmoobuExtractorFormatter-1.2.9/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.2.8/LICENSE.txt` & `SmoobuExtractorFormatter-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.2.8/PKG-INFO` & `SmoobuExtractorFormatter-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.8
+Version: 1.2.9
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,23 +186,23 @@
                 
                 number_menage = bookings[names['name_menage']].shape[0]
                 number_sejour = bookings[names['name_taxe']].shape[0]
                 
                 # merging every columns into one : baseprice
                 
                 try :
-                    bookings['basePrice_'] = bookings[names['name_baseprice']].apply(lambda x: [val for val in x if pd.notna(val)], axis = 1)
+                    bookings['base_price_'] = bookings[names['name_baseprice']].apply(lambda x: [val for val in x if pd.notna(val)], axis = 1)
                     
-                    lens1 = bookings['basePrice_'].apply(len_value)
+                    lens1 = bookings['base_price_'].apply(len_value)
                     
                     del bookings[names['name_baseprice']]
                     
-                    bookings['basePrice_'] = bookings['basePrice_'].apply(one_value)
+                    bookings['base_price_'] = bookings['base_price_'].apply(one_value)
                 except :
-                    bookings.rename(columns = {'basePrice':'basePrice_'}, inplace = True)
+                    bookings.rename(columns = {'base_price':'base_price_'}, inplace = True)
                     print("multiple baseprice not found")
                 
                 
                 # merging every columns into one : frais de menage
                 
                 try : 
                     bookings['frais_menage_'] = bookings[names['name_menage']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
@@ -316,15 +316,15 @@
                 try : 
                     del bookings['addon']
                 except :
                     print("addon not found")
 
 
                 # New column
-                payé_voyageur_calculated = ['basePrice_', 'frais_menage_', 'taxe_sejour_', 'frais_gestion_', 'frais_linge_serviettes_','frais_electricite_']
+                payé_voyageur_calculated = ['base_price_', 'frais_menage_', 'taxe_sejour_', 'frais_gestion_', 'frais_linge_serviettes_','frais_electricite_']
                 bookings['payé-voyageur_calculated'] = 0.0
 
                 for frais in payé_voyageur_calculated:
                     if frais in bookings.columns:
                         bookings['payé-voyageur_calculated'] += bookings[frais].fillna(0.0)
 
                 try:
```

### Comparing `SmoobuExtractorFormatter-1.2.8/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.2.9/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.8
+Version: 1.2.9
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.8/setup.py` & `SmoobuExtractorFormatter-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.2.8',
+    version='1.2.9',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

