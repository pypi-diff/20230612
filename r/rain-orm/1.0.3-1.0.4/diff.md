# Comparing `tmp/rain_orm-1.0.3.tar.gz` & `tmp/rain_orm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rain_orm-1.0.3.tar", last modified: Wed May 31 18:11:26 2023, max compression
+gzip compressed data, was "rain_orm-1.0.4.tar", last modified: Mon Jun 12 11:26:25 2023, max compression
```

## Comparing `rain_orm-1.0.3.tar` & `rain_orm-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.511297 rain_orm-1.0.3/
--rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3049 2023-05-31 18:11:26.512316 rain_orm-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2768 2023-05-31 18:03:33.000000 rain_orm-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.494241 rain_orm-1.0.3/rain_orm/
--rw-rw-rw-   0        0        0      139 2023-05-31 18:07:58.000000 rain_orm-1.0.3/rain_orm/__init__.py
--rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.3/rain_orm/common.py
--rw-rw-rw-   0        0        0      781 2023-05-30 18:06:06.000000 rain_orm-1.0.3/rain_orm/db.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.505288 rain_orm-1.0.3/rain_orm/error/
--rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.3/rain_orm/error/__init__.py
--rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.3/rain_orm/error/error.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.509286 rain_orm-1.0.3/rain_orm/sql_builder/
--rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.3/rain_orm/sql_builder/__init__.py
--rw-rw-rw-   0        0        0       29 2023-05-30 17:52:43.000000 rain_orm-1.0.3/rain_orm/sql_builder/ddl_builder.py
--rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.3/rain_orm/sql_builder/dmldql_builder.py
--rw-rw-rw-   0        0        0     5918 2023-05-31 18:02:57.000000 rain_orm-1.0.3/rain_orm/table.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.501280 rain_orm-1.0.3/rain_orm.egg-info/
--rw-rw-rw-   0        0        0     3049 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-31 18:11:26.000000 rain_orm-1.0.3/rain_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-31 18:11:26.513287 rain_orm-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      474 2023-05-31 18:07:58.000000 rain_orm-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:11:26.510292 rain_orm-1.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.359308 rain_orm-1.0.4/
+-rw-rw-rw-   0        0        0    11555 2023-05-28 17:49:39.000000 rain_orm-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3399 2023-06-12 11:26:25.360304 rain_orm-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3118 2023-06-12 11:21:58.000000 rain_orm-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.326174 rain_orm-1.0.4/rain_orm/
+-rw-rw-rw-   0        0        0      139 2023-06-12 11:25:53.000000 rain_orm-1.0.4/rain_orm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.346175 rain_orm-1.0.4/rain_orm/column/
+-rw-rw-rw-   0        0        0      153 2023-06-05 03:57:35.000000 rain_orm-1.0.4/rain_orm/column/__init__.py
+-rw-rw-rw-   0        0        0     1576 2023-06-05 11:20:16.000000 rain_orm-1.0.4/rain_orm/column/base.py
+-rw-rw-rw-   0        0        0      271 2023-06-05 03:57:35.000000 rain_orm-1.0.4/rain_orm/column/date.py
+-rw-rw-rw-   0        0        0      400 2023-06-05 03:57:35.000000 rain_orm-1.0.4/rain_orm/column/number.py
+-rw-rw-rw-   0        0        0      688 2023-06-05 10:24:07.000000 rain_orm-1.0.4/rain_orm/column/string.py
+-rw-rw-rw-   0        0        0      311 2023-05-29 18:48:08.000000 rain_orm-1.0.4/rain_orm/common.py
+-rw-rw-rw-   0        0        0      781 2023-06-05 00:52:45.000000 rain_orm-1.0.4/rain_orm/db.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.349175 rain_orm-1.0.4/rain_orm/error/
+-rw-rw-rw-   0        0        0      153 2023-05-30 17:55:36.000000 rain_orm-1.0.4/rain_orm/error/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-05-30 16:40:48.000000 rain_orm-1.0.4/rain_orm/error/error.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.356308 rain_orm-1.0.4/rain_orm/sql_builder/
+-rw-rw-rw-   0        0        0      178 2023-05-30 17:56:14.000000 rain_orm-1.0.4/rain_orm/sql_builder/__init__.py
+-rw-rw-rw-   0        0        0     1280 2023-06-08 12:04:47.000000 rain_orm-1.0.4/rain_orm/sql_builder/ddl_builder.py
+-rw-rw-rw-   0        0        0     5961 2023-05-30 17:43:33.000000 rain_orm-1.0.4/rain_orm/sql_builder/dmldql_builder.py
+-rw-rw-rw-   0        0        0     6977 2023-06-08 02:54:13.000000 rain_orm-1.0.4/rain_orm/table.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.335176 rain_orm-1.0.4/rain_orm.egg-info/
+-rw-rw-rw-   0        0        0     3399 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 11:26:25.000000 rain_orm-1.0.4/rain_orm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 11:26:25.360304 rain_orm-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      474 2023-06-12 11:25:53.000000 rain_orm-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 11:26:25.358307 rain_orm-1.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:46:43.000000 rain_orm-1.0.4/tests/__init__.py
```

### Comparing `rain_orm-1.0.3/LICENSE` & `rain_orm-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.3/PKG-INFO` & `rain_orm-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: rain_orm
-Version: 1.0.3
-Summary: a tiny orm frame
-Home-page: https://github.com/cgynb/rain-orm
-Author: rain
-Author-email: 948628463@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # rain-orm
 
 a tiny orm frame
 
 # Install
 
 it's easy to install via pip
