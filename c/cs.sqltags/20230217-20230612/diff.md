# Comparing `tmp/cs.sqltags-20230217.tar.gz` & `tmp/cs.sqltags-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.sqltags-20230217.tar", last modified: Fri Feb 17 00:42:57 2023, max compression
+gzip compressed data, was "cs.sqltags-20230612.tar", last modified: Mon Jun 12 04:30:46 2023, max compression
```

## Comparing `cs.sqltags-20230217.tar` & `cs.sqltags-20230612.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:42:57.708959 cs.sqltags-20230217/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-02-17 00:42:33.000000 cs.sqltags-20230217/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    18635 2023-02-17 00:42:57.709094 cs.sqltags-20230217/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    33059 2023-02-17 00:42:38.000000 cs.sqltags-20230217/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:42:57.704196 cs.sqltags-20230217/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:42:57.704435 cs.sqltags-20230217/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:42:57.706058 cs.sqltags-20230217/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    82178 2023-02-17 00:42:25.000000 cs.sqltags-20230217/lib/python/cs/sqltags.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-17 00:42:57.708606 cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    18635 2023-02-17 00:42:57.000000 cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      352 2023-02-17 00:42:57.000000 cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-02-17 00:42:57.000000 cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       44 2023-02-17 00:42:57.000000 cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      299 2023-02-17 00:42:57.000000 cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-02-17 00:42:57.000000 cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    19227 2023-02-17 00:42:49.000000 cs.sqltags-20230217/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1289 2023-02-17 00:42:57.709640 cs.sqltags-20230217/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-02-17 00:42:38.000000 cs.sqltags-20230217/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:30:46.569514 cs.sqltags-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 04:30:18.000000 cs.sqltags-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18943 2023-06-12 04:30:46.569709 cs.sqltags-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    33487 2023-06-12 04:30:23.000000 cs.sqltags-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:30:46.562739 cs.sqltags-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:30:46.563106 cs.sqltags-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:30:46.565373 cs.sqltags-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    83124 2023-06-12 04:30:09.000000 cs.sqltags-20230612/lib/python/cs/sqltags.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:30:46.568825 cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18943 2023-06-12 04:30:46.000000 cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      352 2023-06-12 04:30:46.000000 cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 04:30:46.000000 cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       44 2023-06-12 04:30:46.000000 cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      299 2023-06-12 04:30:46.000000 cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 04:30:46.000000 cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    19535 2023-06-12 04:30:37.000000 cs.sqltags-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1289 2023-06-12 04:30:46.570479 cs.sqltags-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 04:30:23.000000 cs.sqltags-20230612/setup.py
```

### Comparing `cs.sqltags-20230217/PKG-INFO` & `cs.sqltags-20230612/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.sqltags
-Version: 20230217
+Version: 20230612
 Summary: Simple SQL based tagging and the associated `sqltags` command line script, supporting both tagged named objects and tagged timestamped log entries.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -17,16 +17,17 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Simple SQL based tagging
 and the associated `sqltags` command line script,
 supporting both tagged named objects and tagged timestamped log entries.
 
-*Latest release 20230217*:
-SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
+*Latest release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
 
 Compared to `cs.fstags` and its associated `fstags` command,
 this is oriented towards large numbers of items
 not naturally associated with filesystem objects.
 
 My initial use case is an activity log
 (unnamed timestamped tag sets)
@@ -374,14 +375,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
+
 *Release 20230217*:
 SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
 
 *Release 20230212.1*:
 Mark SQLTags as promotable.
 
 *Release 20230212*:
```

### Comparing `cs.sqltags-20230217/README.md` & `cs.sqltags-20230612/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Simple SQL based tagging
 and the associated `sqltags` command line script,
 supporting both tagged named objects and tagged timestamped log entries.
 
-*Latest release 20230217*:
-SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
+*Latest release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
 
 Compared to `cs.fstags` and its associated `fstags` command,
 this is oriented towards large numbers of items
 not naturally associated with filesystem objects.
 
 My initial use case is an activity log
 (unnamed timestamped tag sets)
@@ -76,23 +77,22 @@
           Run an interactive Python prompt with some predefined local names.
         tag {-|entity-name} {tag[=value]|-tag}...
           Tag an entity with multiple tags.
           With the form "-tag", remove that tag from the direct tags.
           A entity-name named "-" indicates that entity-names should
           be read from the standard input.
 
+*`BaseSQLTagsCommand.Options`*
+
 *`BaseSQLTagsCommand.TAGSETS_CLASS`*
 
 *`BaseSQLTagsCommand.TAGSET_CRITERION_CLASS`*
 
 *`BaseSQLTagsCommand.TAG_BASED_TEST_CLASS`*
 
