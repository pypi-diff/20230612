# Comparing `tmp/ardilla-0.3.4b0.tar.gz` & `tmp/ardilla-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.3.4b0.tar", last modified: Tue Jun  6 17:58:43 2023, max compression
+gzip compressed data, was "ardilla-0.4.0b0.tar", last modified: Mon Jun 12 03:09:36 2023, max compression
```

## Comparing `ardilla-0.3.4b0.tar` & `ardilla-0.4.0b0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.810375 ardilla-0.3.4b0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1078 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/LICENCE
--rw-rw-r--   0 chris     (1000) chris     (1000)     5078 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     4200 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.802375 ardilla-0.3.4b0/ardilla/
--rw-rw-r--   0 chris     (1000) chris     (1000)      142 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4968 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/abc.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/ardilla/asyncio/
--rw-rw-r--   0 chris     (1000) chris     (1000)       77 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/asyncio/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9469 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/asyncio/crud.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2540 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/asyncio/engine.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9542 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/crud.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2647 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/engine.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      476 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/errors.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2522 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/fields.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      213 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/logging.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2774 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1053 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/ordering.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7111 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/queries.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5514 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/ardilla/schemas.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/ardilla.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)     5078 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      524 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      210 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        8 2023-06-06 17:58:43.000000 ardilla-0.3.4b0/ardilla.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)     1181 2023-06-06 17:51:53.000000 ardilla-0.3.4b0/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-06-06 17:58:43.810375 ardilla-0.3.4b0/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-06 17:58:43.806375 ardilla-0.3.4b0/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     6260 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/tests/test_async.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/tests/test_models.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5626 2023-06-05 16:57:07.000000 ardilla-0.3.4b0/tests/test_sync.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-12 03:09:36.549716 ardilla-0.4.0b0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1078 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/LICENCE
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4818 2023-06-12 03:09:36.549716 ardilla-0.4.0b0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3941 2023-06-12 03:08:18.000000 ardilla-0.4.0b0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-12 03:09:36.545716 ardilla-0.4.0b0/ardilla/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      142 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4968 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/abc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-12 03:09:36.549716 ardilla-0.4.0b0/ardilla/asyncio/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       77 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/asyncio/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9469 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/asyncio/crud.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2540 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/asyncio/engine.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9542 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/crud.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2647 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/engine.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      526 2023-06-12 02:12:21.000000 ardilla-0.4.0b0/ardilla/errors.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2522 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/fields.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      213 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/logging.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3378 2023-06-12 02:53:02.000000 ardilla-0.4.0b0/ardilla/migration.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2774 2023-06-11 20:47:00.000000 ardilla-0.4.0b0/ardilla/models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1053 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/ordering.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7111 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/ardilla/queries.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4848 2023-06-11 22:01:16.000000 ardilla-0.4.0b0/ardilla/schemas.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-12 03:09:36.545716 ardilla-0.4.0b0/ardilla.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4818 2023-06-12 03:09:36.000000 ardilla-0.4.0b0/ardilla.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      545 2023-06-12 03:09:36.000000 ardilla-0.4.0b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-06-12 03:09:36.000000 ardilla-0.4.0b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      210 2023-06-12 03:09:36.000000 ardilla-0.4.0b0/ardilla.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        8 2023-06-12 03:09:36.000000 ardilla-0.4.0b0/ardilla.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1181 2023-06-11 20:48:55.000000 ardilla-0.4.0b0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-06-12 03:09:36.549716 ardilla-0.4.0b0/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-06-12 03:09:36.549716 ardilla-0.4.0b0/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6260 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/tests/test_async.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2080 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/tests/test_models.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5626 2023-06-05 16:57:07.000000 ardilla-0.4.0b0/tests/test_sync.py
```

### Comparing `ardilla-0.3.4b0/LICENCE` & `ardilla-0.4.0b0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/PKG-INFO` & `ardilla-0.4.0b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.3.4b0
+Version: 0.4.0b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -108,18 +108,7 @@
 
 ## Examples:
 
 - A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
 - A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
 - [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
 - [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
-
-## To-dos
-
-- [x] Add testing
-- [x] Add a schema generator 
-- [X] Add filtering
-- [X] Add limiting
-- [X] Docstring everything using Google format
-- [ ] Start a changelog when out of alpha
-- [X] Add proper documentation
-  - propper as in a site with how to use
```

### Comparing `ardilla-0.3.4b0/README.md` & `ardilla-0.4.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,18 +85,7 @@
 
 ## Examples:
 
 - A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
 - A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
 - [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
 - [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
-
-## To-dos
-
-- [x] Add testing
-- [x] Add a schema generator 
-- [X] Add filtering
-- [X] Add limiting
-- [X] Docstring everything using Google format
-- [ ] Start a changelog when out of alpha
-- [X] Add proper documentation
-  - propper as in a site with how to use
```

### Comparing `ardilla-0.3.4b0/ardilla/abc.py` & `ardilla-0.4.0b0/ardilla/abc.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/asyncio/crud.py` & `ardilla-0.4.0b0/ardilla/asyncio/crud.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/asyncio/engine.py` & `ardilla-0.4.0b0/ardilla/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/crud.py` & `ardilla-0.4.0b0/ardilla/crud.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/engine.py` & `ardilla-0.4.0b0/ardilla/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/fields.py` & `ardilla-0.4.0b0/ardilla/fields.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/models.py` & `ardilla-0.4.0b0/ardilla/models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/ordering.py` & `ardilla-0.4.0b0/ardilla/ordering.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/queries.py` & `ardilla-0.4.0b0/ardilla/queries.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/ardilla/schemas.py` & `ardilla-0.4.0b0/ardilla/schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 variables and functions here are used to generate and work with the Model's schemas
 """
 import re
 from typing import Optional, Union
 from datetime import datetime, date, time
 from pydantic import BaseModel, Json
+from pydantic.fields import ModelField
+
 from .errors import ModelIntegrityError
 
 
 SCHEMA_TEMPLATE: str = "CREATE TABLE IF NOT EXISTS {tablename} (\n{fields}\n);"
 
-SQLFieldType = Union[int,float,str,bool,datetime,bytes,date,time]
+SQLFieldType = Union[int, float, str, bool, datetime, bytes, date, time]
 
 FIELD_MAPPING: dict[type, str] = {
     int: "INTEGER",
     float: "REAL",
     str: "TEXT",
     bool: "INTEGER",
     datetime: "DATETIME",
@@ -23,131 +25,129 @@
     time: "TIME",
 }
 
 AUTOFIELDS = {
     int: " AUTOINCREMENT",
     datetime: " DEFAULT CURRENT_TIMESTAMP",
     date: " DEFAULT CURRENT_DATE",
-    time: " DEFAULT CURRENT_TIME"
+    time: " DEFAULT CURRENT_TIME",
 }
 
+
 def get_tablename(model: type[BaseModel]) -> str:
     """returns the tablename of a model either from the attribute __tablenam__
     or from the lowercase model's name
 
     Args:
         model (type[BaseModel]): the model
 
     Returns:
         str: the name of the table
     """
     return getattr(model, "__tablename__", model.__name__.lower())
 
 
-def get_fields_schemas(Model: type[BaseModel]) -> list[str]:
-    """Generates the fields for the table schema of the passed model
+def make_field_schema(field: ModelField) -> dict:
+    output = {}
+    name = field.name
+    T = field.type_
+    default = field.default
+    extra = field.field_info.extra
+    auto = output["auto"] = extra.get("auto")
+    unique = output["unique"] = extra.get("unique")
+    is_pk = False
+    constraint = None
+
+    if default and unique:
+        raise ModelIntegrityError(
+            "field {name} has both unique and default constrains which are incompatible"
+        )
 
-    Args:
-        model (type[BaseModel]): the model
+    autoerror = ModelIntegrityError(
+        f'field {name} has a type of "{T}" which does not support "auto"'
+    )
+    schema = f"{name} {FIELD_MAPPING[T]}"
 
-    Raises:
-        TypeError: if the field is not listed in ardilla.schemas.FIELD_MAPPING
-        ModelIntegrityError: if there's a Model field that is marked as pk but
-            the model's __pk__ attr points to a different field
+    primary_field_keys = {"pk", "primary", "primary_key"}
+    if len(extra.keys() & primary_field_keys) > 1:
+        raise ModelIntegrityError(f'Multiple keywords for a primary field in "{name}"')
 
-    Returns:
-        str: a string containing the formatted fields to be added to a table schema
-    """
-    schemas = []
-    constrains = []
-    pk = None
-    for field in Model.__fields__.values():
-        name = field.name
-        T = field.type_
-        default = field.default
-        extra = field.field_info.extra
-        auto = extra.get('auto')
-        unique = extra.get('unique')
-        if default and unique:
-            raise ModelIntegrityError("field {name} has both unique and default constrains which are incompatible")
-        
-        autoerror = ModelIntegrityError(f'field {name} has a type of "{T}" which does not support "auto"')
-        schema = f'{name} {FIELD_MAPPING[T]}'
-        
-        primary_field_keys = {'pk', 'primary', 'primary_key'}
-        if len(extra.keys() & primary_field_keys) >1:
-            raise ModelIntegrityError(f'Multiple keywords for a primary field in "{name}"')
-        
-        for k in primary_field_keys:
-            if k in extra and extra[k]:
-                if pk is not None:
-                    raise ModelIntegrityError('Only one primary key per model is allowed')
-                elif hasattr(Model, '__pk__') and Model.__pk__ != name:
-                    raise ModelIntegrityError(f"field {name} is marked as pk, but __pk__ points to another field.")
-                
-                pk = name
-                
-                schema += ' PRIMARY KEY'
-
-                if auto and T in AUTOFIELDS:
-                    schema += AUTOFIELDS[T]
-                    # make the field not required
-                    # this allows users to create
-                    # objects from the model without knowing the final 
-                    # value in the database
-                    field.required = False
-                elif auto:
-                    raise autoerror
-                break
-        else:
-            if auto and T in AUTOFIELDS.keys() - {int}:
+    for k in primary_field_keys:
+        if k in extra and extra[k]:
+            is_pk = True
+
+            schema += " PRIMARY KEY"
+
+            if auto and T in AUTOFIELDS:
                 schema += AUTOFIELDS[T]
+                field.required = (
+                    False  # to allow users to create the objs without this field
+                )
+
             elif auto:
                 raise autoerror
-            elif default is not None:
-                if T in {int, str, float, bool}:
-                    schema += f' DEFAULT {default!r}'
-                elif T in {datetime, date, time}:
-                    schema += f' DEFAULT {default}'
-                elif T is bytes:
-                    schema += f" DEFAULT (X'{default.hex()}')"
-            elif field.required:
-                    schema += ' NOT NULL'
-            if unique:
-                schema += ' UNIQUE'
-                    
-        schemas.append(schema)
-
-        if extra.get('references'):
-            references, fk, on_delete, on_update = (extra.get(f) for f in ['references', 'fk', 'on_delete', 'on_update'])
-            constrains.append(
-                f'FOREIGN KEY ({name}) '
-                f'REFERENCES {references}({fk}) '
-                f'ON UPDATE {on_update} '
-                f'ON DELETE {on_delete}'
-            )
-            
-    return schemas + constrains
 
+            break
+    else:
+        if auto and T in AUTOFIELDS.keys() - {int}:
+            schema += AUTOFIELDS[T]
+        elif auto:
+            raise autoerror
+        elif default is not None:
+            if T in {int, str, float, bool}:
+                schema += f" DEFAULT {default!r}"
+            elif T in {datetime, date, time}:
+                schema += f" DEFAULT {default}"
+            elif T is bytes:
+                schema += f" DEFAULT (X'{default.hex()}')"
+        elif field.required:
+            schema += " NOT NULL"
+        if unique:
+            schema += " UNIQUE"
+
+    if extra.get("references"):
+        references, fk, on_delete, on_update = (
+            extra.get(f) for f in ["references", "fk", "on_delete", "on_update"]
+        )
+        constraint = (
+            f"FOREIGN KEY ({name}) "
+            f"REFERENCES {references}({fk}) "
+            f"ON UPDATE {on_update} "
+            f"ON DELETE {on_delete}"
+        )
 
-def make_table_schema(Model: type[BaseModel]) -> str:
-    """Generates the schema from a model based on its field configuration
+    output.update({"pk": is_pk, "schema": schema, "constraint": constraint})
 
-    Args:
-        Model (type[BaseModel]): the model
+    return output
 
-    Returns:
-        str: the generated schema
-    """
+
+def make_table_schema(Model: type[BaseModel]) -> str:
     tablename = get_tablename(Model)
-    fields = get_fields_schemas(Model)
+    fields = []
+    constrains = []
+    pk = None
+    for field in Model.__fields__.values():
+        name = field
+        field_schema = make_field_schema(field)
+        if field_schema["pk"] is True:
+            if pk is not None:
+                raise ModelIntegrityError(
+                    f'field "{name}" is marked as primary but there is already a primary key field "{pk}"'
+                )
+            pk = field.name
+        fields.append(field_schema["schema"])
+
+        constrains.append(field_schema["constraint"]) if field_schema[
+            "constraint"
+        ] else None
+
     schema = (
-        f'CREATE TABLE IF NOT EXISTS {tablename}(\n' +
-        ',\n'.join(f'\r    {f}' for f in fields) +
-        '\n);'
+        f"CREATE TABLE IF NOT EXISTS {tablename}(\n"
+        + ",\n".join(f"\r    {f}" for f in (fields + constrains))
+        + "\n);"
     )
     return schema
 
 
 def get_pk(schema: str) -> Optional[str]:
     """Gets the primary key field name from the passed schema
```

### Comparing `ardilla-0.3.4b0/ardilla.egg-info/PKG-INFO` & `ardilla-0.4.0b0/ardilla.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.3.4b0
+Version: 0.4.0b0
 Summary: Ardilla ORM. Easy to use, fast to implement, with sync and async flavors
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
@@ -108,18 +108,7 @@
 
 ## Examples:
 
 - A simple [FastAPI](https://github.com/chrisdewa/ardilla/blob/master/examples/fastapi_app.py) application
 - A reputation based discord [bot](https://github.com/chrisdewa/ardilla/blob/master/examples/rep_discord_bot.py)
 - [basic usage](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage.py)
 - [basic usage with foreign keys](https://github.com/chrisdewa/ardilla/blob/master/examples/basic_usage_fk.py)
-
-## To-dos
-
-- [x] Add testing
-- [x] Add a schema generator 
-- [X] Add filtering
-- [X] Add limiting
-- [X] Docstring everything using Google format
-- [ ] Start a changelog when out of alpha
-- [X] Add proper documentation
-  - propper as in a site with how to use
```

### Comparing `ardilla-0.3.4b0/ardilla.egg-info/SOURCES.txt` & `ardilla-0.4.0b0/ardilla.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ardilla/__init__.py
 ardilla/abc.py
 ardilla/crud.py
 ardilla/engine.py
 ardilla/errors.py
 ardilla/fields.py
 ardilla/logging.py
+ardilla/migration.py
 ardilla/models.py
 ardilla/ordering.py
 ardilla/queries.py
 ardilla/schemas.py
 ardilla.egg-info/PKG-INFO
 ardilla.egg-info/SOURCES.txt
 ardilla.egg-info/dependency_links.txt
```

### Comparing `ardilla-0.3.4b0/pyproject.toml` & `ardilla-0.4.0b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.3.4-beta"
+version = "0.4.0-beta"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ardilla-0.3.4b0/tests/test_async.py` & `ardilla-0.4.0b0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/tests/test_models.py` & `ardilla-0.4.0b0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.4b0/tests/test_sync.py` & `ardilla-0.4.0b0/tests/test_sync.py`

 * *Files identical despite different names*