@@ -30,46 +18,48 @@
 
 | id  | name | password | class_id |
 |-----|------|----------|----------|
 |     |      |          |          |
 
 ```python
 import rain_orm
+from rain_orm.column import Int, VarChar
 
-rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
+rain_orm.connect(host="localhost", port=3306, user="root", password="123456", database="student_management")
 
 
 class StudentModel(rain_orm.Table):
     __table__ = "students"
     __fields__ = {
-        "id": None,
-        "name": None,
-        "password": None,
-        "class_id": None
+        "id": Int(auto_increment=True, primary_key=True),
+        "name": VarChar(30, unique=True),
+        "password": VarChar(30),
+        "class_id": Int(default=1)
     }
 
 if __name__ == "__main__":
+    rain_orm.Table.auto_migrate()
     stu = StudentModel().where("id=?", 1).one()
-    print("id: ", stu.id)
-    print("name: ", stu.name)
     print(stu)
+
 ```
 result
 
 ```cmd
 id: 1
 name: cgy
-<<StudentModel 2109293369984
-    .table = students
-    .instance = {
-        id: 1,
-        name: cgy,
-        password: None,
-        class_id: 1,
-    }
+<< StudentModel 1951412882544
+	.table = students
+	.fields = ['id', 'name', 'password', 'gender', 'origin', 'class_id']
+	.instance = {
+		id: 1,
+		name: cgy,
+		password: 123456,
+		class_id: 1,
+	}
 >>
 ```
 
 # Basic Usage
 
 it's easy to use rain-orm
 
@@ -89,24 +79,33 @@
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 ```
 
 ## Define Model
 
 each data must have a unique "id"
 ```python
-class StudentModel(RainORM):
+import rain_orm
+from rain_orm.column import Int, VarChar
+
+class StudentModel(rain_orm.Table):
     __table__ = "students"
     __fields__ = {
-        "id": None,
-        "name": None,
-        "password": None,
-        "class_id": None
+        "id": Int(auto_increment=True, primary_key=True),
+        "name": VarChar(30, unique=True),
+        "password": VarChar(30),
+        "class_id": Int(default=1)
     }
+
+```
+## Auto Migrate
+```python
+rain_orm.Table.auto_migrate()
 ```
 
+
 ## CRUD Example
 
 ### Read
 
 ```python
 # student list
 stu_lst = StudentModel().all()
@@ -137,15 +136,15 @@
 		class_id: 1,
 	}
 >>
 ```
 
 ### Update
 
-there 2 ways to update data
+there are 2 ways to update data
 
 ```python
 StudentModel().where("id = ?", 22).one()  # get student instance first
 # 1. set attribute (recommend)
 stu.name = "your name"
 # 2. call update methods
 ok = stu.update("name", "your name")
```

### Comparing `rain_orm-1.0.3/README.md` & `rain_orm-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: rain_orm
+Version: 1.0.4
+Summary: a tiny orm frame
+Home-page: https://github.com/cgynb/rain-orm
+Author: rain
+Author-email: 948628463@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # rain-orm
 
 a tiny orm frame
 
 # Install
 
 it's easy to install via pip
