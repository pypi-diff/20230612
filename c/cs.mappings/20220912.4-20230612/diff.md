# Comparing `tmp/cs.mappings-20220912.4.tar.gz` & `tmp/cs.mappings-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.mappings-20220912.4.tar", last modified: Mon Sep 12 07:22:50 2022, max compression
+gzip compressed data, was "cs.mappings-20230612.tar", last modified: Mon Jun 12 03:23:09 2023, max compression
```

## Comparing `cs.mappings-20220912.4.tar` & `cs.mappings-20230612.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-12 07:22:50.748367 cs.mappings-20220912.4/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2022-09-12 07:22:21.000000 cs.mappings-20220912.4/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    19988 2022-09-12 07:22:50.748511 cs.mappings-20220912.4/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    24450 2022-09-12 07:22:27.000000 cs.mappings-20220912.4/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-12 07:22:50.744740 cs.mappings-20220912.4/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-12 07:22:50.744967 cs.mappings-20220912.4/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-12 07:22:50.746423 cs.mappings-20220912.4/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    47927 2022-09-12 07:22:13.000000 cs.mappings-20220912.4/lib/python/cs/mappings.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-12 07:22:50.748105 cs.mappings-20220912.4/lib/python/cs.mappings.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    19988 2022-09-12 07:22:50.000000 cs.mappings-20220912.4/lib/python/cs.mappings.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      310 2022-09-12 07:22:50.000000 cs.mappings-20220912.4/lib/python/cs.mappings.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2022-09-12 07:22:50.000000 cs.mappings-20220912.4/lib/python/cs.mappings.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      115 2022-09-12 07:22:50.000000 cs.mappings-20220912.4/lib/python/cs.mappings.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2022-09-12 07:22:50.000000 cs.mappings-20220912.4/lib/python/cs.mappings.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    20316 2022-09-12 07:22:43.000000 cs.mappings-20220912.4/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      951 2022-09-12 07:22:50.749134 cs.mappings-20220912.4/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2022-09-12 07:22:27.000000 cs.mappings-20220912.4/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:23:09.864583 cs.mappings-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 03:22:34.000000 cs.mappings-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    20403 2023-06-12 03:23:09.864767 cs.mappings-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    24852 2023-06-12 03:22:41.000000 cs.mappings-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:23:09.859411 cs.mappings-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:23:09.859770 cs.mappings-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:23:09.862304 cs.mappings-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    48444 2023-06-12 03:22:25.000000 cs.mappings-20230612/lib/python/cs/mappings.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 03:23:09.864296 cs.mappings-20230612/lib/python/cs.mappings.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    20403 2023-06-12 03:23:09.000000 cs.mappings-20230612/lib/python/cs.mappings.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      310 2023-06-12 03:23:09.000000 cs.mappings-20230612/lib/python/cs.mappings.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 03:23:09.000000 cs.mappings-20230612/lib/python/cs.mappings.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      115 2023-06-12 03:23:09.000000 cs.mappings-20230612/lib/python/cs.mappings.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 03:23:09.000000 cs.mappings-20230612/lib/python/cs.mappings.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    20735 2023-06-12 03:23:01.000000 cs.mappings-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)      949 2023-06-12 03:23:09.865579 cs.mappings-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 03:22:41.000000 cs.mappings-20230612/setup.py
```

### Comparing `cs.mappings-20220912.4/PKG-INFO` & `cs.mappings-20230612/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.mappings
-Version: 20220912.4
+Version: 20230612
 Summary: Facilities for mappings and objects associated with mappings.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -15,27 +15,31 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Facilities for mappings and objects associated with mappings.
 
-*Latest release 20220912.4*:
-* TypedKeyMixin: add .get() and .setdefault().
-* Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
+*Latest release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for "ATTRABLE_MAPPING_DEFAULT", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
 
 In particular `named_column_tuple(column_names)`,
 a function returning a factory
 for namedtuples subclasses derived from the supplied column names,
 and `named_column_tuples(rows)`,
 a function returning a namedtuple factory and an iterable of instances
 containing the row data.
 These are used by the `csv_import` and `xl_import` functions
 from `cs.csvutils`.
 
