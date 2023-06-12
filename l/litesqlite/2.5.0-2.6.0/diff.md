# Comparing `tmp/litesqlite-2.5.0.tar.gz` & `tmp/litesqlite-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.5.0.tar", last modified: Sun Jun 11 18:14:14 2023, max compression
+gzip compressed data, was "litesqlite-2.6.0.tar", last modified: Mon Jun 12 07:12:28 2023, max compression
```

## Comparing `litesqlite-2.5.0.tar` & `litesqlite-2.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:14:14.649854 litesqlite-2.5.0/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.5.0/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 18:14:14.649854 litesqlite-2.5.0/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.5.0/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:14:14.649854 litesqlite-2.5.0/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.5.0/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.5.0/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8652 2023-06-11 18:11:02.000000 litesqlite-2.5.0/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-11 18:14:14.649854 litesqlite-2.5.0/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-11 18:14:14.000000 litesqlite-2.5.0/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-11 18:14:14.649854 litesqlite-2.5.0/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-11 18:12:38.000000 litesqlite-2.5.0/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:12:28.181785 litesqlite-2.6.0/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.6.0/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:12:28.181785 litesqlite-2.6.0/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     3028 2023-06-10 20:40:52.000000 litesqlite-2.6.0/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:12:28.181785 litesqlite-2.6.0/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.6.0/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.6.0/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     7714 2023-06-12 07:11:31.000000 litesqlite-2.6.0/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-12 07:12:28.181785 litesqlite-2.6.0/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-12 07:12:27.000000 litesqlite-2.6.0/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-12 07:12:28.181785 litesqlite-2.6.0/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-12 07:12:14.000000 litesqlite-2.6.0/setup.py
```

### Comparing `litesqlite-2.5.0/LICENSE` & `litesqlite-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.5.0/PKG-INFO` & `litesqlite-2.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.5.0
+Version: 2.6.0
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.5.0/README.md` & `litesqlite-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.5.0/litesqlite/datatypes.py` & `litesqlite-2.6.0/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.5.0/litesqlite/lite_sqlite.py` & `litesqlite-2.6.0/litesqlite/lite_sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,75 @@
 import aiosqlite
 import sqlite3
 from typing import Dict, Union, Tuple, List
-from .datatypes import DataTypes
+from datatypes import DataTypes
 
 
 class Sqlite:
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
-    def open_conn(self) -> None:
-        try:
-            self.__conn = sqlite3.connect(self.__db_name)
-            self.__cursor = self.__conn.cursor()
-        except:
-            pass
-
     def __enter__(self) -> 'Sqlite':
-        self.open_conn()
+        self.__conn = sqlite3.connect(self.__db_name)
+        self.__cursor = self.__conn.cursor()
         return self
 
     def create_table(self,
                      table_name: str,
                      columns: Dict[str, Union[DataTypes, str]]) -> None:
-        with self:
-            columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
-            self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
-            self.__conn.commit()
+        columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
+        self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
+        self.__conn.commit()
 
     def insert_data(self,
                     table_name: str,
                     data: Dict[str, Union[str, int, float]]) -> None:
-        with self:
-            columns = ', '.join(data.keys())
-            placeholders = ', '.join(['?' for _ in range(len(data))])
-            values = tuple(data.values())
-            self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
-            self.__conn.commit()
+        columns = ', '.join(data.keys())
+        placeholders = ', '.join(['?' for _ in range(len(data))])
+        values = tuple(data.values())
+        self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
+        self.__conn.commit()
 
     def select_data(self,
                     table_name: str,
                     columns: Union[List[str], str, None] = None,
                     where: Union[str, Dict[str, Union[str, int, float]], None] = None,
                     limit: Union[int, None] = None,
                     offset: Union[int, None] = None,
                     fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
-        with self:
-            if columns:
-                columns = ', '.join(columns)
-            else:
-                columns = '*'
-            if where:
-                where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
-                values = tuple(where.values())
-            else:
-                where_clause = ''
-                values = ()
-            if limit:
-                limit_clause = f"LIMIT {limit}"
-            else:
-                limit_clause = ""
-            if offset:
-                offset_clause = f'OFFSET {offset}'
-            else:
-                offset_clause = ""
-            self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
-                                  values)
-
-            if fetch == DataTypes.Fetch.FETCHONE:
-                result = self.__cursor.fetchone()
-            elif fetch == DataTypes.Fetch.FETCHALL:
-                result = self.__cursor.fetchall()
-            return result
+        if columns:
+            columns = ', '.join(columns)
+        else:
+            columns = '*'
+        if where:
+            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(where.values())
+        else:
+            where_clause = ''
+            values = ()
+        if limit:
+            limit_clause = f"LIMIT {limit}"
+        else:
+            limit_clause = ""
+        if offset:
+            offset_clause = f'OFFSET {offset}'
+        else:
+            offset_clause = ""
+        self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
+                              values)
+
+        if fetch == DataTypes.Fetch.FETCHONE:
+            result = self.__cursor.fetchone()
+        elif fetch == DataTypes.Fetch.FETCHALL:
+            result = self.__cursor.fetchall()
+        return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
                     where: Dict[str, Union[str, int, float]],
                     sign: Union[str, None] = None) -> None:
         with self:
