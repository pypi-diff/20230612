# Comparing `tmp/dtfield-0.1.7.tar.gz` & `tmp/dtfield-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.1.7.tar", max compression
+gzip compressed data, was "dtfield-0.1.8.tar", max compression
```

## Comparing `dtfield-0.1.7.tar` & `dtfield-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.7/dtfield/__init__.py
--rw-r--r--   0        0        0     1918 2023-06-12 03:58:10.452251 dtfield-0.1.7/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.7/dtfield/base_enum.py
--rw-r--r--   0        0        0    21914 2023-06-12 12:23:02.279150 dtfield-0.1.7/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.7/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.7/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.7/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.7/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.7/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.7/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.7/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.7/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.7/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.1.7/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.7/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.7/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.7/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.7/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.7/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.7/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.7/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-12 12:28:28.062361 dtfield-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-12 12:28:32.896607 dtfield-0.1.7/setup.py
--rw-r--r--   0        0        0      503 2023-06-12 12:28:32.896808 dtfield-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.8/dtfield/__init__.py
+-rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.1.8/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.8/dtfield/base_enum.py
+-rw-r--r--   0        0        0    21781 2023-06-12 16:27:27.493539 dtfield-0.1.8/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.8/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.8/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.8/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.8/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.8/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.8/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.8/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.8/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.8/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.1.8/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.8/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.8/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.8/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.8/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.8/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.8/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.8/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      387 2023-06-12 17:15:19.554397 dtfield-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-12 17:15:24.642666 dtfield-0.1.8/setup.py
+-rw-r--r--   0        0        0      503 2023-06-12 17:15:24.642883 dtfield-0.1.8/PKG-INFO
```

### Comparing `dtfield-0.1.7/dtfield/_imports.py` & `dtfield-0.1.8/dtfield/_imports.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         'HTMLResponse',
         'JSONResponse',
         'RedirectResponse',
         'Request',
         're',
         'asdict',
         'astuple',
-        'Protocol'
+        'Protocol',
+        'descdataclass'
 ]
 
 import datetime
 import json
 import asyncio
 import re
 import uvicorn
@@ -70,7 +71,10 @@
 from dataclasses import fields, MISSING, field, Field, is_dataclass, dataclass, InitVar, asdict, astuple
 from decimal import Decimal
 from anyio import create_task_group
 from typing_extensions import Self
 from starlette.requests import Request
 from starlette.responses import Response, HTMLResponse, JSONResponse, RedirectResponse
 
+
+
+descdataclass = partial(dataclass, eq=False, repr=False, order=False)
```

### Comparing `dtfield-0.1.7/dtfield/base_enum.py` & `dtfield-0.1.8/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/engine.py` & `dtfield-0.1.8/dtfield/engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,18 +57,21 @@
     ) -> dict[str, T]:
     return {key_func(item): value_func(item) for item in iterable if condition(item) is True}
 
 
 def filter_dict(data: Mapping[str, T], condition: Callable[[T], bool]) -> dict[str, T]:
     return make_dict(data.items(), key_func=lambda x: x[0], value_func=lambda x: x[1], condition=condition)
 
+def dict_items(data: Mapping) -> list[tuple[Any, Any]]:
+    return list(data.items())
+
 normalize_lower_if_string = partial(lambda x: x if not isinstance(x, str) else normalize_lower(x))
 descriptorsmap = partial(lambda cls: cls.descriptorsmap())
 descriptors = partial(lambda cls: cls.descriptorsmap().values())
-descriptors_items = partial(lambda x: descriptorsmap(x).items())
+descriptors_items = partial(lambda cls: dict_items(descriptorsmap(cls)))
 compare_descriptors = partial(lambda x: filter_dict(descriptorsmap(x), condition=lambda x: x[1].compare is True))
 compare_dict = partial(lambda x: {k: normalize_lower_if_string(v.__get__(x)) for k, v in compare_descriptors(x).items()})
 compare_tuple = partial(lambda x: tuple(compare_dict(x).values()))
 check_compare = partial(lambda self, other: compare_tuple(self) == compare_tuple(other))
 hash_descriptors = partial(lambda x: filter_dict(descriptorsmap(x), condition=lambda x: x[1].hash is True))
 hash_dict = partial(lambda x: {k: v.__get__(x) for k, v in hash_descriptors(x).items()})
 hash_tuple = partial(lambda x: tuple(hash_dict(x).values()))
