# Comparing `tmp/tinydb-4.7.1.tar.gz` & `tmp/tinydb-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinydb-4.7.1.tar", max compression
+gzip compressed data, was "tinydb-4.8.0.tar", max compression
```

## Comparing `tinydb-4.7.1.tar` & `tinydb-4.8.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0     1080 2023-01-14 16:22:55.213797 tinydb-4.7.1/LICENSE
--rw-r--r--   0        0        0     4720 2023-01-14 16:22:55.213797 tinydb-4.7.1/README.rst
--rw-r--r--   0        0        0     1919 2023-01-14 16:22:55.217798 tinydb-4.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/__init__.py
--rw-r--r--   0        0        0      625 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/conftest.py
--rw-r--r--   0        0        0     2412 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/test_middlewares.py
--rw-r--r--   0        0        0     1021 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/test_operations.py
--rw-r--r--   0        0        0    12331 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/test_queries.py
--rw-r--r--   0        0        0     6489 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/test_storages.py
--rw-r--r--   0        0        0     3899 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/test_tables.py
--rw-r--r--   0        0        0    17882 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/test_tinydb.py
--rw-r--r--   0        0        0     2123 2023-01-14 16:22:55.217798 tinydb-4.7.1/tests/test_utils.py
--rw-r--r--   0        0        0      939 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/__init__.py
--rw-r--r--   0        0        0     8712 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/database.py
--rw-r--r--   0        0        0     3942 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/middlewares.py
--rw-r--r--   0        0        0     1070 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/mypy_plugin.py
--rw-r--r--   0        0        0     1155 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/operations.py
--rw-r--r--   0        0        0        0 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/py.typed
--rw-r--r--   0        0        0    16016 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/queries.py
--rw-r--r--   0        0        0     4726 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/storages.py
--rw-r--r--   0        0        0    25207 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/table.py
--rw-r--r--   0        0        0     4598 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/utils.py
--rw-r--r--   0        0        0       22 2023-01-14 16:22:55.217798 tinydb-4.7.1/tinydb/version.py
--rw-r--r--   0        0        0     5601 1970-01-01 00:00:00.000000 tinydb-4.7.1/setup.py
--rw-r--r--   0        0        0     6496 1970-01-01 00:00:00.000000 tinydb-4.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-12 19:06:07.709448 tinydb-4.8.0/LICENSE
+-rw-r--r--   0        0        0     4720 2023-06-12 19:06:07.709448 tinydb-4.8.0/README.rst
+-rw-r--r--   0        0        0     1914 2023-06-12 19:06:07.709448 tinydb-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 19:06:07.709448 tinydb-4.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      625 2023-06-12 19:06:07.709448 tinydb-4.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     2412 2023-06-12 19:06:07.713448 tinydb-4.8.0/tests/test_middlewares.py
+-rw-r--r--   0        0        0     1021 2023-06-12 19:06:07.713448 tinydb-4.8.0/tests/test_operations.py
+-rw-r--r--   0        0        0    12331 2023-06-12 19:06:07.713448 tinydb-4.8.0/tests/test_queries.py
+-rw-r--r--   0        0        0     6489 2023-06-12 19:06:07.713448 tinydb-4.8.0/tests/test_storages.py
+-rw-r--r--   0        0        0     3899 2023-06-12 19:06:07.713448 tinydb-4.8.0/tests/test_tables.py
+-rw-r--r--   0        0        0    18110 2023-06-12 19:06:07.713448 tinydb-4.8.0/tests/test_tinydb.py
+-rw-r--r--   0        0        0     2123 2023-06-12 19:06:07.713448 tinydb-4.8.0/tests/test_utils.py
+-rw-r--r--   0        0        0      939 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/__init__.py
+-rw-r--r--   0        0        0     8712 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/database.py
+-rw-r--r--   0        0        0     3942 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/middlewares.py
+-rw-r--r--   0        0        0     1070 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/mypy_plugin.py
+-rw-r--r--   0        0        0     1155 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/operations.py
+-rw-r--r--   0        0        0        0 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/py.typed
+-rw-r--r--   0        0        0    16016 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/queries.py
+-rw-r--r--   0        0        0     5084 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/storages.py
+-rw-r--r--   0        0        0    26044 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/table.py
+-rw-r--r--   0        0        0     4598 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/utils.py
+-rw-r--r--   0        0        0       22 2023-06-12 19:06:07.713448 tinydb-4.8.0/tinydb/version.py
+-rw-r--r--   0        0        0     6191 1970-01-01 00:00:00.000000 tinydb-4.8.0/PKG-INFO
```

### Comparing `tinydb-4.7.1/LICENSE` & `tinydb-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/README.rst` & `tinydb-4.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/pyproject.toml` & `tinydb-4.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinydb"
-version = "4.7.1"
+version = "4.8.0"
 description = "TinyDB is a tiny, document oriented database optimized for your happiness :)"
 authors = ["Markus Siemens <markus@m-siemens.de>"]
 license = "MIT"
 
 readme = "README.rst"
 
 homepage = "https://github.com/msiemens/tinydb"