@@ -90,128 +81,106 @@
             values = tuple(set_data.values()) + tuple(where.values())
             self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
             self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
                     where: Dict[str, Union[str, int, float]]) -> None:
-        with self:
-            where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
-            self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
-            self.__conn.commit()
-
-    def close_conn(self) -> None:
-        self.__conn.close()
+        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+        values = tuple(where.values())
+        self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
+        self.__conn.commit()
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        try:
-            self.close_conn()
-        except:
-            pass
+        if self.__conn:
+            self.__conn.close()
 
 
 class AioSqlite:
 
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
-    async def open_conn(self) -> None:
-        try:
-            self.__conn = await aiosqlite.connect(self.__db_name)
-            self.__cursor = await self.__conn.cursor()
-        except:
-            pass
-
     async def __aenter__(self) -> 'AioSqlite':
-        await self.open_conn()
+        self.__conn = await aiosqlite.connect(self.__db_name)
+        self.__cursor = await self.__conn.cursor()
         return self
 
     async def create_table(self,
                            table_name: str,
                            columns: Dict[str, Union[DataTypes, str]]) -> None:
-        async with self:
-            columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
-            await self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
-            await self.__conn.commit()
+        columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
+        await self.__cursor.execute(f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})")
+        await self.__conn.commit()
 
     async def insert_data(self,
                           table_name: str,
                           data: Dict[str, Union[str, int, float]]) -> None:
-        async with self:
-            columns = ', '.join(data.keys())
-            placeholders = ', '.join(['?' for _ in range(len(data))])
-            values = tuple(data.values())
-            await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
-            await self.__conn.commit()
+        columns = ', '.join(data.keys())
+        placeholders = ', '.join(['?' for _ in range(len(data))])
+        values = tuple(data.values())
+        await self.__cursor.execute(f"INSERT INTO {table_name} ({columns}) VALUES ({placeholders})", values)
+        await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
                           columns: Union[List[str], None] = None,
                           where: Union[str, Dict[str, Union[str, int, float]], None] = None,
                           limit: Union[int, None] = None,
                           offset: Union[int, None] = None,
                           fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
-        async with self:
-            if columns:
-                columns = ', '.join(columns)
-            else:
-                columns = '*'
-            if where:
-                where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
-                values = tuple(where.values())
-            else:
-                where_clause = ''
-                values = ()
-            if limit:
-                limit_clause = f"LIMIT {limit}"
-            else:
-                limit_clause = ""
-            if offset:
-                offset_clause = f'OFFSET {offset}'
-            else:
-                offset_clause = ""
-            await self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
-                                        values)
-
-            if fetch == DataTypes.Fetch.FETCHONE:
-                result = await self.__cursor.fetchone()
-            elif fetch == DataTypes.Fetch.FETCHALL:
-                result = await self.__cursor.fetchall()
-            return result
+        if columns:
+            columns = ', '.join(columns)
+        else:
+            columns = '*'
+        if where:
+            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
+            values = tuple(where.values())
+        else:
+            where_clause = ''
+            values = ()
+        if limit:
+            limit_clause = f"LIMIT {limit}"
+        else:
+            limit_clause = ""
+        if offset:
+            offset_clause = f'OFFSET {offset}'
+        else:
+            offset_clause = ""
+        await self.__cursor.execute(f"SELECT {columns} FROM {table_name} {where_clause} {limit_clause} {offset_clause}",
+                                    values)
+
+        if fetch == DataTypes.Fetch.FETCHONE:
+            result = await self.__cursor.fetchone()
+        elif fetch == DataTypes.Fetch.FETCHALL:
+            result = await self.__cursor.fetchall()
+        return result
 
     async def update_data(self,
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
-            await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
-            await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
-            await self.__conn.commit()
+        if sign:
+            set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
+        else:
+            set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
+        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+        values = tuple(set_data.values()) + tuple(where.values())
+        await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+        await self.__cursor.execute(f"UPDATE {table_name} SET {set_clause} WHERE {where_clause}", values)
+        await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
                           where: Dict[str, Union[str, int, float]]) -> None:
-        with self:
-            where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
-            await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
-            await self.__conn.commit()
-
-    async def close_conn(self) -> None:
-        await self.__conn.close()
+        where_clause = ' AND '.join([f'{col}=?' for col in where.keys()])
+        values = tuple(where.values())
+        await self.__cursor.execute(f"DELETE FROM {table_name} WHERE {where_clause}", values)
+        await self.__conn.commit()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        try:
-            await self.close_conn()
-        except:
-            pass
+        if self.__conn:
+            await self.__conn.close()
```

### Comparing `litesqlite-2.5.0/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.6.0/litesqlite.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.5.0
+Version: 2.6.0
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.5.0/setup.py` & `litesqlite-2.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.5.0',
+    version='2.6.0',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