@@ -18,46 +30,48 @@
 
 | id  | name | password | class_id |
 |-----|------|----------|----------|
 |     |      |          |          |
 
 ```python
 import rain_orm
+from rain_orm.column import Int, VarChar
 
-rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
+rain_orm.connect(host="localhost", port=3306, user="root", password="123456", database="student_management")
 
 
 class StudentModel(rain_orm.Table):
     __table__ = "students"
     __fields__ = {
-        "id": None,
-        "name": None,
-        "password": None,
-        "class_id": None
+        "id": Int(auto_increment=True, primary_key=True),
+        "name": VarChar(30, unique=True),
+        "password": VarChar(30),
+        "class_id": Int(default=1)
     }
 
 if __name__ == "__main__":
+    rain_orm.Table.auto_migrate()
     stu = StudentModel().where("id=?", 1).one()
-    print("id: ", stu.id)
-    print("name: ", stu.name)
     print(stu)
+
 ```
 result
 
 ```cmd
 id: 1
 name: cgy
-<<StudentModel 2109293369984
-    .table = students
-    .instance = {
-        id: 1,
-        name: cgy,
-        password: None,
-        class_id: 1,
-    }
+<< StudentModel 1951412882544
+	.table = students
+	.fields = ['id', 'name', 'password', 'gender', 'origin', 'class_id']
+	.instance = {
+		id: 1,
+		name: cgy,
+		password: 123456,
+		class_id: 1,
+	}
 >>
 ```
 
 # Basic Usage
 
 it's easy to use rain-orm
 
@@ -77,24 +91,33 @@
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 ```
 
 ## Define Model
 
 each data must have a unique "id"
 ```python
-class StudentModel(RainORM):
+import rain_orm
+from rain_orm.column import Int, VarChar
+
+class StudentModel(rain_orm.Table):
     __table__ = "students"
     __fields__ = {
-        "id": None,
-        "name": None,
-        "password": None,
-        "class_id": None
+        "id": Int(auto_increment=True, primary_key=True),
+        "name": VarChar(30, unique=True),
+        "password": VarChar(30),
+        "class_id": Int(default=1)
     }
+
+```
+## Auto Migrate
+```python
+rain_orm.Table.auto_migrate()
 ```
 
+
 ## CRUD Example
 
 ### Read
 
 ```python
 # student list
 stu_lst = StudentModel().all()
@@ -125,23 +148,26 @@
 		class_id: 1,
 	}
 >>
 ```
 
 ### Update
 
-there 2 ways to update data
+there are 2 ways to update data
 
 ```python
 StudentModel().where("id = ?", 22).one()  # get student instance first
 # 1. set attribute (recommend)
 stu.name = "your name"
 # 2. call update methods
 ok = stu.update("name", "your name")
 ```
 
 ### Delete
 
 ```python
 StudentModel().where("id = ?", 22).one()  # get student instance first
 ok = stu.delete()  # call delete method
-```
+```
+
+
+
```

### Comparing `rain_orm-1.0.3/rain_orm/db.py` & `rain_orm-1.0.4/rain_orm/db.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.3/rain_orm/sql_builder/dmldql_builder.py` & `rain_orm-1.0.4/rain_orm/sql_builder/dmldql_builder.py`

 * *Files identical despite different names*

### Comparing `rain_orm-1.0.3/rain_orm/table.py` & `rain_orm-1.0.4/rain_orm/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,106 @@
 try:
     from rain_orm.error import DefineError, SqlBuildError, UpdateError
-    from rain_orm.sql_builder import DMLDQLBuilder
+    from rain_orm.sql_builder import DMLDQLBuilder, DDLBuilder
+    from rain_orm.column import Type
     from rain_orm.db import DB
 except ImportError as e:
     print(e)
     from error import DefineError, SqlBuildError, UpdateError
-    from sql_builder import DMLDQLBuilder
+    from sql_builder import DMLDQLBuilder, DDLBuilder
+    from column import Type
     from db import DB
 import pymysql
 import threading
 import copy
 
 
 class Table(object):
     __db = None
     __lock = threading.Lock()
 
     @classmethod
     def set_db(cls, db):
         cls.__db = db
 
-    # @classmethod
-    # def auto_migrate(cls):
-    #     # TODO: DDL
-    #     print(cls.__subclasses__())
+    @classmethod
+    def auto_migrate(cls):
+        ddls = []
+        for subcls in cls.__subclasses__():
+            ddl_builder = DDLBuilder(subcls.__table__)
+            for k, v in subcls.__fields__.items():
+                ddl_builder.add_field(field_name=k, field_type=v.type_name, **v.constraint)
+            ddls.append(ddl_builder.create_sql)
+        with cls.__lock:
+            for ddl in ddls:
+                cls.__db.cursor.execute(ddl)
+            cls.__db.commit()
 
     def __init__(self, **kwargs):
         if not isinstance(self.__table__, str):
-            raise DefineError(f"type(__table__) should be str, but is {type(self.__table__)}")
+            raise ValueError(f"type(__table__) should be str, but is {type(self.__table__)}")
         if not isinstance(self.__fields__, dict):
