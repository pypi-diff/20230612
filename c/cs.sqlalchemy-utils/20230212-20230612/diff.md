# Comparing `tmp/cs.sqlalchemy_utils-20230212.tar.gz` & `tmp/cs.sqlalchemy_utils-20230612.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.sqlalchemy_utils-20230212.tar", last modified: Sat Feb 11 21:17:28 2023, max compression
+gzip compressed data, was "cs.sqlalchemy_utils-20230612.tar", last modified: Mon Jun 12 04:24:09 2023, max compression
```

## Comparing `cs.sqlalchemy_utils-20230212.tar` & `cs.sqlalchemy_utils-20230612.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-11 21:17:28.611726 cs.sqlalchemy_utils-20230212/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-02-11 21:17:03.000000 cs.sqlalchemy_utils-20230212/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    14075 2023-02-11 21:17:28.611867 cs.sqlalchemy_utils-20230212/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    15208 2023-02-11 21:17:08.000000 cs.sqlalchemy_utils-20230212/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-11 21:17:28.607729 cs.sqlalchemy_utils-20230212/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-11 21:17:28.608043 cs.sqlalchemy_utils-20230212/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-11 21:17:28.609726 cs.sqlalchemy_utils-20230212/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    28690 2023-02-11 21:16:23.000000 cs.sqlalchemy_utils-20230212/lib/python/cs/sqlalchemy_utils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-02-11 21:17:28.611507 cs.sqlalchemy_utils-20230212/lib/python/cs.sqlalchemy_utils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    14075 2023-02-11 21:17:28.000000 cs.sqlalchemy_utils-20230212/lib/python/cs.sqlalchemy_utils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      358 2023-02-11 21:17:28.000000 cs.sqlalchemy_utils-20230212/lib/python/cs.sqlalchemy_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-02-11 21:17:28.000000 cs.sqlalchemy_utils-20230212/lib/python/cs.sqlalchemy_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      193 2023-02-11 21:17:28.000000 cs.sqlalchemy_utils-20230212/lib/python/cs.sqlalchemy_utils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-02-11 21:17:28.000000 cs.sqlalchemy_utils-20230212/lib/python/cs.sqlalchemy_utils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    14503 2023-02-11 21:17:20.000000 cs.sqlalchemy_utils-20230212/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      998 2023-02-11 21:17:28.612451 cs.sqlalchemy_utils-20230212/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-02-11 21:17:08.000000 cs.sqlalchemy_utils-20230212/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:24:09.859231 cs.sqlalchemy_utils-20230612/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-12 04:23:40.000000 cs.sqlalchemy_utils-20230612/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    14599 2023-06-12 04:24:09.859405 cs.sqlalchemy_utils-20230612/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15775 2023-06-12 04:23:45.000000 cs.sqlalchemy_utils-20230612/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:24:09.853953 cs.sqlalchemy_utils-20230612/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:24:09.854315 cs.sqlalchemy_utils-20230612/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:24:09.856922 cs.sqlalchemy_utils-20230612/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    29101 2023-06-12 04:23:29.000000 cs.sqlalchemy_utils-20230612/lib/python/cs/sqlalchemy_utils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-12 04:24:09.858924 cs.sqlalchemy_utils-20230612/lib/python/cs.sqlalchemy_utils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    14599 2023-06-12 04:24:09.000000 cs.sqlalchemy_utils-20230612/lib/python/cs.sqlalchemy_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      358 2023-06-12 04:24:09.000000 cs.sqlalchemy_utils-20230612/lib/python/cs.sqlalchemy_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-12 04:24:09.000000 cs.sqlalchemy_utils-20230612/lib/python/cs.sqlalchemy_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      198 2023-06-12 04:24:09.000000 cs.sqlalchemy_utils-20230612/lib/python/cs.sqlalchemy_utils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-12 04:24:09.000000 cs.sqlalchemy_utils-20230612/lib/python/cs.sqlalchemy_utils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    15032 2023-06-12 04:24:01.000000 cs.sqlalchemy_utils-20230612/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1003 2023-06-12 04:24:09.860074 cs.sqlalchemy_utils-20230612/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-12 04:23:45.000000 cs.sqlalchemy_utils-20230612/setup.py
```

### Comparing `cs.sqlalchemy_utils-20230212/PKG-INFO` & `cs.sqlalchemy_utils-20230612/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.sqlalchemy_utils
-Version: 20230212
+Version: 20230612
 Summary: Assorted utility functions to support working with SQLAlchemy.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -15,16 +15,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted utility functions to support working with SQLAlchemy.
 
