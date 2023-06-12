# Comparing `tmp/denpy-1.0.4.tar.gz` & `tmp/denpy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-1.0.4.tar", last modified: Fri Jun  9 21:50:28 2023, max compression
+gzip compressed data, was "denpy-1.0.5.tar", last modified: Mon Jun 12 14:43:29 2023, max compression
```

## Comparing `denpy-1.0.4.tar` & `denpy-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 21:50:28.574699 denpy-1.0.4/
--rw-rw-rw-   0        0        0      112 2023-06-09 21:50:28.574699 denpy-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 21:50:28.569744 denpy-1.0.4/denpy/
--rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.4/denpy/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.4/denpy/color.py
--rw-rw-rw-   0        0        0     1716 2023-06-09 21:49:51.000000 denpy-1.0.4/denpy/database.py
--rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.4/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 21:50:28.573701 denpy-1.0.4/denpy.egg-info/
--rw-rw-rw-   0        0        0      112 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-09 21:50:28.000000 denpy-1.0.4/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 21:50:28.574699 denpy-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      205 2023-06-09 21:50:22.000000 denpy-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:43:29.111917 denpy-1.0.5/
+-rw-rw-rw-   0        0        0      112 2023-06-12 14:43:29.110919 denpy-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 14:43:29.105933 denpy-1.0.5/denpy/
+-rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.5/denpy/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.5/denpy/color.py
+-rw-rw-rw-   0        0        0     1775 2023-06-12 14:43:22.000000 denpy-1.0.5/denpy/database.py
+-rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.5/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:43:29.109922 denpy-1.0.5/denpy.egg-info/
+-rw-rw-rw-   0        0        0      112 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:43:29.111917 denpy-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      205 2023-06-12 14:43:22.000000 denpy-1.0.5/setup.py
```

### Comparing `denpy-1.0.4/denpy/database.py` & `denpy-1.0.5/denpy/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import sqlite3
 
 def connect(__file__: str) -> tuple[sqlite3.Connection, sqlite3.Cursor]:
-    path = __file__.split('/')
+    path = __file__.replace('\\', '/').split('/')
     path.pop(-1)
     path.pop(-1)
     path.append('database.db')
     database = sqlite3.connect('/'.join(path))
     cursor = database.cursor()
     return database, cursor
 
 def disconnect(database: sqlite3.Connection, cursor: sqlite3.Cursor):
     database.commit()
     cursor.close()
     database.close()
 
 def add(table: str, data: str, values: list, __file__: str):
-    database, cursor = connect(__file__)
+    database, cursor = connect(__file__=__file__)
     cursor.execute(f'INSERT INTO {table}({data}) VALUES({", ".join(values)})')
     disconnect(database, cursor)
 
 def get(table: str, data: str, __file__: str, where: str = None) -> str or None:
-    database, cursor = connect(__file__)
+    database, cursor = connect(__file__=__file__)
     if where is None:
         data = cursor.execute(f'SELECT {data} FROM {table}').fetchone()
     else:
         data = cursor.execute(f'SELECT {data} FROM {table} WHERE {where}').fetchone()
     disconnect(database, cursor)
     return data if data is None else data[0]
 
 def edit(table: str, data: str, new_data: str, __file__: str, where: str = None):
-    database, cursor = connect(__file__)
+    database, cursor = connect(__file__=__file__)
     if where is None:
         cursor.execute(f'UPDATE {table} SET {data} = {new_data}')
     else:
-        cursor.execute(f'UPDATE {table} SET {data} WHERE {where}')
+        cursor.execute(f'UPDATE {table} SET {data} WHERE ?', (where,))
     disconnect(database, cursor)
 
 def remove(table: str, __file__: str, where: str = None):
-    database, cursor = connect(__file__)
+    database, cursor = connect(__file__=__file__)
     if where is None:
         cursor.execute(f'DELETE FROM {table}')
     else:
         cursor.execute(f'DELETE FROM {table} WHERE {where.split(" = ")[0]} = ?', (where.split(" = ")[1],))
     disconnect(database, cursor)
```

### Comparing `denpy-1.0.4/denpy/utils.py` & `denpy-1.0.5/denpy/utils.py`

 * *Files identical despite different names*