-            raise DefineError(f"type(__fields__) should be dict, but is {type(self.__fields__)}")
+            raise ValueError(f"type(__fields__) should be dict, but is {type(self.__fields__)}")
+        if not all([isinstance(item, Type) for _, item in self.__fields__.items()]):
+            raise ValueError(f"items of __fields__ should be instance of rain_orm.column.Type")
 
         self.instance = copy.deepcopy(self.__fields__)
         self.__dmldql_builder = DMLDQLBuilder(self.__table__)
         for k, v in kwargs.items():
-            self.instance[k] = v
+            self.instance[k].value = v
 
     def __str__(self):
         table = self.__table__
+        fields = list(self.__fields__.keys())
         instance = "{\n"
         for k, v in self.instance.items():
+            if isinstance(v.value, str):
+                v = f"'{v.value}'"
             instance += f"\t\t{k}: {v},\n"
         instance += "\t}"
         return f"\033[0;36m<< {self.__class__.__name__} {id(self)}\033[0m\n" \
                f"\t\033[0;32m.table\033[0m = {table}\n" \
+               f"\t\033[0;32m.fields\033[0m = {fields}\n" \
                f"\t\033[0;32m.instance\033[0m = {instance}\n" \
                f"\033[0;36m>>\033[0m\n"
 
     def __repr__(self):
         return str(self)
 
     def __getattr__(self, key):
-        return self.instance.get(key)
+        return self.instance.get(key).value
 
     # update
     def __setattr__(self, key, value):
         if key in ["instance", "_Table__dmldql_builder"]:
             self.__dict__[key] = value
         else:
             self.update(key, value)
 
     # select condition
     def where(self, condition, value=None):
         self.__dmldql_builder.where(condition, value)
         return self
 
-    # update
-    def update(self, key, value):
-        if self.instance.get(key) is None:
-            raise UpdateError(f"there is no field called '{key}'")
-        else:
-            self.__dmldql_builder.clear_set()
-            self.__dmldql_builder.set(**{key: value})
-            self.__dmldql_builder.clear_where()
-            for field, val in self.instance.items():
-                v = f"'{val}'" if isinstance(val, str) else val
-                self.__dmldql_builder.where(f"{field} = {v}")
-            with self.__lock:
-                try:
-                    self.__db.cursor.execute(self.__dmldql_builder.update_sql)
-                    self.__db.commit()
-                except pymysql.MySQLError as e:
-                    print(e)
-                    self.__db.rollback()
-                    return False
-                else:
-                    self.instance[key] = value
-                    return True
-
     # select
     def one(self):
         target = sorted(self.instance.keys()) if len(
             self.__dmldql_builder.select_items) == 0 else self.__dmldql_builder.select_items
         self.__dmldql_builder.select(*sorted(self.instance.keys()))
+        data = None
         with self.__lock:
             try:
                 self.__db.cursor.execute(self.__dmldql_builder.select_sql)
                 data = self.__db.cursor.fetchone()
             except pymysql.MySQLError as e:
                 print(e)
                 self.__db.rollback()
         if data is not None:
             for field, key in zip(data, target):
-                self.instance[key] = field
+                self.instance[key].value = field
             return self
         else:
             return None
 
     # select
     def all(self):
         new_instances = list()
@@ -125,42 +119,69 @@
             for field, key in zip(data, target):
                 new_instance.instance[key] = field
             new_instances.append(new_instance)
         return new_instances
 
     # insert
     def create(self):
-        self.__dmldql_builder.set(**self.instance)
+        raw_instance = dict()
+        for k, v in self.instance.items():
+            raw_instance[k] = v.value
+        self.__dmldql_builder.set(**raw_instance)
         with self.__lock:
             try:
                 self.__db.cursor.execute(self.__dmldql_builder.insert_sql)
-                self.instance["id"] = self.__db.insert_id()
+                self.instance["id"].value = self.__db.insert_id()
                 self.__db.commit()
             except pymysql.MySQLError as e:
                 print(e)
                 self.__db.rollback()
                 return False
             else:
                 return True
 
+    # update
+    def update(self, key, value):
+        if self.instance.get(key) is None:
+            raise UpdateError(f"there is no field called '{key}'")
+        else:
+            self.__dmldql_builder.clear_set()
+            self.__dmldql_builder.set(**{key: value})
+            self.__dmldql_builder.clear_where()
+            for field, val in self.instance.items():
+                v = f"'{val.value}'" if isinstance(val.value, str) else val
+                self.__dmldql_builder.where(f"{field} = {v}")
+            with self.__lock:
+                try:
+                    self.__db.cursor.execute(self.__dmldql_builder.update_sql)
+                    self.__db.commit()
+                except pymysql.MySQLError as e:
+                    print(e)
+                    self.__db.rollback()
+                    return False
+                else:
+                    self.instance[key].value = value
+                    return True
+
+    # delete
     def delete(self):
         self.__dmldql_builder.clear_where()
         for field, val in self.instance.items():
