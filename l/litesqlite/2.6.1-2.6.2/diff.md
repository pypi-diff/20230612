# Comparing `tmp/litesqlite-2.6.1.tar.gz` & `tmp/litesqlite-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.6.1.tar", last modified: Mon Jun 12 07:56:39 2023, max compression
+gzip compressed data, was "litesqlite-2.6.2.tar", last modified: Mon Jun 12 11:14:10 2023, max compression
```

## Comparing `litesqlite-2.6.1.tar` & `litesqlite-2.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:56:39.172356 litesqlite-2.6.1/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.1/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:56:39.172356 litesqlite-2.6.1/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.1/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:56:39.172356 litesqlite-2.6.1/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.1/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.1/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     7715 2023-06-12 07:56:30.000000 litesqlite-2.6.1/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:56:39.172356 litesqlite-2.6.1/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 07:56:38.000000 litesqlite-2.6.1/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 07:56:39.172356 litesqlite-2.6.1/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 07:56:30.000000 litesqlite-2.6.1/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:14:10.505861 litesqlite-2.6.2/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.2/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:14:10.505861 litesqlite-2.6.2/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.2/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:14:10.501861 litesqlite-2.6.2/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.2/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.2/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8316 2023-06-12 11:13:52.000000 litesqlite-2.6.2/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 11:14:10.505861 litesqlite-2.6.2/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 11:14:10.000000 litesqlite-2.6.2/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 11:14:10.505861 litesqlite-2.6.2/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 11:08:41.000000 litesqlite-2.6.2/setup.py
```

### Comparing `litesqlite-2.6.1/LICENSE` & `litesqlite-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.1/PKG-INFO` & `litesqlite-2.6.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.1
+Version: 2.6.2
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.1/README.md` & `litesqlite-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.1/litesqlite/datatypes.py` & `litesqlite-2.6.2/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.6.1/litesqlite/lite_sqlite.py` & `litesqlite-2.6.2/litesqlite/lite_sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,36 @@
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
     def __enter__(self) -> 'Sqlite':
-        self.__conn = sqlite3.connect(self.__db_name)
-        self.__cursor = self.__conn.cursor()
+        if not self.__conn:
+            self.__conn = sqlite3.connect(self.__db_name)
+            self.__cursor = self.__conn.cursor()
         return self
 
     def create_table(self,
                      table_name: str,
                      columns: Dict[str, Union[DataTypes, str]]) -> None:
         columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
+        if not self.__conn:
+            self.__enter__()
         self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
         self.__conn.commit()
 
     def insert_data(self,
                     table_name: str,
                     data: Dict[str, Union[str, int, float]]) -> None:
         columns = ', '.join(data.keys())
         placeholders = ', '.join(['?' for _ in range(len(data))])
         values = tuple(data.values())
+        if not self.__conn:
+            self.__enter__()
         self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
         self.__conn.commit()
 
     def select_data(self,
                     table_name: str,
                     columns: Union[List[str], str, None] = None,
                     where: Union[str, Dict[str, Union[str, int, float]], None] = None,
@@ -54,43 +59,48 @@
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
         if offset:
             offset_clause = f'OFFSET {offset}'
         else:
             offset_clause = ""
+        if not self.__conn:
+            self.__enter__()
         self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
                               values)
 
         if fetch == DataTypes.Fetch.FETCHONE:
             result = self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = self.__cursor.fetchall()
         return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
                     where: Dict[str, Union[str, int, float]],
                     sign: Union[str, None] = None) -> None:
-        with self:
-            if sign:
-                set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
-            else:
-                set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
-            where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(set_data.values()) + tuple(where.values())
-            self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
-            self.__conn.commit()
+        if sign:
+            set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
+        else:
+            set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
+        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+        values = tuple(set_data.values()) + tuple(where.values())
+        if not self.__conn:
+            self.__enter__()
+        self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+        self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
                     where: Dict[str, Union[str, int, float]]) -> None:
         where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
         values = tuple(where.values())
+        if not self.__conn:
+            self.__enter__()
         self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
         self.__conn.commit()
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         if self.__conn:
             self.__conn.close()
 
@@ -100,37 +110,42 @@
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
     async def __aenter__(self) -> 'AioSqlite':
-        self.__conn = await aiosqlite.connect(self.__db_name)
-        self.__cursor = await self.__conn.cursor()
+        if not self.__conn:
+            self.__conn = await aiosqlite.connect(self.__db_name)
+            self.__cursor = await self.__conn.cursor()
         return self
 
     async def create_table(self,
                            table_name: str,
                            columns: Dict[str, Union[DataTypes, str]]) -> None:
         columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
+        if not self.__conn:
+            self.__aenter__()
         await self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
         await self.__conn.commit()
 
     async def insert_data(self,
                           table_name: str,
                           data: Dict[str, Union[str, int, float]]) -> None:
         columns = ', '.join(data.keys())
         placeholders = ', '.join(['?' for _ in range(len(data))])
         values = tuple(data.values())
+        if not self.__conn:
+            self.__aenter__()
         await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
         await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
-                          columns: Union[List[str], None] = None,
+                          columns: Union[List[str], str, None] = None,
                           where: Union[str, Dict[str, Union[str, int, float]], None] = None,
                           limit: Union[int, None] = None,
                           offset: Union[int, None] = None,
                           fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         if columns:
             columns = ', '.join(columns)
         else:
@@ -145,14 +160,16 @@
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
         if offset:
             offset_clause = f'OFFSET {offset}'
         else:
             offset_clause = ""
+        if not self.__conn:
+            self.__aenter__()
         await self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
                                     values)
 
         if fetch == DataTypes.Fetch.FETCHONE:
             result = await self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = await self.__cursor.fetchall()
@@ -165,22 +182,26 @@
                           sign: Union[str, None] = None) -> None:
         if sign:
             set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
         else:
             set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
         where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
         values = tuple(set_data.values()) + tuple(where.values())
+        if not self.__conn:
+            self.__aenter__()
         await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
         await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
         await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
                           where: Dict[str, Union[str, int, float]]) -> None:
         where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
         values = tuple(where.values())
+        if not self.__conn:
+            self.__aenter__()
         await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
         await self.__conn.commit()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if self.__conn:
             await self.__conn.close()
```

### Comparing `litesqlite-2.6.1/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.2/litesqlite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.6.1
+Version: 2.6.2
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.6.1/setup.py` & `litesqlite-2.6.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.6.1',
+    version='2.6.2',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