-*Method `BaseSQLTagsCommand.apply_defaults(self)`*:
-Set up the default values in `options`.
-
 *Method `BaseSQLTagsCommand.apply_opt(self, opt, val)`*:
 Apply a command line option.
 
 *Method `BaseSQLTagsCommand.cmd_dbshell(self, argv)`*:
 Usage: {cmd}
 Start an interactive database shell.
 
@@ -470,16 +470,15 @@
 Constrain the names to those starting with `prefix`
 if not `None`.
 
 *Property `SQLTags.metanode`*:
 The metadata node.
 
 *Method `SQLTags.startup_shutdown(self)`*:
-Empty stub startup/shutdown since we use autosessions.
-Particularly, we do not want to keep SQLite dbs open.
+Open the ORM while the `SQLTags` is open.
 
 *Method `SQLTags.values(self, *, prefix=None)`*:
 Return an iterable of the named `TagSet`s.
 Excludes unnamed `TagSet`s.
 
 Constrain the names to those starting with `prefix`
 if not `None`.
@@ -638,14 +637,22 @@
 *Method `SQLTagSet.from_polyvalue(tag_name: str, pv: cs.sqltags.PolyValue)`*:
 Convert an SQL `PolyValue` to a tag value.
 
 This can be overridden by subclasses along with `to_polyvalue`.
 The `tag_name` is provided for context
 in case it should influence the normalisation.
 
+*Method `SQLTagSet.jsonable(value)`*:
+Convert `value` to a form which can be directly JSON serialised.
+
+In particular this converts non-list/set/tuple Sequences to lists
+and non-dict Mappings to dicts.
+
+Warning: this is not robust against cycles.
+
 *Property `SQLTagSet.name`*:
 Return the `.name`.
 
 *Method `SQLTagSet.parent_tagset(self, tag_name='parent')`*:
 Return the parent `TagSet` as defined by a `Tag`,
 by default the `Tag` named `'parent'`.
 
@@ -791,14 +798,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
+
 *Release 20230217*:
 SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
 
 *Release 20230212.1*:
 Mark SQLTags as promotable.
 
 *Release 20230212*:
```

### Comparing `cs.sqltags-20230217/lib/python/cs/sqltags.py` & `cs.sqltags-20230612/lib/python/cs/sqltags.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,26 +25,27 @@
 '''
 
 from abc import abstractmethod
 from builtins import id as builtin_id
 from collections import defaultdict, namedtuple
 from contextlib import contextmanager
 import csv
+from dataclasses import dataclass, field
 from datetime import date, datetime
 from fnmatch import fnmatchcase
 from getopt import getopt, GetoptError
 import operator
 import os
 from os.path import expanduser, isabs as isabspath
 import re
 import sys
 from subprocess import run
 from threading import RLock
 import time
-from typing import List, Optional
+from typing import List, Mapping, Optional, Sequence
 
 from icontract import ensure, require
 from sqlalchemy import (
     Column,
     Integer,
     Float,
     String,
@@ -70,18 +71,18 @@
     BasicTableMixin,
     HasIdMixin,
 )
 from cs.tagset import (
     TagSet, Tag, TagFile, TagSetCriterion, TagBasedTest, TagsCommandMixin,
     TagsOntology, BaseTagSets, tag_or_tag_value, as_unixtime
 )
-from cs.threads import locked, State as ThreadState
+from cs.threads import locked, ThreadState
 from cs.upd import print  # pylint: disable=redefined-builtin
 
-__version__ = '20230217'
+__version__ = '20230612'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -669,15 +670,15 @@
           criterion=self,
           alias=alias,
           entity_id_column=entity_id_column,
           constraint=constraint if self.choice else -alias.has(constraint),
       )
     else:
       # general tag_name
-      sqlp = SQLTagProxy(orm, tag.self.tag_name).by_op_text(
+      sqlp = SQLTagProxy(orm, tag_name).by_op_text(
           self.comparison, tag_value, alias=alias
       )
     return sqlp
 
   def match_tagged_entity(self, te: TagSet) -> bool:
     ''' Match this criterion against `te`.
     '''
@@ -776,16 +777,16 @@
     '''
     return PolyValue(
         float_value=self.float_value,
         string_value=self.string_value,
         structured_value=self.structured_value,
     )
 
-  @typechecked
   @require(lambda pv: pv.is_valid())
+  @typechecked
   def set_polyvalue(self, pv: PolyValue):
     ''' Set all the value fields.
     '''
     self.float_value = pv.float_value
     self.string_value = pv.string_value
     self.structured_value = pv.structured_value
 
