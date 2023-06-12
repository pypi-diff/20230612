# Comparing `tmp/cd2t-2.0.1.tar.gz` & `tmp/cd2t-2.0.2.tar.gz`

## Comparing `cd2t-2.0.1.tar` & `cd2t-2.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/DataParser.py
--rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/References.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/RunTimeEnv.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/results.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/schema.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/utils.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/List.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/NoneDataType.py
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/ParserDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/__init__.py
--rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/base.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/bool.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/datatype.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/enum.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/float.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/fqdn.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/hostname.py
--rw-r--r--   0        0        0     8465 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/idlist.py
--rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/integer.py
--rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/ip.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/multitype.py
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/object.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/schema.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 cd2t-2.0.1/cd2t/types/string.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-2.0.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-2.0.1/LICENSE
--rw-r--r--   0        0        0    31959 2020-02-02 00:00:00.000000 cd2t-2.0.1/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    32606 2020-02-02 00:00:00.000000 cd2t-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/DataParser.py
+-rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/References.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/RunTimeEnv.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/results.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/schema.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/utils.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/List.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/NoneDataType.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/ParserDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/__init__.py
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/base.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/bool.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/datatype.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/enum.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/float.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/fqdn.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/hostname.py
+-rw-r--r--   0        0        0     8500 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/idlist.py
+-rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/integer.py
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/ip.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/multitype.py
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/object.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/schema.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 cd2t-2.0.2/cd2t/types/string.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-2.0.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-2.0.2/LICENSE
+-rw-r--r--   0        0        0    31954 2020-02-02 00:00:00.000000 cd2t-2.0.2/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    32601 2020-02-02 00:00:00.000000 cd2t-2.0.2/PKG-INFO
```

### Comparing `cd2t-2.0.1/cd2t/DataParser.py` & `cd2t-2.0.2/cd2t/DataParser.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/References.py` & `cd2t-2.0.2/cd2t/References.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/RunTimeEnv.py` & `cd2t-2.0.2/cd2t/RunTimeEnv.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/results.py` & `cd2t-2.0.2/cd2t/results.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/schema.py` & `cd2t-2.0.2/cd2t/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/utils.py` & `cd2t-2.0.2/cd2t/utils.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/List.py` & `cd2t-2.0.2/cd2t/types/List.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             schema_obj=schema_obj,
         )
         self.element_data_type = (
             cd2t.types.ParserDataType.ParserDataType().build_schema(
                 schema=self.elements,
                 path=path + ".elements",
                 RTE=RTE,
+                schema_obj=schema_obj,
             )
         )
         return self
 
     def build_sub_references(self, data: any, path: str, RTE: RunTimeEnv):
         i = 0
         for element in data:
```

### Comparing `cd2t-2.0.1/cd2t/types/ParserDataType.py` & `cd2t-2.0.2/cd2t/types/ParserDataType.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         float=cd2t.types.float.Float,
         idlist=cd2t.types.idlist.IDList_V2,
         integer=cd2t.types.integer.Integer,
         list=cd2t.types.List.List,
         multitype=cd2t.types.multitype.Multitype,
         none=cd2t.types.NoneDataType.NoneDataType,
         object=cd2t.types.object.Object_V2,
-        schema=cd2t.types.schema.SchemaDataType,
         string=cd2t.types.string.String,
     ),
 }
 
 
 class ParserDataType:
     def __init__(self) -> None:
```

### Comparing `cd2t-2.0.1/cd2t/types/base.py` & `cd2t-2.0.2/cd2t/types/base.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/bool.py` & `cd2t-2.0.2/cd2t/types/bool.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/enum.py` & `cd2t-2.0.2/cd2t/types/enum.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/float.py` & `cd2t-2.0.2/cd2t/types/float.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/fqdn.py` & `cd2t-2.0.2/cd2t/types/fqdn.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/hostname.py` & `cd2t-2.0.2/cd2t/types/hostname.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/idlist.py` & `cd2t-2.0.2/cd2t/types/idlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             schema_obj=schema_obj,
         )
 
         self.element_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
             schema=self.elements,
             path=path + ".elements",
             RTE=RTE,
+            schema_obj=schema_obj,
         )
         return self
 
     def build_sub_references(self, data: any, path: str, RTE: RunTimeEnv):
         i = 0
         for id, element in data.items():
             self.element_type.build_references(
```

### Comparing `cd2t-2.0.1/cd2t/types/integer.py` & `cd2t-2.0.2/cd2t/types/integer.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/ip.py` & `cd2t-2.0.2/cd2t/types/ip.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/multitype.py` & `cd2t-2.0.2/cd2t/types/multitype.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,15 @@
             RTE=RTE,
             schema_obj=schema_obj,
         )
         i = 0
         for _type in self.types:
             _path = "%s.types[%d]" % (path, i)
             data_type = cd2t.types.ParserDataType.ParserDataType().build_schema(
-                schema=_type,
-                path=_path,
-                RTE=RTE,
+                schema=_type, path=_path, RTE=RTE, schema_obj=schema_obj
             )
             if data_type.data_type_name == self.data_type_name:
                 raise SchemaError("Multitype in Multitype not supported", _path)
             self.type_objects.append(data_type)
             self.matching_classes.extend(data_type.matching_classes)
             i += 1
         return self
