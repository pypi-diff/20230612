# Comparing `tmp/junkpy-0.0.3.tar.gz` & `tmp/junkpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/junkpy-0.0.3.tar", last modified: Wed May 31 11:02:16 2023, max compression
+gzip compressed data, was "dist/junkpy-0.1.0.tar", last modified: Mon Jun 12 13:23:27 2023, max compression
```

## Comparing `junkpy-0.0.3.tar` & `junkpy-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-05-31 11:02:16.000000 junkpy-0.0.3/
--rw-rw-r--   0 jose      (1000) jose      (1000)    19100 2023-05-31 11:02:16.000000 junkpy-0.0.3/PKG-INFO
--rw-r--r--   0 jose      (1000) jose      (1000)    16595 2023-05-31 10:34:26.000000 junkpy-0.0.3/README.md
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-05-31 11:02:16.000000 junkpy-0.0.3/junkpy/
--rw-r--r--   0 jose      (1000) jose      (1000)       91 2023-05-30 14:13:49.000000 junkpy-0.0.3/junkpy/__init__.py
--rw-r--r--   0 jose      (1000) jose      (1000)     3232 2023-05-30 14:12:45.000000 junkpy-0.0.3/junkpy/base.py
--rw-r--r--   0 jose      (1000) jose      (1000)     3552 2023-05-30 14:13:12.000000 junkpy-0.0.3/junkpy/dataclasses.py
--rw-r--r--   0 jose      (1000) jose      (1000)     2641 2023-05-30 14:13:39.000000 junkpy-0.0.3/junkpy/extensions.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-05-31 11:02:16.000000 junkpy-0.0.3/junkpy.egg-info/
--rw-rw-r--   0 jose      (1000) jose      (1000)    19100 2023-05-31 11:02:16.000000 junkpy-0.0.3/junkpy.egg-info/PKG-INFO
--rw-rw-r--   0 jose      (1000) jose      (1000)      257 2023-05-31 11:02:16.000000 junkpy-0.0.3/junkpy.egg-info/SOURCES.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        1 2023-05-31 11:02:16.000000 junkpy-0.0.3/junkpy.egg-info/dependency_links.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        5 2023-05-31 11:02:16.000000 junkpy-0.0.3/junkpy.egg-info/requires.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)        7 2023-05-31 11:02:16.000000 junkpy-0.0.3/junkpy.egg-info/top_level.txt
--rw-rw-r--   0 jose      (1000) jose      (1000)       38 2023-05-31 11:02:16.000000 junkpy-0.0.3/setup.cfg
--rw-r--r--   0 jose      (1000) jose      (1000)      401 2023-05-31 10:59:10.000000 junkpy-0.0.3/setup.py
-drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-05-31 11:02:16.000000 junkpy-0.0.3/test/
--rwxrwxr-x   0 jose      (1000) jose      (1000)      767 2023-05-31 08:09:23.000000 junkpy-0.0.3/test/test.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-06-12 13:23:27.000000 junkpy-0.1.0/
+-rw-rw-r--   0 jose      (1000) jose      (1000)    19128 2023-06-12 13:23:27.000000 junkpy-0.1.0/PKG-INFO
+-rw-r--r--   0 jose      (1000) jose      (1000)    16595 2023-06-12 13:18:13.000000 junkpy-0.1.0/README.md
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-06-12 13:23:27.000000 junkpy-0.1.0/junkpy/
+-rw-r--r--   0 jose      (1000) jose      (1000)       91 2023-06-12 13:18:13.000000 junkpy-0.1.0/junkpy/__init__.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     4488 2023-06-12 13:18:13.000000 junkpy-0.1.0/junkpy/base.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     4255 2023-06-12 13:18:13.000000 junkpy-0.1.0/junkpy/dataclasses.py
+-rw-r--r--   0 jose      (1000) jose      (1000)     2641 2023-06-12 13:18:13.000000 junkpy-0.1.0/junkpy/extensions.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-06-12 13:23:27.000000 junkpy-0.1.0/junkpy.egg-info/
+-rw-rw-r--   0 jose      (1000) jose      (1000)    19128 2023-06-12 13:23:27.000000 junkpy-0.1.0/junkpy.egg-info/PKG-INFO
+-rw-rw-r--   0 jose      (1000) jose      (1000)      388 2023-06-12 13:23:27.000000 junkpy-0.1.0/junkpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        1 2023-06-12 13:23:27.000000 junkpy-0.1.0/junkpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        5 2023-06-12 13:23:27.000000 junkpy-0.1.0/junkpy.egg-info/requires.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)        7 2023-06-12 13:23:27.000000 junkpy-0.1.0/junkpy.egg-info/top_level.txt
+-rw-rw-r--   0 jose      (1000) jose      (1000)       38 2023-06-12 13:23:27.000000 junkpy-0.1.0/setup.cfg
+-rw-r--r--   0 jose      (1000) jose      (1000)      447 2023-06-12 13:18:13.000000 junkpy-0.1.0/setup.py
+drwxrwxr-x   0 jose      (1000) jose      (1000)        0 2023-06-12 13:23:27.000000 junkpy-0.1.0/test/
+-rwxr-xr-x   0 jose      (1000) jose      (1000)     1119 2023-06-12 13:18:13.000000 junkpy-0.1.0/test/test_autodetect_types.py
+-rwxr-xr-x   0 jose      (1000) jose      (1000)     1094 2023-06-12 13:18:13.000000 junkpy-0.1.0/test/test_builtin_forced_types.py
+-rwxr-xr-x   0 jose      (1000) jose      (1000)     2138 2023-06-12 13:18:13.000000 junkpy-0.1.0/test/test_custom_classes.py
+-rwxr-xr-x   0 jose      (1000) jose      (1000)      763 2023-06-12 13:18:13.000000 junkpy-0.1.0/test/test_data_load.py
+-rwxr-xr-x   0 jose      (1000) jose      (1000)     2718 2023-06-12 13:18:13.000000 junkpy-0.1.0/test/test_non_JSON_syntax.py
```

### Comparing `junkpy-0.0.3/PKG-INFO` & `junkpy-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: junkpy
-Version: 0.0.3
+Version: 0.1.0
 Summary: Extended JSON Library for Configuration Files
