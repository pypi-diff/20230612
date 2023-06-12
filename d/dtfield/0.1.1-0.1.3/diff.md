# Comparing `tmp/dtfield-0.1.1.tar.gz` & `tmp/dtfield-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.1.1.tar", max compression
+gzip compressed data, was "dtfield-0.1.3.tar", max compression
```

## Comparing `dtfield-0.1.1.tar` & `dtfield-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       91 2023-06-11 22:49:23.831378 dtfield-0.1.1/dtfield/__init__.py
--rw-r--r--   0        0        0     1888 2023-06-12 01:48:15.527391 dtfield-0.1.1/dtfield/_imports.py
--rw-r--r--   0        0        0     1094 2023-06-11 22:23:16.619926 dtfield-0.1.1/dtfield/base_enum.py
--rw-r--r--   0        0        0    19428 2023-06-12 03:22:00.100166 dtfield-0.1.1/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.1/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.1/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.1/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.1/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.1/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.1/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.1/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.1/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11825 2023-06-11 21:21:41.254529 dtfield-0.1.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.1/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.1/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.1/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.1/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.1/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.1/dtfield/parse/string.py
--rw-r--r--   0        0        0    10904 2023-06-11 21:21:40.293530 dtfield-0.1.1/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-12 03:22:10.729165 dtfield-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-12 03:22:19.443166 dtfield-0.1.1/setup.py
--rw-r--r--   0        0        0      503 2023-06-12 03:22:19.443372 dtfield-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.3/dtfield/__init__.py
+-rw-r--r--   0        0        0     1918 2023-06-12 03:58:10.452251 dtfield-0.1.3/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.3/dtfield/base_enum.py
+-rw-r--r--   0        0        0    19428 2023-06-12 03:22:00.100166 dtfield-0.1.3/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.3/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.3/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.3/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.3/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.3/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.3/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.3/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.3/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.3/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11825 2023-06-11 21:21:41.254529 dtfield-0.1.3/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.3/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.3/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.3/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.3/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.3/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.3/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10677 2023-06-12 03:58:10.458484 dtfield-0.1.3/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      387 2023-06-12 03:58:10.454135 dtfield-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-12 03:58:16.444203 dtfield-0.1.3/setup.py
+-rw-r--r--   0        0        0      503 2023-06-12 03:58:16.444415 dtfield-0.1.3/PKG-INFO
```

### Comparing `dtfield-0.1.1/dtfield/_imports.py` & `dtfield-0.1.3/dtfield/_imports.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,26 +46,27 @@
         'Response',
         'HTMLResponse',
         'JSONResponse',
         'RedirectResponse',
         'Request',
         're',
         'asdict',
-        'astuple'
+        'astuple',
+        'Protocol'
 ]
 
 import datetime
 import json
 import asyncio
 import re
 import uvicorn
 from enum import Enum
 from abc import ABC, abstractmethod
 from typing import Union, Optional, Any, Callable, TypeVar, Iterable, Type, NamedTuple, Mapping, get_type_hints, \
-    get_args, get_origin, ClassVar
+    get_args, get_origin, ClassVar, Protocol
 from collections import UserString, UserDict, UserList, deque, defaultdict, ChainMap
 from contextvars import Context, ContextVar, copy_context
 from functools import wraps, partialmethod, cache, partial
 from itertools import groupby
 from dataclasses import fields, MISSING, field, Field, is_dataclass, dataclass, InitVar, asdict, astuple
 from decimal import Decimal
 from anyio import create_task_group
```

### Comparing `dtfield-0.1.1/dtfield/base_enum.py` & `dtfield-0.1.3/dtfield/base_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 
 
 from dtfield import Enum
 
 class BaseEnum(Enum):
     """Enum base model class"""
     
+    def __eq__(self, other):
+        if isinstance(other, type(self)):
+            return self.name == other.name
+        return NotImplemented
+
+    def __lt__(self, other):
+        if isinstance(other, type(self)):
+            return self.value < other.value
+        return NotImplemented
+    
     @classmethod
     def table(cls):
         return cls.__name__
     
     def json(self):
         return self.name
```

### Comparing `dtfield-0.1.1/dtfield/engine.py` & `dtfield-0.1.3/dtfield/engine.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/functions.py` & `dtfield-0.1.3/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.1.3/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.1.3/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.1.3/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.1.3/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.1.3/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.1.3/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/dates.py` & `dtfield-0.1.3/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/json_encoder.py` & `dtfield-0.1.3/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/number.py` & `dtfield-0.1.3/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/string.py` & `dtfield-0.1.3/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.1/dtfield/parse/type_hint.py` & `dtfield-0.1.3/dtfield/parse/type_hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 __all__ = [
         'TypeHint',
         'parser',
         'Parser'
 ]
 
-import re
-import datetime
-from abc import ABC
-from collections import ChainMap, deque, UserList, UserDict
-from typing import Union, TypeVar, Protocol
-from decimal import Decimal
-from dataclasses import is_dataclass
 
-from typing import Any, get_args, get_origin
+from .._imports import *
 from .null import *
 from dtfield.base_enum import *
 
 
 JsonPrimitive = Union[str, float, int, bool, None]
 DetaData = Union[dict, list, str, float, int, bool]
 DetaKey = Union[str, None]
@@ -96,15 +89,15 @@
             return cls.list_engine
         elif cast_type is set:
             return cls.set_engine
         elif cast_type is tuple:
             return cls.tuple_engine
         elif hasattr(cast_type, 'CTXVAR'):
             return cls.str_engine
-        elif issubclass(cast_type, BaseEnum):
+        elif issubclass(cast_type, (BaseEnum, Enum)):
             return lambda value: cls.enum_engine(value, cast_type)
         else:
             return cast_type
 
     @classmethod
     def sequence_engine(cls, value: ParserEntry, origin: type, args: tuple[type]) -> ParserReturn:
         if origin is list:
```

### Comparing `dtfield-0.1.1/setup.py` & `dtfield-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.1.1',
+    'version': '0.1.3',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