-*Latest release 20230212*:
-ORM.__init__: drop case_sensitive, no longer supported?
+*Latest release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
 
 ## Function `auto_session(function)`
 
 Decorator to run a function in a session if one is not presupplied.
 The function `function` runs within a transaction,
 nested if the session already exists.
 
@@ -161,15 +163,15 @@
 and provides various Session related convenience methods.
 It is also a `MultiOpenMixin` subclass
 supporting nested open/close sequences and use as a context manager.
 
 *Method `ORM.__init__(self, db_url, serial_sessions=None)`*:
 Initialise the ORM.
 
-If `serial_sessions` is true (default `False`)
+If `serial_sessions` is true (default `True` for SQLite, `False` otherwise)
 then allocate a lock to serialise session allocation.
 This might be chosen with SQL backends which do not support
 concurrent sessions such as SQLite.
 
 In the case of SQLite there's a small inbuilt timeout in
 an attempt to serialise transactions but it is possible to
 exceed it easily and recovery is usually infeasible.
@@ -276,15 +278,15 @@
         ...
     KeyError: 'b'
     >>> set_json_field({'a': 2}, 'b.c', 4, infill=True)
     {'a': 2, 'b': {'c': 4}}
     >>> set_json_field(None, 'b.c', 4, infill=True)
     {'b': {'c': 4}}
 
-## Class `SQLAState(cs.threads.State, _thread._local)`
+## Class `SQLAState(cs.threads.ThreadState, _thread._local)`
 
 Thread local state for SQLAlchemy ORM and session.
 
 ## Function `using_session(orm=None, session=None)`
 
 A context manager to prepare an SQLAlchemy session
 for use by a suite.
@@ -334,14 +336,19 @@
 The `session` is also passed to `function` as
 the keyword parameter `session` to support nested calls.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
+
 *Release 20230212*:
 ORM.__init__: drop case_sensitive, no longer supported?
 
 *Release 20220606*:
 * BasicTableMixin: provide DEFAULT_ID_COLUMN='id', by_id() has new optional id_column parameter.
 * RelationProxy factory to make base classes which proxy a relation, for circumstances where you want to minimise access to the db itself.
 * ORM.engine_keywords: turn on echo mode only if "SQL" in $DEBUG.
```

### Comparing `cs.sqlalchemy_utils-20230212/README.md` & `cs.sqlalchemy_utils-20230612/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Assorted utility functions to support working with SQLAlchemy.
 
-*Latest release 20230212*:
-ORM.__init__: drop case_sensitive, no longer supported?
+*Latest release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
 
 ## Function `auto_session(function)`
 
 Decorator to run a function in a session if one is not presupplied.
 The function `function` runs within a transaction,
 nested if the session already exists.
 
@@ -154,28 +156,25 @@
 and provides various Session related convenience methods.
 It is also a `MultiOpenMixin` subclass
 supporting nested open/close sequences and use as a context manager.
 
 *Method `ORM.__init__(self, db_url, serial_sessions=None)`*:
 Initialise the ORM.
 
-If `serial_sessions` is true (default `False`)
+If `serial_sessions` is true (default `True` for SQLite, `False` otherwise)
 then allocate a lock to serialise session allocation.
 This might be chosen with SQL backends which do not support
 concurrent sessions such as SQLite.
 
 In the case of SQLite there's a small inbuilt timeout in
 an attempt to serialise transactions but it is possible to
 exceed it easily and recovery is usually infeasible.
 Instead we use the `serial_sessions` option to obtain a
 mutex before allocating a session.
 