-Home-page: UNKNOWN
+Home-page: https://github.com/Samoxiaki/Junkpy
 Author: Samoxiaki
 Author-email: samoxiaki@yahoo.com
 License: UNKNOWN
 Description: # Junkpy: Extended JSON Library for Configuration Files.
         
         Junkpy is a Python library specifically designed for working with configuration files in JSON format. It offers a flexible approach to handling JSON objects, allowing for easier modification and manipulation of configuration data. With Junkpy, you can work with a more lenient syntax, accommodating variations in JSON structure commonly found in configuration files.
         
@@ -250,22 +250,22 @@
         | decimal    | decimal.Decimal     | Decimal values                                                                                | (decimal) "3.14"                                                                                               |
         | bool       | bool                | Boolean values                                                                                | (bool) true                                                                                                    |
         | set        | set                 | Sets of values                                                                                | (set) [1, 2, 3]                                                                                                |
         | timestamp  | datetime.datetime   | Unix timestamp values                                                                         | (timestamp) 1623345600                                                                                         |
         | timedelta  | datetime.timedelta  | Time differences in seconds                                                                   | (timedelta) 60                                                                                                 |
         |            |                     | Time differences in a list [DAYS, SECONDS, MICROSECONDS, MILLISECONDS, MINUTES, HOURS, WEEKS] | (timedelta) [5, 10, 200, 150, 3, 4, 8]                                                                         |
         |            |                     | Time differences in a dict with keyword arguments as keys                                     | (timedelta) {"days": 1, "seconds": 3600}                                                                       |
-        | time       | datetime.time       | Time values in HH:MM:SS format                                                                | (time) "12:30:45"                                                                                              |
-        |            |                     | Time values in a list [HOUR, MINUTE, SECOND]                                                  | (time) [12, 30, 45]                                                                                            |
+        | time       | datetime.time       | Time values in ISO 8601 format, [HH[:MM[:SS[.mmm[uuu]]]]][+HH:MM]                             | (time) "12:30:45"                                                                                              |
+        |            |                     | Time values in a list [HOUR, MINUTE, SECOND, MICROSECOND]                                     | (time) [12, 30, 45, 152]                                                                                       |
         |            |                     | Time values in a dict with keyword arguments as keys                                          | (time) {"hour": 12, "minute": 30, "second": 45}                                                                |
