# Comparing `tmp/menousdb-0.1.2.tar.gz` & `tmp/menousdb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menousdb-0.1.2.tar", last modified: Wed May 10 12:36:00 2023, max compression
+gzip compressed data, was "menousdb-0.1.3.tar", last modified: Mon Jun 12 11:32:17 2023, max compression
```

## Comparing `menousdb-0.1.2.tar` & `menousdb-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:36:00.866471 menousdb-0.1.2/
--rw-r--r--   0 sumanlaskar   (501) staff       (20)     2334 2023-05-10 12:36:00.864407 menousdb-0.1.2/PKG-INFO
--rw-r--r--   0 sumanlaskar   (501) staff       (20)      595 2023-05-10 12:23:09.000000 menousdb-0.1.2/README.md
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:36:00.855256 menousdb-0.1.2/menousdb/
--rw-r--r--   0 sumanlaskar   (501) staff       (20)     8305 2023-05-10 12:22:11.000000 menousdb-0.1.2/menousdb/__init__.py
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:36:00.863818 menousdb-0.1.2/menousdb.egg-info/
--rw-r--r--   0 sumanlaskar   (501) staff       (20)     2334 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/PKG-INFO
--rw-r--r--   0 sumanlaskar   (501) staff       (20)      198 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/SOURCES.txt
--rw-r--r--   0 sumanlaskar   (501) staff       (20)        1 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/dependency_links.txt
--rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/requires.txt
--rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/top_level.txt
--rw-r--r--   0 sumanlaskar   (501) staff       (20)       38 2023-05-10 12:36:00.866722 menousdb-0.1.2/setup.cfg
--rw-r--r--   0 sumanlaskar   (501) staff       (20)     2116 2023-05-10 12:35:45.000000 menousdb-0.1.2/setup.py
+drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-06-12 11:32:17.787049 menousdb-0.1.3/
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     7535 2023-06-12 11:32:17.785935 menousdb-0.1.3/PKG-INFO
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     5796 2023-06-12 11:22:31.000000 menousdb-0.1.3/README.md
+drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-06-12 11:32:17.767125 menousdb-0.1.3/menousdb/
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     8801 2023-06-12 11:20:06.000000 menousdb-0.1.3/menousdb/__init__.py
+drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-06-12 11:32:17.785031 menousdb-0.1.3/menousdb.egg-info/
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     7535 2023-06-12 11:32:17.000000 menousdb-0.1.3/menousdb.egg-info/PKG-INFO
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)      198 2023-06-12 11:32:17.000000 menousdb-0.1.3/menousdb.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)        1 2023-06-12 11:32:17.000000 menousdb-0.1.3/menousdb.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-06-12 11:32:17.000000 menousdb-0.1.3/menousdb.egg-info/requires.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-06-12 11:32:17.000000 menousdb-0.1.3/menousdb.egg-info/top_level.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)       38 2023-06-12 11:32:17.787279 menousdb-0.1.3/setup.cfg
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     2061 2023-06-12 11:06:43.000000 menousdb-0.1.3/setup.py
```

### Comparing `menousdb-0.1.2/menousdb/__init__.py` & `menousdb-0.1.3/menousdb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,28 @@
     def __init__(self, url, key, database):
         self.url = url
         self.key = key
         self.database = database
         if self.url[-1] != '/':
             self.url += '/'
 
-    def readDB(self):
+    def readDb(self):
 
         if self.database == None:
             raise Exception('No database')
 
         Headers = {
             'key': self.key,
             'database': self.database
         }
         ans = req.get(self.url + 'read-db', headers=Headers)
         try:
             return ans.json()
         except:
-            return ans.text
+            raise Exception(ans.text)
 
 
     def createDb(self):
 
         if self.database == None:
             raise Exception('No database')
         try:
@@ -74,15 +74,15 @@
 
             ans = req.post(self.url + 'create-db', headers=Headers)
             return ans.text
 
         except Exception as ex:
             raise ex
 
-    def deleteDatabase(self):
+    def deleteDb(self):
         if self.database == None:
             raise Exception('No database')
         try:
 
             Headers = {
                 'key': self.key,
                 'database': self.database
@@ -167,15 +167,32 @@
                 'values': values,
             }
 
             ans = req.post(self.url + 'insert-into-table', headers=Headers, json=Json)
             return ans.text
 
         except Exception as ex:
-            print(ex)
+            raise ex
+
+    def getTable(self,table):
+        if self.database is None:
+            raise Exception("No database ")
+        try:
+            Headers = {
+                'key': self.key,
+                'database': self.database,
+                'table': table
+            }
+            ans = req.get(self.url + 'get-table', headers=Headers, json=Json)
+            try:
+                return ans.json()
+            except:
+                return ans.text
+        except Exception as ex:
+            raise ex
 
     def selectWhere(self, table, conditions):
         if self.database == None:
             raise Exception('No database')
         try:
 
             Headers = {
@@ -240,15 +257,15 @@
                 return ans.json()
             except:
                 return ans.text
 
         except Exception as ex:
             raise ex
 
-    def delete_where(self, table, conditions):
+    def deleteWhere(self, table, conditions):
         if self.database == None:
             raise Exception('No Database')
         try:
             Headers = {
                 'key': self.key,
                 'database': self.database,
                 'table': table,
@@ -259,35 +276,35 @@
 
             ans = req.delete(self.url+"delete-where", headers = Headers, json = Json)
             try:
                 return ans.json()
             except:
                 return ans.text
         except Exception as ex:
-            return ex
+            raise ex
 
-    def delete_table(self, table):
+    def deleteTable(self, table):
             if self.database == None:
                 raise Exception('No Database')
             try:
                 Headers = {
                     'key': self.key,
                     'database': self.database,
                     'table': table,
                 }
                 ans = req.delete(self.url + "delete-table", headers=Headers)
                 try:
                     return ans.json()
                 except:
                     return ans.text
             except Exception as ex:
-                return ex
+                raise ex
 
 
-    def update_table(self, table, conditions, values):
+    def updateWhere(self, table, conditions, values):
         try:
             Headers = {
                 'key': self.key,
                 'database': self.database,
                 'table': table,
             }
             Json = {
@@ -296,23 +313,23 @@
             }
             ans = req.post(self.url+'update-table', headers=Headers, json = Json)
             try:
                 return ans.json()
             except:
                 return ans.text
         except Exception as ex:
-            return ex
+            raise ex
         
-    def get_databases(self):
+    def getDatabases(self):
         try:
             Headers = {
                 'key': self.key,
             }
             ans = req.get(self.url+'get-databases', headers=Headers)
             try:
                 return ans.json()
             except:
                 return ans.text()
         except Exception as ex:
-            return ex
+            raise ex
```

### Comparing `menousdb-0.1.2/setup.py` & `menousdb-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'A SDK for Menous DB'
-LONG_DESCRIPTION = 'A package that allows to interact with Menous DB directly in python.'
+LONG_DESCRIPTION = long_description
 LICENSE="""
 MIT License
 
 Copyright (c) 2022 Snehashish Laskar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