@@ -1383,15 +1384,15 @@
 
         Subclasses wanting extra type support
         should either:
         (usual approach) provide their own `TYPE_JS_MAPPING` class attribute
         as described at the top of this class
         or (for unusual requirements) override this method and also `from_js_str`.
     '''
-    with Pfx("as_js_str(%r, %s:%r)", tag_name, type(tag_value).__name__,
+    with Pfx("to_js_str(%r, %s:%r)", tag_name, type(tag_value).__name__,
              tag_value):
       for typelabel, (type_, to_str, from_str) in cls.TYPE_JS_MAPPING.items():
         assert ':' not in typelabel, "bad typelabel %r: colons forbidden" % (
             typelabel,
         )
         if isinstance(tag_value, type_):
           with Pfx("typelabel=%r", typelabel):
@@ -1411,16 +1412,16 @@
         or (for unusual requirements) override this method and also `to_js_str`.
     '''
     typelabel, js_s = js.split(':', 1)
     type_, to_str, from_str = cls.TYPE_JS_MAPPING[typelabel]
     return from_str(js_s)
 
   @classmethod
-  @typechecked
   @require(lambda pv: pv.is_valid())
+  @typechecked
   def from_polyvalue(cls, tag_name: str, pv: PolyValue):
     ''' Convert an SQL `PolyValue` to a tag value.
 
         This can be overridden by subclasses along with `to_polyvalue`.
         The `tag_name` is provided for context
         in case it should influence the normalisation.
     '''
@@ -1437,16 +1438,48 @@
     if js is None:
       return None
     if isinstance(js, str):
       return cls.from_js_str(tag_name, js)
     return js
 
   @classmethod
-  @typechecked
+  @pfx_method
+  def jsonable(cls, value):
+    ''' Convert `value` to a form which can be directly JSON serialised.
+
+        In particular this converts non-list/set/tuple Sequences to lists
+        and non-dict Mappings to dicts.
+
+        Warning: this is not robust against cycles.
+    '''
+    if value is None:
+      return None
+    if isinstance(value, (int, str, float)):
+      return value
+    # mapping?
+    if (isinstance(value, Mapping)
+        or hasattr(value, 'items') and callable(value.items)):
+      # mapping
+      return {
+          str(field): cls.jsonable(subvalue)
+          for field, subvalue in value.items()
+      }
+    if isinstance(value, (set, tuple, list, Sequence)):
+      return [cls.jsonable(subvalue) for subvalue in value]
+    try:
+      d = value._asdict()
+    except AttributeError:
+      pass
+    else:
+      return cls.jsonable(d)
+    raise TypeError('no JSONable value for %s:%r' % (type(value), value))
+
+  @classmethod
   @ensure(lambda result: result.is_valid())
+  @typechecked
   def to_polyvalue(cls, tag_name: str, tag_value) -> PolyValue:
     ''' Normalise `Tag` values for storage via SQL.
         Preserve things directly expressable in JSON.
         Convert other values via `to_js_str`.
         Return `PolyValue` for use with the SQL rows.
     '''
     if tag_value is None:
@@ -1456,15 +1489,15 @@
     if isinstance(tag_value, int):
       f = float(tag_value)
       if f == tag_value:
         return PolyValue(f, None, None)
     if isinstance(tag_value, str):
       return PolyValue(None, tag_value, None)
     if isinstance(tag_value, (list, tuple, dict)):
-      return PolyValue(None, None, tag_value)
+      return PolyValue(None, None, cls.jsonable(tag_value))
     # convert to a special string
     return PolyValue(None, None, cls.to_js_str(tag_name, tag_value))
 
   # pylint: disable=arguments-differ
   @tag_or_tag_value
   def set(self, tag_name, value, *, skip_db=False, verbose=None):
     if tag_name == 'id':
@@ -1582,18 +1615,18 @@
       _sqltags = self
     else:
       assert _sqltags is self
     return SQLTagSet(*a, _sqltags=_sqltags, **kw)
 
   @contextmanager
   def startup_shutdown(self):
-    ''' Empty stub startup/shutdown since we use autosessions.
-        Particularly, we do not want to keep SQLite dbs open.
+    ''' Open the ORM while the `SQLTags` is open.
     '''
-    yield self
+    with self.orm:
+      yield self
 
   @contextmanager
   def db_session(self, *, new=False):
     ''' Context manager to obtain a db session if required
         (or if `new` is true).
     '''
     orm_state = self.orm.sqla_state
@@ -1966,21 +1999,20 @@
             Default from ${DBURL_ENVVAR} (default '{DBURL_DEFAULT}').'''
 
   USAGE_KEYWORDS = {
       'DBURL_DEFAULT': DBURL_DEFAULT,
       'DBURL_ENVVAR': DBURL_ENVVAR,
   }
 