-        | date       | datetime.date       | Date values in YYYY-MM-DD format                                                              | (date) "2021-07-10"                                                                                            |
+        | date       | datetime.date       | Date values in ISO 8601 format, YYYY-MM-DD                                                    | (date) "2021-07-10"                                                                                            |
         |            |                     | Date values in a list [YEAR, MONTH, DAY]                                                      | (date) [2021, 7, 10]                                                                                           |
         |            |                     | Date values in a dict with keyword arguments as keys                                          | (date) {"year": 2021, "month": 7, "day": 10}                                                                   |
-        | datetime   | datetime.datetime   | Date and time values in YYYY-MM-DD HH:MM:SS format                                            | (datetime) "2021-07-10 12:30:45"                                                                               |
-        |            |                     | Date and time values in a list [YEAR, MONTH, DAY, HOUR, MINUTE, SECOND]                       | (datetime) [2021, 7, 10, 12, 30, 45]                                                                           |
+        | datetime   | datetime.datetime   | Date and time values in ISO 8601 format, YYYY-MM-DD [HH[:MM[:SS[.mmm[uuu]]]]][+HH:MM]         | (datetime) "2021-07-10 12:30:45"                                                                               |
+        |            |                     | Date and time values in a list [YEAR, MONTH, DAY, HOUR, MINUTE, SECOND, MICROSECOND]          | (datetime) [2021, 7, 10, 12, 30, 45, 580]                                                                      |
         |            |                     | Date and time values in a dict with keyword arguments as keys                                 | (datetime) {"year": 2021, "month": 7, "day": 10, "hour": 12, "minute": 30, "second": 45}                       |
         
         
         ## Contributing
         
         Contributions to Junkpy are welcome! If you encounter any issues, have suggestions for improvements, or would like to add new features, please feel free to submit a pull request.
```

### Comparing `junkpy-0.0.3/README.md` & `junkpy-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -242,22 +242,22 @@
 | decimal    | decimal.Decimal     | Decimal values                                                                                | (decimal) "3.14"                                                                                               |
 | bool       | bool                | Boolean values                                                                                | (bool) true                                                                                                    |
 | set        | set                 | Sets of values                                                                                | (set) [1, 2, 3]                                                                                                |
 | timestamp  | datetime.datetime   | Unix timestamp values                                                                         | (timestamp) 1623345600                                                                                         |
 | timedelta  | datetime.timedelta  | Time differences in seconds                                                                   | (timedelta) 60                                                                                                 |
 |            |                     | Time differences in a list [DAYS, SECONDS, MICROSECONDS, MILLISECONDS, MINUTES, HOURS, WEEKS] | (timedelta) [5, 10, 200, 150, 3, 4, 8]                                                                         |
 |            |                     | Time differences in a dict with keyword arguments as keys                                     | (timedelta) {"days": 1, "seconds": 3600}                                                                       |
-| time       | datetime.time       | Time values in HH:MM:SS format                                                                | (time) "12:30:45"                                                                                              |
-|            |                     | Time values in a list [HOUR, MINUTE, SECOND]                                                  | (time) [12, 30, 45]                                                                                            |
+| time       | datetime.time       | Time values in ISO 8601 format, [HH[:MM[:SS[.mmm[uuu]]]]][+HH:MM]                             | (time) "12:30:45"                                                                                              |
+|            |                     | Time values in a list [HOUR, MINUTE, SECOND, MICROSECOND]                                     | (time) [12, 30, 45, 152]                                                                                       |
 |            |                     | Time values in a dict with keyword arguments as keys                                          | (time) {"hour": 12, "minute": 30, "second": 45}                                                                |