-            if isinstance(val, str):
-                self.__dmldql_builder.where(f"{field} = '{val}'")
-            elif val is None:
+            if isinstance(val.value, str):
+                self.__dmldql_builder.where(f"{field} = '{val.value}'")
+            elif val.value is None:
                 self.__dmldql_builder.where(f"{field} is null")
             else:
-                self.__dmldql_builder.where(f"{field} = {val}")
+                self.__dmldql_builder.where(f"{field} = {val.value}")
         with self.__lock:
             try:
                 self.__db.cursor.execute(self.__dmldql_builder.delete_sql)
                 self.__db.commit()
             except pymysql.MySQLError as e:
                 print(e)
                 self.__db.rollback()
                 return False
             else:
                 for key in self.instance.keys():
-                    self.instance[key] = None
+                    self.instance[key].value = None
                 return True
```

### Comparing `rain_orm-1.0.3/rain_orm.egg-info/PKG-INFO` & `rain_orm-1.0.4/rain_orm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rain-orm
-Version: 1.0.3
+Version: 1.0.4
 Summary: a tiny orm frame
 Home-page: https://github.com/cgynb/rain-orm
 Author: rain
 Author-email: 948628463@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -30,46 +30,48 @@
 
 | id  | name | password | class_id |
 |-----|------|----------|----------|
 |     |      |          |          |
 
 ```python
 import rain_orm
+from rain_orm.column import Int, VarChar
 
-rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
+rain_orm.connect(host="localhost", port=3306, user="root", password="123456", database="student_management")
 
 
 class StudentModel(rain_orm.Table):
     __table__ = "students"
     __fields__ = {
-        "id": None,
-        "name": None,
-        "password": None,
-        "class_id": None
+        "id": Int(auto_increment=True, primary_key=True),
+        "name": VarChar(30, unique=True),
+        "password": VarChar(30),
+        "class_id": Int(default=1)
     }
 
 if __name__ == "__main__":
+    rain_orm.Table.auto_migrate()
     stu = StudentModel().where("id=?", 1).one()
-    print("id: ", stu.id)
-    print("name: ", stu.name)
     print(stu)
+
 ```
 result
 
 ```cmd
 id: 1
 name: cgy
-<<StudentModel 2109293369984
-    .table = students
-    .instance = {
-        id: 1,
-        name: cgy,
-        password: None,
-        class_id: 1,
-    }
+<< StudentModel 1951412882544
+	.table = students
+	.fields = ['id', 'name', 'password', 'gender', 'origin', 'class_id']
+	.instance = {
+		id: 1,
+		name: cgy,
+		password: 123456,
+		class_id: 1,
+	}
 >>
 ```
 
 # Basic Usage
 
 it's easy to use rain-orm
 
@@ -89,24 +91,33 @@
 rain_orm.connect(host="you host", port=3306, user="root", password="your password", database="student_management")
 ```
 
 ## Define Model
 
 each data must have a unique "id"
 ```python
-class StudentModel(RainORM):
+import rain_orm
+from rain_orm.column import Int, VarChar
+
+class StudentModel(rain_orm.Table):
     __table__ = "students"
     __fields__ = {
-        "id": None,
-        "name": None,
-        "password": None,
-        "class_id": None
+        "id": Int(auto_increment=True, primary_key=True),
+        "name": VarChar(30, unique=True),
+        "password": VarChar(30),
+        "class_id": Int(default=1)
     }
+
+```
+## Auto Migrate
+```python
+rain_orm.Table.auto_migrate()
 ```
 
+
 ## CRUD Example
 
 ### Read
 
 ```python
 # student list
 stu_lst = StudentModel().all()
@@ -137,15 +148,15 @@
 		class_id: 1,
 	}
 >>
 ```
 
 ### Update
 
-there 2 ways to update data
+there are 2 ways to update data
 
 ```python
 StudentModel().where("id = ?", 22).one()  # get student instance first
 # 1. set attribute (recommend)
 stu.name = "your name"
 # 2. call update methods
 ok = stu.update("name", "your name")
@@ -154,7 +165,9 @@
 ### Delete
 
 ```python
 StudentModel().where("id = ?", 22).one()  # get student instance first
 ok = stu.delete()  # call delete method
 ```
 
+
+
```