@@ -34,15 +34,15 @@
 
 packages = [
     { include = "tinydb" },
     { include = "tests", format = "sdist" }
 ]
 
 [tool.poetry.urls]
-"Changelog" = "https://github.com/msiemens/tinydb/en/latest/changelog.html"
+"Changelog" = "https://tinydb.readthedocs.io/en/latest/changelog.html"
 "Issues" = "https://github.com/msiemens/tinydb/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typing-extensions = { version = "^3.10.0 || ^4.0.0", python = "<=3.7" }
 
 [tool.poetry.dev-dependencies]
```

### Comparing `tinydb-4.7.1/tests/conftest.py` & `tinydb-4.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tests/test_middlewares.py` & `tinydb-4.8.0/tests/test_middlewares.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tests/test_operations.py` & `tinydb-4.8.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tests/test_queries.py` & `tinydb-4.8.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tests/test_storages.py` & `tinydb-4.8.0/tests/test_storages.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tests/test_tables.py` & `tinydb-4.8.0/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tests/test_tinydb.py` & `tinydb-4.8.0/tests/test_tinydb.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,29 +302,32 @@
     db.upsert({'int': 5}, where('char') == 'a')
     assert db.count(where('int') == 5) == 1
 
     # Document missing
     assert db.upsert({'int': 9, 'char': 'x'}, where('char') == 'x') == [4]
     assert db.count(where('int') == 9) == 1
 
+
 def test_upsert_by_id(db: TinyDB):
     assert len(db) == 3
 
     # Single document existing
     extant_doc = Document({'char': 'v'}, doc_id=1)
     assert db.upsert(extant_doc) == [1]
     doc = db.get(where('char') == 'v')
+    assert isinstance(doc, Document)
     assert doc is not None
     assert doc.doc_id == 1
     assert len(db) == 3
 
     # Single document missing
     missing_doc = Document({'int': 5, 'char': 'w'}, doc_id=5)
     assert db.upsert(missing_doc) == [5]
     doc = db.get(where('char') == 'w')
+    assert isinstance(doc, Document)
     assert doc is not None
     assert doc.doc_id == 5
     assert len(db) == 4
 
     # Missing doc_id and condition
     with pytest.raises(ValueError, match=r"(?=.*\bdoc_id\b)(?=.*\bquery\b)"):
         db.upsert({'no_Document': 'no_query'})
@@ -353,24 +356,30 @@
 def test_search_no_results_cache(db: TinyDB):
     assert len(db.search(where('missing').exists())) == 0
     assert len(db.search(where('missing').exists())) == 0
 
 
 def test_get(db: TinyDB):
     item = db.get(where('char') == 'b')
+    assert isinstance(item, Document)
     assert item is not None
     assert item['char'] == 'b'
 
 
 def test_get_ids(db: TinyDB):
     el = db.all()[0]
     assert db.get(doc_id=el.doc_id) == el
     assert db.get(doc_id=float('NaN')) is None  # type: ignore
 
 
+def test_get_multiple_ids(db: TinyDB):
+    el = db.all()
+    assert db.get(doc_ids=[x.doc_id for x in el]) == el
+
+
 def test_get_invalid(db: TinyDB):
     with pytest.raises(RuntimeError):
         db.get()
 
 
 def test_count(db: TinyDB):
     assert db.count(where('int') == 1) == 3