-| date       | datetime.date       | Date values in YYYY-MM-DD format                                                              | (date) "2021-07-10"                                                                                            |
+| date       | datetime.date       | Date values in ISO 8601 format, YYYY-MM-DD                                                    | (date) "2021-07-10"                                                                                            |
 |            |                     | Date values in a list [YEAR, MONTH, DAY]                                                      | (date) [2021, 7, 10]                                                                                           |
 |            |                     | Date values in a dict with keyword arguments as keys                                          | (date) {"year": 2021, "month": 7, "day": 10}                                                                   |
-| datetime   | datetime.datetime   | Date and time values in YYYY-MM-DD HH:MM:SS format                                            | (datetime) "2021-07-10 12:30:45"                                                                               |
-|            |                     | Date and time values in a list [YEAR, MONTH, DAY, HOUR, MINUTE, SECOND]                       | (datetime) [2021, 7, 10, 12, 30, 45]                                                                           |
+| datetime   | datetime.datetime   | Date and time values in ISO 8601 format, YYYY-MM-DD [HH[:MM[:SS[.mmm[uuu]]]]][+HH:MM]         | (datetime) "2021-07-10 12:30:45"                                                                               |
+|            |                     | Date and time values in a list [YEAR, MONTH, DAY, HOUR, MINUTE, SECOND, MICROSECOND]          | (datetime) [2021, 7, 10, 12, 30, 45, 580]                                                                      |
 |            |                     | Date and time values in a dict with keyword arguments as keys                                 | (datetime) {"year": 2021, "month": 7, "day": 10, "hour": 12, "minute": 30, "second": 45}                       |
 
 
 ## Contributing
 
 Contributions to Junkpy are welcome! If you encounter any issues, have suggestions for improvements, or would like to add new features, please feel free to submit a pull request.
```

### Comparing `junkpy-0.0.3/junkpy/base.py` & `junkpy-0.1.0/junkpy/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List, Optional, Type, IO
 from lark import Lark, Transformer
 from .dataclasses import JunkpyDataClass, JunkpyBaseDataClassMeta
 
 
 
 class JunkpyTransformer(Transformer):
 	def __init__(self, data_classes:list=None):
@@ -29,51 +30,62 @@
 		
 		
 	def typed_value_parser(self, type_cls, type_kwargs, value):
 		data_class = self._data_class_keyword_dict.get(type_cls, None)
 		if(data_class is None):
 			raise ValueError(f"Unsupported type <{type_cls}>")
 		
-		return data_class.load(value, **type_kwargs)
+		loaded_value = data_class.load(value, **type_kwargs)
+		if(not isinstance(loaded_value, data_class.CLASS)):
+			raise TypeError(f"Unexpected output type for data class ({type_cls}). Expected {data_class.CLASS}, got {type(loaded_value)}")
+			
+		return loaded_value
+	
 	
-
 	list = list
+	empty_list = lambda self, value: list()
 	dict = dict
+	empty_dict = lambda self, value: dict()
 	pair = tuple
 	type_option = tuple
 	type_kwargs = dict
-	null_pair = lambda self, value: (value[0], None)
+	null_pair = lambda self, value: (value[0], None)		
 	var_name = lambda self, value: str(value[0])
 	string = lambda self, value: value[0][1:-1]
 	float_n = lambda self, value: float(value[0])
 	integer_n = lambda self, value: int(value[0])
 	null = lambda self, _: None
 	true = lambda self, _: True
 	false = lambda self, _: False
 
 
 
 class Junkpy:
 	__JUNKPY_GRAMMAR = r"""
 		?value: dict
-			  | list
-			  | string
-			  | integer_n
-			  | float_n
-			  | true
-			  | false
-			  | null
+			| empty_dict
+			| list
+			| empty_list
+			| string
+			| integer_n
+			| float_n
+			| true
+			| false
+			| null
 		
 		typed_value: "(" ((string | var_name) | (string | var_name) type_kwargs) ")" (value | typed_value | typed_null_value)
 		typed_null_value: "(" ((string | var_name) | (string | var_name) type_kwargs) ")" 
 		pair : (string | var_name) ":" (value | typed_value | typed_null_value)
 		null_pair : (string | var_name) ":" 
 		
-		dict : "{" [(pair|null_pair) ("," (pair|null_pair))*] ("}" | "," "}")
-		list : "[" [(value | typed_value | typed_null_value) ("," (value | typed_value | typed_null_value))*] ("]" | "," "]")
+		dict : "{" (pair|null_pair) ("," (pair|null_pair))* ("}" | "," "}")
+		empty_dict : "{" "}"
+		
+		list : "[" (value | typed_value | typed_null_value) ("," (value | typed_value | typed_null_value))* ("]" | "," "]")
+		empty_list : "[" "]"
 		
 		integer_n: SIGNED_INT
 		float_n: SIGNED_FLOAT
 		true: "true"
 		false: "false"
 		null: "null"
 		string : ESCAPED_STRING
@@ -91,24 +103,61 @@
 		%import common.SIGNED_FLOAT
 		%import common.WS
 		%ignore WS
 		%ignore SH_COMMENT
 	"""
 	
 
