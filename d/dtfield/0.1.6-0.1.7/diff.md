# Comparing `tmp/dtfield-0.1.6.tar.gz` & `tmp/dtfield-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.1.6.tar", max compression
+gzip compressed data, was "dtfield-0.1.7.tar", max compression
```

## Comparing `dtfield-0.1.6.tar` & `dtfield-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.6/dtfield/__init__.py
--rw-r--r--   0        0        0     1918 2023-06-12 03:58:10.452251 dtfield-0.1.6/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.6/dtfield/base_enum.py
--rw-r--r--   0        0        0    19467 2023-06-12 04:58:08.747657 dtfield-0.1.6/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.6/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.6/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.6/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.6/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.6/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.6/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.6/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.6/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.6/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11825 2023-06-11 21:21:41.254529 dtfield-0.1.6/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.6/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.6/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.6/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.6/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.6/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.6/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.6/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-12 04:58:37.467436 dtfield-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-12 04:58:40.680323 dtfield-0.1.6/setup.py
--rw-r--r--   0        0        0      503 2023-06-12 04:58:40.680547 dtfield-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.7/dtfield/__init__.py
+-rw-r--r--   0        0        0     1918 2023-06-12 03:58:10.452251 dtfield-0.1.7/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.7/dtfield/base_enum.py
+-rw-r--r--   0        0        0    21914 2023-06-12 12:23:02.279150 dtfield-0.1.7/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.7/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.7/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.7/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.7/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.7/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.7/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.7/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.7/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.7/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.1.7/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.7/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.7/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.7/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.7/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.7/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.7/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.7/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      387 2023-06-12 12:28:28.062361 dtfield-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-12 12:28:32.896607 dtfield-0.1.7/setup.py
+-rw-r--r--   0        0        0      503 2023-06-12 12:28:32.896808 dtfield-0.1.7/PKG-INFO
```

### Comparing `dtfield-0.1.6/dtfield/_imports.py` & `dtfield-0.1.7/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/base_enum.py` & `dtfield-0.1.7/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/engine.py` & `dtfield-0.1.7/dtfield/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,32 @@
         'BaseDescriptor',
         'BaseValidator',
         'ContextBase',
         'Descriptor',
         'Validator',
         'DescriptorModel',
         'compare_descriptors',
-        'descriptors',
+        'descriptorsmap',
         'descriptors_items',
         'compare_dict',
         'compare_tuple',
         'hash_tuple',
         'hash_dict',
         'hash_descriptors',
         'check_hash',
         'check_compare',
         'instance_hash',
         'lesser_than',
         'orderby',
         'ordered',
-        'reversed_dict'
+        'reversed_dict',
+        'db_descriptors',
+        'query_from_string',
+        'exist_query',
+        'descriptors'
 ]
 
 
 from deta.base import FetchResponse
 from dtfield._imports import *
 from dtbase import *
 from .parse import *
@@ -54,32 +58,49 @@
     return {key_func(item): value_func(item) for item in iterable if condition(item) is True}
 
 
 def filter_dict(data: Mapping[str, T], condition: Callable[[T], bool]) -> dict[str, T]:
     return make_dict(data.items(), key_func=lambda x: x[0], value_func=lambda x: x[1], condition=condition)
 
 normalize_lower_if_string = partial(lambda x: x if not isinstance(x, str) else normalize_lower(x))
-descriptors = partial(lambda cls: cls.descriptors())
-descriptors_items = partial(lambda x: descriptors(x).items())
-compare_descriptors = partial(lambda x: filter_dict(descriptors(x), condition=lambda x: x[1].compare is True))
+descriptorsmap = partial(lambda cls: cls.descriptorsmap())
+descriptors = partial(lambda cls: cls.descriptorsmap().values())
+descriptors_items = partial(lambda x: descriptorsmap(x).items())
+compare_descriptors = partial(lambda x: filter_dict(descriptorsmap(x), condition=lambda x: x[1].compare is True))
 compare_dict = partial(lambda x: {k: normalize_lower_if_string(v.__get__(x)) for k, v in compare_descriptors(x).items()})
 compare_tuple = partial(lambda x: tuple(compare_dict(x).values()))
 check_compare = partial(lambda self, other: compare_tuple(self) == compare_tuple(other))
-hash_descriptors = partial(lambda x: filter_dict(descriptors(x), condition=lambda x: x[1].hash is True))
+hash_descriptors = partial(lambda x: filter_dict(descriptorsmap(x), condition=lambda x: x[1].hash is True))
 hash_dict = partial(lambda x: {k: v.__get__(x) for k, v in hash_descriptors(x).items()})
 hash_tuple = partial(lambda x: tuple(hash_dict(x).values()))
 check_hash = partial(lambda self, other: hash(hash_tuple(self)) == hash(hash_tuple(other)))
 instance_hash = partial(lambda self: hash(hash_tuple(self)))
 reversed_dict = partial(lambda x: {k: x[k] for k in reversed(x.keys())})
 lesser_than = partial(lambda self, other: compare_tuple(self) < compare_tuple(other))
 greater_than = partial(lambda self, other: compare_tuple(self) > compare_tuple(other))
 orderby = partial(lambda iterable, public_name: sorted(iterable, key=lambda item: normalize_lower_if_string(getattr(item, public_name))))