+## Function `attrable(o)`
+
+Like `jsonable`, return `o` with `dicts` replaced by `AttrableMapping`s.
+
 ## Class `AttrableMapping(builtins.dict, AttrableMappingMixin)`
 
 A `dict` subclass using `AttrableMappingMixin`.
 
 ## Class `AttrableMappingMixin`
 
 Provides a `__getattr__` which accesses the mapping value.
@@ -501,14 +505,18 @@
 Initialise the `TypedKeyDict`. The first positional parameter
 is the type for keys.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for "ATTRABLE_MAPPING_DEFAULT", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
+
 *Release 20220912.4*:
 * TypedKeyMixin: add .get() and .setdefault().
 * Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
 
 *Release 20220912.3*:
 * New TypedKeyClass class factory.
 * Redo StrKeyedDict and UUIDKeyedDict using TypedKeyClass.
```

### Comparing `cs.mappings-20220912.4/README.md` & `cs.mappings-20230612/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Facilities for mappings and objects associated with mappings.
 
-*Latest release 20220912.4*:
-* TypedKeyMixin: add .get() and .setdefault().
-* Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
+*Latest release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for "ATTRABLE_MAPPING_DEFAULT", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
 
 In particular `named_column_tuple(column_names)`,
 a function returning a factory
 for namedtuples subclasses derived from the supplied column names,
 and `named_column_tuples(rows)`,
 a function returning a namedtuple factory and an iterable of instances
 containing the row data.
 These are used by the `csv_import` and `xl_import` functions
 from `cs.csvutils`.
 
+## Function `attrable(o)`
+
+Like `jsonable`, return `o` with `dicts` replaced by `AttrableMapping`s.
+
 ## Class `AttrableMapping(builtins.dict, AttrableMappingMixin)`
 
 A `dict` subclass using `AttrableMappingMixin`.
 
 ## Class `AttrableMappingMixin`
 
 Provides a `__getattr__` which accesses the mapping value.
@@ -160,15 +164,15 @@
 
 If the instance's class has `json_default` or `json_separators` these
 are used for the `default` and `separators` parameters of the `json.dumps()`
 call.
 Note that the default value of `separators` is `(',',':')`
 which produces the most compact JSON form.
 
-*Method `JSONableMappingMixin.append_ndjson(arg, *a, **kw)`*:
+*Method `JSONableMappingMixin.append_ndjson(self, f)`*:
 Append this object to `f`, a file or filename, as NDJSON.
 
 *Method `JSONableMappingMixin.as_json(self)`*:
 Return the `dict` transcribed as JSON.
 
 If the instance's class has `json_default` or `json_separators` these
 are used for the `default` and `separators` parameters of the `json.dumps()`
@@ -432,21 +436,21 @@
     'prefix.key'
     >>> proxy.key('prefix.key')
     'key'
 
 *Method `RemappedMappingProxy.get(self, key, default=None)`*:
 Return the value for key `key` or `default`.
 
-*Method `RemappedMappingProxy.key(self, *a, **kw)`*:
+*Method `RemappedMappingProxy.key(self, subk)`*:
 Return the external key for `subk`.
 
 *Method `RemappedMappingProxy.keys(self, select_key=None)`*:
 Yield the external keys.
 
-*Method `RemappedMappingProxy.subkey(self, *a, **kw)`*:
+*Method `RemappedMappingProxy.subkey(self, key)`*:
 Return the internal key for `key`.
 
 ## Class `SeenSet`
 
 A set-like collection with optional backing store file.
 
 *Method `SeenSet.add(self, s, foreign=False)`*:
@@ -633,14 +637,18 @@
 Initialise the `TypedKeyDict`. The first positional parameter
 is the type for keys.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for "ATTRABLE_MAPPING_DEFAULT", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
+
 *Release 20220912.4*:
 * TypedKeyMixin: add .get() and .setdefault().
 * Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
 
 *Release 20220912.3*:
 * New TypedKeyClass class factory.
 * Redo StrKeyedDict and UUIDKeyedDict using TypedKeyClass.
