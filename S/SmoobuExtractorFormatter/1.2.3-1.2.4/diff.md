# Comparing `tmp/SmoobuExtractorFormatter-1.2.3.tar.gz` & `tmp/SmoobuExtractorFormatter-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmoobuExtractorFormatter-1.2.3.tar", last modified: Mon Jun 12 01:22:36 2023, max compression
+gzip compressed data, was "SmoobuExtractorFormatter-1.2.4.tar", last modified: Mon Jun 12 01:25:49 2023, max compression
```

## Comparing `SmoobuExtractorFormatter-1.2.3.tar` & `SmoobuExtractorFormatter-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 01:22:36.326144 SmoobuExtractorFormatter-1.2.3/
--rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      751 2023-06-12 01:22:36.325143 SmoobuExtractorFormatter-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 01:22:36.308135 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter/
--rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter/__init__.py
--rw-rw-rw-   0        0        0    11095 2023-06-12 01:22:20.000000 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter/smoobuOutput.py
-drwxrwxrwx   0        0        0        0 2023-06-12 01:22:36.324141 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter.egg-info/
--rw-rw-rw-   0        0        0      751 2023-06-12 01:22:36.000000 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-12 01:22:36.000000 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 01:22:36.000000 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-12 01:22:36.000000 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-12 01:22:36.000000 SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 01:22:36.326144 SmoobuExtractorFormatter-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-12 01:22:33.000000 SmoobuExtractorFormatter-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:25:49.555561 SmoobuExtractorFormatter-1.2.4/
+-rw-rw-rw-   0        0        0       81 2023-05-11 18:17:25.000000 SmoobuExtractorFormatter-1.2.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1067 2023-05-11 16:56:07.000000 SmoobuExtractorFormatter-1.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-05-11 16:54:04.000000 SmoobuExtractorFormatter-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      751 2023-06-12 01:25:49.554560 SmoobuExtractorFormatter-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      104 2023-05-11 16:52:09.000000 SmoobuExtractorFormatter-1.2.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 01:25:49.536036 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter/
+-rw-rw-rw-   0        0        0       62 2023-05-11 19:07:25.000000 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter/__init__.py
+-rw-rw-rw-   0        0        0    11039 2023-06-12 01:25:23.000000 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter/smoobuOutput.py
+drwxrwxrwx   0        0        0        0 2023-06-12 01:25:49.552565 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-06-12 01:25:49.000000 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-12 01:25:49.000000 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 01:25:49.000000 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-12 01:25:49.000000 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-12 01:25:49.000000 SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 01:25:49.555561 SmoobuExtractorFormatter-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-12 01:25:45.000000 SmoobuExtractorFormatter-1.2.4/setup.py
```

### Comparing `SmoobuExtractorFormatter-1.2.3/LICENSE.txt` & `SmoobuExtractorFormatter-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SmoobuExtractorFormatter-1.2.3/PKG-INFO` & `SmoobuExtractorFormatter-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.3
+Version: 1.2.4
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter/smoobuOutput.py` & `SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter/smoobuOutput.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,80 +187,80 @@
                 
                 
                 number_menage = bookings[names['name_menage']].shape[0]
                 number_sejour = bookings[names['name_taxe']].shape[0]
                 
                 # merging every columns into one : baseprice
                 
-                bookings['basePrice_'] = bookings[names['name_baseprice']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                bookings['basePrice_'] = bookings[names['name_baseprice']].apply(lambda x: [val for val in x if pd.notna(val)])
                 
                 lens1 = bookings['basePrice_'].apply(len_value)
                 
                 del bookings[names['name_baseprice']]
                 
                 bookings['basePrice_'] = bookings['basePrice_'].apply(one_value)
                 
                 
                 # merging every columns into one : frais de menage
                 
-                bookings['frais_menage_'] = bookings[names['name_menage']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                bookings['frais_menage_'] = bookings[names['name_menage']].apply(lambda x: [val for val in x if pd.notna(val)])
                 
 
                 lens = bookings['frais_menage_'].apply(len_value)
                 
                 del bookings[names['name_menage']]
                 
                 bookings['frais_menage_'] = bookings['frais_menage_'].apply(one_value)
                 
                 
                 # merging every columns into one : taxe de sejour
             
             
                 print(bookings[names['name_taxe']].head())
-                bookings['taxe_sejour_'] = bookings[names['name_taxe']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                bookings['taxe_sejour_'] = bookings[names['name_taxe']].apply(lambda x: [val for val in x if pd.notna(val)])
                 lens2 = bookings['taxe_sejour_'].apply(len_value)
                 
                 del bookings[names['name_taxe']]
                 
                 bookings['taxe_sejour_'] = bookings['taxe_sejour_'].apply(one_value)
                 
                 # merge every column into one : commission 
                 
-                bookings['commission_'] = bookings[names['name_commission']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                bookings['commission_'] = bookings[names['name_commission']].apply(lambda x: [val for val in x if pd.notna(val)])
 
                 lens3 = bookings['commission_'].apply(len_value)
                 
                 del bookings[names['name_commission']]
                 
                 bookings['commission_'] = bookings['commission_'].apply(one_value)
                 
                 # merge evry column into one : gestion 
                 
-                bookings['frais_gestion_'] = bookings[names['name_gestion']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                bookings['frais_gestion_'] = bookings[names['name_gestion']].apply(lambda x: [val for val in x if pd.notna(val)])
                 
                 lens4 = bookings['frais_gestion_'].apply(len_value)
                 
                 del bookings[names['name_gestion']]
                 
                 bookings['frais_gestion_'] = bookings['frais_gestion_'].apply(one_value)
                 
                 # merge every column into one : frais_electricite
                 
-                bookings['frais_electricite_'] = bookings[names['name_electricite']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                bookings['frais_electricite_'] = bookings[names['name_electricite']].apply(lambda x: [val for val in x if pd.notna(val)])
                 
                 lens5 = bookings['frais_electricite_'].apply(len_value)
                 
                 del bookings[names['name_electricite']]
                 
                 bookings['frais_electricite_'] = bookings['frais_electricite_'].apply(one_value)
                 
                 
                 # sum every column into one : linge de lit et serviettes 
                 
-                bookings['frais_linge_serviettes_'] = bookings[names['name_linge']].apply(lambda x: [val for val in x if pd.notna(val)], axis=1)
+                bookings['frais_linge_serviettes_'] = bookings[names['name_linge']].apply(lambda x: [val for val in x if pd.notna(val)])
                 
                 lens6 = bookings['frais_linge_serviettes_'].apply(len_value)
                 
                 del bookings[names['name_linge']]
                 
                 bookings['frais_linge_serviettes_'] = bookings['frais_linge_serviettes_'].apply(sum_value)
```

### Comparing `SmoobuExtractorFormatter-1.2.3/SmoobuExtractorFormatter.egg-info/PKG-INFO` & `SmoobuExtractorFormatter-1.2.4/SmoobuExtractorFormatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmoobuExtractorFormatter
-Version: 1.2.3
+Version: 1.2.4
 Summary: A library to format the output of the Smoobu application
 Home-page: UNKNOWN
 Author: Badji Rayane
 Author-email: rayanebadji.freelance@gmail.com
 License: MIT
 Keywords: Smoobu
 Platform: UNKNOWN
```

### Comparing `SmoobuExtractorFormatter-1.2.3/setup.py` & `SmoobuExtractorFormatter-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='SmoobuExtractorFormatter',
-    version='1.2.3',
+    version='1.2.4',
     description='A library to format the output of the Smoobu application',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     uri='',
     author='Badji Rayane',
     author_email='rayanebadji.freelance@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