+db_descriptors = partial(lambda x: filter_dict(descriptorsmap(x), condition=lambda x: x[1].db is True))
+query_from_string = partial(lambda self, query_string: filter_dict(asdict(self), condition=lambda x: all([x[0] in query_string.split(), is_null(x[1]) is False])))
+
+def exist_query(self: ContextBase):
+    if not self.exist_params():
+        raise ValueError(f'{self.clsname()} não definiu EXIST_PARAMS')
+    qr = None
+    if isinstance(self.exist_params(), str):
+        qr = json_parse(query_from_string(self, self.exist_params()))
+    elif isinstance(self.exist_params(), list):
+        qr = json_parse(list(filter(lambda x: is_null(x) is False, [query_from_string(self, i) for i in self.exist_params()])))
+    if isinstance(qr, list):
+        if len(qr) == 1:
+            return qr[0]
+    return qr
+    
 
 def repr_func(self: ContextBase):
-    items = (f'{k}={getattr(self, v.public_name)!r}' for k, v in self.descriptors().items() if v.public == True)
+    items = (f'{k}={getattr(self, v.public_name)!r}' for k, v in self.descriptorsmap().items() if v.public == True)
     return '{}({})'.format(self.clsname(), ', '.join(items))
 
 def display_items(self: ContextBase) -> list[tuple[str, Any]]:
     if self.display_properties():
         return [(i.split('.')[-1], getter(self, i)) for i in self.display_properties()]
     return []
 
@@ -117,60 +138,104 @@
     
     @classmethod
     @cache
     def initfields_keys(cls) -> list[str]:
         return [i.name for i in cls.initfields()]
     
     @classmethod
-    def post_init_descriptors(cls):
-        return filter_dict(cls.descriptors(), lambda x: x[1].post_init_factory is not MISSING)
+    def post_init_descriptors(cls) -> dict[str, BaseDescriptor]:
+        return filter_dict(cls.descriptorsmap(), lambda x: x[1].post_init_factory is not MISSING)
     
     @classmethod
     def fields(cls) -> tuple[Field, ...]:
         return fields(cls)
     
     @classmethod
     def fieldsmap(cls) -> dict[str, Field]:
-        return make_dict(cls.fields(),  lambda x: get_attr_or_item(x, 'public_name'))
+        return make_dict(cls.fields(),  key_func=lambda x: get_attr_or_item(x, 'public_name'))
 
     
     @classmethod
     def safe_create(cls, *args, **kwargs) -> Self:
         return cls(*args, **{k: v for k, v in kwargs.items() if k in cls.initfields_keys()})
     
     @classmethod
-    def dataclass_bases(cls):
+    def dataclass_bases(cls) -> tuple:
         return tuple([b for b in cls.mro() if is_dataclass(b)])
     
     @classmethod
-    def clsname(cls):
+    def clsname(cls) -> str:
         return cls.__name__
     
     @classmethod
-    def fullvars(cls):
+    def fullvars(cls) -> dict[str, Any]:
         return {**ChainMap(*[vars(b) for b in cls.mro()])}
     
     @classmethod
-    def descriptors(cls):
+    def descriptorsmap(cls) -> dict[str, BaseDescriptor]:
         return filter_dict(cls.fullvars(), condition=lambda x: isinstance(x[1], BaseDescriptor))
     
+    @classmethod
+    def descriptors(cls):
+        return tuple(descriptors(cls))
+    
+    @classmethod
+    def descriptorskeys(cls):
+        return tuple([i.public_name for i in cls.descriptors()])
+    
     def asjson(self):
         return json_parse(asdict(self))
+    
+    def asjson_to_db(self):
+        return json_parse(filter_dict(asdict(self), condition=lambda x: x[0] in db_descriptors(self).keys()))
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
-
+    EXIST_PARAMS: ClassVar[DetaQuery] = None
+    FROZEN: ClassVar[bool] = False
+    
+    async def delete(self):
+        if not self.FROZEN:
+            return await DetaBase(self.table()).delete(getattr(self, 'key'))
+        print(f'{self.clsname()}.FROZEN is True and cannot be deleted')
+        return
+    
+    @classmethod
+    def exist_params(cls):
+        return cls.EXIST_PARAMS
+    
+    async def exist_response(self):
+        return await DetaBase(self.table()).fetch(exist_query(self))
+    
+    async def save(self):
+        new = await DetaBase(self.table()).put(self.asjson_to_db())
+        if new:
+            await self.update_context()
+            return self.safe_create(**new)
+        return None
+    
+    async def save_new(self):
+        exist = await self.exist_response()
+        if exist.count == 0:
+            return await self.save()
+        elif exist.count == 1:
+            return self.safe_create(**exist.items[0])
+        else:
+            return None
+    
+    
     @classmethod
     def singular(cls):
         return cls.SINGULAR or cls.clsname()
     
     @classmethod
     def plural(cls):
         return cls.PLURAL or f'{cls.singular()}s'
@@ -185,15 +250,15 @@
     
     @classmethod
     def table(cls):
         return cls.TABLE or cls.clsname()
     
     @classmethod
     def dependant_descriptors(cls):
-        return {d.public_name: d for d in cls.descriptors().values() if d.has_dependants is True}
+        return {d.public_name: d for d in cls.descriptorsmap().values() if d.has_dependants is True}
     
     @classmethod
     def model_dependants(cls, collection: list = None):
         return model_dependants(cls, collection or list())
 
     @classmethod
     def from_context(cls, key: str) -> Self:
```

### Comparing `dtfield-0.1.6/dtfield/functions.py` & `dtfield-0.1.7/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.1.7/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.1.7/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.1.7/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.1.7/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.1.7/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/dates.py` & `dtfield-0.1.7/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/json_encoder.py` & `dtfield-0.1.7/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/number.py` & `dtfield-0.1.7/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/string.py` & `dtfield-0.1.7/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/dtfield/parse/type_hint.py` & `dtfield-0.1.7/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.6/setup.py` & `dtfield-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