-*Method `ORM.arranged_session(self)`*:
-Arrange a new session for this `Thread`.
-
 *Method `ORM.declare_schema(self)`*:
 Declare the database schema / ORM mapping.
 This just defines the relation types etc.
 It *does not* act on the database itself.
 It is called automatically at the end of `__init__`.
 
 Example:
@@ -194,23 +193,27 @@
 
 *Property `ORM.default_session`*:
 The current per-`Thread` session.
 
 *Property `ORM.engine`*:
 SQLAlchemy engine, made on demand.
 
+*Method `ORM.orchestrated_session(self)`*:
+Orchestrate a new session for this `Thread`,
+honouring `self.serial_session`.
+
 *Method `ORM.startup_shutdown(self)`*:
 Default startup/shutdown context manager.
 
 This base method operates a lockfile to manage concurrent access
 by other programmes (which would also need to honour this file).
 If you actually expect this to be common
 you should try to keep the `ORM` "open" as briefly as possible.
 The lock file is only operated if `self.db_fspath`,
-current set only for filesystem SQLite database URLs.
+currently set only for filesystem SQLite database URLs.
 
 ## Function `orm_auto_session(method)`
 
 Decorator to run a method in a session derived from `self.orm`
 if a session is not presupplied.
 Intended to assist classes with a `.orm` attribute.
 
@@ -308,15 +311,15 @@
         ...
     KeyError: 'b'
     >>> set_json_field({'a': 2}, 'b.c', 4, infill=True)
     {'a': 2, 'b': {'c': 4}}
     >>> set_json_field(None, 'b.c', 4, infill=True)
     {'b': {'c': 4}}
 
-## Class `SQLAState(cs.threads.State, _thread._local)`
+## Class `SQLAState(cs.threads.ThreadState, _thread._local)`
 
 Thread local state for SQLAlchemy ORM and session.
 
 *Method `SQLAState.auto_session(self, *, orm=None)`*:
 Context manager to use the current session
 if not `None`, otherwise to make one using `orm` or `self.orm`.
 
@@ -373,14 +376,19 @@
 The `session` is also passed to `function` as
 the keyword parameter `session` to support nested calls.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
+
 *Release 20230212*:
 ORM.__init__: drop case_sensitive, no longer supported?
 
 *Release 20220606*:
 * BasicTableMixin: provide DEFAULT_ID_COLUMN='id', by_id() has new optional id_column parameter.
 * RelationProxy factory to make base classes which proxy a relation, for circumstances where you want to minimise access to the db itself.
 * ORM.engine_keywords: turn on echo mode only if "SQL" in $DEBUG.
```

### Comparing `cs.sqlalchemy_utils-20230212/lib/python/cs/sqlalchemy_utils.py` & `cs.sqlalchemy_utils-20230612/lib/python/cs/sqlalchemy_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,56 +10,68 @@
 import os
 from os.path import abspath
 from threading import current_thread, Lock
 from typing import Any, Optional, Union, List, Tuple
 
 from icontract import require
 from sqlalchemy import Column, Integer, create_engine
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import sessionmaker as sqla_sessionmaker
+from sqlalchemy.orm import declarative_base, sessionmaker as sqla_sessionmaker
 from sqlalchemy.orm.attributes import flag_modified
 from sqlalchemy.pool import NullPool
 from typeguard import typechecked
 
 from cs.deco import decorator, contextdecorator
-from cs.fileutils import makelockfile
+from cs.fileutils import lockfile
 from cs.lex import cutprefix
 from cs.logutils import warning
 from cs.pfx import Pfx, pfx_call, pfx_method
 from cs.py.func import funccite, funcname
 from cs.resources import MultiOpenMixin
-from cs.threads import State
+from cs.threads import ThreadState
 
-__version__ = '20230212'
+##def CHECK():
+##  ''' Debug function to check for open sqltags.sqlite files,
+##      called when there should be done.
+##  '''
+##  X("CHECK")
+##  if os.system(
+##      f'lsof -n -p {os.getpid()} | fgrep "/Users/cameron/var/sqltags.sqlite"'
+##  ) == 0:
+##    os.system(f'lsof -n -p {os.getpid()}')
+##    raise RuntimeError
+##  from cs.py.stack import caller
+##  X("CHECK from %r", caller())
+
+__version__ = '20230612'
 
 DISTINFO = {
     'description':
     'Assorted utility functions to support working with SQLAlchemy.',
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Database",
     ],
     'install_requires': [
         'icontract',
-        'sqlalchemy',
+        'sqlalchemy>=2.0',
         'typeguard',
         'cs.deco',
         'cs.fileutils',
         'cs.lex',
         'cs.logutils',
         'cs.pfx',
         'cs.py.func',
         'cs.resources',
         'cs.threads',
     ],
 }
 