```

### Comparing `tinydb-4.7.1/tests/test_utils.py` & `tinydb-4.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tinydb/__init__.py` & `tinydb-4.8.0/tinydb/__init__.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tinydb/database.py` & `tinydb-4.8.0/tinydb/database.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tinydb/middlewares.py` & `tinydb-4.8.0/tinydb/middlewares.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tinydb/mypy_plugin.py` & `tinydb-4.8.0/tinydb/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tinydb/operations.py` & `tinydb-4.8.0/tinydb/operations.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tinydb/queries.py` & `tinydb-4.8.0/tinydb/queries.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/tinydb/storages.py` & `tinydb-4.8.0/tinydb/storages.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Contains the :class:`base class <tinydb.storages.Storage>` for storages and
 implementations.
 """
 
 import io
 import json
 import os
+import warnings
 from abc import ABC, abstractmethod
 from typing import Dict, Any, Optional
 
 __all__ = ('Storage', 'JSONStorage', 'MemoryStorage')
 
 
 def touch(path: str, create_dirs: bool):
@@ -80,26 +81,36 @@
     Store the data in a JSON file.
     """
 
     def __init__(self, path: str, create_dirs=False, encoding=None, access_mode='r+', **kwargs):
         """
         Create a new instance.
 
-        Also creates the storage file, if it doesn't exist and the access mode is appropriate for writing.
+        Also creates the storage file, if it doesn't exist and the access mode
+        is appropriate for writing.
+
+        Note: Using an access mode other than `r` or `r+` will probably lead to
+        data loss or data corruption!
 
         :param path: Where to store the JSON data.
-        :param access_mode: mode in which the file is opened (r, r+, w, a, x, b, t, +, U)
+        :param access_mode: mode in which the file is opened (r, r+)
         :type access_mode: str
         """
 
         super().__init__()
 
         self._mode = access_mode
         self.kwargs = kwargs
 
+        if access_mode not in ('r', 'rb', 'r+', 'rb+'):
+            warnings.warn(
+                'Using an `access_mode` other than \'r\', \'rb\', \'r+\' '
+                'or \'rb+\' can cause data loss or corruption'
+            )
+
         # Create the file if it doesn't exist and creating is allowed by the
         # access mode
         if any([character in self._mode for character in ('+', 'w', 'a')]):  # any of the writing modes
             touch(path, create_dirs=create_dirs)
 
         # Open the file for reading/writing
         self._handle = open(path, mode=self._mode, encoding=encoding)
```

### Comparing `tinydb-4.7.1/tinydb/table.py` & `tinydb-4.8.0/tinydb/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,37 +276,56 @@
 
         return docs
 
     def get(
         self,
         cond: Optional[QueryLike] = None,
         doc_id: Optional[int] = None,
-    ) -> Optional[Document]:
+        doc_ids: Optional[List] = None
+    ) -> Optional[Union[Document, List[Document]]]:
         """
         Get exactly one document specified by a query or a document ID.
-
+        However, if multiple document IDs are given then returns all
+        documents in a list.
+        
         Returns ``None`` if the document doesn't exist.
 
         :param cond: the condition to check against
         :param doc_id: the document's ID
+        :param doc_ids: the document's IDs(multiple)
 
-        :returns: the document or ``None``
+        :returns: the document(s) or ``None``
         """
+        table = self._read_table()
 
         if doc_id is not None:
             # Retrieve a document specified by its ID
-            table = self._read_table()
             raw_doc = table.get(str(doc_id), None)
 
             if raw_doc is None:
                 return None
 
             # Convert the raw data to the document class
             return self.document_class(raw_doc, doc_id)
 
+        elif doc_ids is not None:
+            # Filter the table by extracting out all those documents which
+            # have doc id specified in the doc_id list.
+
+            # Since document IDs will be unique, we make it a set to ensure
+            # constant time lookup
+            doc_ids_set = set(str(doc_id) for doc_id in doc_ids)
+
+            # Now return the filtered documents in form of list
+            return [
+                self.document_class(doc, self.document_id_class(doc_id))
+                for doc_id, doc in table.items()
+                if doc_id in doc_ids_set
+            ]
+
         elif cond is not None:
             # Find a document specified by a query
             # The trailing underscore in doc_id_ is needed so MyPy
             # doesn't think that `doc_id_` (which is a string) needs
             # to have the same type as `doc_id` which is this function's
             # parameter and is an optional `int`.
             for doc_id_, doc in self._read_table().items():