@@ -77,14 +80,15 @@
 reversed_dict = partial(lambda x: {k: x[k] for k in reversed(x.keys())})
 lesser_than = partial(lambda self, other: compare_tuple(self) < compare_tuple(other))
 greater_than = partial(lambda self, other: compare_tuple(self) > compare_tuple(other))
 orderby = partial(lambda iterable, public_name: sorted(iterable, key=lambda item: normalize_lower_if_string(getattr(item, public_name))))
 db_descriptors = partial(lambda x: filter_dict(descriptorsmap(x), condition=lambda x: x[1].db is True))
 query_from_string = partial(lambda self, query_string: filter_dict(asdict(self), condition=lambda x: all([x[0] in query_string.split(), is_null(x[1]) is False])))
 
+
 def exist_query(self: ContextBase):
     if not self.exist_params():
         raise ValueError(f'{self.clsname()} não definiu EXIST_PARAMS')
     qr = None
     if isinstance(self.exist_params(), str):
         qr = json_parse(query_from_string(self, self.exist_params()))
     elif isinstance(self.exist_params(), list):
@@ -184,30 +188,30 @@
     
     def asjson(self):
         return json_parse(asdict(self))
     
     def asjson_to_db(self):
         return json_parse(filter_dict(asdict(self), condition=lambda x: x[0] in db_descriptors(self).keys()))
 
-        
+
         
 @dataclass
 class ContextBase(DescriptorModel):
     CTXVAR: ClassVar[ContextVar] = None
     DETA_QUERY: ClassVar[Optional[DetaQuery]] = None
     TABLE: ClassVar[Optional[str]] = None
     ITEM_NAME: ClassVar[Optional[str]] = None
     DISPLAY_PROPERTIES: ClassVar[Optional[list[str]]] = None
     SINGULAR: ClassVar[Optional[str]] = None
     PLURAL: ClassVar[Optional[str]] = None
     EXIST_PARAMS: ClassVar[DetaQuery] = None
-    FROZEN: ClassVar[bool] = False
+    DELETABLE: ClassVar[bool] = True
     
     async def delete(self):
-        if not self.FROZEN:
+        if self.DELETABLE:
             return await DetaBase(self.table()).delete(getattr(self, 'key'))
         print(f'{self.clsname()}.FROZEN is True and cannot be deleted')
         return
     
     @classmethod
     def exist_params(cls):
         return cls.EXIST_PARAMS
@@ -286,20 +290,29 @@
     
     @classmethod
     async def update_context(cls):
         async with create_task_group() as tks:
             for item in cls.model_dependants():
                 tks.start_soon(item.set_context)
                 
+    def __lt__(self, other):
+        return normalize_lower(str(self)) < normalize_lower(str(other))
+    
     @classmethod
     def instances_list(cls) -> list[Self]:
-        return ordered([cls.safe_create(**i) for i in cls.get_context().values()])
+        return [cls.from_context(i) for i in cls.get_context().keys()]
+    
+    @classmethod
+    def sorted_instances_list(cls) -> list[Self]:
+        return sorted(cls.instances_list())
+    
+    @classmethod
+    def ordered_instances_list(cls) -> list[Self]:
+        return ordered(cls.instances_list())
     
-
-
 
 def model_dependants(obj: type[ContextBase], collection: list = None):
     collection = collection or list()
     for item in obj.dependant_descriptors().values():
         models = item.dependants
         for model in models:
             if not model in collection:
@@ -313,19 +326,18 @@
 ModelMap: ChainMap[str, type[ContextBase]] = ChainMap()
 
 
 def context_model(cls: type[ContextBase]):
     @wraps(cls)
     def wrapper():
         cls.CTXVAR = ContextVar(f'{cls.__name__}Var')
-        ModelMap[cls.__name__] = cls
         cls.__repr__ = partialmethod(repr_func)
-        cls.__eq__ = partialmethod(check_hash)
-        cls.__lt__ = partialmethod(lesser_than)
-        cls.__gt__ = partialmethod(greater_than)
+        cls.__eq__ = partialmethod(eq_function)
+
+        ModelMap[cls.__name__] = cls
         return cls
     
     return wrapper()
 
 
 class BaseDescriptor:
     BASE_NUMBER_TYPES: ClassVar[TupleOfTypes] = (int, float, Decimal)
@@ -356,15 +368,15 @@
             # maps
             metadata: Optional[Mapping] = None,
             # strings
             label: Optional[str] = None,
             table: Optional[str] = None,
             item_name: Optional[str] = None,
             # lists
-            tables: Optional[list[str]] = None,
+            tables: Optional[list[str]] = None
     ):
         self._default = default
         self.private = private
         self.auto = auto
         self.update_auto = update_auto
         self.default_factory = default_factory
         self.post_init_factory = post_init_factory