-class SQLAState(State):
+class SQLAState(ThreadState):
   ''' Thread local state for SQLAlchemy ORM and session.
   '''
 
   def __init__(
       self, *, orm, engine=None, session=None, sessionmaker=None, **kw
   ):
     # enforce provision of an ORM, default session=None
@@ -76,29 +88,31 @@
     if orm is None:
       orm = self.orm
       if orm is None:
         raise ValueError(
             "%s.new_session: no orm supplied and no self.orm" %
             (type(self).__name__,)
         )
-    with orm.arranged_session() as session:
+    with orm.orchestrated_session() as session:
       with session.begin_nested():
         with self(orm=orm, session=session):
           yield session
+    session.close()
 
   @contextmanager
   def auto_session(self, *, orm=None):
     ''' Context manager to use the current session
         if not `None`, otherwise to make one using `orm` or `self.orm`.
     '''
     session = self.session
     if session is None or (orm is not None and orm is not self.orm):
       # new session required
       with self.new_session(orm=orm) as session:
         yield session
+      session.close()
     else:
       with session.begin_nested():
         yield session
 
 # global state, not tied to any specific ORM or session
 state = SQLAState(orm=None, session=None)
 
@@ -242,15 +256,15 @@
       supporting nested open/close sequences and use as a context manager.
   '''
 
   @pfx_method
   def __init__(self, db_url, serial_sessions=None):
     ''' Initialise the ORM.
 
-        If `serial_sessions` is true (default `False`)
+        If `serial_sessions` is true (default `True` for SQLite, `False` otherwise)
         then allocate a lock to serialise session allocation.
         This might be chosen with SQL backends which do not support
         concurrent sessions such as SQLite.
 
         In the case of SQLite there's a small inbuilt timeout in
         an attempt to serialise transactions but it is possible to
         exceed it easily and recovery is usually infeasible.
@@ -281,15 +295,14 @@
         warning(
             "serial_sessions specified as %r, but is_sqlite=%s:"
             " this may cause trouble with multithreaded use",
             serial_sessions,
             is_sqlite,
         )
     self.serial_sessions = serial_sessions or is_sqlite
-    self._lockfilepath = None
     self.Base = declarative_base()
     self.sqla_state = SQLAState(
         orm=self, engine=None, sessionmaker=None, session=None
     )
     if serial_sessions:
       self._serial_sessions_lock = Lock()
     else:
@@ -337,22 +350,21 @@
     ''' Default startup/shutdown context manager.
 
         This base method operates a lockfile to manage concurrent access
         by other programmes (which would also need to honour this file).
         If you actually expect this to be common
         you should try to keep the `ORM` "open" as briefly as possible.
         The lock file is only operated if `self.db_fspath`,
-        current set only for filesystem SQLite database URLs.
+        currently set only for filesystem SQLite database URLs.
     '''
     if self.db_fspath:
-      self._lockfilepath = makelockfile(self.db_fspath, poll_interval=0.2)
-    yield
-    if self._lockfilepath is not None:
-      pfx_call(os.remove, self._lockfilepath)
-      self._lockfilepath = None
+      with lockfile(self.db_fspath, poll_interval=0.2):
+        yield
+    else:
+      yield
 
   @property
   def engine(self):
     ''' SQLAlchemy engine, made on demand.
     '''
     orm_state = self.sqla_state
     if self.serial_sessions:
@@ -378,16 +390,17 @@
       sessionmaker = sqla_sessionmaker(bind=self.engine)
       self._sessionmaker_raw = sessionmaker
       orm_state.sessionmaker = sessionmaker  # pylint: disable=attribute-defined-outside-init
     return sessionmaker
 
   @contextmanager
   @pfx_method(use_str=True)