@@ -314,15 +333,15 @@
                     return self.document_class(
                         doc,
                         self.document_id_class(doc_id_)
                     )
 
             return None
 
-        raise RuntimeError('You have to pass either cond or doc_id')
+        raise RuntimeError('You have to pass either cond or doc_id or doc_ids')
 
     def contains(
         self,
         cond: Optional[QueryLike] = None,
         doc_id: Optional[int] = None
     ) -> bool:
         """
```

### Comparing `tinydb-4.7.1/tinydb/utils.py` & `tinydb-4.8.0/tinydb/utils.py`

 * *Files identical despite different names*

### Comparing `tinydb-4.7.1/setup.py` & `tinydb-4.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,170 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tinydb
+Version: 4.8.0
+Summary: TinyDB is a tiny, document oriented database optimized for your happiness :)
+Home-page: https://github.com/msiemens/tinydb
+License: MIT
+Keywords: database,nosql
+Author: Markus Siemens
+Author-email: markus@m-siemens.de
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Database
+Classifier: Topic :: Database :: Database Engines/Servers
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: typing-extensions (>=3.10.0,<5.0.0) ; python_full_version <= "3.7.0"
+Project-URL: Changelog, https://tinydb.readthedocs.io/en/latest/changelog.html
+Project-URL: Documentation, https://tinydb.readthedocs.org/
+Project-URL: Issues, https://github.com/msiemens/tinydb/issues
+Description-Content-Type: text/x-rst
+
+.. image:: https://raw.githubusercontent.com/msiemens/tinydb/master/artwork/logo.png
+    :scale: 100%
+    :height: 150px
+
+|Build Status| |Coverage| |Version|
+
+Quick Links
+***********
+
+- `Example Code`_
+- `Supported Python Versions`_
+- `Documentation <http://tinydb.readthedocs.org/>`_
+- `Changelog <https://tinydb.readthedocs.io/en/latest/changelog.html>`_
+- `Extensions <https://tinydb.readthedocs.io/en/latest/extensions.html>`_
+- `Contributing`_
+
+Introduction
+************
+
+TinyDB is a lightweight document oriented database optimized for your happiness :)
+It's written in pure Python and has no external dependencies. The target are
+small apps that would be blown away by a SQL-DB or an external database server.
+
+TinyDB is:
+
+- **tiny:** The current source code has 1800 lines of code (with about 40%
+  documentation) and 1600 lines tests.
+
+- **document oriented:** Like MongoDB_, you can store any document
+  (represented as ``dict``) in TinyDB.
+
+- **optimized for your happiness:** TinyDB is designed to be simple and
+  fun to use by providing a simple and clean API.
+
+- **written in pure Python:** TinyDB neither needs an external server (as
+  e.g. `PyMongo <https://api.mongodb.org/python/current/>`_) nor any dependencies
+  from PyPI.
+
+- **works on Python 3.7+ and PyPy3:** TinyDB works on all modern versions of Python
+  and PyPy.
+
+- **powerfully extensible:** You can easily extend TinyDB by writing new
+  storages or modify the behaviour of storages with Middlewares.
+
+- **100% test coverage:** No explanation needed.
+
+To dive straight into all the details, head over to the `TinyDB docs
+<https://tinydb.readthedocs.io/>`_. You can also discuss everything related
+to TinyDB like general development, extensions or showcase your TinyDB-based
+projects on the `discussion forum <http://forum.m-siemens.de/.>`_.
+
+Supported Python Versions
+*************************
+
+TinyDB has been tested with Python 3.7 - 3.11 and PyPy3.
+
+Example Code
+************
+
+.. code-block:: python
+
+    >>> from tinydb import TinyDB, Query
+    >>> db = TinyDB('/path/to/db.json')
+    >>> db.insert({'int': 1, 'char': 'a'})
+    >>> db.insert({'int': 1, 'char': 'b'})
+
+Query Language
+==============
+
+.. code-block:: python
+
+    >>> User = Query()
+    >>> # Search for a field value
+    >>> db.search(User.name == 'John')
+    [{'name': 'John', 'age': 22}, {'name': 'John', 'age': 37}]
+
+    >>> # Combine two queries with logical and
+    >>> db.search((User.name == 'John') & (User.age <= 30))
+    [{'name': 'John', 'age': 22}]
+
+    >>> # Combine two queries with logical or
+    >>> db.search((User.name == 'John') | (User.name == 'Bob'))
+    [{'name': 'John', 'age': 22}, {'name': 'John', 'age': 37}, {'name': 'Bob', 'age': 42}]
+
+    >>> # Apply transformation to field with `map`
+    >>> db.search((User.age.map(lambda x: x + x) == 44))
+    >>> [{'name': 'John', 'age': 22}]
+
+    >>> # More possible comparisons:  !=  <  >  <=  >=
+    >>> # More possible checks: where(...).matches(regex), where(...).test(your_test_func)
+
+Tables
+======
+
+.. code-block:: python
+
+    >>> table = db.table('name')
+    >>> table.insert({'value': True})
+    >>> table.all()
+    [{'value': True}]
+
+Using Middlewares
+=================
+
+.. code-block:: python
+
+    >>> from tinydb.storages import JSONStorage
+    >>> from tinydb.middlewares import CachingMiddleware
+    >>> db = TinyDB('/path/to/db.json', storage=CachingMiddleware(JSONStorage))
+
+
+Contributing
+************
+
+Whether reporting bugs, discussing improvements and new ideas or writing
+extensions: Contributions to TinyDB are welcome! Here's how to get started:
+
+1. Check for open issues or open a fresh issue to start a discussion around
+   a feature idea or a bug
+2. Fork `the repository <https://github.com/msiemens/tinydb/>`_ on Github,
+   create a new branch off the `master` branch and start making your changes
+   (known as `GitHub Flow <https://guides.github.com/introduction/flow/index.html>`_)
+3. Write a test which shows that the bug was fixed or that the feature works
+   as expected
+4. Send a pull request and bug the maintainer until it gets merged and
+   published ☺
+
+.. |Build Status| image:: https://img.shields.io/azure-devops/build/msiemens/3e5baa75-12ec-43ac-9728-89823ee8c7e2/2.svg?style=flat-square
+   :target: https://dev.azure.com/msiemens/github/_build?definitionId=2
+.. |Coverage| image:: http://img.shields.io/coveralls/msiemens/tinydb.svg?style=flat-square
+   :target: https://coveralls.io/r/msiemens/tinydb
+.. |Version| image:: http://img.shields.io/pypi/v/tinydb.svg?style=flat-square
+   :target: https://pypi.python.org/pypi/tinydb/
+.. _Buzhug: http://buzhug.sourceforge.net/
+.. _CodernityDB: https://github.com/perchouli/codernitydb
+.. _MongoDB: http://mongodb.org/
 
-packages = \
-['tests', 'tinydb']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{':python_full_version <= "3.7.0"': ['typing-extensions>=3.10.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'tinydb',
-    'version': '4.7.1',
-    'description': 'TinyDB is a tiny, document oriented database optimized for your happiness :)',
-    'long_description': ".. image:: https://raw.githubusercontent.com/msiemens/tinydb/master/artwork/logo.png\n    :scale: 100%\n    :height: 150px\n\n|Build Status| |Coverage| |Version|\n\nQuick Links\n***********\n\n- `Example Code`_\n- `Supported Python Versions`_\n- `Documentation <http://tinydb.readthedocs.org/>`_\n- `Changelog <https://tinydb.readthedocs.io/en/latest/changelog.html>`_\n- `Extensions <https://tinydb.readthedocs.io/en/latest/extensions.html>`_\n- `Contributing`_\n\nIntroduction\n************\n\nTinyDB is a lightweight document oriented database optimized for your happiness :)\nIt's written in pure Python and has no external dependencies. The target are\nsmall apps that would be blown away by a SQL-DB or an external database server.\n\nTinyDB is:\n\n- **tiny:** The current source code has 1800 lines of code (with about 40%\n  documentation) and 1600 lines tests.\n\n- **document oriented:** Like MongoDB_, you can store any document\n  (represented as ``dict``) in TinyDB.\n\n- **optimized for your happiness:** TinyDB is designed to be simple and\n  fun to use by providing a simple and clean API.\n\n- **written in pure Python:** TinyDB neither needs an external server (as\n  e.g. `PyMongo <https://api.mongodb.org/python/current/>`_) nor any dependencies\n  from PyPI.\n\n- **works on Python 3.7+ and PyPy3:** TinyDB works on all modern versions of Python\n  and PyPy.\n\n- **powerfully extensible:** You can easily extend TinyDB by writing new\n  storages or modify the behaviour of storages with Middlewares.\n\n- **100% test coverage:** No explanation needed.\n\nTo dive straight into all the details, head over to the `TinyDB docs\n<https://tinydb.readthedocs.io/>`_. You can also discuss everything related\nto TinyDB like general development, extensions or showcase your TinyDB-based\nprojects on the `discussion forum <http://forum.m-siemens.de/.>`_.\n\nSupported Python Versions\n*************************\n\nTinyDB has been tested with Python 3.7 - 3.11 and PyPy3.\n\nExample Code\n************\n\n.. code-block:: python\n\n    >>> from tinydb import TinyDB, Query\n    >>> db = TinyDB('/path/to/db.json')\n    >>> db.insert({'int': 1, 'char': 'a'})\n    >>> db.insert({'int': 1, 'char': 'b'})\n\nQuery Language\n==============\n\n.. code-block:: python\n\n    >>> User = Query()\n    >>> # Search for a field value\n    >>> db.search(User.name == 'John')\n    [{'name': 'John', 'age': 22}, {'name': 'John', 'age': 37}]\n\n    >>> # Combine two queries with logical and\n    >>> db.search((User.name == 'John') & (User.age <= 30))\n    [{'name': 'John', 'age': 22}]\n\n    >>> # Combine two queries with logical or\n    >>> db.search((User.name == 'John') | (User.name == 'Bob'))\n    [{'name': 'John', 'age': 22}, {'name': 'John', 'age': 37}, {'name': 'Bob', 'age': 42}]\n\n    >>> # Apply transformation to field with `map`\n    >>> db.search((User.age.map(lambda x: x + x) == 44))\n    >>> [{'name': 'John', 'age': 22}]\n\n    >>> # More possible comparisons:  !=  <  >  <=  >=\n    >>> # More possible checks: where(...).matches(regex), where(...).test(your_test_func)\n\nTables\n======\n\n.. code-block:: python\n\n    >>> table = db.table('name')\n    >>> table.insert({'value': True})\n    >>> table.all()\n    [{'value': True}]\n\nUsing Middlewares\n=================\n\n.. code-block:: python\n\n    >>> from tinydb.storages import JSONStorage\n    >>> from tinydb.middlewares import CachingMiddleware\n    >>> db = TinyDB('/path/to/db.json', storage=CachingMiddleware(JSONStorage))\n\n\nContributing\n************\n\nWhether reporting bugs, discussing improvements and new ideas or writing\nextensions: Contributions to TinyDB are welcome! Here's how to get started:\n\n1. Check for open issues or open a fresh issue to start a discussion around\n   a feature idea or a bug\n2. Fork `the repository <https://github.com/msiemens/tinydb/>`_ on Github,\n   create a new branch off the `master` branch and start making your changes\n   (known as `GitHub Flow <https://guides.github.com/introduction/flow/index.html>`_)\n3. Write a test which shows that the bug was fixed or that the feature works\n   as expected\n4. Send a pull request and bug the maintainer until it gets merged and\n   published ☺\n\n.. |Build Status| image:: https://img.shields.io/azure-devops/build/msiemens/3e5baa75-12ec-43ac-9728-89823ee8c7e2/2.svg?style=flat-square\n   :target: https://dev.azure.com/msiemens/github/_build?definitionId=2\n.. |Coverage| image:: http://img.shields.io/coveralls/msiemens/tinydb.svg?style=flat-square\n   :target: https://coveralls.io/r/msiemens/tinydb\n.. |Version| image:: http://img.shields.io/pypi/v/tinydb.svg?style=flat-square\n   :target: https://pypi.python.org/pypi/tinydb/\n.. _Buzhug: http://buzhug.sourceforge.net/\n.. _CodernityDB: https://github.com/perchouli/codernitydb\n.. _MongoDB: http://mongodb.org/\n",
-    'author': 'Markus Siemens',
-    'author_email': 'markus@m-siemens.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/msiemens/tinydb',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