-	def __init__(self, data_classes:list=None):
+	def __init__(self, data_classes: Optional[List[Type[JunkpyDataClass]]] = None):
+		"""
+		Initializes the Junkpy parser.
+
+		Args:
+			data_classes (Optional[List[JunkpyDataClass]]): List of data classes to be used for typed value conversion.
+		"""
+		
 		self.__parser = Lark(self.__JUNKPY_GRAMMAR, start='value', parser='lalr', transformer=JunkpyTransformer(data_classes))
 
 	
-	def loads(self, string):
+	def loads(self, string: str) -> object:
+		"""
+		Parses a Junkpy string and returns the corresponding Python object.
+
+		Args:
+			string (str): The Junkpy string to parse.
+
+		Returns:
+			object: The parsed Python object.
+		"""
+		
 		return self.__parser.parse(string)
 		
 	
-	def load(self, fp):
+	def load(self, fp: IO) -> object:
+		"""
+		Parses a Junkpy file-like object and returns the corresponding Python object.
+
+		Args:
+			fp (file-like): The file-like object containing the Junkpy data.
+
+		Returns:
+			object: The parsed Python object.
+		"""
+		
 		with fp as opened_fp:
 			return self.loads(opened_fp.read())	
 		
 		
-	def load_file(self, file_path):
+	def load_file(self, file_path: str) -> object:
+		"""
+		Parses a Junkpy file and returns the corresponding Python object.
+
+		Args:
+			file_path (str): The path to the Junkpy file.
+
+		Returns:
+			object: The parsed Python object.
+		"""
+		
 		return self.load(open(file_path, "rt"))
```

### Comparing `junkpy-0.0.3/junkpy/dataclasses.py` & `junkpy-0.1.0/junkpy/dataclasses.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 from decimal import Decimal
 from datetime import datetime, timedelta, date, time
-from path import Path
+from pathlib import Path
 from re import Pattern
 import os
 import re
 
 
 
 class JunkpyDataClass:
+	"""
+	Represents a data class used in Junkpy for parsing and loading data.
+
+	Attributes:
+		CLASS (type): The Python object type to be returned by the data class.
+		KEYWORD (str): The keyword used to identify this data class in Junkpy syntax.
+
+	Methods:
+		load(cls, value, **kwargs): A class method that loads the given value and returns a python object of the type defined by CLASS attribute.
+
+	"""
 	CLASS = None
 	KEYWORD = None
 	
 	@classmethod
-	def load(cls, value, **kwargs):
+	def load(cls, value: object, **kwargs) -> object:
+		"""
+		Loads the given value and returns an instance of a python object.
+
+		Args:
+			value: The parsed value to be modified or loaded.
+			**kwargs: Modifiers included when forcing the type in a Junkpy file.
+
+		Returns:
+			object: An instance of the modified or loaded value.
+
+		"""
 		return cls.CLASS(value)
 
 
 
 class JunkpyBaseDataClassMeta(type):
 	BASE_DATA_CLASSES = []
```

### Comparing `junkpy-0.0.3/junkpy/extensions.py` & `junkpy-0.1.0/junkpy/extensions.py`

 * *Files identical despite different names*

### Comparing `junkpy-0.0.3/junkpy.egg-info/PKG-INFO` & `junkpy-0.1.0/junkpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: junkpy
-Version: 0.0.3
+Version: 0.1.0
 Summary: Extended JSON Library for Configuration Files