```

### Comparing `cs.mappings-20220912.4/lib/python/cs/mappings.py` & `cs.mappings-20230612/lib/python/cs/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from cs.deco import strable
 from cs.lex import isUC_, parseUC_sAttr, cutprefix, r, snakecase, stripped_dedent
 from cs.logutils import warning
 from cs.pfx import Pfx, pfx_method
 from cs.seq import Seq
 from cs.sharedfile import SharedAppendLines
 
-__version__ = '20220912.4'
+__version__ = '20230612'
 
 DISTINFO = {
     'description':
     "Facilities for mappings and objects associated with mappings.",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
@@ -1001,14 +1001,16 @@
     ''' Unknown attributes are obtained from the mapping entries.
 
         Note that this first consults `self.__dict__`.
         For many classes that is redundant, but subclasses of
         `dict` at least seem not to consult that with attribute
         lookup, likely because a pure `dict` has no `__dict__`.
     '''
+    if attr == 'ATTRABLE_MAPPING_DEFAULT':
+      raise AttributeError("%s.%s" % (self.__class__.__name__, attr))
     # try self.__dict__ first - this is because it appears that
     # getattr(dict,...) does not consult __dict__
     try:
       _d = self.__dict__
     except AttributeError:
       # no __dict__? skip this step
       pass
@@ -1248,14 +1250,22 @@
     '''
     self.mapping[record[self.IndexedSetMixin__pk]] = record
 
 class AttrableMapping(dict, AttrableMappingMixin):
   ''' A `dict` subclass using `AttrableMappingMixin`.
   '''
 
+def attrable(o):
+  ''' Like `jsonable`, return `o` with `dicts` replaced by `AttrableMapping`s. '''
+  if isinstance(o, dict):
+    o = AttrableMapping({k: attrable(v) for k, v in o.items()})
+  elif isinstance(o, list):
+    o = list(map(attrable, o))
+  return o
+
 class UUIDedDict(dict, JSONableMappingMixin, AttrableMappingMixin):
   ''' A handy `dict` subtype providing the basis for mapping classes
       indexed by `UUID`s.
 
       The `'uuid'` attribute is always a `UUID` instance.
   '''
 
@@ -1366,14 +1376,15 @@
       self._mapped_subkeys[subk] = key
     return subk
 
   @pfx_method
   def key(self, subk):
     ''' Return the external key for `subk`.
     '''
+    X("%s.key(subk=%r)...", self.__class__.__name__, subk)
     try:
       k = self._mapped_subkeys[subk]
     except KeyError:
       k = self._from_subkey(subk)
       assert k not in self._mapped_keys
       self._mapped_keys[k] = subk
       self._mapped_subkeys[subk] = k
@@ -1430,23 +1441,26 @@
         type(self).__name__, type(self).__mro__, self.prefix, r(self.mapping)
     )
 
   @staticmethod
   def prefixify_subkey(subk, prefix):
     ''' Return the external (prefixed) key from a subkey `subk`.
     '''
-    assert not subk.startswith(prefix)
+    assert not subk.startswith(prefix), (
+        "subkey %r already starts with the prefix %r" % (subk, prefix)
+    )
     return prefix + subk
 
   @staticmethod
   def unprefixify_key(key, prefix):
     ''' Return the internal subkey (unprefixed) from the external `key`.
     '''
-    assert key.startswith(prefix), \
+    assert key.startswith(prefix), (
         "key:%r does not start with prefix:%r" % (key, prefix)
+    )
     return cutprefix(key, prefix)
 
   # pylint: disable=arguments-differ
   def keys(self):
     ''' Yield the post-prefix suffix of the keys in `self.mapping`.
     '''
     return super().keys(
```

### Comparing `cs.mappings-20220912.4/lib/python/cs.mappings.egg-info/PKG-INFO` & `cs.mappings-20230612/lib/python/cs.mappings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.mappings
-Version: 20220912.4
+Version: 20230612
 Summary: Facilities for mappings and objects associated with mappings.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -15,27 +15,31 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Facilities for mappings and objects associated with mappings.
 
-*Latest release 20220912.4*:
-* TypedKeyMixin: add .get() and .setdefault().
-* Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
+*Latest release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for "ATTRABLE_MAPPING_DEFAULT", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
 
 In particular `named_column_tuple(column_names)`,
 a function returning a factory
 for namedtuples subclasses derived from the supplied column names,
 and `named_column_tuples(rows)`,
 a function returning a namedtuple factory and an iterable of instances
 containing the row data.
 These are used by the `csv_import` and `xl_import` functions
 from `cs.csvutils`.
 
+## Function `attrable(o)`
+
+Like `jsonable`, return `o` with `dicts` replaced by `AttrableMapping`s.
+
 ## Class `AttrableMapping(builtins.dict, AttrableMappingMixin)`
 
 A `dict` subclass using `AttrableMappingMixin`.
 
 ## Class `AttrableMappingMixin`
 
 Provides a `__getattr__` which accesses the mapping value.
@@ -501,14 +505,18 @@
 Initialise the `TypedKeyDict`. The first positional parameter
 is the type for keys.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for "ATTRABLE_MAPPING_DEFAULT", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
+
 *Release 20220912.4*:
 * TypedKeyMixin: add .get() and .setdefault().
 * Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
 
 *Release 20220912.3*:
 * New TypedKeyClass class factory.
 * Redo StrKeyedDict and UUIDKeyedDict using TypedKeyClass.
```

### Comparing `cs.mappings-20220912.4/pyproject.toml` & `cs.mappings-20230612/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,55 +5,59 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.deco>=20220905",
-    "cs.lex>=20220626",
-    "cs.logutils>=20220531",
-    "cs.pfx>=20220523",
-    "cs.seq>=20220530",
+    "cs.deco>=20230331",
+    "cs.lex>=20230401",
+    "cs.logutils>=20230212",
+    "cs.pfx>=20230604",
+    "cs.seq>=20221118",
     "cs.sharedfile>=20211208",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20220912.4"
+version = "20230612"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Facilities for mappings and objects associated with mappings.
 
-*Latest release 20220912.4*:
-* TypedKeyMixin: add .get() and .setdefault().
-* Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
+*Latest release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for \"ATTRABLE_MAPPING_DEFAULT\", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
 
 In particular `named_column_tuple(column_names)`,
 a function returning a factory
 for namedtuples subclasses derived from the supplied column names,
 and `named_column_tuples(rows)`,
 a function returning a namedtuple factory and an iterable of instances
 containing the row data.
 These are used by the `csv_import` and `xl_import` functions
 from `cs.csvutils`.
 
+## Function `attrable(o)`
+
+Like `jsonable`, return `o` with `dicts` replaced by `AttrableMapping`s.
+
 ## Class `AttrableMapping(builtins.dict, AttrableMappingMixin)`
 
 A `dict` subclass using `AttrableMappingMixin`.
 
 ## Class `AttrableMappingMixin`
 
 Provides a `__getattr__` which accesses the mapping value.
@@ -519,14 +523,18 @@
 Initialise the `TypedKeyDict`. The first positional parameter
 is the type for keys.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* AttrableMappingMixin.__getattr__: fast path the check for \"ATTRABLE_MAPPING_DEFAULT\", fixes unbound recursion.
+* New attrable() function returning an object with dicts transmuted to AttrableMapping instances.
+
 *Release 20220912.4*:
 * TypedKeyMixin: add .get() and .setdefault().
 * Provide names for UUIDKeyedDict, StrKeyedDefaultDict, UUIDKeyedDefaultDict.
 
 *Release 20220912.3*:
 * New TypedKeyClass class factory.
 * Redo StrKeyedDict and UUIDKeyedDict using TypedKeyClass.
```

### Comparing `cs.mappings-20220912.4/setup.cfg` & `cs.mappings-20230612/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.mappings
-version = 20220912.4
+version = 20230612
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Facilities for mappings and objects associated with mappings.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -18,18 +18,18 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
-	cs.deco>=20220905
-	cs.lex>=20220626
-	cs.logutils>=20220531
-	cs.pfx>=20220523
-	cs.seq>=20220530
+	cs.deco>=20230331
+	cs.lex>=20230401
+	cs.logutils>=20230212
+	cs.pfx>=20230604
+	cs.seq>=20221118
 	cs.sharedfile>=20211208
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