```

### Comparing `cd2t-2.0.1/cd2t/types/object.py` & `cd2t-2.0.2/cd2t/types/object.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/schema.py` & `cd2t-2.0.2/cd2t/types/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/cd2t/types/string.py` & `cd2t-2.0.2/cd2t/types/string.py`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/LICENSE` & `cd2t-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cd2t-2.0.1/README.md` & `cd2t-2.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
   reason.
 
 ## Change Log
 
 **Version 2.0.0**:
 - *Changed*: Templates replaces subschemas.
 - *New*: Schema version 2 introduced
-- *New*: IDs in 'id_list' are defined by any other data type
+- *New*: IDs in 'idlist' are defined by any other data type
   in schema version 2.
 - *New*: Reference attributes definition changed in 'object'
   in schema version 2.
 - *New*: Custom pre-defined data types can be defined in schema.
 - *New*: Reference credit support - Producer values and consumer values can
   be assignet with credits to detect 'overloaded' producers.
 - *New*: ruamel.yaml support - If data is loaded with ruamel.yaml module,
@@ -334,48 +334,48 @@
 ##### 'idlist' Limitations
 
 - *autogeneration* is not supported
 
 ##### 'idlist' Schema (in Version 2)
 
 ```yaml
-type: 'id_list'
+type: 'idlist'
 description: < str > # Information about data type and value
 reference: { unique options }
 # Note: Every ID is referenced as a value with the 'reference.key'.
 
 minimum: <int | default -> 0 > # >= 0
 # Minimum required amount of IDs
 
 maximum: < int > # >= 0
 # Maximum allowed amount of IDs
-# If omitted, even an empty id_list is allowed.
+# If omitted, even an empty idlist is allowed.
 
 elements: { data type schema } # required
 # Data schema defining element data type
 
 id: { data type schema }
 # Data schema defining IDs
 # If omitted, ID type defaults to 'string'.
 ```
 
 ##### 'idlist' Schema (in Version 1)
 
 ```yaml
-type: 'id_list'
+type: 'idlist'
 description: < str > # Information about data type and value
 reference: { unique options }
 # Note: Every ID is referenced as a value with the 'reference.key'.
 
 minimum: <int | default -> 0 > # >= 0
 # Minimum required amount of IDs
 
 maximum: < int > # >= 0
 # Maximum allowed amount of IDs
-# If omitted, even an empty id_list is allowed.
+# If omitted, even an empty idlist is allowed.
 
 elements: { data type schema } # required
 # Data schema defining element data type
 
 id_type: < 'integer' | 'string' | default -> 'string' >
 # Indicates if IDs are integer or string
```

### Comparing `cd2t-2.0.1/pyproject.toml` & `cd2t-2.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/cd2t",
 ]
 
 [project]
 name = "cd2t"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "cd2t validates data structure, data types and values with templates"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cd2t-2.0.1/PKG-INFO` & `cd2t-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cd2t
-Version: 2.0.1
+Version: 2.0.2
 Summary: cd2t validates data structure, data types and values with templates
 Project-URL: Homepage, https://gitlab.com/ko.no/cd2t
 Project-URL: Bug Tracker, https://gitlab.com/ko.no/cd2t/-/issues
 Author-email: Korte Noack <korte@8lacht.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -78,15 +78,15 @@
   reason.
 
 ## Change Log
 
 **Version 2.0.0**:
 - *Changed*: Templates replaces subschemas.
 - *New*: Schema version 2 introduced
-- *New*: IDs in 'id_list' are defined by any other data type
+- *New*: IDs in 'idlist' are defined by any other data type
   in schema version 2.
 - *New*: Reference attributes definition changed in 'object'
   in schema version 2.
 - *New*: Custom pre-defined data types can be defined in schema.
 - *New*: Reference credit support - Producer values and consumer values can
   be assignet with credits to detect 'overloaded' producers.
 - *New*: ruamel.yaml support - If data is loaded with ruamel.yaml module,
@@ -350,48 +350,48 @@
 ##### 'idlist' Limitations
 
 - *autogeneration* is not supported
 
 ##### 'idlist' Schema (in Version 2)
 
 ```yaml
-type: 'id_list'
+type: 'idlist'
 description: < str > # Information about data type and value
 reference: { unique options }
 # Note: Every ID is referenced as a value with the 'reference.key'.
 
 minimum: <int | default -> 0 > # >= 0
 # Minimum required amount of IDs
 
 maximum: < int > # >= 0
 # Maximum allowed amount of IDs
-# If omitted, even an empty id_list is allowed.
+# If omitted, even an empty idlist is allowed.
 
 elements: { data type schema } # required
 # Data schema defining element data type
 
 id: { data type schema }
 # Data schema defining IDs
 # If omitted, ID type defaults to 'string'.
 ```
 
 ##### 'idlist' Schema (in Version 1)
 
 ```yaml
-type: 'id_list'
+type: 'idlist'
 description: < str > # Information about data type and value
 reference: { unique options }
 # Note: Every ID is referenced as a value with the 'reference.key'.
 
 minimum: <int | default -> 0 > # >= 0
 # Minimum required amount of IDs
 
 maximum: < int > # >= 0
 # Maximum allowed amount of IDs
-# If omitted, even an empty id_list is allowed.
+# If omitted, even an empty idlist is allowed.
 
 elements: { data type schema } # required
 # Data schema defining element data type
 
 id_type: < 'integer' | 'string' | default -> 'string' >
 # Indicates if IDs are integer or string
```