@@ -379,14 +391,16 @@
         self.multiple = multiple
         self._item_name = item_name
         self.db = db
         self._tablekey = tablekey
         self.frozen = frozen
         self.post_parse = post_parse
         self.pre_parse = pre_parse
+        if self.hash is True:
+            assert any([self.granted is True, self.required is True]), f'If "hash" is True, the attribute is "granted" or "required" need be True'
         
     def __repr__(self):
         return '{}({})'.format(
                 type(self).__name__,
                 ', '.join([f'{k}={getattr(self, k)!r}' for k in [
                         'field_type', 'public_name', 'required', 'owner', 'dependants', 'db'
                 ]])
@@ -423,28 +437,43 @@
         if self.tables:
             return tuple([ModelMap.get(item) for item in self.tables])
         elif self.table:
             return tuple([ModelMap.get(self.table)])
         return tuple()
     
     @property
-    def required(self):
-        return True if all([
-                self._default is MISSING,
-                self.default_factory is MISSING,
-                self.auto is MISSING,
-                self.cls_auto is MISSING,
-                self.update_auto is MISSING,
-                self.post_init_factory is MISSING,
+    def auto_or_factory(self):
+        return True if any([
+                self.default_factory is not MISSING,
+                self.auto is not MISSING,
+                self.cls_auto is not MISSING,
+                self.update_auto is not MISSING,
+                self.post_init_factory is not MISSING,
         ]) else False
     
     @property
+    def required(self):
+        return all([self._default is MISSING, self.auto_or_factory is False])
+        # return True if all([
+        #         self._default is MISSING,
+        #         self.default_factory is MISSING,
+        #         self.auto is MISSING,
+        #         self.cls_auto is MISSING,
+        #         self.update_auto is MISSING,
+        #         self.post_init_factory is MISSING,
+        # ]) else False
+    
+    @property
+    def granted(self):
+        return any([is_null(self._default) is False, self.auto_or_factory is True])
+    
+    @property
     def default(self):
         if self._default is MISSING:
-            if self.required is False:
+            if self.auto_or_factory is True:
                 return None
         return self._default
     
     @property
     def label(self):
         return self._label or self.public_name
     
@@ -496,27 +525,14 @@
     def parse(self, instance, value):
         if all([is_null(value) is False, is_null(self.pre_parse) is False]):
             value = self.pre_parse(value)
         value = Parser.get(value, self.field_type)
         if all([is_null(value) is False, is_null(self.post_parse) is False]):
             value = self.post_parse(value)
         return value
-        # print(self.expected_type)
-        # if is_null(value):
-        #     return ''
-        # elif isinstance(value, self.expected_type):
-        #     return value
-        # elif self.type in self.STRING_TYPES:
-        #     return parse_str(value) if self.type is str else parse_bytes(value)
-        # elif self.type in self.BASE_DATETIME_TYPES:
-        #     return parse_datetime(value) if self.type is datetime.datetime else parse_date(value)
-        # elif self.type in self.BASE_NUMBER_TYPES:
-        #     return parse_int(value) if self.type is int else parse_float(
-        #         value) if self.type is float else parse_decimal(value)
-        # return value
     
     def validate(self, instance, value):
         pass
     
     @property
     def name(self):
         return '{}.{}'.format(self.owner.__name__, self.public_name)
@@ -524,28 +540,14 @@
     @property
     def type_hint(self):
         return TypeHint(self.field_type)
     
     @property
     def expected_type(self):
         return self.type_hint.expected_type
-        # if self.type in self.BASE_TYPES:
-        #     return self.type
-        # elif is_dataclass(self.type):
-        #     return str
-        # elif self.tables:
-        #     return (i for i in [list, str])
-        # elif isinstance(self.type, type):
-        #     return self.type
-        # elif get_args(self.type):
-        #     if get_origin(self.type) in [Union]:
-        #         return tuple([*get_args(self.type)])
-        #     else:
-        #         return get_origin(self.type)
-        # return self.type
 
 
 class BaseValidator(BaseDescriptor):
     def __init__(
             self,
             step: Optional[int, float] = None,
             min: Optional[int, float] = None,
```

### Comparing `dtfield-0.1.7/dtfield/functions.py` & `dtfield-0.1.8/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.1.8/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.1.8/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.1.8/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.1.8/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.1.8/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.1.8/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/dates.py` & `dtfield-0.1.8/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/json_encoder.py` & `dtfield-0.1.8/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/number.py` & `dtfield-0.1.8/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/string.py` & `dtfield-0.1.8/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/dtfield/parse/type_hint.py` & `dtfield-0.1.8/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.7/setup.py` & `dtfield-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