-  def apply_defaults(self):
-    ''' Set up the default values in `options`.
-    '''
-    options = self.options
-    db_url = self.TAGSETS_CLASS.infer_db_url()
-    options.db_url = db_url
-    options.sqltags = None
+  @dataclass
+  class Options(BaseCommand.Options):
+    db_url: str = field(
+        default_factory=lambda: BaseSQLTagsCommand.TAGSETS_CLASS.infer_db_url()
+    )
+    sqltags: Optional[SQLTags] = None
 
   def apply_opt(self, opt, val):
     ''' Apply a command line option.
     '''
     options = self.options
     if opt == '-f':
       options.db_url = val
```

### Comparing `cs.sqltags-20230217/lib/python/cs.sqltags.egg-info/PKG-INFO` & `cs.sqltags-20230612/lib/python/cs.sqltags.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.sqltags
-Version: 20230217
+Version: 20230612
 Summary: Simple SQL based tagging and the associated `sqltags` command line script, supporting both tagged named objects and tagged timestamped log entries.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
@@ -17,16 +17,17 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Simple SQL based tagging
 and the associated `sqltags` command line script,
 supporting both tagged named objects and tagged timestamped log entries.
 
-*Latest release 20230217*:
-SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
+*Latest release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
 
 Compared to `cs.fstags` and its associated `fstags` command,
 this is oriented towards large numbers of items
 not naturally associated with filesystem objects.
 
 My initial use case is an activity log
 (unnamed timestamped tag sets)
@@ -374,14 +375,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
+
 *Release 20230217*:
 SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
 
 *Release 20230212.1*:
 Mark SQLTags as promotable.
 
 *Release 20230212*:
```

### Comparing `cs.sqltags-20230217/pyproject.toml` & `cs.sqltags-20230612/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,55 +5,56 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python3",
 ]
 dependencies = [
     "cs.cmdutils>=20210404",
-    "cs.context>=20230212",
+    "cs.context>=20230331",
     "cs.dateutils>=20230210",
-    "cs.deco>=20230212",
-    "cs.fileutils>=20221118",
-    "cs.lex>=20230217",
+    "cs.deco>=20230331",
+    "cs.fileutils>=20230421",
+    "cs.lex>=20230401",
     "cs.logutils>=20230212",
     "cs.obj>=20220918",
-    "cs.pfx>=20221118",
+    "cs.pfx>=20230604",
     "cs.sqlalchemy_utils>=20210420",
     "cs.tagset>=20211212",
     "cs.threads>=20201025",
-    "cs.upd>=20230217",
+    "cs.upd>=20230401",
     "icontract",
     "sqlalchemy",
     "typeguard",
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
-version = "20230217"
+version = "20230612"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Simple SQL based tagging
 and the associated `sqltags` command line script,
 supporting both tagged named objects and tagged timestamped log entries.
 
-*Latest release 20230217*:
-SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
+*Latest release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
 
 Compared to `cs.fstags` and its associated `fstags` command,
 this is oriented towards large numbers of items
 not naturally associated with filesystem objects.
 
 My initial use case is an activity log
 (unnamed timestamped tag sets)
@@ -401,14 +402,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* SQLTagBasedTest.sql_parameters: fix general tag name.
+* SQLTagSet: new jsonable class method to produce a JSON serialisable object - converts sets and Sequences to flat lists, etc.
+
 *Release 20230217*:
 SQLTagsORM.search: previous changes seem to have dropped SQTCriterion support.
 
 *Release 20230212.1*:
 Mark SQLTags as promotable.
 
 *Release 20230212*:
```

### Comparing `cs.sqltags-20230217/setup.cfg` & `cs.sqltags-20230612/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.sqltags
-version = 20230217
+version = 20230612
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Simple SQL based tagging and the associated `sqltags` command line script, supporting both tagged named objects and tagged timestamped log entries.
 keywords = python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -19,26 +19,26 @@
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
 	cs.cmdutils>=20210404
-	cs.context>=20230212
+	cs.context>=20230331
 	cs.dateutils>=20230210
-	cs.deco>=20230212
-	cs.fileutils>=20221118
-	cs.lex>=20230217
+	cs.deco>=20230331
+	cs.fileutils>=20230421
+	cs.lex>=20230401
 	cs.logutils>=20230212
 	cs.obj>=20220918
-	cs.pfx>=20221118
+	cs.pfx>=20230604
 	cs.sqlalchemy_utils>=20210420
 	cs.tagset>=20211212
 	cs.threads>=20201025
-	cs.upd>=20230217
+	cs.upd>=20230401
 	icontract
 	sqlalchemy
 	typeguard
 
 [options.entry_points]
 console_scripts = 
 	sqltags = cs.sqltags:main
```

