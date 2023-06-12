# Comparing `tmp/denpy-1.0.5.tar.gz` & `tmp/denpy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-1.0.5.tar", last modified: Mon Jun 12 14:43:29 2023, max compression
+gzip compressed data, was "denpy-1.0.6.tar", last modified: Mon Jun 12 14:48:14 2023, max compression
```

## Comparing `denpy-1.0.5.tar` & `denpy-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:43:29.111917 denpy-1.0.5/
--rw-rw-rw-   0        0        0      112 2023-06-12 14:43:29.110919 denpy-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 14:43:29.105933 denpy-1.0.5/denpy/
--rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.5/denpy/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.5/denpy/color.py
--rw-rw-rw-   0        0        0     1775 2023-06-12 14:43:22.000000 denpy-1.0.5/denpy/database.py
--rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.5/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:43:29.109922 denpy-1.0.5/denpy.egg-info/
--rw-rw-rw-   0        0        0      112 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 14:43:29.000000 denpy-1.0.5/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 14:43:29.111917 denpy-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      205 2023-06-12 14:43:22.000000 denpy-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:48:14.780609 denpy-1.0.6/
+-rw-rw-rw-   0        0        0      112 2023-06-12 14:48:14.779611 denpy-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 14:48:14.774624 denpy-1.0.6/denpy/
+-rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.6/denpy/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.6/denpy/color.py
+-rw-rw-rw-   0        0        0     1784 2023-06-12 14:47:58.000000 denpy-1.0.6/denpy/database.py
+-rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.6/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:48:14.778614 denpy-1.0.6/denpy.egg-info/
+-rw-rw-rw-   0        0        0      112 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-12 14:48:14.000000 denpy-1.0.6/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:48:14.780609 denpy-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      205 2023-06-12 14:48:10.000000 denpy-1.0.6/setup.py
```

### Comparing `denpy-1.0.5/denpy/database.py` & `denpy-1.0.6/denpy/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     return data if data is None else data[0]
 
 def edit(table: str, data: str, new_data: str, __file__: str, where: str = None):
     database, cursor = connect(__file__=__file__)
     if where is None:
         cursor.execute(f'UPDATE {table} SET {data} = {new_data}')
     else:
-        cursor.execute(f'UPDATE {table} SET {data} WHERE ?', (where,))
+        cursor.execute(f'UPDATE {table} SET {data} = {new_data} WHERE {where}')
     disconnect(database, cursor)
 
 def remove(table: str, __file__: str, where: str = None):
     database, cursor = connect(__file__=__file__)
     if where is None:
         cursor.execute(f'DELETE FROM {table}')
     else:
```

### Comparing `denpy-1.0.5/denpy/utils.py` & `denpy-1.0.6/denpy/utils.py`

 * *Files identical despite different names*