-  def arranged_session(self):
-    ''' Arrange a new session for this `Thread`.
+  def orchestrated_session(self):
+    ''' Orchestrate a new session for this `Thread`,
+        honouring `self.serial_session`.
     '''
     orm_state = self.sqla_state
     with self:
       if self.serial_sessions:
         if orm_state.session is not None:
           T = current_thread()
           tid = "Thread:%d:%s" % (T.ident, T.name)
@@ -397,18 +410,20 @@
                   orm_state.session,
               )
           )
         with self._serial_sessions_lock:
           new_session = self._sessionmaker()
           with new_session.begin_nested():
             yield new_session
+          new_session.close()
       else:
         new_session = self._sessionmaker()
         with new_session.begin_nested():
           yield new_session
+        new_session.close()
 
   @property
   def default_session(self):
     ''' The current per-`Thread` session.
     '''
     return self.sqla_state.session
```

### Comparing `cs.sqlalchemy_utils-20230212/lib/python/cs.sqlalchemy_utils.egg-info/PKG-INFO` & `cs.sqlalchemy_utils-20230612/lib/python/cs.sqlalchemy_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.sqlalchemy-utils
-Version: 20230212
+Version: 20230612
 Summary: Assorted utility functions to support working with SQLAlchemy.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -15,16 +15,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted utility functions to support working with SQLAlchemy.
 
-*Latest release 20230212*:
-ORM.__init__: drop case_sensitive, no longer supported?
+*Latest release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
 
 ## Function `auto_session(function)`
 
 Decorator to run a function in a session if one is not presupplied.
 The function `function` runs within a transaction,
 nested if the session already exists.
 
@@ -161,15 +163,15 @@
 and provides various Session related convenience methods.
 It is also a `MultiOpenMixin` subclass
 supporting nested open/close sequences and use as a context manager.
 
 *Method `ORM.__init__(self, db_url, serial_sessions=None)`*:
 Initialise the ORM.
 
-If `serial_sessions` is true (default `False`)
+If `serial_sessions` is true (default `True` for SQLite, `False` otherwise)
 then allocate a lock to serialise session allocation.
 This might be chosen with SQL backends which do not support
 concurrent sessions such as SQLite.
 
 In the case of SQLite there's a small inbuilt timeout in
 an attempt to serialise transactions but it is possible to
 exceed it easily and recovery is usually infeasible.
@@ -276,15 +278,15 @@
         ...
     KeyError: 'b'
     >>> set_json_field({'a': 2}, 'b.c', 4, infill=True)
     {'a': 2, 'b': {'c': 4}}
     >>> set_json_field(None, 'b.c', 4, infill=True)
     {'b': {'c': 4}}
 
-## Class `SQLAState(cs.threads.State, _thread._local)`
+## Class `SQLAState(cs.threads.ThreadState, _thread._local)`
 
 Thread local state for SQLAlchemy ORM and session.
 
 ## Function `using_session(orm=None, session=None)`
 
 A context manager to prepare an SQLAlchemy session
 for use by a suite.
@@ -334,14 +336,19 @@
 The `session` is also passed to `function` as
 the keyword parameter `session` to support nested calls.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
+
 *Release 20230212*:
 ORM.__init__: drop case_sensitive, no longer supported?
 
 *Release 20220606*:
 * BasicTableMixin: provide DEFAULT_ID_COLUMN='id', by_id() has new optional id_column parameter.
 * RelationProxy factory to make base classes which proxy a relation, for circumstances where you want to minimise access to the db itself.
 * ORM.engine_keywords: turn on echo mode only if "SQL" in $DEBUG.
```

### Comparing `cs.sqlalchemy_utils-20230212/pyproject.toml` & `cs.sqlalchemy_utils-20230612/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,49 +5,51 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.deco>=20230210",
-    "cs.fileutils>=20221118",
-    "cs.lex>=20230210",
-    "cs.logutils>=20220531",
-    "cs.pfx>=20221118",
-    "cs.py.func>=20230210",
-    "cs.resources>=20230125",
-    "cs.threads>=20230125",
+    "cs.deco>=20230331",
+    "cs.fileutils>=20230421",
+    "cs.lex>=20230401",
+    "cs.logutils>=20230212",
+    "cs.pfx>=20230604",
+    "cs.py.func>=20230331",
+    "cs.resources>=20230503",
+    "cs.threads>=20230331",
     "icontract",
-    "sqlalchemy",
+    "sqlalchemy>=2.0",
     "typeguard",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Database",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230212"
+version = "20230612"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted utility functions to support working with SQLAlchemy.
 
-*Latest release 20230212*:
-ORM.__init__: drop case_sensitive, no longer supported?
+*Latest release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
 
 ## Function `auto_session(function)`
 
 Decorator to run a function in a session if one is not presupplied.
 The function `function` runs within a transaction,
 nested if the session already exists.
 
@@ -184,15 +186,15 @@
 and provides various Session related convenience methods.
 It is also a `MultiOpenMixin` subclass
 supporting nested open/close sequences and use as a context manager.
 
 *Method `ORM.__init__(self, db_url, serial_sessions=None)`*:
 Initialise the ORM.
 
-If `serial_sessions` is true (default `False`)
+If `serial_sessions` is true (default `True` for SQLite, `False` otherwise)
 then allocate a lock to serialise session allocation.
 This might be chosen with SQL backends which do not support
 concurrent sessions such as SQLite.
 
 In the case of SQLite there's a small inbuilt timeout in
 an attempt to serialise transactions but it is possible to
 exceed it easily and recovery is usually infeasible.
@@ -299,15 +301,15 @@
         ...
     KeyError: 'b'
     >>> set_json_field({'a': 2}, 'b.c', 4, infill=True)
     {'a': 2, 'b': {'c': 4}}
     >>> set_json_field(None, 'b.c', 4, infill=True)
     {'b': {'c': 4}}
 
-## Class `SQLAState(cs.threads.State, _thread._local)`
+## Class `SQLAState(cs.threads.ThreadState, _thread._local)`
 
 Thread local state for SQLAlchemy ORM and session.
 
 ## Function `using_session(orm=None, session=None)`
 
 A context manager to prepare an SQLAlchemy session
 for use by a suite.
@@ -357,14 +359,19 @@
 The `session` is also passed to `function` as
 the keyword parameter `session` to support nested calls.
 
 # Release Log
 
 
 
+*Release 20230612*:
+* Use cs.fileutils.lockfile context manager instead of makelockfile.
+* Rename arranged_session to orchestrated_session.
+* Some tweaks around connection closes, still edging towards a good work practice for easily doing short lived stuff (for cs.ebooks.calibre).
+
 *Release 20230212*:
 ORM.__init__: drop case_sensitive, no longer supported?
 
 *Release 20220606*:
 * BasicTableMixin: provide DEFAULT_ID_COLUMN='id', by_id() has new optional id_column parameter.
 * RelationProxy factory to make base classes which proxy a relation, for circumstances where you want to minimise access to the db itself.
 * ORM.engine_keywords: turn on echo mode only if \"SQL\" in $DEBUG.
```

### Comparing `cs.sqlalchemy_utils-20230212/setup.cfg` & `cs.sqlalchemy_utils-20230612/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.sqlalchemy_utils
-version = 20230212
+version = 20230612
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Assorted utility functions to support working with SQLAlchemy.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers = 
@@ -18,23 +18,23 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 package_dir = 
 	= lib/python
 install_requires = 
-	cs.deco>=20230210
-	cs.fileutils>=20221118
-	cs.lex>=20230210
-	cs.logutils>=20220531
-	cs.pfx>=20221118
-	cs.py.func>=20230210
-	cs.resources>=20230125
-	cs.threads>=20230125
+	cs.deco>=20230331
+	cs.fileutils>=20230421
+	cs.lex>=20230401
+	cs.logutils>=20230212
+	cs.pfx>=20230604
+	cs.py.func>=20230331
+	cs.resources>=20230503
+	cs.threads>=20230331
 	icontract
-	sqlalchemy
+	sqlalchemy>=2.0
 	typeguard
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