-Home-page: UNKNOWN
+Home-page: https://github.com/Samoxiaki/Junkpy
 Author: Samoxiaki
 Author-email: samoxiaki@yahoo.com
 License: UNKNOWN
 Description: # Junkpy: Extended JSON Library for Configuration Files.
         
         Junkpy is a Python library specifically designed for working with configuration files in JSON format. It offers a flexible approach to handling JSON objects, allowing for easier modification and manipulation of configuration data. With Junkpy, you can work with a more lenient syntax, accommodating variations in JSON structure commonly found in configuration files.
         
@@ -250,22 +250,22 @@
         | decimal    | decimal.Decimal     | Decimal values                                                                                | (decimal) "3.14"                                                                                               |
         | bool       | bool                | Boolean values                                                                                | (bool) true                                                                                                    |
         | set        | set                 | Sets of values                                                                                | (set) [1, 2, 3]                                                                                                |
         | timestamp  | datetime.datetime   | Unix timestamp values                                                                         | (timestamp) 1623345600                                                                                         |
         | timedelta  | datetime.timedelta  | Time differences in seconds                                                                   | (timedelta) 60                                                                                                 |
         |            |                     | Time differences in a list [DAYS, SECONDS, MICROSECONDS, MILLISECONDS, MINUTES, HOURS, WEEKS] | (timedelta) [5, 10, 200, 150, 3, 4, 8]                                                                         |
         |            |                     | Time differences in a dict with keyword arguments as keys                                     | (timedelta) {"days": 1, "seconds": 3600}                                                                       |
-        | time       | datetime.time       | Time values in HH:MM:SS format                                                                | (time) "12:30:45"                                                                                              |
-        |            |                     | Time values in a list [HOUR, MINUTE, SECOND]                                                  | (time) [12, 30, 45]                                                                                            |
+        | time       | datetime.time       | Time values in ISO 8601 format, [HH[:MM[:SS[.mmm[uuu]]]]][+HH:MM]                             | (time) "12:30:45"                                                                                              |
+        |            |                     | Time values in a list [HOUR, MINUTE, SECOND, MICROSECOND]                                     | (time) [12, 30, 45, 152]                                                                                       |
         |            |                     | Time values in a dict with keyword arguments as keys                                          | (time) {"hour": 12, "minute": 30, "second": 45}                                                                |
-        | date       | datetime.date       | Date values in YYYY-MM-DD format                                                              | (date) "2021-07-10"                                                                                            |
+        | date       | datetime.date       | Date values in ISO 8601 format, YYYY-MM-DD                                                    | (date) "2021-07-10"                                                                                            |
         |            |                     | Date values in a list [YEAR, MONTH, DAY]                                                      | (date) [2021, 7, 10]                                                                                           |
         |            |                     | Date values in a dict with keyword arguments as keys                                          | (date) {"year": 2021, "month": 7, "day": 10}                                                                   |
-        | datetime   | datetime.datetime   | Date and time values in YYYY-MM-DD HH:MM:SS format                                            | (datetime) "2021-07-10 12:30:45"                                                                               |
-        |            |                     | Date and time values in a list [YEAR, MONTH, DAY, HOUR, MINUTE, SECOND]                       | (datetime) [2021, 7, 10, 12, 30, 45]                                                                           |
+        | datetime   | datetime.datetime   | Date and time values in ISO 8601 format, YYYY-MM-DD [HH[:MM[:SS[.mmm[uuu]]]]][+HH:MM]         | (datetime) "2021-07-10 12:30:45"                                                                               |
+        |            |                     | Date and time values in a list [YEAR, MONTH, DAY, HOUR, MINUTE, SECOND, MICROSECOND]          | (datetime) [2021, 7, 10, 12, 30, 45, 580]                                                                      |
         |            |                     | Date and time values in a dict with keyword arguments as keys                                 | (datetime) {"year": 2021, "month": 7, "day": 10, "hour": 12, "minute": 30, "second": 45}                       |
         
         
         ## Contributing
         
         Contributions to Junkpy are welcome! If you encounter any issues, have suggestions for improvements, or would like to add new features, please feel free to submit a pull request.
```

